# Comparing `tmp/omni-pro-0.1.27.tar.gz` & `tmp/omni-pro-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-pro-0.1.27.tar", last modified: Thu Jul 27 21:28:09 2023, max compression
+gzip compressed data, was "omni-pro-0.1.28.tar", last modified: Fri Jul 28 16:58:32 2023, max compression
```

## Comparing `omni-pro-0.1.27.tar` & `omni-pro-0.1.28.tar`

### file list

```diff
@@ -1,341 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.767410 omni-pro-0.1.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 21:27:44.000000 omni-pro-0.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-27 21:28:09.767410 omni-pro-0.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-27 21:27:44.000000 omni-pro-0.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/data/models.user.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/common/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/custom_fields/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/models/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.731410 omni-pro-0.1.27/omni/pro/models/sql/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/catalog/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/models/sql/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/common/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/models/sql/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_category_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_locality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/rules/warehouse_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/models/sql/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/stock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/models/sql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/utilities/country.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/utilities/territory_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/sql/utilities/territory_matrix_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/models/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/models/utilities/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/protos/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/common/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/common/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/common/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/grpc_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.735410 omni-pro-0.1.27/omni/pro/protos/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.739410 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.739410 omni-pro-0.1.27/omni/pro/protos/v1/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.747410 omni-pro-0.1.27/omni/pro/protos/v1/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.755410 omni-pro-0.1.27/omni/pro/protos/v1/sales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.763410 omni-pro-0.1.27/omni/pro/protos/v1/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.763410 omni-pro-0.1.27/omni/pro/protos/v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.767410 omni-pro-0.1.27/omni/pro/protos/v1/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/timezone_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/timezone_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.767410 omni-pro-0.1.27/omni/pro/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/user/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-27 21:27:44.000000 omni-pro-0.1.27/omni/pro/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:09.767410 omni-pro-0.1.27/omni_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-27 21:28:09.000000 omni-pro-0.1.27/omni_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-07-27 21:28:09.000000 omni-pro-0.1.27/omni_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:28:09.000000 omni-pro-0.1.27/omni_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 21:28:09.000000 omni-pro-0.1.27/omni_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 21:28:09.000000 omni-pro-0.1.27/omni_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:28:09.767410 omni-pro-0.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-27 21:28:03.000000 omni-pro-0.1.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.863568 omni-pro-0.1.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-28 16:58:04.000000 omni-pro-0.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-28 16:58:32.863568 omni-pro-0.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-28 16:58:04.000000 omni-pro-0.1.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.819567 omni-pro-0.1.28/omni/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.819567 omni-pro-0.1.28/omni/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.819567 omni-pro-0.1.28/omni/pro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/data/models.user.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.819567 omni-pro-0.1.28/omni/pro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/common/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/custom_fields/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/catalog/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/common/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_category_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_locality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/rules/warehouse_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/stock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.823567 omni-pro-0.1.28/omni/pro/models/sql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/utilities/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/utilities/territory_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/sql/utilities/territory_matrix_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/models/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/models/utilities/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/protos/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/common/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/common/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/common/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/grpc_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/protos/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.827567 omni-pro-0.1.28/omni/pro/protos/v1/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.839568 omni-pro-0.1.28/omni/pro/protos/v1/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.847568 omni-pro-0.1.28/omni/pro/protos/v1/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.851568 omni-pro-0.1.28/omni/pro/protos/v1/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.851568 omni-pro-0.1.28/omni/pro/protos/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.863568 omni-pro-0.1.28/omni/pro/protos/v1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.863568 omni-pro-0.1.28/omni/pro/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/user/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-28 16:58:04.000000 omni-pro-0.1.28/omni/pro/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:32.863568 omni-pro-0.1.28/omni_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-28 16:58:32.000000 omni-pro-0.1.28/omni_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-28 16:58:32.000000 omni-pro-0.1.28/omni_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:58:32.000000 omni-pro-0.1.28/omni_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-28 16:58:32.000000 omni-pro-0.1.28/omni_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 16:58:32.000000 omni-pro-0.1.28/omni_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:58:32.863568 omni-pro-0.1.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-28 16:58:25.000000 omni-pro-0.1.28/setup.py
```

### Comparing `omni-pro-0.1.27/LICENSE` & `omni-pro-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/PKG-INFO` & `omni-pro-0.1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.27
+Version: 0.1.28
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.27/README.md` & `omni-pro-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/aws.py` & `omni-pro-0.1.28/omni/pro/aws.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/cloudmap.py` & `omni-pro-0.1.28/omni/pro/cloudmap.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/config.py` & `omni-pro-0.1.28/omni/pro/config.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/database.py` & `omni-pro-0.1.28/omni/pro/database.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/decorators.py` & `omni-pro-0.1.28/omni/pro/decorators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/initial.py` & `omni-pro-0.1.28/omni/pro/initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import csv
 from pathlib import Path
 
-import grpc
-from google.protobuf import wrappers_pb2
 from omni.pro import redis, util
-from omni.pro.cloudmap import CloudMap
 from omni.pro.config import Config
 from omni.pro.database import DatabaseManager
 from omni.pro.logger import LoggerTraceback, configure_logger
-from omni.pro.models.common.ms import MicroService
-from omni.pro.protos.v1.users import user_pb2, user_pb2_grpc
+from omni.pro.models.common.ms import MicroService as MicroServiceDocument
+from omni.pro.protos.grpc_connector import Event, GRPClient
+from omni.pro.protos.v1.users import user_pb2
+from omni.pro.stack import ExitStackDocument
+from omni.pro.user.access import MicroService
 from omni.pro.validators import MicroServiceValidator
 
 logger = configure_logger(name=__name__)
 
 
 class LoadData(object):
     def __init__(self, base_app: Path):
@@ -40,27 +40,26 @@
                     context["user"] = response.user.username
                 else:
                     # TODO: Validate if user exists in database
                     context["user"] = user[0].get("username")
                 db_params = self.redis_manager.get_mongodb_config(Config.SERVICE_ID, tenant)
                 db_params["db"] = db_params.pop("name")
                 self.db_manager = DatabaseManager(**db_params)
-                with self.db_manager.get_connection():
-                    if not self.manifest:
-                        continue
-                    micro = self.load_manifest(context=context)
-                    self.load_data_micro(micro, context)
+                db_alias = f"{tenant}_{db_params['db']}"
+                if not self.manifest:
+                    continue
+                micro = self.load_manifest(context=context, db_alias=db_alias)
+                self.load_data_micro(micro, context, db_alias)
                 list_contexts.append(context)
         return list_contexts
 
     def create_user_admin(self, context, rc):
         values = self.load_data_dict(Path(__file__).parent / "data" / "models.user.csv")
-        user = UserStub()
-        response = user.create_users(context, values)
-        success = response.response_standard.status_code in range(200, 300)
+        user = UserChannel(context)
+        response, success = user.create_users(values)
         if success:
             rc.json().set(
                 context.get("tenant"), "$.user_admin", {"id": response.user.id, "username": response.user.username}
             )
         return response, success
 
     def _get_manifest_ms(self):
@@ -68,45 +67,48 @@
         if not file_name.exists():
             logger.warning(f"Manifest file not found {file_name}")
             return {}
         with open(file_name, "r") as f:
             data = f.read()
         return eval(data)
 
-    def load_manifest(self, context: dict):
-        tenant = context.get("tenant")
-        filters = {"code": self.manifest.get("code"), "tenant_code": tenant}
-        micro: MicroService = self.db_manager.get_document(
-            db_name=None, tenant=tenant, document_class=MicroService, **filters
-        )
-        self.manifest["tenant_code"] = tenant
-        data_validated = MicroServiceValidator(self.base_app, micro.data if micro else []).load(
-            self.manifest | {"context": context}
-        )
-        if not micro:
-            micro = self.db_manager.create_document(db_name=None, document_class=MicroService, **data_validated)
-        else:
-            micro.data = data_validated.get("data")
-            micro.save()
-        self.microservice = micro
-        return micro
+    def load_manifest(self, context: dict, db_alias: str):
+        with ExitStackDocument(MicroServiceDocument.reference_list(), db_alias=db_alias):
+            tenant = context.get("tenant")
+            filters = {"code": self.manifest.get("code"), "tenant_code": tenant}
+            micro: MicroServiceDocument = self.db_manager.get_document(
+                db_name=None, tenant=tenant, document_class=MicroServiceDocument, **filters
+            )
+            self.manifest["tenant_code"] = tenant
+            data_validated = MicroServiceValidator(self.base_app, micro.data if micro else []).load(
+                self.manifest | {"context": context}
+            )
+            if not micro:
+                micro = self.db_manager.create_document(
+                    db_name=None, document_class=MicroServiceDocument, **data_validated
+                )
+            else:
+                micro.data = data_validated.get("data")
+                micro.save()
+            self.microservice = micro
+            return micro
 
     def load_data_dict(self, name_file):
         try:
             with open(name_file, mode="r", encoding="utf-8-sig") as csv_file:
                 reader = csv.DictReader(csv_file, delimiter=";")
                 for row in reader:
                     yield row
                 return reader
         except FileNotFoundError as e:
             LoggerTraceback.error("File not found exception", e, logger)
         except Exception as e:
             LoggerTraceback.error("An unexpected error has occurred", e, logger)
 
-    def load_data_micro(self, micro: MicroService, context: dict):
+    def load_data_micro(self, micro: MicroServiceDocument, context: dict, db_alias):
         tenant = context.get("tenant")
         for idx, file in enumerate(micro.data):
             if file.get("load"):
                 continue
             name_file = self.base_app / file.get("path")
             reader = self.load_data_dict(name_file)
             models, file_py, model_str = file.get("path").split("/")[1].split(".")[:-1]
@@ -116,64 +118,61 @@
                 logger.error(f"File not found {ruta_modulo}")
                 continue
             modulo = util.load_file_module(ruta_modulo, model_str)
             if not hasattr(modulo, model_str):
                 logger.error(f"Class not found {model_str} in {ruta_modulo}")
                 continue
             load = False
-            for row in reader:
-                row = row | {"context": context}
-                self.db_manager.create_document(db_name=None, document_class=getattr(modulo, model_str), **row)
-                if not load:
-                    load = True
-            attr_data = {f"set__data__{idx}__load": load}
-            self.db_manager.update(micro, **attr_data)
-            if load:
-                logger.info(f"Load data {micro.code} - {tenant} - {file.get('path')}")
-
-
-class UserStub(object):
-    def __init__(self):
-        cloud_map = CloudMap(service_name=Config.SERVICE_NAME_BALANCER)
-        response = cloud_map.discover_instances()
-        self.port = None
-        self.host = None
-        for instance in response:
-            if instance.get("InstanceId") == Config.SAAS_MS_USER:
-                self.host = instance.get("Attributes").get("host")
-                self.port = instance.get("Attributes").get("port")
-                break
-
-    def create_users(self, context: dict, list_value: list) -> user_pb2.UserCreateResponse:
-        credentials = grpc.ssl_channel_credentials()
-        with grpc.secure_channel(
-            f"{self.host}:{self.port}",
-            credentials,
-            options=[("grpc.ssl_target_name_override", "omni.pro")],
-        ) as channel:
-            stub = user_pb2_grpc.UsersServiceStub(channel)
-            response = user_pb2.UserCreateResponse()
-            for value in list_value:
-                context["user"] = context.get("user") or value.get("username")
-                response = self._create_user(context, value, stub)
-                if response.response_standard.status_code in range(200, 300):
-                    logger.info(f"User created {response.user.username}")
-                else:
-                    logger.error(f"User not created {context.get('user')}")
-            return response
-
-    def _create_user(self, context: dict, value: dict, stub) -> user_pb2.UserCreateResponse:
-        user = user_pb2.UserCreateRequest(
-            **{
-                "context": context,
-                "email": value.get("email"),
-                "email_confirm": value.get("email"),
-                "language": {"code": "01", "code_name": "CO"},
-                "name": value.get("name"),
-                "password": value.get("password"),
-                "password_confirm": value.get("password"),
-                "timezone": {"code": "01", "code_name": "CO"},
-                "username": value.get("username"),
-                "is_superuser": wrappers_pb2.BoolValue(value=util.parse_bool(value.get("is_superuser") or False)),
-            }
+            with ExitStackDocument(
+                (doc_class := getattr(modulo, model_str)).reference_list() + MicroServiceDocument.reference_list(),
+                db_alias=db_alias,
+            ):
+                for row in reader:
+                    row = row | {"context": context}
+                    self.db_manager.create_document(db_name=None, document_class=doc_class, **row)
+                    if not load:
+                        load = True
+                attr_data = {f"set__data__{idx}__load": load}
+                self.db_manager.update(micro, **attr_data)
+                if load:
+                    logger.info(f"Load data {micro.code} - {tenant} - {file.get('path')}")
+
+
+class UserChannel(object):
+    def __init__(self, context: dict) -> None:
+        self.context = context
+        self.service_id = MicroService.SAAS_MS_USER.value
+        self.user_module_grpc = "v1.users.user_pb2_grpc"
+        self.user_stub_classname = "UsersServiceStub"
+        self.user_module_pb2 = "v1.users.user_pb2"
+
+        self.event = Event(
+            module_grpc=self.user_module_grpc,
+            stub_classname=self.user_stub_classname,
+            rpc_method="",
+            module_pb2=self.user_module_pb2,
+            request_class="",
+            params={},
         )
-        return stub.UserCreate(user)
+
+    def create_users(self, list_value):
+        response = user_pb2.UserCreateResponse(), False
+        for value in list_value:
+            self.context["user"] = self.context.get("user") or value.get("sub")
+            self.event.update(
+                rpc_method="UserCreate",
+                request_class="UserCreateRequest",
+                params={
+                    "context": self.context,
+                    "email": value.get("email"),
+                    "email_confirm": value.get("email"),
+                    "language": {"code": "01", "code_name": "CO"},
+                    "name": value.get("name"),
+                    "password": value.get("password"),
+                    "password_confirm": value.get("password"),
+                    "timezone": {"code": "01", "code_name": "CO"},
+                    "username": value.get("username"),
+                    "is_superuser": True,
+                },
+            )
+            response = GRPClient(service_id=self.service_id).call_rpc_fuction(self.event)
+        return response
```

### Comparing `omni-pro-0.1.27/omni/pro/logger.py` & `omni-pro-0.1.28/omni/pro/logger.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/base.py` & `omni-pro-0.1.28/omni/pro/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,19 @@
     active = BooleanField(default=True)
 
     meta = {
         "abstract": True,
         "strict": False,
     }
 
+    @classmethod
+    @property
+    def db(cls):
+        return cls._get_db()
+
     def save(self, *args, **kwargs):
         if not self.context:
             self.context = Context()
         if not self.audit:
             self.audit = Audit(created_by=self.context.user)
         self.audit.updated_by = self.context.user
         self.audit.updated_at = datetime.utcnow()
```

### Comparing `omni-pro-0.1.27/omni/pro/models/custom_fields/enum.py` & `omni-pro-0.1.28/omni/pro/models/custom_fields/enum.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/common/country.py` & `omni-pro-0.1.28/omni/pro/models/sql/common/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_category.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_category_category.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_category_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_locality.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_locality.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method_ref.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method_ref.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_method_warehouse.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_method_warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/delivery_schedule.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/delivery_schedule.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work_line.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/sql/rules/warehouse_hierarchy.py` & `omni-pro-0.1.28/omni/pro/models/sql/rules/warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/models/utilities/country.py` & `omni-pro-0.1.28/omni/pro/models/utilities/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/common/base_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/common/base_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/common/base_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/common/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/grpc_connector.py` & `omni-pro-0.1.28/omni/pro/protos/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/response.py` & `omni-pro-0.1.28/omni/pro/protos/response.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/family_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/family_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/catalogs/template_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/catalogs/template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/address_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/clients/client_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/clients/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17v1/rules/calendar.proto\x12"pro.omni.oms.api.v1.rules.calendar\x1a\x11\x63ommon/base.proto"u\n\x08\x43\x61lendar\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12?\n\x0cobject_audit\x18\x04 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"]\n\x15\x43\x61lendarCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61lendarCreateResponse\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43\x61lendarReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14\x43\x61lendarReadResponse\x12?\n\tcalendars\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15\x43\x61lendarUpdateRequest\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61lendarUpdateResponse\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43\x61lendarDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43\x61lendarDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43\x61lendarService\x12\x89\x01\n\x0e\x43\x61lendarCreate\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarCreateRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarCreateResponse"\x00\x12\x83\x01\n\x0c\x43\x61lendarRead\x12\x37.pro.omni.oms.api.v1.rules.calendar.CalendarReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.calendar.CalendarReadResponse"\x00\x12\x89\x01\n\x0e\x43\x61lendarUpdate\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarUpdateResponse"\x00\x12\x89\x01\n\x0e\x43\x61lendarDelete\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/rules/calendar.proto\x12"pro.omni.oms.api.v1.rules.calendar\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x91\x01\n\x08\x43\x61lendar\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12*\n\x06\x61\x63tive\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x04 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"]\n\x15\x43\x61lendarCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61lendarCreateResponse\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43\x61lendarReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14\x43\x61lendarReadResponse\x12?\n\tcalendars\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15\x43\x61lendarUpdateRequest\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61lendarUpdateResponse\x12>\n\x08\x63\x61lendar\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43\x61lendarDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43\x61lendarDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43\x61lendarService\x12\x89\x01\n\x0e\x43\x61lendarCreate\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarCreateRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarCreateResponse"\x00\x12\x83\x01\n\x0c\x43\x61lendarRead\x12\x37.pro.omni.oms.api.v1.rules.calendar.CalendarReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.calendar.CalendarReadResponse"\x00\x12\x89\x01\n\x0e\x43\x61lendarUpdate\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarUpdateResponse"\x00\x12\x89\x01\n\x0e\x43\x61lendarDelete\x12\x39.pro.omni.oms.api.v1.rules.calendar.CalendarDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.calendar.CalendarDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.calendar_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CALENDAR"]._serialized_start = 82
-    _globals["_CALENDAR"]._serialized_end = 199
-    _globals["_CALENDARCREATEREQUEST"]._serialized_start = 201
-    _globals["_CALENDARCREATEREQUEST"]._serialized_end = 294
-    _globals["_CALENDARCREATERESPONSE"]._serialized_start = 297
-    _globals["_CALENDARCREATERESPONSE"]._serialized_end = 460
-    _globals["_CALENDARREADREQUEST"]._serialized_start = 463
-    _globals["_CALENDARREADREQUEST"]._serialized_end = 832
-    _globals["_CALENDARREADRESPONSE"]._serialized_start = 835
-    _globals["_CALENDARREADRESPONSE"]._serialized_end = 1056
-    _globals["_CALENDARUPDATEREQUEST"]._serialized_start = 1059
-    _globals["_CALENDARUPDATEREQUEST"]._serialized_end = 1202
-    _globals["_CALENDARUPDATERESPONSE"]._serialized_start = 1205
-    _globals["_CALENDARUPDATERESPONSE"]._serialized_end = 1368
-    _globals["_CALENDARDELETEREQUEST"]._serialized_start = 1370
-    _globals["_CALENDARDELETEREQUEST"]._serialized_end = 1461
-    _globals["_CALENDARDELETERESPONSE"]._serialized_start = 1463
-    _globals["_CALENDARDELETERESPONSE"]._serialized_end = 1562
-    _globals["_CALENDARSERVICE"]._serialized_start = 1565
-    _globals["_CALENDARSERVICE"]._serialized_end = 2136
+    _globals["_CALENDAR"]._serialized_start = 115
+    _globals["_CALENDAR"]._serialized_end = 260
+    _globals["_CALENDARCREATEREQUEST"]._serialized_start = 262
+    _globals["_CALENDARCREATEREQUEST"]._serialized_end = 355
+    _globals["_CALENDARCREATERESPONSE"]._serialized_start = 358
+    _globals["_CALENDARCREATERESPONSE"]._serialized_end = 521
+    _globals["_CALENDARREADREQUEST"]._serialized_start = 524
+    _globals["_CALENDARREADREQUEST"]._serialized_end = 893
+    _globals["_CALENDARREADRESPONSE"]._serialized_start = 896
+    _globals["_CALENDARREADRESPONSE"]._serialized_end = 1117
+    _globals["_CALENDARUPDATEREQUEST"]._serialized_start = 1120
+    _globals["_CALENDARUPDATEREQUEST"]._serialized_end = 1263
+    _globals["_CALENDARUPDATERESPONSE"]._serialized_start = 1266
+    _globals["_CALENDARUPDATERESPONSE"]._serialized_end = 1429
+    _globals["_CALENDARDELETEREQUEST"]._serialized_start = 1431
+    _globals["_CALENDARDELETEREQUEST"]._serialized_end = 1522
+    _globals["_CALENDARDELETERESPONSE"]._serialized_start = 1524
+    _globals["_CALENDARDELETERESPONSE"]._serialized_end = 1623
+    _globals["_CALENDARSERVICE"]._serialized_start = 1626
+    _globals["_CALENDARSERVICE"]._serialized_end = 2197
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Calendar(_message.Message):
     __slots__ = ["id", "name", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class CalendarCreateRequest(_message.Message):
     __slots__ = ["name", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/calendar_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/calendar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17v1/rules/category.proto\x12"pro.omni.oms.api.v1.rules.category\x1a\x11\x63ommon/base.proto"\x9c\x01\n\x08\x43\x61tegory\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0f\x63\x61tegory_doc_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x84\x01\n\x15\x43\x61tegoryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0f\x63\x61tegory_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61tegoryCreateResponse\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43\x61tegoryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x14\x43\x61tegoryReadResponse\x12@\n\ncategories\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15\x43\x61tegoryUpdateRequest\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61tegoryUpdateResponse\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43\x61tegoryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43\x61tegoryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43\x61tegoryService\x12\x89\x01\n\x0e\x43\x61tegoryCreate\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryCreateRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryCreateResponse"\x00\x12\x83\x01\n\x0c\x43\x61tegoryRead\x12\x37.pro.omni.oms.api.v1.rules.category.CategoryReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.category.CategoryReadResponse"\x00\x12\x89\x01\n\x0e\x43\x61tegoryUpdate\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryUpdateResponse"\x00\x12\x89\x01\n\x0e\x43\x61tegoryDelete\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/rules/category.proto\x12"pro.omni.oms.api.v1.rules.category\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb9\x01\n\x08\x43\x61tegory\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x18\n\x10\x61ttribute_doc_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x85\x01\n\x15\x43\x61tegoryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x18\n\x10\x61ttribute_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61tegoryCreateResponse\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43\x61tegoryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x14\x43\x61tegoryReadResponse\x12@\n\ncategories\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15\x43\x61tegoryUpdateRequest\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43\x61tegoryUpdateResponse\x12>\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43\x61tegoryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43\x61tegoryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43\x61tegoryService\x12\x89\x01\n\x0e\x43\x61tegoryCreate\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryCreateRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryCreateResponse"\x00\x12\x83\x01\n\x0c\x43\x61tegoryRead\x12\x37.pro.omni.oms.api.v1.rules.category.CategoryReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.category.CategoryReadResponse"\x00\x12\x89\x01\n\x0e\x43\x61tegoryUpdate\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryUpdateResponse"\x00\x12\x89\x01\n\x0e\x43\x61tegoryDelete\x12\x39.pro.omni.oms.api.v1.rules.category.CategoryDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.category.CategoryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.category_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CATEGORY"]._serialized_start = 83
-    _globals["_CATEGORY"]._serialized_end = 239
-    _globals["_CATEGORYCREATEREQUEST"]._serialized_start = 242
-    _globals["_CATEGORYCREATEREQUEST"]._serialized_end = 374
-    _globals["_CATEGORYCREATERESPONSE"]._serialized_start = 377
-    _globals["_CATEGORYCREATERESPONSE"]._serialized_end = 540
-    _globals["_CATEGORYREADREQUEST"]._serialized_start = 543
-    _globals["_CATEGORYREADREQUEST"]._serialized_end = 912
-    _globals["_CATEGORYREADRESPONSE"]._serialized_start = 915
-    _globals["_CATEGORYREADRESPONSE"]._serialized_end = 1137
-    _globals["_CATEGORYUPDATEREQUEST"]._serialized_start = 1140
-    _globals["_CATEGORYUPDATEREQUEST"]._serialized_end = 1283
-    _globals["_CATEGORYUPDATERESPONSE"]._serialized_start = 1286
-    _globals["_CATEGORYUPDATERESPONSE"]._serialized_end = 1449
-    _globals["_CATEGORYDELETEREQUEST"]._serialized_start = 1451
-    _globals["_CATEGORYDELETEREQUEST"]._serialized_end = 1542
-    _globals["_CATEGORYDELETERESPONSE"]._serialized_start = 1544
-    _globals["_CATEGORYDELETERESPONSE"]._serialized_end = 1643
-    _globals["_CATEGORYSERVICE"]._serialized_start = 1646
-    _globals["_CATEGORYSERVICE"]._serialized_end = 2217
+    _globals["_CATEGORY"]._serialized_start = 115
+    _globals["_CATEGORY"]._serialized_end = 300
+    _globals["_CATEGORYCREATEREQUEST"]._serialized_start = 303
+    _globals["_CATEGORYCREATEREQUEST"]._serialized_end = 436
+    _globals["_CATEGORYCREATERESPONSE"]._serialized_start = 439
+    _globals["_CATEGORYCREATERESPONSE"]._serialized_end = 602
+    _globals["_CATEGORYREADREQUEST"]._serialized_start = 605
+    _globals["_CATEGORYREADREQUEST"]._serialized_end = 974
+    _globals["_CATEGORYREADRESPONSE"]._serialized_start = 977
+    _globals["_CATEGORYREADRESPONSE"]._serialized_end = 1199
+    _globals["_CATEGORYUPDATEREQUEST"]._serialized_start = 1202
+    _globals["_CATEGORYUPDATEREQUEST"]._serialized_end = 1345
+    _globals["_CATEGORYUPDATERESPONSE"]._serialized_start = 1348
+    _globals["_CATEGORYUPDATERESPONSE"]._serialized_end = 1511
+    _globals["_CATEGORYDELETEREQUEST"]._serialized_start = 1513
+    _globals["_CATEGORYDELETEREQUEST"]._serialized_end = 1604
+    _globals["_CATEGORYDELETERESPONSE"]._serialized_start = 1606
+    _globals["_CATEGORYDELETERESPONSE"]._serialized_end = 1705
+    _globals["_CATEGORYSERVICE"]._serialized_start = 1708
+    _globals["_CATEGORYSERVICE"]._serialized_end = 2279
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,58 +2,59 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Category(_message.Message):
-    __slots__ = ["id", "name", "code", "category_doc_id", "active", "object_audit"]
+    __slots__ = ["id", "name", "code", "attribute_doc_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CATEGORY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    ATTRIBUTE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    category_doc_id: str
-    active: bool
+    attribute_doc_id: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        category_doc_id: _Optional[str] = ...,
-        active: bool = ...,
+        attribute_doc_id: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class CategoryCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "category_doc_id", "context"]
+    __slots__ = ["name", "code", "attribute_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CATEGORY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    ATTRIBUTE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    category_doc_id: str
+    attribute_doc_id: str
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        category_doc_id: _Optional[str] = ...,
+        attribute_doc_id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class CategoryCreateResponse(_message.Message):
     __slots__ = ["category", "response_standard"]
     CATEGORY_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/category_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -7,63 +7,129 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryCategoryCategory(_message.Message):
-    __slots__ = ["id", "delivery_category_id", "category_id", "active", "object_audit"]
+class Order(_message.Message):
+    __slots__ = [
+        "id",
+        "name",
+        "sale_id",
+        "ship_address_id",
+        "delivery_method_id",
+        "carrier_id",
+        "payment_method_id",
+        "tax_total",
+        "subtotal",
+        "total",
+        "active",
+        "object_audit",
+    ]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_CATEGORY_ID_FIELD_NUMBER: _ClassVar[int]
-    CATEGORY_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    SALE_ID_FIELD_NUMBER: _ClassVar[int]
+    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
+    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
+    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    delivery_category_id: int
-    category_id: int
+    name: str
+    sale_id: int
+    ship_address_id: int
+    delivery_method_id: int
+    carrier_id: int
+    payment_method_id: int
+    tax_total: float
+    subtotal: float
+    total: float
     active: bool
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        delivery_category_id: _Optional[int] = ...,
-        category_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        sale_id: _Optional[int] = ...,
+        ship_address_id: _Optional[int] = ...,
+        delivery_method_id: _Optional[int] = ...,
+        carrier_id: _Optional[int] = ...,
+        payment_method_id: _Optional[int] = ...,
+        tax_total: _Optional[float] = ...,
+        subtotal: _Optional[float] = ...,
+        total: _Optional[float] = ...,
         active: bool = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryCreateRequest(_message.Message):
-    __slots__ = ["delivery_category_id", "category_id", "context"]
-    DELIVERY_CATEGORY_ID_FIELD_NUMBER: _ClassVar[int]
-    CATEGORY_ID_FIELD_NUMBER: _ClassVar[int]
+class OrderCreateRequest(_message.Message):
+    __slots__ = [
+        "name",
+        "sale_id",
+        "ship_address_id",
+        "delivery_method_id",
+        "carrier_id",
+        "payment_method_id",
+        "tax_total",
+        "subtotal",
+        "total",
+        "context",
+    ]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    SALE_ID_FIELD_NUMBER: _ClassVar[int]
+    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
+    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
+    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_category_id: int
-    category_id: int
+    name: str
+    sale_id: int
+    ship_address_id: int
+    delivery_method_id: int
+    carrier_id: int
+    payment_method_id: int
+    tax_total: float
+    subtotal: float
+    total: float
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_category_id: _Optional[int] = ...,
-        category_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        sale_id: _Optional[int] = ...,
+        ship_address_id: _Optional[int] = ...,
+        delivery_method_id: _Optional[int] = ...,
+        carrier_id: _Optional[int] = ...,
+        payment_method_id: _Optional[int] = ...,
+        tax_total: _Optional[float] = ...,
+        subtotal: _Optional[float] = ...,
+        total: _Optional[float] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryCreateResponse(_message.Message):
-    __slots__ = ["delivery_category_category", "response_standard"]
-    DELIVERY_CATEGORY_CATEGORY_FIELD_NUMBER: _ClassVar[int]
+class OrderCreateResponse(_message.Message):
+    __slots__ = ["order", "response_standard"]
+    ORDER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_category_category: DeliveryCategoryCategory
+    order: Order
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_category_category: _Optional[_Union[DeliveryCategoryCategory, _Mapping]] = ...,
+        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryReadRequest(_message.Message):
+class OrderReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -82,61 +148,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryReadResponse(_message.Message):
-    __slots__ = ["delivery_category_categories", "meta_data", "response_standard"]
-    DELIVERY_CATEGORY_CATEGORIES_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+class OrderReadResponse(_message.Message):
+    __slots__ = ["order", "response_standard", "meta_data"]
+    ORDER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_category_categories: _containers.RepeatedCompositeFieldContainer[DeliveryCategoryCategory]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    order: _containers.RepeatedCompositeFieldContainer[Order]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
     def __init__(
         self,
-        delivery_category_categories: _Optional[_Iterable[_Union[DeliveryCategoryCategory, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        order: _Optional[_Iterable[_Union[Order, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryUpdateRequest(_message.Message):
-    __slots__ = ["delivery_category_category", "context"]
-    DELIVERY_CATEGORY_CATEGORY_FIELD_NUMBER: _ClassVar[int]
+class OrderUpdateRequest(_message.Message):
+    __slots__ = ["order", "context"]
+    ORDER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_category_category: DeliveryCategoryCategory
+    order: Order
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_category_category: _Optional[_Union[DeliveryCategoryCategory, _Mapping]] = ...,
+        order: _Optional[_Union[Order, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryUpdateResponse(_message.Message):
-    __slots__ = ["delivery_category_category", "response_standard"]
-    DELIVERY_CATEGORY_CATEGORY_FIELD_NUMBER: _ClassVar[int]
+class OrderUpdateResponse(_message.Message):
+    __slots__ = ["order", "response_standard"]
+    ORDER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_category_category: DeliveryCategoryCategory
+    order: Order
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_category_category: _Optional[_Union[DeliveryCategoryCategory, _Mapping]] = ...,
+        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryCategoryCategoryDeleteRequest(_message.Message):
+class OrderDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryCategoryCategoryDeleteResponse(_message.Message):
+class OrderDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import category_pb2 as v1_dot_rules_dot_category__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n v1/rules/delivery_category.proto\x12+pro.omni.oms.api.v1.rules.delivery_category\x1a\x11\x63ommon/base.proto\x1a\x17v1/rules/category.proto"\xc1\x01\n\x10\x44\x65liveryCategory\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x42\n\x0c\x63\x61tegory_ids\x18\x03 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"{\n\x1d\x44\x65liveryCategoryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x63\x61tegory_ids\x18\x02 \x03(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryCategoryCreateResponse\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryCategoryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1c\x44\x65liveryCategoryReadResponse\x12Z\n\x13\x64\x65livery_categories\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryCategoryUpdateRequest\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryCategoryUpdateResponse\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryCategoryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryCategoryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryCategoryService\x12\xb3\x01\n\x16\x44\x65liveryCategoryCreate\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryCategoryRead\x12H.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryCategoryUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryCategoryDelete\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryDeleteResponse"\x00\x62\x06proto3'
+    b'\n v1/rules/delivery_category.proto\x12+pro.omni.oms.api.v1.rules.delivery_category\x1a\x11\x63ommon/base.proto\x1a\x17v1/rules/category.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xdb\x01\n\x10\x44\x65liveryCategory\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12@\n\ncategories\x18\x03 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.category.Category\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"{\n\x1d\x44\x65liveryCategoryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x63\x61tegory_ids\x18\x02 \x03(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryCategoryCreateResponse\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryCategoryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1c\x44\x65liveryCategoryReadResponse\x12Z\n\x13\x64\x65livery_categories\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryCategoryUpdateRequest\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryCategoryUpdateResponse\x12X\n\x11\x64\x65livery_category\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryCategoryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryCategoryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryCategoryService\x12\xb3\x01\n\x16\x44\x65liveryCategoryCreate\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryCategoryRead\x12H.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryCategoryUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryCategoryDelete\x12J.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategoryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_category_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYCATEGORY"]._serialized_start = 126
-    _globals["_DELIVERYCATEGORY"]._serialized_end = 319
-    _globals["_DELIVERYCATEGORYCREATEREQUEST"]._serialized_start = 321
-    _globals["_DELIVERYCATEGORYCREATEREQUEST"]._serialized_end = 444
-    _globals["_DELIVERYCATEGORYCREATERESPONSE"]._serialized_start = 447
-    _globals["_DELIVERYCATEGORYCREATERESPONSE"]._serialized_end = 644
-    _globals["_DELIVERYCATEGORYREADREQUEST"]._serialized_start = 647
-    _globals["_DELIVERYCATEGORYREADREQUEST"]._serialized_end = 1024
-    _globals["_DELIVERYCATEGORYREADRESPONSE"]._serialized_start = 1027
-    _globals["_DELIVERYCATEGORYREADRESPONSE"]._serialized_end = 1283
-    _globals["_DELIVERYCATEGORYUPDATEREQUEST"]._serialized_start = 1286
-    _globals["_DELIVERYCATEGORYUPDATEREQUEST"]._serialized_end = 1463
-    _globals["_DELIVERYCATEGORYUPDATERESPONSE"]._serialized_start = 1466
-    _globals["_DELIVERYCATEGORYUPDATERESPONSE"]._serialized_end = 1663
-    _globals["_DELIVERYCATEGORYDELETEREQUEST"]._serialized_start = 1665
-    _globals["_DELIVERYCATEGORYDELETEREQUEST"]._serialized_end = 1764
-    _globals["_DELIVERYCATEGORYDELETERESPONSE"]._serialized_start = 1766
-    _globals["_DELIVERYCATEGORYDELETERESPONSE"]._serialized_end = 1873
-    _globals["_DELIVERYCATEGORYSERVICE"]._serialized_start = 1876
-    _globals["_DELIVERYCATEGORYSERVICE"]._serialized_end = 2623
+    _globals["_DELIVERYCATEGORY"]._serialized_start = 158
+    _globals["_DELIVERYCATEGORY"]._serialized_end = 377
+    _globals["_DELIVERYCATEGORYCREATEREQUEST"]._serialized_start = 379
+    _globals["_DELIVERYCATEGORYCREATEREQUEST"]._serialized_end = 502
+    _globals["_DELIVERYCATEGORYCREATERESPONSE"]._serialized_start = 505
+    _globals["_DELIVERYCATEGORYCREATERESPONSE"]._serialized_end = 702
+    _globals["_DELIVERYCATEGORYREADREQUEST"]._serialized_start = 705
+    _globals["_DELIVERYCATEGORYREADREQUEST"]._serialized_end = 1082
+    _globals["_DELIVERYCATEGORYREADRESPONSE"]._serialized_start = 1085
+    _globals["_DELIVERYCATEGORYREADRESPONSE"]._serialized_end = 1341
+    _globals["_DELIVERYCATEGORYUPDATEREQUEST"]._serialized_start = 1344
+    _globals["_DELIVERYCATEGORYUPDATEREQUEST"]._serialized_end = 1521
+    _globals["_DELIVERYCATEGORYUPDATERESPONSE"]._serialized_start = 1524
+    _globals["_DELIVERYCATEGORYUPDATERESPONSE"]._serialized_end = 1721
+    _globals["_DELIVERYCATEGORYDELETEREQUEST"]._serialized_start = 1723
+    _globals["_DELIVERYCATEGORYDELETEREQUEST"]._serialized_end = 1822
+    _globals["_DELIVERYCATEGORYDELETERESPONSE"]._serialized_start = 1824
+    _globals["_DELIVERYCATEGORYDELETERESPONSE"]._serialized_end = 1931
+    _globals["_DELIVERYCATEGORYSERVICE"]._serialized_start = 1934
+    _globals["_DELIVERYCATEGORYSERVICE"]._serialized_end = 2681
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import category_pb2 as _category_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DeliveryCategory(_message.Message):
-    __slots__ = ["id", "name", "category_ids", "active", "object_audit"]
+    __slots__ = ["id", "name", "categories", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    CATEGORY_IDS_FIELD_NUMBER: _ClassVar[int]
+    CATEGORIES_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
-    category_ids: _containers.RepeatedCompositeFieldContainer[_category_pb2.Category]
-    active: bool
+    categories: _containers.RepeatedCompositeFieldContainer[_category_pb2.Category]
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        category_ids: _Optional[_Iterable[_Union[_category_pb2.Category, _Mapping]]] = ...,
-        active: bool = ...,
+        categories: _Optional[_Iterable[_Union[_category_pb2.Category, _Mapping]]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryCategoryCreateRequest(_message.Message):
     __slots__ = ["name", "category_ids", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CATEGORY_IDS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n.v1/rules/delivery_locality_matrix_values.proto\x12\x39pro.omni.oms.api.v1.rules.delivery_locality_matrix_values\x1a\x11\x63ommon/base.proto"\xbd\x01\n\x1c\x44\x65liveryLocalityMatrixValues\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1c\n\x14\x64\x65livery_locality_id\x18\x02 \x01(\x05\x12"\n\x1aterritory_matrix_values_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xa5\x01\n)DeliveryLocalityMatrixValuesCreateRequest\x12\x1c\n\x14\x64\x65livery_locality_id\x18\x01 \x01(\x05\x12"\n\x1aterritory_matrix_values_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfa\x01\n*DeliveryLocalityMatrixValuesCreateResponse\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x85\x03\n\'DeliveryLocalityMatrixValuesReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb4\x02\n(DeliveryLocalityMatrixValuesReadResponse\x12\x81\x01\n delivery_locality_matrix_valuess\x18\x01 \x03(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xe6\x01\n)DeliveryLocalityMatrixValuesUpdateRequest\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfa\x01\n*DeliveryLocalityMatrixValuesUpdateResponse\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"o\n)DeliveryLocalityMatrixValuesDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"w\n*DeliveryLocalityMatrixValuesDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf7\x07\n#DeliveryLocalityMatrixValuesService\x12\xf3\x01\n"DeliveryLocalityMatrixValuesCreate\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesCreateRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesCreateResponse"\x00\x12\xed\x01\n DeliveryLocalityMatrixValuesRead\x12\x62.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesReadRequest\x1a\x63.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesReadResponse"\x00\x12\xf3\x01\n"DeliveryLocalityMatrixValuesUpdate\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesUpdateRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesUpdateResponse"\x00\x12\xf3\x01\n"DeliveryLocalityMatrixValuesDelete\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesDeleteRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesDeleteResponse"\x00\x62\x06proto3'
+    b'\n.v1/rules/delivery_locality_matrix_values.proto\x12\x39pro.omni.oms.api.v1.rules.delivery_locality_matrix_values\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xd9\x01\n\x1c\x44\x65liveryLocalityMatrixValues\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1c\n\x14\x64\x65livery_locality_id\x18\x02 \x01(\x05\x12"\n\x1aterritory_matrix_values_id\x18\x03 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xa5\x01\n)DeliveryLocalityMatrixValuesCreateRequest\x12\x1c\n\x14\x64\x65livery_locality_id\x18\x01 \x01(\x05\x12"\n\x1aterritory_matrix_values_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfa\x01\n*DeliveryLocalityMatrixValuesCreateResponse\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x85\x03\n\'DeliveryLocalityMatrixValuesReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb4\x02\n(DeliveryLocalityMatrixValuesReadResponse\x12\x81\x01\n delivery_locality_matrix_valuess\x18\x01 \x03(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xe6\x01\n)DeliveryLocalityMatrixValuesUpdateRequest\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfa\x01\n*DeliveryLocalityMatrixValuesUpdateResponse\x12\x80\x01\n\x1f\x64\x65livery_locality_matrix_values\x18\x01 \x01(\x0b\x32W.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValues\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"o\n)DeliveryLocalityMatrixValuesDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"w\n*DeliveryLocalityMatrixValuesDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf7\x07\n#DeliveryLocalityMatrixValuesService\x12\xf3\x01\n"DeliveryLocalityMatrixValuesCreate\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesCreateRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesCreateResponse"\x00\x12\xed\x01\n DeliveryLocalityMatrixValuesRead\x12\x62.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesReadRequest\x1a\x63.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesReadResponse"\x00\x12\xf3\x01\n"DeliveryLocalityMatrixValuesUpdate\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesUpdateRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesUpdateResponse"\x00\x12\xf3\x01\n"DeliveryLocalityMatrixValuesDelete\x12\x64.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesDeleteRequest\x1a\x65.pro.omni.oms.api.v1.rules.delivery_locality_matrix_values.DeliveryLocalityMatrixValuesDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_locality_matrix_values_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYLOCALITYMATRIXVALUES"]._serialized_start = 129
-    _globals["_DELIVERYLOCALITYMATRIXVALUES"]._serialized_end = 318
-    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATEREQUEST"]._serialized_start = 321
-    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATEREQUEST"]._serialized_end = 486
-    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATERESPONSE"]._serialized_start = 489
-    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATERESPONSE"]._serialized_end = 739
-    _globals["_DELIVERYLOCALITYMATRIXVALUESREADREQUEST"]._serialized_start = 742
-    _globals["_DELIVERYLOCALITYMATRIXVALUESREADREQUEST"]._serialized_end = 1131
-    _globals["_DELIVERYLOCALITYMATRIXVALUESREADRESPONSE"]._serialized_start = 1134
-    _globals["_DELIVERYLOCALITYMATRIXVALUESREADRESPONSE"]._serialized_end = 1442
-    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATEREQUEST"]._serialized_start = 1445
-    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATEREQUEST"]._serialized_end = 1675
-    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATERESPONSE"]._serialized_start = 1678
-    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATERESPONSE"]._serialized_end = 1928
-    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETEREQUEST"]._serialized_start = 1930
-    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETEREQUEST"]._serialized_end = 2041
-    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETERESPONSE"]._serialized_start = 2043
-    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETERESPONSE"]._serialized_end = 2162
-    _globals["_DELIVERYLOCALITYMATRIXVALUESSERVICE"]._serialized_start = 2165
-    _globals["_DELIVERYLOCALITYMATRIXVALUESSERVICE"]._serialized_end = 3180
+    _globals["_DELIVERYLOCALITYMATRIXVALUES"]._serialized_start = 161
+    _globals["_DELIVERYLOCALITYMATRIXVALUES"]._serialized_end = 378
+    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATEREQUEST"]._serialized_start = 381
+    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATEREQUEST"]._serialized_end = 546
+    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATERESPONSE"]._serialized_start = 549
+    _globals["_DELIVERYLOCALITYMATRIXVALUESCREATERESPONSE"]._serialized_end = 799
+    _globals["_DELIVERYLOCALITYMATRIXVALUESREADREQUEST"]._serialized_start = 802
+    _globals["_DELIVERYLOCALITYMATRIXVALUESREADREQUEST"]._serialized_end = 1191
+    _globals["_DELIVERYLOCALITYMATRIXVALUESREADRESPONSE"]._serialized_start = 1194
+    _globals["_DELIVERYLOCALITYMATRIXVALUESREADRESPONSE"]._serialized_end = 1502
+    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATEREQUEST"]._serialized_start = 1505
+    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATEREQUEST"]._serialized_end = 1735
+    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATERESPONSE"]._serialized_start = 1738
+    _globals["_DELIVERYLOCALITYMATRIXVALUESUPDATERESPONSE"]._serialized_end = 1988
+    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETEREQUEST"]._serialized_start = 1990
+    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETEREQUEST"]._serialized_end = 2101
+    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETERESPONSE"]._serialized_start = 2103
+    _globals["_DELIVERYLOCALITYMATRIXVALUESDELETERESPONSE"]._serialized_end = 2222
+    _globals["_DELIVERYLOCALITYMATRIXVALUESSERVICE"]._serialized_start = 2225
+    _globals["_DELIVERYLOCALITYMATRIXVALUESSERVICE"]._serialized_end = 3240
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DeliveryLocalityMatrixValues(_message.Message):
     __slots__ = ["id", "delivery_locality_id", "territory_matrix_values_id", "active", "object_audit"]
@@ -17,22 +18,22 @@
     DELIVERY_LOCALITY_ID_FIELD_NUMBER: _ClassVar[int]
     TERRITORY_MATRIX_VALUES_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     delivery_locality_id: int
     territory_matrix_values_id: int
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         delivery_locality_id: _Optional[int] = ...,
         territory_matrix_values_id: _Optional[int] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryLocalityMatrixValuesCreateRequest(_message.Message):
     __slots__ = ["delivery_locality_id", "territory_matrix_values_id", "context"]
     DELIVERY_LOCALITY_ID_FIELD_NUMBER: _ClassVar[int]
     TERRITORY_MATRIX_VALUES_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n v1/rules/delivery_locality.proto\x12+pro.omni.oms.api.v1.rules.delivery_locality\x1a\x11\x63ommon/base.proto"\xd3\x01\n\x10\x44\x65liveryLocality\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\t\x12\x1b\n\x13territory_matrix_id\x18\x04 \x01(\t\x12#\n\x1bterritory_matrix_values_ids\x18\x05 \x03(\t\x12\x0e\n\x06\x61\x63tive\x18\x06 \x01(\x08\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x01\n\x1d\x44\x65liveryLocalityCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncountry_id\x18\x02 \x01(\t\x12\x1b\n\x13territory_matrix_id\x18\x03 \x01(\t\x12#\n\x1bterritory_matrix_values_ids\x18\x04 \x03(\t\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryLocalityCreateResponse\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryLocalityReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1c\x44\x65liveryLocalityReadResponse\x12Z\n\x13\x64\x65livery_localities\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryLocalityUpdateRequest\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryLocalityUpdateResponse\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryLocalityDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryLocalityDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryLocalityService\x12\xb3\x01\n\x16\x44\x65liveryLocalityCreate\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryLocalityRead\x12H.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryLocalityUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryLocalityDelete\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityDeleteResponse"\x00\x62\x06proto3'
+    b'\n v1/rules/delivery_locality.proto\x12+pro.omni.oms.api.v1.rules.delivery_locality\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xeb\x01\n\x10\x44\x65liveryLocality\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\t\x12\x1b\n\x13territory_matrix_id\x18\x04 \x01(\t\x12\x1f\n\x17territory_matrix_values\x18\x05 \x03(\t\x12*\n\x06\x61\x63tive\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x01\n\x1d\x44\x65liveryLocalityCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncountry_id\x18\x02 \x01(\t\x12\x1b\n\x13territory_matrix_id\x18\x03 \x01(\t\x12#\n\x1bterritory_matrix_values_ids\x18\x04 \x03(\t\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryLocalityCreateResponse\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryLocalityReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1c\x44\x65liveryLocalityReadResponse\x12Z\n\x13\x64\x65livery_localities\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryLocalityUpdateRequest\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryLocalityUpdateResponse\x12X\n\x11\x64\x65livery_locality\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryLocalityDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryLocalityDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryLocalityService\x12\xb3\x01\n\x16\x44\x65liveryLocalityCreate\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryLocalityRead\x12H.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryLocalityUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryLocalityDelete\x12J.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocalityDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_locality_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYLOCALITY"]._serialized_start = 101
-    _globals["_DELIVERYLOCALITY"]._serialized_end = 312
-    _globals["_DELIVERYLOCALITYCREATEREQUEST"]._serialized_start = 315
-    _globals["_DELIVERYLOCALITYCREATEREQUEST"]._serialized_end = 502
-    _globals["_DELIVERYLOCALITYCREATERESPONSE"]._serialized_start = 505
-    _globals["_DELIVERYLOCALITYCREATERESPONSE"]._serialized_end = 702
-    _globals["_DELIVERYLOCALITYREADREQUEST"]._serialized_start = 705
-    _globals["_DELIVERYLOCALITYREADREQUEST"]._serialized_end = 1082
-    _globals["_DELIVERYLOCALITYREADRESPONSE"]._serialized_start = 1085
-    _globals["_DELIVERYLOCALITYREADRESPONSE"]._serialized_end = 1341
-    _globals["_DELIVERYLOCALITYUPDATEREQUEST"]._serialized_start = 1344
-    _globals["_DELIVERYLOCALITYUPDATEREQUEST"]._serialized_end = 1521
-    _globals["_DELIVERYLOCALITYUPDATERESPONSE"]._serialized_start = 1524
-    _globals["_DELIVERYLOCALITYUPDATERESPONSE"]._serialized_end = 1721
-    _globals["_DELIVERYLOCALITYDELETEREQUEST"]._serialized_start = 1723
-    _globals["_DELIVERYLOCALITYDELETEREQUEST"]._serialized_end = 1822
-    _globals["_DELIVERYLOCALITYDELETERESPONSE"]._serialized_start = 1824
-    _globals["_DELIVERYLOCALITYDELETERESPONSE"]._serialized_end = 1931
-    _globals["_DELIVERYLOCALITYSERVICE"]._serialized_start = 1934
-    _globals["_DELIVERYLOCALITYSERVICE"]._serialized_end = 2681
+    _globals["_DELIVERYLOCALITY"]._serialized_start = 133
+    _globals["_DELIVERYLOCALITY"]._serialized_end = 368
+    _globals["_DELIVERYLOCALITYCREATEREQUEST"]._serialized_start = 371
+    _globals["_DELIVERYLOCALITYCREATEREQUEST"]._serialized_end = 558
+    _globals["_DELIVERYLOCALITYCREATERESPONSE"]._serialized_start = 561
+    _globals["_DELIVERYLOCALITYCREATERESPONSE"]._serialized_end = 758
+    _globals["_DELIVERYLOCALITYREADREQUEST"]._serialized_start = 761
+    _globals["_DELIVERYLOCALITYREADREQUEST"]._serialized_end = 1138
+    _globals["_DELIVERYLOCALITYREADRESPONSE"]._serialized_start = 1141
+    _globals["_DELIVERYLOCALITYREADRESPONSE"]._serialized_end = 1397
+    _globals["_DELIVERYLOCALITYUPDATEREQUEST"]._serialized_start = 1400
+    _globals["_DELIVERYLOCALITYUPDATEREQUEST"]._serialized_end = 1577
+    _globals["_DELIVERYLOCALITYUPDATERESPONSE"]._serialized_start = 1580
+    _globals["_DELIVERYLOCALITYUPDATERESPONSE"]._serialized_end = 1777
+    _globals["_DELIVERYLOCALITYDELETEREQUEST"]._serialized_start = 1779
+    _globals["_DELIVERYLOCALITYDELETEREQUEST"]._serialized_end = 1878
+    _globals["_DELIVERYLOCALITYDELETERESPONSE"]._serialized_start = 1880
+    _globals["_DELIVERYLOCALITYDELETERESPONSE"]._serialized_end = 1987
+    _globals["_DELIVERYLOCALITYSERVICE"]._serialized_start = 1990
+    _globals["_DELIVERYLOCALITYSERVICE"]._serialized_end = 2737
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,51 +2,44 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DeliveryLocality(_message.Message):
-    __slots__ = [
-        "id",
-        "name",
-        "country_id",
-        "territory_matrix_id",
-        "territory_matrix_values_ids",
-        "active",
-        "object_audit",
-    ]
+    __slots__ = ["id", "name", "country_id", "territory_matrix_id", "territory_matrix_values", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
     TERRITORY_MATRIX_ID_FIELD_NUMBER: _ClassVar[int]
-    TERRITORY_MATRIX_VALUES_IDS_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIX_VALUES_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     country_id: str
     territory_matrix_id: str
-    territory_matrix_values_ids: _containers.RepeatedScalarFieldContainer[str]
-    active: bool
+    territory_matrix_values: _containers.RepeatedScalarFieldContainer[str]
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         country_id: _Optional[str] = ...,
         territory_matrix_id: _Optional[str] = ...,
-        territory_matrix_values_ids: _Optional[_Iterable[str]] = ...,
-        active: bool = ...,
+        territory_matrix_values: _Optional[_Iterable[str]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryLocalityCreateRequest(_message.Message):
     __slots__ = ["name", "country_id", "territory_matrix_id", "territory_matrix_values_ids", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,51 +8,52 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import delivery_category_pb2 as v1_dot_rules_dot_delivery__category__pb2
 from omni.pro.protos.v1.rules import delivery_locality_pb2 as v1_dot_rules_dot_delivery__locality__pb2
-from omni.pro.protos.v1.rules import delivery_method_warehouse_pb2 as v1_dot_rules_dot_delivery__method__warehouse__pb2
 from omni.pro.protos.v1.rules import delivery_schedule_pb2 as v1_dot_rules_dot_delivery__schedule__pb2
+from omni.pro.protos.v1.rules import delivery_warehouse_pb2 as v1_dot_rules_dot_delivery__warehouse__pb2
 from omni.pro.protos.v1.rules import location_pb2 as v1_dot_rules_dot_location__pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1ev1/rules/delivery_method.proto\x12)pro.omni.oms.api.v1.rules.delivery_method\x1a\x11\x63ommon/base.proto\x1a\x18v1/rules/warehouse.proto\x1a\x17v1/rules/location.proto\x1a(v1/rules/delivery_method_warehouse.proto\x1a v1/rules/delivery_category.proto\x1a v1/rules/delivery_locality.proto\x1a v1/rules/delivery_schedule.proto"\xd6\x07\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12N\n\x16\x64\x65livery_warehouse_ids\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12]\n\x15type_picking_transfer\x18\x04 \x01(\x0e\x32>.pro.omni.oms.api.v1.rules.delivery_method.TypePickingTransfer\x12\x61\n\x17validate_warehouse_code\x18\x05 \x01(\x0e\x32@.pro.omni.oms.api.v1.rules.delivery_method.ValidateWarehouseCode\x12\x19\n\x11quantity_security\x18\x06 \x01(\x02\x12\x0c\n\x04\x63ode\x18\x07 \x01(\t\x12N\n\rtype_delivery\x18\x08 \x01(\x0e\x32\x37.pro.omni.oms.api.v1.rules.delivery_method.TypeDelivery\x12J\n\x14\x64\x65livery_location_id\x18\t \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12j\n\x14transfer_template_id\x18\n \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouse\x12[\n\x14\x63\x61tegory_template_id\x18\x0b \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\\\n\x15locality_available_id\x18\x0c \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12[\n\x14schedule_template_id\x18\r \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12\x0e\n\x06\x61\x63tive\x18\x0e \x01(\x08\x12?\n\x0cobject_audit\x18\x0f \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xd5\x04\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65livery_warehouse_ids\x18\x02 \x03(\t\x12]\n\x15type_picking_transfer\x18\x03 \x01(\x0e\x32>.pro.omni.oms.api.v1.rules.delivery_method.TypePickingTransfer\x12\x61\n\x17validate_warehouse_code\x18\x04 \x01(\x0e\x32@.pro.omni.oms.api.v1.rules.delivery_method.ValidateWarehouseCode\x12\x19\n\x11quantity_security\x18\x05 \x01(\x02\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12N\n\rtype_delivery\x18\x07 \x01(\x0e\x32\x37.pro.omni.oms.api.v1.rules.delivery_method.TypeDelivery\x12\x1c\n\x14\x64\x65livery_location_id\x18\x08 \x01(\t\x12\x1c\n\x14transfer_template_id\x18\t \x01(\t\x12\x1c\n\x14\x63\x61tegory_template_id\x18\n \x01(\t\x12\x1d\n\x15locality_available_id\x18\x0b \x01(\t\x12\x1c\n\x14schedule_template_id\x18\x0c \x01(\t\x12\x36\n\x07\x63ontext\x18\r \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*4\n\x13TypePickingTransfer\x12\x0b\n\x07PARTIAL\x10\x00\x12\x10\n\x0c\x43ONSOLIDATED\x10\x01*D\n\x15ValidateWarehouseCode\x12\x0c\n\x08OPTIONAL\x10\x00\x12\x0c\n\x08REQUIRED\x10\x01\x12\x0f\n\x0bUNNECESSARY\x10\x02*\'\n\x0cTypeDelivery\x12\t\n\x05STORE\x10\x00\x12\x0c\n\x08SHIPPING\x10\x01\x32\xc1\x05\n\x15\x44\x65liveryMethodService\x12\xa9\x01\n\x14\x44\x65liveryMethodCreate\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodCreateResponse"\x00\x12\xa3\x01\n\x12\x44\x65liveryMethodRead\x12\x44.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodReadResponse"\x00\x12\xa9\x01\n\x14\x44\x65liveryMethodUpdate\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodUpdateResponse"\x00\x12\xa9\x01\n\x14\x44\x65liveryMethodDelete\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1ev1/rules/delivery_method.proto\x12)pro.omni.oms.api.v1.rules.delivery_method\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18v1/rules/warehouse.proto\x1a\x17v1/rules/location.proto\x1a!v1/rules/delivery_warehouse.proto\x1a v1/rules/delivery_category.proto\x1a v1/rules/delivery_locality.proto\x1a v1/rules/delivery_schedule.proto"\xe2\x07\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12K\n\x13\x64\x65livery_warehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12]\n\x15type_picking_transfer\x18\x04 \x01(\x0e\x32>.pro.omni.oms.api.v1.rules.delivery_method.TypePickingTransfer\x12\x61\n\x17validate_warehouse_code\x18\x05 \x01(\x0e\x32@.pro.omni.oms.api.v1.rules.delivery_method.ValidateWarehouseCode\x12\x19\n\x11quantity_security\x18\x06 \x01(\x02\x12\x0c\n\x04\x63ode\x18\x07 \x01(\t\x12N\n\rtype_delivery\x18\x08 \x01(\x0e\x32\x37.pro.omni.oms.api.v1.rules.delivery_method.TypeDelivery\x12J\n\x14\x64\x65livery_location_id\x18\t \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12]\n\x14transfer_template_id\x18\n \x01(\x0b\x32?.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouse\x12[\n\x14\x63\x61tegory_template_id\x18\x0b \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_category.DeliveryCategory\x12\\\n\x15locality_available_id\x18\x0c \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_locality.DeliveryLocality\x12[\n\x14schedule_template_id\x18\r \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12*\n\x06\x61\x63tive\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0f \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xd5\x04\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16\x64\x65livery_warehouse_ids\x18\x02 \x03(\t\x12]\n\x15type_picking_transfer\x18\x03 \x01(\x0e\x32>.pro.omni.oms.api.v1.rules.delivery_method.TypePickingTransfer\x12\x61\n\x17validate_warehouse_code\x18\x04 \x01(\x0e\x32@.pro.omni.oms.api.v1.rules.delivery_method.ValidateWarehouseCode\x12\x19\n\x11quantity_security\x18\x05 \x01(\x02\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12N\n\rtype_delivery\x18\x07 \x01(\x0e\x32\x37.pro.omni.oms.api.v1.rules.delivery_method.TypeDelivery\x12\x1c\n\x14\x64\x65livery_location_id\x18\x08 \x01(\t\x12\x1c\n\x14transfer_template_id\x18\t \x01(\t\x12\x1c\n\x14\x63\x61tegory_template_id\x18\n \x01(\t\x12\x1d\n\x15locality_available_id\x18\x0b \x01(\t\x12\x1c\n\x14schedule_template_id\x18\x0c \x01(\t\x12\x36\n\x07\x63ontext\x18\r \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*4\n\x13TypePickingTransfer\x12\x0b\n\x07PARTIAL\x10\x00\x12\x10\n\x0c\x43ONSOLIDATED\x10\x01*D\n\x15ValidateWarehouseCode\x12\x0c\n\x08OPTIONAL\x10\x00\x12\x0c\n\x08REQUIRED\x10\x01\x12\x0f\n\x0bUNNECESSARY\x10\x02*\'\n\x0cTypeDelivery\x12\t\n\x05STORE\x10\x00\x12\x0c\n\x08SHIPPING\x10\x01\x32\xc1\x05\n\x15\x44\x65liveryMethodService\x12\xa9\x01\n\x14\x44\x65liveryMethodCreate\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodCreateResponse"\x00\x12\xa3\x01\n\x12\x44\x65liveryMethodRead\x12\x44.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodReadResponse"\x00\x12\xa9\x01\n\x14\x44\x65liveryMethodUpdate\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodUpdateResponse"\x00\x12\xa9\x01\n\x14\x44\x65liveryMethodDelete\x12\x46.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_method_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TYPEPICKINGTRANSFER"]._serialized_start = 3266
-    _globals["_TYPEPICKINGTRANSFER"]._serialized_end = 3318
-    _globals["_VALIDATEWAREHOUSECODE"]._serialized_start = 3320
-    _globals["_VALIDATEWAREHOUSECODE"]._serialized_end = 3388
-    _globals["_TYPEDELIVERY"]._serialized_start = 3390
-    _globals["_TYPEDELIVERY"]._serialized_end = 3429
-    _globals["_DELIVERYMETHOD"]._serialized_start = 292
-    _globals["_DELIVERYMETHOD"]._serialized_end = 1274
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 1277
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 1874
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 1877
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 2066
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 2069
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 2444
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 2447
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 2694
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 2697
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 2866
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 2869
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 3058
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 3060
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 3157
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 3159
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 3264
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 3432
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 4137
+    _globals["_TYPEPICKINGTRANSFER"]._serialized_start = 3303
+    _globals["_TYPEPICKINGTRANSFER"]._serialized_end = 3355
+    _globals["_VALIDATEWAREHOUSECODE"]._serialized_start = 3357
+    _globals["_VALIDATEWAREHOUSECODE"]._serialized_end = 3425
+    _globals["_TYPEDELIVERY"]._serialized_start = 3427
+    _globals["_TYPEDELIVERY"]._serialized_end = 3466
+    _globals["_DELIVERYMETHOD"]._serialized_start = 317
+    _globals["_DELIVERYMETHOD"]._serialized_end = 1311
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 1314
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 1911
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 1914
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 2103
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 2106
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 2481
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 2484
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 2731
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 2734
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 2903
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 2906
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 3095
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 3097
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 3194
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 3196
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 3301
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 3469
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 4174
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import delivery_category_pb2 as _delivery_category_pb2
 from omni.pro.protos.v1.rules import delivery_locality_pb2 as _delivery_locality_pb2
-from omni.pro.protos.v1.rules import delivery_method_warehouse_pb2 as _delivery_method_warehouse_pb2
 from omni.pro.protos.v1.rules import delivery_schedule_pb2 as _delivery_schedule_pb2
+from omni.pro.protos.v1.rules import delivery_warehouse_pb2 as _delivery_warehouse_pb2
 from omni.pro.protos.v1.rules import location_pb2 as _location_pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as _warehouse_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TypePickingTransfer(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
@@ -42,15 +43,15 @@
 STORE: TypeDelivery
 SHIPPING: TypeDelivery
 
 class DeliveryMethod(_message.Message):
     __slots__ = [
         "id",
         "name",
-        "delivery_warehouse_ids",
+        "delivery_warehouses",
         "type_picking_transfer",
         "validate_warehouse_code",
         "quantity_security",
         "code",
         "type_delivery",
         "delivery_location_id",
         "transfer_template_id",
@@ -58,58 +59,58 @@
         "locality_available_id",
         "schedule_template_id",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
+    DELIVERY_WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
     TYPE_PICKING_TRANSFER_FIELD_NUMBER: _ClassVar[int]
     VALIDATE_WAREHOUSE_CODE_FIELD_NUMBER: _ClassVar[int]
     QUANTITY_SECURITY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     TYPE_DELIVERY_FIELD_NUMBER: _ClassVar[int]
     DELIVERY_LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
     TRANSFER_TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
     CATEGORY_TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
     LOCALITY_AVAILABLE_ID_FIELD_NUMBER: _ClassVar[int]
     SCHEDULE_TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
-    delivery_warehouse_ids: _containers.RepeatedCompositeFieldContainer[_warehouse_pb2.Warehouse]
+    delivery_warehouses: _containers.RepeatedCompositeFieldContainer[_warehouse_pb2.Warehouse]
     type_picking_transfer: TypePickingTransfer
     validate_warehouse_code: ValidateWarehouseCode
     quantity_security: float
     code: str
     type_delivery: TypeDelivery
     delivery_location_id: _location_pb2.Location
-    transfer_template_id: _delivery_method_warehouse_pb2.DeliveryMethodWarehouse
+    transfer_template_id: _delivery_warehouse_pb2.DeliveryWarehouse
     category_template_id: _delivery_category_pb2.DeliveryCategory
     locality_available_id: _delivery_locality_pb2.DeliveryLocality
     schedule_template_id: _delivery_schedule_pb2.DeliverySchedule
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        delivery_warehouse_ids: _Optional[_Iterable[_Union[_warehouse_pb2.Warehouse, _Mapping]]] = ...,
+        delivery_warehouses: _Optional[_Iterable[_Union[_warehouse_pb2.Warehouse, _Mapping]]] = ...,
         type_picking_transfer: _Optional[_Union[TypePickingTransfer, str]] = ...,
         validate_warehouse_code: _Optional[_Union[ValidateWarehouseCode, str]] = ...,
         quantity_security: _Optional[float] = ...,
         code: _Optional[str] = ...,
         type_delivery: _Optional[_Union[TypeDelivery, str]] = ...,
         delivery_location_id: _Optional[_Union[_location_pb2.Location, _Mapping]] = ...,
-        transfer_template_id: _Optional[_Union[_delivery_method_warehouse_pb2.DeliveryMethodWarehouse, _Mapping]] = ...,
+        transfer_template_id: _Optional[_Union[_delivery_warehouse_pb2.DeliveryWarehouse, _Mapping]] = ...,
         category_template_id: _Optional[_Union[_delivery_category_pb2.DeliveryCategory, _Mapping]] = ...,
         locality_available_id: _Optional[_Union[_delivery_locality_pb2.DeliveryLocality, _Mapping]] = ...,
         schedule_template_id: _Optional[_Union[_delivery_schedule_pb2.DeliverySchedule, _Mapping]] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryMethodCreateRequest(_message.Message):
     __slots__ = [
         "name",
         "delivery_warehouse_ids",
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_method_warehouse_hierarchy.proto
+# source: v1/rules/warehouse_hierarchy.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
+from omni.pro.protos.v1.rules import location_pb2 as v1_dot_rules_dot_location__pb2
+from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n2v1/rules/delivery_method_warehouse_hierarchy.proto\x12=pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy\x1a\x11\x63ommon/base.proto"\xc5\x01\n DeliveryMethodWarehouseHierarchy\x12\n\n\x02id\x18\x01 \x01(\x05\x12$\n\x1c\x64\x65livery_method_warehouse_id\x18\x02 \x01(\x05\x12\x1e\n\x16warehouse_hierarchy_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n-DeliveryMethodWarehouseHierarchyCreateRequest\x12$\n\x1c\x64\x65livery_method_warehouse_id\x18\x01 \x01(\x05\x12\x1e\n\x16warehouse_hierarchy_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8a\x02\n.DeliveryMethodWarehouseHierarchyCreateResponse\x12\x8c\x01\n#delivery_method_warehouse_hierarchy\x18\x01 \x01(\x0b\x32_.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x89\x03\n+DeliveryMethodWarehouseHierarchyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc4\x02\n,DeliveryMethodWarehouseHierarchyReadResponse\x12\x8d\x01\n$delivery_method_warehouse_hierarchys\x18\x01 \x03(\x0b\x32_.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchy\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf6\x01\n-DeliveryMethodWarehouseHierarchyUpdateRequest\x12\x8c\x01\n#delivery_method_warehouse_hierarchy\x18\x01 \x01(\x0b\x32_.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchy\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8a\x02\n.DeliveryMethodWarehouseHierarchyUpdateResponse\x12\x8c\x01\n#delivery_method_warehouse_hierarchy\x18\x01 \x01(\x0b\x32_.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"s\n-DeliveryMethodWarehouseHierarchyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"{\n.DeliveryMethodWarehouseHierarchyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xcb\x08\n\'DeliveryMethodWarehouseHierarchyService\x12\x87\x02\n&DeliveryMethodWarehouseHierarchyCreate\x12l.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyCreateRequest\x1am.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyCreateResponse"\x00\x12\x81\x02\n$DeliveryMethodWarehouseHierarchyRead\x12j.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyReadRequest\x1ak.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyReadResponse"\x00\x12\x87\x02\n&DeliveryMethodWarehouseHierarchyUpdate\x12l.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyUpdateRequest\x1am.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyUpdateResponse"\x00\x12\x87\x02\n&DeliveryMethodWarehouseHierarchyDelete\x12l.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyDeleteRequest\x1am.pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyDeleteResponse"\x00\x62\x06proto3'
+    b'\n"v1/rules/warehouse_hierarchy.proto\x12-pro.omni.oms.api.v1.rules.warehouse_hierarchy\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x18v1/rules/warehouse.proto\x1a\x17v1/rules/location.proto"\xf7\x02\n\x12WarehouseHierarchy\x12\n\n\x02id\x18\x01 \x01(\t\x12\x44\n\x0cwarehouse_id\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x41\n\x0blocation_id\x18\t \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x19\n\x11quantity_security\x18\x04 \x01(\x02\x12\x10\n\x08sequence\x18\x05 \x01(\x05\x12\x32\n\x0esequence_order\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12*\n\x06\x61\x63tive\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe5\x01\n\x1fWarehouseHierarchyCreateRequest\x12\x14\n\x0cwarehouse_id\x18\x01 \x01(\t\x12\x13\n\x0blocation_id\x18\x02 \x01(\t\x12\x19\n\x11quantity_security\x18\x03 \x01(\x02\x12\x10\n\x08sequence\x18\x04 \x01(\x05\x12\x32\n\x0esequence_order\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n WarehouseHierarchyCreateResponse\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfb\x02\n\x1dWarehouseHierarchyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x87\x02\n\x1eWarehouseHierarchyReadResponse\x12_\n\x14warehouses_hierarchy\x18\x01 \x03(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb9\x01\n\x1fWarehouseHierarchyUpdateRequest\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n WarehouseHierarchyUpdateResponse\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"e\n\x1fWarehouseHierarchyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"m\n WarehouseHierarchyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x95\x06\n\x19WarehouseHierarchyService\x12\xbd\x01\n\x18WarehouseHierarchyCreate\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyCreateRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyCreateResponse"\x00\x12\xb7\x01\n\x16WarehouseHierarchyRead\x12L.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyReadRequest\x1aM.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyReadResponse"\x00\x12\xbd\x01\n\x18WarehouseHierarchyUpdate\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyUpdateRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyUpdateResponse"\x00\x12\xbd\x01\n\x18WarehouseHierarchyDelete\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyDeleteRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_method_warehouse_hierarchy_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.warehouse_hierarchy_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHY"]._serialized_start = 137
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHY"]._serialized_end = 334
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_start = 337
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_end = 510
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_start = 513
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_end = 779
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYREADREQUEST"]._serialized_start = 782
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYREADREQUEST"]._serialized_end = 1175
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYREADRESPONSE"]._serialized_start = 1178
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYREADRESPONSE"]._serialized_end = 1502
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_start = 1505
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_end = 1751
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_start = 1754
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_end = 2020
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_start = 2022
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_end = 2137
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_start = 2139
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_end = 2262
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYSERVICE"]._serialized_start = 2265
-    _globals["_DELIVERYMETHODWAREHOUSEHIERARCHYSERVICE"]._serialized_end = 3364
+    _globals["_WAREHOUSEHIERARCHY"]._serialized_start = 188
+    _globals["_WAREHOUSEHIERARCHY"]._serialized_end = 563
+    _globals["_WAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_start = 566
+    _globals["_WAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_end = 795
+    _globals["_WAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_start = 798
+    _globals["_WAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_end = 1003
+    _globals["_WAREHOUSEHIERARCHYREADREQUEST"]._serialized_start = 1006
+    _globals["_WAREHOUSEHIERARCHYREADREQUEST"]._serialized_end = 1385
+    _globals["_WAREHOUSEHIERARCHYREADRESPONSE"]._serialized_start = 1388
+    _globals["_WAREHOUSEHIERARCHYREADRESPONSE"]._serialized_end = 1651
+    _globals["_WAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_start = 1654
+    _globals["_WAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_end = 1839
+    _globals["_WAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_start = 1842
+    _globals["_WAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_end = 2047
+    _globals["_WAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_start = 2049
+    _globals["_WAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_end = 2150
+    _globals["_WAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_start = 2152
+    _globals["_WAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_end = 2261
+    _globals["_WAREHOUSEHIERARCHYSERVICE"]._serialized_start = 2264
+    _globals["_WAREHOUSEHIERARCHYSERVICE"]._serialized_end = 3053
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,143 +2,171 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
+from omni.pro.protos.v1.rules import location_pb2 as _location_pb2
+from omni.pro.protos.v1.rules import warehouse_pb2 as _warehouse_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryMethodWarehouseHierarchy(_message.Message):
-    __slots__ = ["id", "delivery_method_warehouse_id", "warehouse_hierarchy_id", "active", "object_audit"]
+class WarehouseHierarchy(_message.Message):
+    __slots__ = [
+        "id",
+        "warehouse_id",
+        "location_id",
+        "quantity_security",
+        "sequence",
+        "sequence_order",
+        "active",
+        "object_audit",
+    ]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_HIERARCHY_ID_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
+    QUANTITY_SECURITY_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_ORDER_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    delivery_method_warehouse_id: int
-    warehouse_hierarchy_id: int
-    active: bool
+    id: str
+    warehouse_id: _warehouse_pb2.Warehouse
+    location_id: _location_pb2.Location
+    quantity_security: float
+    sequence: int
+    sequence_order: _wrappers_pb2.BoolValue
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        delivery_method_warehouse_id: _Optional[int] = ...,
-        warehouse_hierarchy_id: _Optional[int] = ...,
-        active: bool = ...,
+        id: _Optional[str] = ...,
+        warehouse_id: _Optional[_Union[_warehouse_pb2.Warehouse, _Mapping]] = ...,
+        location_id: _Optional[_Union[_location_pb2.Location, _Mapping]] = ...,
+        quantity_security: _Optional[float] = ...,
+        sequence: _Optional[int] = ...,
+        sequence_order: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyCreateRequest(_message.Message):
-    __slots__ = ["delivery_method_warehouse_id", "warehouse_hierarchy_id", "context"]
-    DELIVERY_METHOD_WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_HIERARCHY_ID_FIELD_NUMBER: _ClassVar[int]
+class WarehouseHierarchyCreateRequest(_message.Message):
+    __slots__ = ["warehouse_id", "location_id", "quantity_security", "sequence", "sequence_order", "context"]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
+    QUANTITY_SECURITY_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_ORDER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse_id: int
-    warehouse_hierarchy_id: int
+    warehouse_id: str
+    location_id: str
+    quantity_security: float
+    sequence: int
+    sequence_order: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_method_warehouse_id: _Optional[int] = ...,
-        warehouse_hierarchy_id: _Optional[int] = ...,
+        warehouse_id: _Optional[str] = ...,
+        location_id: _Optional[str] = ...,
+        quantity_security: _Optional[float] = ...,
+        sequence: _Optional[int] = ...,
+        sequence_order: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyCreateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse_hierarchy", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class WarehouseHierarchyCreateResponse(_message.Message):
+    __slots__ = ["warehouse_hierarchy", "response_standard"]
+    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse_hierarchy: DeliveryMethodWarehouseHierarchy
+    warehouse_hierarchy: WarehouseHierarchy
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse_hierarchy: _Optional[_Union[DeliveryMethodWarehouseHierarchy, _Mapping]] = ...,
+        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyReadRequest(_message.Message):
+class WarehouseHierarchyReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyReadResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse_hierarchys", "meta_data", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_HIERARCHYS_FIELD_NUMBER: _ClassVar[int]
+class WarehouseHierarchyReadResponse(_message.Message):
+    __slots__ = ["warehouses_hierarchy", "meta_data", "response_standard"]
+    WAREHOUSES_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse_hierarchys: _containers.RepeatedCompositeFieldContainer[DeliveryMethodWarehouseHierarchy]
+    warehouses_hierarchy: _containers.RepeatedCompositeFieldContainer[WarehouseHierarchy]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse_hierarchys: _Optional[
-            _Iterable[_Union[DeliveryMethodWarehouseHierarchy, _Mapping]]
-        ] = ...,
+        warehouses_hierarchy: _Optional[_Iterable[_Union[WarehouseHierarchy, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyUpdateRequest(_message.Message):
-    __slots__ = ["delivery_method_warehouse_hierarchy", "context"]
-    DELIVERY_METHOD_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class WarehouseHierarchyUpdateRequest(_message.Message):
+    __slots__ = ["warehouse_hierarchy", "context"]
+    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse_hierarchy: DeliveryMethodWarehouseHierarchy
+    warehouse_hierarchy: WarehouseHierarchy
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_method_warehouse_hierarchy: _Optional[_Union[DeliveryMethodWarehouseHierarchy, _Mapping]] = ...,
+        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyUpdateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse_hierarchy", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class WarehouseHierarchyUpdateResponse(_message.Message):
+    __slots__ = ["warehouse_hierarchy", "response_standard"]
+    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse_hierarchy: DeliveryMethodWarehouseHierarchy
+    warehouse_hierarchy: WarehouseHierarchy
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse_hierarchy: _Optional[_Union[DeliveryMethodWarehouseHierarchy, _Mapping]] = ...,
+        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyDeleteRequest(_message.Message):
+class WarehouseHierarchyDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryMethodWarehouseHierarchyDeleteResponse(_message.Message):
+class WarehouseHierarchyDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,214 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.rules import (
-    delivery_method_warehouse_hierarchy_pb2 as v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2,
-)
+from omni.pro.protos.v1.rules import delivery_time_warehouse_pb2 as v1_dot_rules_dot_delivery__time__warehouse__pb2
 
 
-class DeliveryMethodWarehouseHierarchyServiceStub(object):
+class DeliveryTimeWarehouseServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.DeliveryMethodWarehouseHierarchyCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyCreate",
-            request_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateResponse.FromString,
+        self.DeliveryTimeWarehouseCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseCreate",
+            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.FromString,
         )
-        self.DeliveryMethodWarehouseHierarchyRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyRead",
-            request_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadResponse.FromString,
+        self.DeliveryTimeWarehouseRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseRead",
+            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.FromString,
         )
-        self.DeliveryMethodWarehouseHierarchyUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyUpdate",
-            request_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateResponse.FromString,
+        self.DeliveryTimeWarehouseUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseUpdate",
+            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.FromString,
         )
-        self.DeliveryMethodWarehouseHierarchyDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyDelete",
-            request_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteResponse.FromString,
+        self.DeliveryTimeWarehouseDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseDelete",
+            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.FromString,
         )
 
 
-class DeliveryMethodWarehouseHierarchyServiceServicer(object):
+class DeliveryTimeWarehouseServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def DeliveryMethodWarehouseHierarchyCreate(self, request, context):
+    def DeliveryTimeWarehouseCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryMethodWarehouseHierarchyRead(self, request, context):
+    def DeliveryTimeWarehouseRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryMethodWarehouseHierarchyUpdate(self, request, context):
+    def DeliveryTimeWarehouseUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryMethodWarehouseHierarchyDelete(self, request, context):
+    def DeliveryTimeWarehouseDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_DeliveryMethodWarehouseHierarchyServiceServicer_to_server(servicer, server):
+def add_DeliveryTimeWarehouseServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "DeliveryMethodWarehouseHierarchyCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryMethodWarehouseHierarchyCreate,
-            request_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateResponse.SerializeToString,
+        "DeliveryTimeWarehouseCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryTimeWarehouseCreate,
+            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.SerializeToString,
         ),
-        "DeliveryMethodWarehouseHierarchyRead": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryMethodWarehouseHierarchyRead,
-            request_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadResponse.SerializeToString,
+        "DeliveryTimeWarehouseRead": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryTimeWarehouseRead,
+            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.SerializeToString,
         ),
-        "DeliveryMethodWarehouseHierarchyUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryMethodWarehouseHierarchyUpdate,
-            request_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateResponse.SerializeToString,
+        "DeliveryTimeWarehouseUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryTimeWarehouseUpdate,
+            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.SerializeToString,
         ),
-        "DeliveryMethodWarehouseHierarchyDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryMethodWarehouseHierarchyDelete,
-            request_deserializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteResponse.SerializeToString,
+        "DeliveryTimeWarehouseDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryTimeWarehouseDelete,
+            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService",
-        rpc_method_handlers,
+        "pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class DeliveryMethodWarehouseHierarchyService(object):
+class DeliveryTimeWarehouseService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def DeliveryMethodWarehouseHierarchyCreate(
+    def DeliveryTimeWarehouseCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyCreate",
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseCreate",
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryMethodWarehouseHierarchyRead(
+    def DeliveryTimeWarehouseRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyRead",
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyReadResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseRead",
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryMethodWarehouseHierarchyUpdate(
+    def DeliveryTimeWarehouseUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyUpdate",
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseUpdate",
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryMethodWarehouseHierarchyDelete(
+    def DeliveryTimeWarehouseDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse_hierarchy.DeliveryMethodWarehouseHierarchyService/DeliveryMethodWarehouseHierarchyDelete",
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__method__warehouse__hierarchy__pb2.DeliveryMethodWarehouseHierarchyDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseDelete",
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_method_warehouse.proto
+# source: v1/rules/delivery_price_warehouse.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
-from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as v1_dot_rules_dot_warehouse__hierarchy__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n(v1/rules/delivery_method_warehouse.proto\x12\x33pro.omni.oms.api.v1.rules.delivery_method_warehouse\x1a\x11\x63ommon/base.proto\x1a"v1/rules/warehouse_hierarchy.proto"\xc9\x02\n\x17\x44\x65liveryMethodWarehouse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12`\n\x1bhierarchi_warehouse_sort_by\x18\x03 \x01(\x0e\x32;.pro.omni.oms.api.v1.rules.delivery_method_warehouse.SortBy\x12\x61\n\x16transfer_warehouse_ids\x18\x04 \x03(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xee\x01\n$DeliveryMethodWarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16transfer_warehouse_ids\x18\x02 \x03(\t\x12`\n\x1bhierarchi_warehouse_sort_by\x18\x03 \x01(\x0e\x32;.pro.omni.oms.api.v1.rules.delivery_method_warehouse.SortBy\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n%DeliveryMethodWarehouseCreateResponse\x12o\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x80\x03\n"DeliveryMethodWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9d\x02\n#DeliveryMethodWarehouseReadResponse\x12p\n\x1a\x64\x65livery_method_warehouses\x18\x01 \x03(\x0b\x32L.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xcf\x01\n$DeliveryMethodWarehouseUpdateRequest\x12o\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n%DeliveryMethodWarehouseUpdateResponse\x12o\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"j\n$DeliveryMethodWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"r\n%DeliveryMethodWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*\x1b\n\x06SortBy\x12\x07\n\x03\x41SC\x10\x00\x12\x08\n\x04\x44\x45SC\x10\x01\x32\x86\x07\n\x1e\x44\x65liveryMethodWarehouseService\x12\xd8\x01\n\x1d\x44\x65liveryMethodWarehouseCreate\x12Y.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseCreateRequest\x1aZ.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseCreateResponse"\x00\x12\xd2\x01\n\x1b\x44\x65liveryMethodWarehouseRead\x12W.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseReadRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseReadResponse"\x00\x12\xd8\x01\n\x1d\x44\x65liveryMethodWarehouseUpdate\x12Y.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseUpdateRequest\x1aZ.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseUpdateResponse"\x00\x12\xd8\x01\n\x1d\x44\x65liveryMethodWarehouseDelete\x12Y.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseDeleteRequest\x1aZ.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryMethodWarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n\'v1/rules/delivery_price_warehouse.proto\x12\x32pro.omni.oms.api.v1.rules.delivery_price_warehouse\x1a\x11\x63ommon/base.proto"\xa6\x01\n\x16\x44\x65liveryPriceWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x19\n\x11\x64\x65livery_price_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8e\x01\n#DeliveryPriceWarehouseCreateRequest\x12\x19\n\x11\x64\x65livery_price_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdf\x01\n$DeliveryPriceWarehouseCreateResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xff\x02\n!DeliveryPriceWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x98\x02\n"DeliveryPriceWarehouseReadResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x03(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xcb\x01\n#DeliveryPriceWarehouseUpdateRequest\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdf\x01\n$DeliveryPriceWarehouseUpdateResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"i\n#DeliveryPriceWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"q\n$DeliveryPriceWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf1\x06\n\x1d\x44\x65liveryPriceWarehouseService\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseCreate\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseCreateRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseCreateResponse"\x00\x12\xcd\x01\n\x1a\x44\x65liveryPriceWarehouseRead\x12U.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseReadRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseReadResponse"\x00\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseUpdate\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseUpdateRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseUpdateResponse"\x00\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseDelete\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseDeleteRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_method_warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_price_warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_SORTBY"]._serialized_start = 2294
-    _globals["_SORTBY"]._serialized_end = 2321
-    _globals["_DELIVERYMETHODWAREHOUSE"]._serialized_start = 153
-    _globals["_DELIVERYMETHODWAREHOUSE"]._serialized_end = 482
-    _globals["_DELIVERYMETHODWAREHOUSECREATEREQUEST"]._serialized_start = 485
-    _globals["_DELIVERYMETHODWAREHOUSECREATEREQUEST"]._serialized_end = 723
-    _globals["_DELIVERYMETHODWAREHOUSECREATERESPONSE"]._serialized_start = 726
-    _globals["_DELIVERYMETHODWAREHOUSECREATERESPONSE"]._serialized_end = 953
-    _globals["_DELIVERYMETHODWAREHOUSEREADREQUEST"]._serialized_start = 956
-    _globals["_DELIVERYMETHODWAREHOUSEREADREQUEST"]._serialized_end = 1340
-    _globals["_DELIVERYMETHODWAREHOUSEREADRESPONSE"]._serialized_start = 1343
-    _globals["_DELIVERYMETHODWAREHOUSEREADRESPONSE"]._serialized_end = 1628
-    _globals["_DELIVERYMETHODWAREHOUSEUPDATEREQUEST"]._serialized_start = 1631
-    _globals["_DELIVERYMETHODWAREHOUSEUPDATEREQUEST"]._serialized_end = 1838
-    _globals["_DELIVERYMETHODWAREHOUSEUPDATERESPONSE"]._serialized_start = 1841
-    _globals["_DELIVERYMETHODWAREHOUSEUPDATERESPONSE"]._serialized_end = 2068
-    _globals["_DELIVERYMETHODWAREHOUSEDELETEREQUEST"]._serialized_start = 2070
-    _globals["_DELIVERYMETHODWAREHOUSEDELETEREQUEST"]._serialized_end = 2176
-    _globals["_DELIVERYMETHODWAREHOUSEDELETERESPONSE"]._serialized_start = 2178
-    _globals["_DELIVERYMETHODWAREHOUSEDELETERESPONSE"]._serialized_end = 2292
-    _globals["_DELIVERYMETHODWAREHOUSESERVICE"]._serialized_start = 2324
-    _globals["_DELIVERYMETHODWAREHOUSESERVICE"]._serialized_end = 3226
+    _globals["_DELIVERYPRICEWAREHOUSE"]._serialized_start = 115
+    _globals["_DELIVERYPRICEWAREHOUSE"]._serialized_end = 281
+    _globals["_DELIVERYPRICEWAREHOUSECREATEREQUEST"]._serialized_start = 284
+    _globals["_DELIVERYPRICEWAREHOUSECREATEREQUEST"]._serialized_end = 426
+    _globals["_DELIVERYPRICEWAREHOUSECREATERESPONSE"]._serialized_start = 429
+    _globals["_DELIVERYPRICEWAREHOUSECREATERESPONSE"]._serialized_end = 652
+    _globals["_DELIVERYPRICEWAREHOUSEREADREQUEST"]._serialized_start = 655
+    _globals["_DELIVERYPRICEWAREHOUSEREADREQUEST"]._serialized_end = 1038
+    _globals["_DELIVERYPRICEWAREHOUSEREADRESPONSE"]._serialized_start = 1041
+    _globals["_DELIVERYPRICEWAREHOUSEREADRESPONSE"]._serialized_end = 1321
+    _globals["_DELIVERYPRICEWAREHOUSEUPDATEREQUEST"]._serialized_start = 1324
+    _globals["_DELIVERYPRICEWAREHOUSEUPDATEREQUEST"]._serialized_end = 1527
+    _globals["_DELIVERYPRICEWAREHOUSEUPDATERESPONSE"]._serialized_start = 1530
+    _globals["_DELIVERYPRICEWAREHOUSEUPDATERESPONSE"]._serialized_end = 1753
+    _globals["_DELIVERYPRICEWAREHOUSEDELETEREQUEST"]._serialized_start = 1755
+    _globals["_DELIVERYPRICEWAREHOUSEDELETEREQUEST"]._serialized_end = 1860
+    _globals["_DELIVERYPRICEWAREHOUSEDELETERESPONSE"]._serialized_start = 1862
+    _globals["_DELIVERYPRICEWAREHOUSEDELETERESPONSE"]._serialized_end = 1975
+    _globals["_DELIVERYPRICEWAREHOUSESERVICE"]._serialized_start = 1978
+    _globals["_DELIVERYPRICEWAREHOUSESERVICE"]._serialized_end = 2859
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,158 +3,140 @@
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
-from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
-from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as _warehouse_hierarchy_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class SortBy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
-    ASC: _ClassVar[SortBy]
-    DESC: _ClassVar[SortBy]
-
-ASC: SortBy
-DESC: SortBy
-
-class DeliveryMethodWarehouse(_message.Message):
-    __slots__ = ["id", "name", "hierarchi_warehouse_sort_by", "transfer_warehouse_ids", "active", "object_audit"]
+class DeliveryShipperWarehouse(_message.Message):
+    __slots__ = ["id", "delivery_shipper_id", "warehouse_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    HIERARCHI_WAREHOUSE_SORT_BY_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
+    DELIVERY_SHIPPER_ID_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: str
-    name: str
-    hierarchi_warehouse_sort_by: SortBy
-    transfer_warehouse_ids: _containers.RepeatedCompositeFieldContainer[_warehouse_hierarchy_pb2.WarehouseHierarchy]
+    id: int
+    delivery_shipper_id: int
+    warehouse_id: int
     active: bool
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[str] = ...,
-        name: _Optional[str] = ...,
-        hierarchi_warehouse_sort_by: _Optional[_Union[SortBy, str]] = ...,
-        transfer_warehouse_ids: _Optional[
-            _Iterable[_Union[_warehouse_hierarchy_pb2.WarehouseHierarchy, _Mapping]]
-        ] = ...,
+        id: _Optional[int] = ...,
+        delivery_shipper_id: _Optional[int] = ...,
+        warehouse_id: _Optional[int] = ...,
         active: bool = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseCreateRequest(_message.Message):
-    __slots__ = ["name", "transfer_warehouse_ids", "hierarchi_warehouse_sort_by", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
-    HIERARCHI_WAREHOUSE_SORT_BY_FIELD_NUMBER: _ClassVar[int]
+class DeliveryShipperWarehouseCreateRequest(_message.Message):
+    __slots__ = ["delivery_shipper_id", "warehouse_id", "context"]
+    DELIVERY_SHIPPER_ID_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    transfer_warehouse_ids: _containers.RepeatedScalarFieldContainer[str]
-    hierarchi_warehouse_sort_by: SortBy
+    delivery_shipper_id: int
+    warehouse_id: int
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
-        transfer_warehouse_ids: _Optional[_Iterable[str]] = ...,
-        hierarchi_warehouse_sort_by: _Optional[_Union[SortBy, str]] = ...,
+        delivery_shipper_id: _Optional[int] = ...,
+        warehouse_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseCreateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryShipperWarehouseCreateResponse(_message.Message):
+    __slots__ = ["delivery_shipper_warehouse", "response_standard"]
+    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryMethodWarehouse
+    delivery_shipper_warehouse: DeliveryShipperWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryMethodWarehouse, _Mapping]] = ...,
+        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseReadRequest(_message.Message):
+class DeliveryShipperWarehouseReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseReadResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouses", "meta_data", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
+class DeliveryShipperWarehouseReadResponse(_message.Message):
+    __slots__ = ["delivery_shipper_warehouse", "meta_data", "response_standard"]
+    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouses: _containers.RepeatedCompositeFieldContainer[DeliveryMethodWarehouse]
+    delivery_shipper_warehouse: _containers.RepeatedCompositeFieldContainer[DeliveryShipperWarehouse]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouses: _Optional[_Iterable[_Union[DeliveryMethodWarehouse, _Mapping]]] = ...,
+        delivery_shipper_warehouse: _Optional[_Iterable[_Union[DeliveryShipperWarehouse, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseUpdateRequest(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "context"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryShipperWarehouseUpdateRequest(_message.Message):
+    __slots__ = ["delivery_shipper_warehouse", "context"]
+    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryMethodWarehouse
+    delivery_shipper_warehouse: DeliveryShipperWarehouse
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryMethodWarehouse, _Mapping]] = ...,
+        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseUpdateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryShipperWarehouseUpdateResponse(_message.Message):
+    __slots__ = ["delivery_shipper_warehouse", "response_standard"]
+    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryMethodWarehouse
+    delivery_shipper_warehouse: DeliveryShipperWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryMethodWarehouse, _Mapping]] = ...,
+        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryMethodWarehouseDeleteRequest(_message.Message):
+class DeliveryShipperWarehouseDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryMethodWarehouseDeleteResponse(_message.Message):
+class DeliveryShipperWarehouseDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_price_warehouse.proto
+# source: v1/rules/delivery_time_warehouse.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\'v1/rules/delivery_price_warehouse.proto\x12\x32pro.omni.oms.api.v1.rules.delivery_price_warehouse\x1a\x11\x63ommon/base.proto"\xa6\x01\n\x16\x44\x65liveryPriceWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x19\n\x11\x64\x65livery_price_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8e\x01\n#DeliveryPriceWarehouseCreateRequest\x12\x19\n\x11\x64\x65livery_price_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdf\x01\n$DeliveryPriceWarehouseCreateResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xff\x02\n!DeliveryPriceWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x98\x02\n"DeliveryPriceWarehouseReadResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x03(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xcb\x01\n#DeliveryPriceWarehouseUpdateRequest\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdf\x01\n$DeliveryPriceWarehouseUpdateResponse\x12l\n\x18\x64\x65livery_price_warehouse\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"i\n#DeliveryPriceWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"q\n$DeliveryPriceWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf1\x06\n\x1d\x44\x65liveryPriceWarehouseService\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseCreate\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseCreateRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseCreateResponse"\x00\x12\xcd\x01\n\x1a\x44\x65liveryPriceWarehouseRead\x12U.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseReadRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseReadResponse"\x00\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseUpdate\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseUpdateRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseUpdateResponse"\x00\x12\xd3\x01\n\x1c\x44\x65liveryPriceWarehouseDelete\x12W.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseDeleteRequest\x1aX.pro.omni.oms.api.v1.rules.delivery_price_warehouse.DeliveryPriceWarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n&v1/rules/delivery_time_warehouse.proto\x12\x31pro.omni.oms.api.v1.rules.delivery_time_warehouse\x1a\x11\x63ommon/base.proto"\xa4\x01\n\x15\x44\x65liveryTimeWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x18\n\x10\x64\x65livery_time_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8c\x01\n"DeliveryTimeWarehouseCreateRequest\x12\x18\n\x10\x64\x65livery_time_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n#DeliveryTimeWarehouseCreateResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfe\x02\n DeliveryTimeWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x94\x02\n!DeliveryTimeWarehouseReadResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x03(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xc7\x01\n"DeliveryTimeWarehouseUpdateRequest\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n#DeliveryTimeWarehouseUpdateResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"h\n"DeliveryTimeWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"p\n#DeliveryTimeWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xdc\x06\n\x1c\x44\x65liveryTimeWarehouseService\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseCreate\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseCreateRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseCreateResponse"\x00\x12\xc8\x01\n\x19\x44\x65liveryTimeWarehouseRead\x12S.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseReadRequest\x1aT.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseReadResponse"\x00\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseUpdate\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseUpdateRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseUpdateResponse"\x00\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseDelete\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseDeleteRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_price_warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_time_warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYPRICEWAREHOUSE"]._serialized_start = 115
-    _globals["_DELIVERYPRICEWAREHOUSE"]._serialized_end = 281
-    _globals["_DELIVERYPRICEWAREHOUSECREATEREQUEST"]._serialized_start = 284
-    _globals["_DELIVERYPRICEWAREHOUSECREATEREQUEST"]._serialized_end = 426
-    _globals["_DELIVERYPRICEWAREHOUSECREATERESPONSE"]._serialized_start = 429
-    _globals["_DELIVERYPRICEWAREHOUSECREATERESPONSE"]._serialized_end = 652
-    _globals["_DELIVERYPRICEWAREHOUSEREADREQUEST"]._serialized_start = 655
-    _globals["_DELIVERYPRICEWAREHOUSEREADREQUEST"]._serialized_end = 1038
-    _globals["_DELIVERYPRICEWAREHOUSEREADRESPONSE"]._serialized_start = 1041
-    _globals["_DELIVERYPRICEWAREHOUSEREADRESPONSE"]._serialized_end = 1321
-    _globals["_DELIVERYPRICEWAREHOUSEUPDATEREQUEST"]._serialized_start = 1324
-    _globals["_DELIVERYPRICEWAREHOUSEUPDATEREQUEST"]._serialized_end = 1527
-    _globals["_DELIVERYPRICEWAREHOUSEUPDATERESPONSE"]._serialized_start = 1530
-    _globals["_DELIVERYPRICEWAREHOUSEUPDATERESPONSE"]._serialized_end = 1753
-    _globals["_DELIVERYPRICEWAREHOUSEDELETEREQUEST"]._serialized_start = 1755
-    _globals["_DELIVERYPRICEWAREHOUSEDELETEREQUEST"]._serialized_end = 1860
-    _globals["_DELIVERYPRICEWAREHOUSEDELETERESPONSE"]._serialized_start = 1862
-    _globals["_DELIVERYPRICEWAREHOUSEDELETERESPONSE"]._serialized_end = 1975
-    _globals["_DELIVERYPRICEWAREHOUSESERVICE"]._serialized_start = 1978
-    _globals["_DELIVERYPRICEWAREHOUSESERVICE"]._serialized_end = 2859
+    _globals["_DELIVERYTIMEWAREHOUSE"]._serialized_start = 113
+    _globals["_DELIVERYTIMEWAREHOUSE"]._serialized_end = 277
+    _globals["_DELIVERYTIMEWAREHOUSECREATEREQUEST"]._serialized_start = 280
+    _globals["_DELIVERYTIMEWAREHOUSECREATEREQUEST"]._serialized_end = 420
+    _globals["_DELIVERYTIMEWAREHOUSECREATERESPONSE"]._serialized_start = 423
+    _globals["_DELIVERYTIMEWAREHOUSECREATERESPONSE"]._serialized_end = 642
+    _globals["_DELIVERYTIMEWAREHOUSEREADREQUEST"]._serialized_start = 645
+    _globals["_DELIVERYTIMEWAREHOUSEREADREQUEST"]._serialized_end = 1027
+    _globals["_DELIVERYTIMEWAREHOUSEREADRESPONSE"]._serialized_start = 1030
+    _globals["_DELIVERYTIMEWAREHOUSEREADRESPONSE"]._serialized_end = 1306
+    _globals["_DELIVERYTIMEWAREHOUSEUPDATEREQUEST"]._serialized_start = 1309
+    _globals["_DELIVERYTIMEWAREHOUSEUPDATEREQUEST"]._serialized_end = 1508
+    _globals["_DELIVERYTIMEWAREHOUSEUPDATERESPONSE"]._serialized_start = 1511
+    _globals["_DELIVERYTIMEWAREHOUSEUPDATERESPONSE"]._serialized_end = 1730
+    _globals["_DELIVERYTIMEWAREHOUSEDELETEREQUEST"]._serialized_start = 1732
+    _globals["_DELIVERYTIMEWAREHOUSEDELETEREQUEST"]._serialized_end = 1836
+    _globals["_DELIVERYTIMEWAREHOUSEDELETERESPONSE"]._serialized_start = 1838
+    _globals["_DELIVERYTIMEWAREHOUSEDELETERESPONSE"]._serialized_end = 1950
+    _globals["_DELIVERYTIMEWAREHOUSESERVICE"]._serialized_start = 1953
+    _globals["_DELIVERYTIMEWAREHOUSESERVICE"]._serialized_end = 2813
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,41 +8,42 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import schedule_work_pb2 as v1_dot_rules_dot_schedule__work__pb2
 from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as v1_dot_rules_dot_warehouse__hierarchy__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n v1/rules/delivery_schedule.proto\x12+pro.omni.oms.api.v1.rules.delivery_schedule\x1a\x11\x63ommon/base.proto\x1a"v1/rules/warehouse_hierarchy.proto\x1a\x1cv1/rules/schedule_work.proto"\xb1\x02\n\x10\x44\x65liverySchedule\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12O\n\x10schedule_work_id\x18\x03 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12\x61\n\x16transfer_warehouse_ids\x18\x04 \x03(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x9f\x01\n\x1d\x44\x65liveryScheduleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10schedule_work_id\x18\x02 \x01(\t\x12\x1e\n\x16transfer_warehouse_ids\x18\x03 \x03(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryScheduleCreateResponse\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryScheduleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xff\x01\n\x1c\x44\x65liveryScheduleReadResponse\x12Y\n\x12\x64\x65livery_schedules\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryScheduleUpdateRequest\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryScheduleUpdateResponse\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryScheduleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryScheduleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryScheduleService\x12\xb3\x01\n\x16\x44\x65liveryScheduleCreate\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryScheduleRead\x12H.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryScheduleUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryScheduleDelete\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleDeleteResponse"\x00\x62\x06proto3'
+    b'\n v1/rules/delivery_schedule.proto\x12+pro.omni.oms.api.v1.rules.delivery_schedule\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a"v1/rules/warehouse_hierarchy.proto\x1a\x1cv1/rules/schedule_work.proto"\xea\x01\n\x10\x44\x65liverySchedule\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12O\n\x10schedule_work_id\x18\x03 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x7f\n\x1d\x44\x65liveryScheduleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10schedule_work_id\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryScheduleCreateResponse\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1b\x44\x65liveryScheduleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xff\x01\n\x1c\x44\x65liveryScheduleReadResponse\x12Y\n\x12\x64\x65livery_schedules\x18\x01 \x03(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb1\x01\n\x1d\x44\x65liveryScheduleUpdateRequest\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc5\x01\n\x1e\x44\x65liveryScheduleUpdateResponse\x12X\n\x11\x64\x65livery_schedule\x18\x01 \x01(\x0b\x32=.pro.omni.oms.api.v1.rules.delivery_schedule.DeliverySchedule\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1d\x44\x65liveryScheduleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1e\x44\x65liveryScheduleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xeb\x05\n\x17\x44\x65liveryScheduleService\x12\xb3\x01\n\x16\x44\x65liveryScheduleCreate\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleCreateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleCreateResponse"\x00\x12\xad\x01\n\x14\x44\x65liveryScheduleRead\x12H.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleReadRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleReadResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryScheduleUpdate\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleUpdateRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleUpdateResponse"\x00\x12\xb3\x01\n\x16\x44\x65liveryScheduleDelete\x12J.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleDeleteRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_schedule.DeliveryScheduleDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_schedule_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYSCHEDULE"]._serialized_start = 167
-    _globals["_DELIVERYSCHEDULE"]._serialized_end = 472
-    _globals["_DELIVERYSCHEDULECREATEREQUEST"]._serialized_start = 475
-    _globals["_DELIVERYSCHEDULECREATEREQUEST"]._serialized_end = 634
-    _globals["_DELIVERYSCHEDULECREATERESPONSE"]._serialized_start = 637
-    _globals["_DELIVERYSCHEDULECREATERESPONSE"]._serialized_end = 834
-    _globals["_DELIVERYSCHEDULEREADREQUEST"]._serialized_start = 837
-    _globals["_DELIVERYSCHEDULEREADREQUEST"]._serialized_end = 1214
-    _globals["_DELIVERYSCHEDULEREADRESPONSE"]._serialized_start = 1217
-    _globals["_DELIVERYSCHEDULEREADRESPONSE"]._serialized_end = 1472
-    _globals["_DELIVERYSCHEDULEUPDATEREQUEST"]._serialized_start = 1475
-    _globals["_DELIVERYSCHEDULEUPDATEREQUEST"]._serialized_end = 1652
-    _globals["_DELIVERYSCHEDULEUPDATERESPONSE"]._serialized_start = 1655
-    _globals["_DELIVERYSCHEDULEUPDATERESPONSE"]._serialized_end = 1852
-    _globals["_DELIVERYSCHEDULEDELETEREQUEST"]._serialized_start = 1854
-    _globals["_DELIVERYSCHEDULEDELETEREQUEST"]._serialized_end = 1953
-    _globals["_DELIVERYSCHEDULEDELETERESPONSE"]._serialized_start = 1955
-    _globals["_DELIVERYSCHEDULEDELETERESPONSE"]._serialized_end = 2062
-    _globals["_DELIVERYSCHEDULESERVICE"]._serialized_start = 2065
-    _globals["_DELIVERYSCHEDULESERVICE"]._serialized_end = 2812
+    _globals["_DELIVERYSCHEDULE"]._serialized_start = 199
+    _globals["_DELIVERYSCHEDULE"]._serialized_end = 433
+    _globals["_DELIVERYSCHEDULECREATEREQUEST"]._serialized_start = 435
+    _globals["_DELIVERYSCHEDULECREATEREQUEST"]._serialized_end = 562
+    _globals["_DELIVERYSCHEDULECREATERESPONSE"]._serialized_start = 565
+    _globals["_DELIVERYSCHEDULECREATERESPONSE"]._serialized_end = 762
+    _globals["_DELIVERYSCHEDULEREADREQUEST"]._serialized_start = 765
+    _globals["_DELIVERYSCHEDULEREADREQUEST"]._serialized_end = 1142
+    _globals["_DELIVERYSCHEDULEREADRESPONSE"]._serialized_start = 1145
+    _globals["_DELIVERYSCHEDULEREADRESPONSE"]._serialized_end = 1400
+    _globals["_DELIVERYSCHEDULEUPDATEREQUEST"]._serialized_start = 1403
+    _globals["_DELIVERYSCHEDULEUPDATEREQUEST"]._serialized_end = 1580
+    _globals["_DELIVERYSCHEDULEUPDATERESPONSE"]._serialized_start = 1583
+    _globals["_DELIVERYSCHEDULEUPDATERESPONSE"]._serialized_end = 1780
+    _globals["_DELIVERYSCHEDULEDELETEREQUEST"]._serialized_start = 1782
+    _globals["_DELIVERYSCHEDULEDELETEREQUEST"]._serialized_end = 1881
+    _globals["_DELIVERYSCHEDULEDELETERESPONSE"]._serialized_start = 1883
+    _globals["_DELIVERYSCHEDULEDELETERESPONSE"]._serialized_end = 1990
+    _globals["_DELIVERYSCHEDULESERVICE"]._serialized_start = 1993
+    _globals["_DELIVERYSCHEDULESERVICE"]._serialized_end = 2740
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,62 +2,55 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import schedule_work_pb2 as _schedule_work_pb2
 from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as _warehouse_hierarchy_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DeliverySchedule(_message.Message):
-    __slots__ = ["id", "name", "schedule_work_id", "transfer_warehouse_ids", "active", "object_audit"]
+    __slots__ = ["id", "name", "schedule_work_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SCHEDULE_WORK_ID_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     schedule_work_id: _schedule_work_pb2.ScheduleWork
-    transfer_warehouse_ids: _containers.RepeatedCompositeFieldContainer[_warehouse_hierarchy_pb2.WarehouseHierarchy]
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         schedule_work_id: _Optional[_Union[_schedule_work_pb2.ScheduleWork, _Mapping]] = ...,
-        transfer_warehouse_ids: _Optional[
-            _Iterable[_Union[_warehouse_hierarchy_pb2.WarehouseHierarchy, _Mapping]]
-        ] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryScheduleCreateRequest(_message.Message):
-    __slots__ = ["name", "schedule_work_id", "transfer_warehouse_ids", "context"]
+    __slots__ = ["name", "schedule_work_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SCHEDULE_WORK_ID_FIELD_NUMBER: _ClassVar[int]
-    TRANSFER_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     schedule_work_id: str
-    transfer_warehouse_ids: _containers.RepeatedScalarFieldContainer[str]
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         schedule_work_id: _Optional[str] = ...,
-        transfer_warehouse_ids: _Optional[_Iterable[str]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryScheduleCreateResponse(_message.Message):
     __slots__ = ["delivery_schedule", "response_standard"]
     DELIVERY_SCHEDULE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_schedule_warehouse_hierarchy.proto
+# source: v1/rules/delivery_shipper.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
+from omni.pro.protos.v1.rules import delivery_method_pb2 as v1_dot_rules_dot_delivery__method__pb2
+from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n4v1/rules/delivery_schedule_warehouse_hierarchy.proto\x12?pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy\x1a\x11\x63ommon/base.proto"\xbf\x01\n"DeliveryScheduleWarehouseHierarchy\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1c\n\x14\x64\x65livery_schedule_id\x18\x02 \x01(\x05\x12\x1e\n\x16warehouse_hierarchy_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xa7\x01\n/DeliveryScheduleWarehouseHierarchyCreateRequest\x12\x1c\n\x14\x64\x65livery_schedule_id\x18\x01 \x01(\x05\x12\x1e\n\x16warehouse_hierarchy_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x92\x02\n0DeliveryScheduleWarehouseHierarchyCreateResponse\x12\x92\x01\n%delivery_schedule_warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x63.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x03\n-DeliveryScheduleWarehouseHierarchyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcb\x02\n.DeliveryScheduleWarehouseHierarchyReadResponse\x12\x92\x01\n%delivery_schedule_warehouse_hierarchy\x18\x01 \x03(\x0b\x32\x63.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchy\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfe\x01\n/DeliveryScheduleWarehouseHierarchyUpdateRequest\x12\x92\x01\n%delivery_schedule_warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x63.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchy\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x92\x02\n0DeliveryScheduleWarehouseHierarchyUpdateResponse\x12\x92\x01\n%delivery_schedule_warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x63.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"u\n/DeliveryScheduleWarehouseHierarchyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"}\n0DeliveryScheduleWarehouseHierarchyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf5\x08\n)DeliveryScheduleWarehouseHierarchyService\x12\x91\x02\n(DeliveryScheduleWarehouseHierarchyCreate\x12p.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyCreateRequest\x1aq.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyCreateResponse"\x00\x12\x8b\x02\n&DeliveryScheduleWarehouseHierarchyRead\x12n.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyReadRequest\x1ao.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyReadResponse"\x00\x12\x91\x02\n(DeliveryScheduleWarehouseHierarchyUpdate\x12p.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyUpdateRequest\x1aq.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyUpdateResponse"\x00\x12\x91\x02\n(DeliveryScheduleWarehouseHierarchyDelete\x12p.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyDeleteRequest\x1aq.pro.omni.oms.api.v1.rules.delivery_schedule_warehouse_hierarchy.DeliveryScheduleWarehouseHierarchyDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1fv1/rules/delivery_shipper.proto\x12*pro.omni.oms.api.v1.rules.delivery_shipper\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xbc\x03\n\x0f\x44\x65liveryShipper\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12G\n\ttime_type\x18\x06 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x85\x02\n\x1c\x44\x65liveryShipperCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12G\n\ttime_type\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperCreateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf8\x02\n\x1a\x44\x65liveryShipperReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfb\x01\n\x1b\x44\x65liveryShipperReadResponse\x12V\n\x11\x64\x65livery_shippers\x18\x01 \x03(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xad\x01\n\x1c\x44\x65liveryShipperUpdateRequest\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperUpdateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"b\n\x1c\x44\x65liveryShipperDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1d\x44\x65liveryShipperDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xd6\x05\n\x16\x44\x65liveryShipperService\x12\xae\x01\n\x15\x44\x65liveryShipperCreate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateResponse"\x00\x12\xa8\x01\n\x13\x44\x65liveryShipperRead\x12\x46.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperUpdate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperDelete\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_schedule_warehouse_hierarchy_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_shipper_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHY"]._serialized_start = 141
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHY"]._serialized_end = 332
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_start = 335
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_end = 502
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_start = 505
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_end = 779
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYREADREQUEST"]._serialized_start = 782
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYREADREQUEST"]._serialized_end = 1177
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYREADRESPONSE"]._serialized_start = 1180
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYREADRESPONSE"]._serialized_end = 1511
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_start = 1514
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_end = 1768
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_start = 1771
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_end = 2045
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_start = 2047
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_end = 2164
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_start = 2166
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_end = 2291
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYSERVICE"]._serialized_start = 2294
-    _globals["_DELIVERYSCHEDULEWAREHOUSEHIERARCHYSERVICE"]._serialized_end = 3435
+    _globals["_TIMETYPE"]._serialized_start = 2276
+    _globals["_TIMETYPE"]._serialized_end = 2333
+    _globals["_DELIVERYSHIPPER"]._serialized_start = 157
+    _globals["_DELIVERYSHIPPER"]._serialized_end = 601
+    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_start = 604
+    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_end = 865
+    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_start = 868
+    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_end = 1061
+    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_start = 1064
+    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_end = 1440
+    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_start = 1443
+    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_end = 1694
+    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_start = 1697
+    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_end = 1870
+    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_start = 1873
+    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_end = 2066
+    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_start = 2068
+    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_end = 2166
+    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_start = 2168
+    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_end = 2274
+    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_start = 2336
+    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_end = 3062
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -7,63 +7,63 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryScheduleWarehouseHierarchy(_message.Message):
-    __slots__ = ["id", "delivery_schedule_id", "warehouse_hierarchy_id", "active", "object_audit"]
+class DeliveryTimeWarehouse(_message.Message):
+    __slots__ = ["id", "delivery_time_id", "warehouse_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_SCHEDULE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_HIERARCHY_ID_FIELD_NUMBER: _ClassVar[int]
+    DELIVERY_TIME_ID_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    delivery_schedule_id: int
-    warehouse_hierarchy_id: int
+    delivery_time_id: int
+    warehouse_id: int
     active: bool
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        delivery_schedule_id: _Optional[int] = ...,
-        warehouse_hierarchy_id: _Optional[int] = ...,
+        delivery_time_id: _Optional[int] = ...,
+        warehouse_id: _Optional[int] = ...,
         active: bool = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyCreateRequest(_message.Message):
-    __slots__ = ["delivery_schedule_id", "warehouse_hierarchy_id", "context"]
-    DELIVERY_SCHEDULE_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_HIERARCHY_ID_FIELD_NUMBER: _ClassVar[int]
+class DeliveryTimeWarehouseCreateRequest(_message.Message):
+    __slots__ = ["delivery_time_id", "warehouse_id", "context"]
+    DELIVERY_TIME_ID_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_schedule_id: int
-    warehouse_hierarchy_id: int
+    delivery_time_id: int
+    warehouse_id: int
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_schedule_id: _Optional[int] = ...,
-        warehouse_hierarchy_id: _Optional[int] = ...,
+        delivery_time_id: _Optional[int] = ...,
+        warehouse_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyCreateResponse(_message.Message):
-    __slots__ = ["delivery_schedule_warehouse_hierarchy", "response_standard"]
-    DELIVERY_SCHEDULE_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class DeliveryTimeWarehouseCreateResponse(_message.Message):
+    __slots__ = ["delivery_time_warehouse", "response_standard"]
+    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_schedule_warehouse_hierarchy: DeliveryScheduleWarehouseHierarchy
+    delivery_time_warehouse: DeliveryTimeWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_schedule_warehouse_hierarchy: _Optional[_Union[DeliveryScheduleWarehouseHierarchy, _Mapping]] = ...,
+        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyReadRequest(_message.Message):
+class DeliveryTimeWarehouseReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -82,65 +82,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyReadResponse(_message.Message):
-    __slots__ = ["delivery_schedule_warehouse_hierarchy", "meta_data", "response_standard"]
-    DELIVERY_SCHEDULE_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class DeliveryTimeWarehouseReadResponse(_message.Message):
+    __slots__ = ["delivery_time_warehouse", "meta_data", "response_standard"]
+    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_schedule_warehouse_hierarchy: _containers.RepeatedCompositeFieldContainer[
-        DeliveryScheduleWarehouseHierarchy
-    ]
+    delivery_time_warehouse: _containers.RepeatedCompositeFieldContainer[DeliveryTimeWarehouse]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_schedule_warehouse_hierarchy: _Optional[
-            _Iterable[_Union[DeliveryScheduleWarehouseHierarchy, _Mapping]]
-        ] = ...,
+        delivery_time_warehouse: _Optional[_Iterable[_Union[DeliveryTimeWarehouse, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyUpdateRequest(_message.Message):
-    __slots__ = ["delivery_schedule_warehouse_hierarchy", "context"]
-    DELIVERY_SCHEDULE_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class DeliveryTimeWarehouseUpdateRequest(_message.Message):
+    __slots__ = ["delivery_time_warehouse", "context"]
+    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_schedule_warehouse_hierarchy: DeliveryScheduleWarehouseHierarchy
+    delivery_time_warehouse: DeliveryTimeWarehouse
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_schedule_warehouse_hierarchy: _Optional[_Union[DeliveryScheduleWarehouseHierarchy, _Mapping]] = ...,
+        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyUpdateResponse(_message.Message):
-    __slots__ = ["delivery_schedule_warehouse_hierarchy", "response_standard"]
-    DELIVERY_SCHEDULE_WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class DeliveryTimeWarehouseUpdateResponse(_message.Message):
+    __slots__ = ["delivery_time_warehouse", "response_standard"]
+    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_schedule_warehouse_hierarchy: DeliveryScheduleWarehouseHierarchy
+    delivery_time_warehouse: DeliveryTimeWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_schedule_warehouse_hierarchy: _Optional[_Union[DeliveryScheduleWarehouseHierarchy, _Mapping]] = ...,
+        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyDeleteRequest(_message.Message):
+class DeliveryTimeWarehouseDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryScheduleWarehouseHierarchyDeleteResponse(_message.Message):
+class DeliveryTimeWarehouseDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_shipper.proto
+# source: v1/rules/delivery_time.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,38 +13,38 @@
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import delivery_method_pb2 as v1_dot_rules_dot_delivery__method__pb2
 from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1fv1/rules/delivery_shipper.proto\x12*pro.omni.oms.api.v1.rules.delivery_shipper\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xbc\x03\n\x0f\x44\x65liveryShipper\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12G\n\ttime_type\x18\x06 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x85\x02\n\x1c\x44\x65liveryShipperCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12G\n\ttime_type\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_shipper.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperCreateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf8\x02\n\x1a\x44\x65liveryShipperReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xfb\x01\n\x1b\x44\x65liveryShipperReadResponse\x12V\n\x11\x64\x65livery_shippers\x18\x01 \x03(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xad\x01\n\x1c\x44\x65liveryShipperUpdateRequest\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc1\x01\n\x1d\x44\x65liveryShipperUpdateResponse\x12U\n\x10\x64\x65livery_shipper\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipper\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"b\n\x1c\x44\x65liveryShipperDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1d\x44\x65liveryShipperDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\xd6\x05\n\x16\x44\x65liveryShipperService\x12\xae\x01\n\x15\x44\x65liveryShipperCreate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperCreateResponse"\x00\x12\xa8\x01\n\x13\x44\x65liveryShipperRead\x12\x46.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadRequest\x1aG.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperReadResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperUpdate\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperUpdateResponse"\x00\x12\xae\x01\n\x15\x44\x65liveryShipperDelete\x12H.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteRequest\x1aI.pro.omni.oms.api.v1.rules.delivery_shipper.DeliveryShipperDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1cv1/rules/delivery_time.proto\x12\'pro.omni.oms.api.v1.rules.delivery_time\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xb6\x03\n\x0c\x44\x65liveryTime\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12\x44\n\ttime_type\x18\x06 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.delivery_time.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xff\x01\n\x19\x44\x65liveryTimeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12\x44\n\ttime_type\x18\x03 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.delivery_time.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1a\x44\x65liveryTimeCreateResponse\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17\x44\x65liveryTimeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18\x44\x65liveryTimeReadResponse\x12M\n\x0e\x64\x65livery_times\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa1\x01\n\x19\x44\x65liveryTimeUpdateRequest\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1a\x44\x65liveryTimeUpdateResponse\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19\x44\x65liveryTimeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"g\n\x1a\x44\x65liveryTimeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\x97\x05\n\x13\x44\x65liveryTimeService\x12\x9f\x01\n\x12\x44\x65liveryTimeCreate\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeCreateRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeCreateResponse"\x00\x12\x99\x01\n\x10\x44\x65liveryTimeRead\x12@.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeReadRequest\x1a\x41.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeReadResponse"\x00\x12\x9f\x01\n\x12\x44\x65liveryTimeUpdate\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeUpdateRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeUpdateResponse"\x00\x12\x9f\x01\n\x12\x44\x65liveryTimeDelete\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeDeleteRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_shipper_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_time_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TIMETYPE"]._serialized_start = 2276
-    _globals["_TIMETYPE"]._serialized_end = 2333
-    _globals["_DELIVERYSHIPPER"]._serialized_start = 157
-    _globals["_DELIVERYSHIPPER"]._serialized_end = 601
-    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_start = 604
-    _globals["_DELIVERYSHIPPERCREATEREQUEST"]._serialized_end = 865
-    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_start = 868
-    _globals["_DELIVERYSHIPPERCREATERESPONSE"]._serialized_end = 1061
-    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_start = 1064
-    _globals["_DELIVERYSHIPPERREADREQUEST"]._serialized_end = 1440
-    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_start = 1443
-    _globals["_DELIVERYSHIPPERREADRESPONSE"]._serialized_end = 1694
-    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_start = 1697
-    _globals["_DELIVERYSHIPPERUPDATEREQUEST"]._serialized_end = 1870
-    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_start = 1873
-    _globals["_DELIVERYSHIPPERUPDATERESPONSE"]._serialized_end = 2066
-    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_start = 2068
-    _globals["_DELIVERYSHIPPERDELETEREQUEST"]._serialized_end = 2166
-    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_start = 2168
-    _globals["_DELIVERYSHIPPERDELETERESPONSE"]._serialized_end = 2274
-    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_start = 2336
-    _globals["_DELIVERYSHIPPERSERVICE"]._serialized_end = 3062
+    _globals["_TIMETYPE"]._serialized_start = 2201
+    _globals["_TIMETYPE"]._serialized_end = 2258
+    _globals["_DELIVERYTIME"]._serialized_start = 151
+    _globals["_DELIVERYTIME"]._serialized_end = 589
+    _globals["_DELIVERYTIMECREATEREQUEST"]._serialized_start = 592
+    _globals["_DELIVERYTIMECREATEREQUEST"]._serialized_end = 847
+    _globals["_DELIVERYTIMECREATERESPONSE"]._serialized_start = 850
+    _globals["_DELIVERYTIMECREATERESPONSE"]._serialized_end = 1031
+    _globals["_DELIVERYTIMEREADREQUEST"]._serialized_start = 1034
+    _globals["_DELIVERYTIMEREADREQUEST"]._serialized_end = 1407
+    _globals["_DELIVERYTIMEREADRESPONSE"]._serialized_start = 1410
+    _globals["_DELIVERYTIMEREADRESPONSE"]._serialized_end = 1649
+    _globals["_DELIVERYTIMEUPDATEREQUEST"]._serialized_start = 1652
+    _globals["_DELIVERYTIMEUPDATEREQUEST"]._serialized_end = 1813
+    _globals["_DELIVERYTIMEUPDATERESPONSE"]._serialized_start = 1816
+    _globals["_DELIVERYTIMEUPDATERESPONSE"]._serialized_end = 1997
+    _globals["_DELIVERYTIMEDELETEREQUEST"]._serialized_start = 1999
+    _globals["_DELIVERYTIMEDELETEREQUEST"]._serialized_end = 2094
+    _globals["_DELIVERYTIMEDELETERESPONSE"]._serialized_start = 2096
+    _globals["_DELIVERYTIMEDELETERESPONSE"]._serialized_end = 2199
+    _globals["_DELIVERYTIMESERVICE"]._serialized_start = 2261
+    _globals["_DELIVERYTIMESERVICE"]._serialized_end = 2924
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_time.proto
+# source: v1/sales/delivery_method.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
-from omni.pro.protos.v1.rules import delivery_method_pb2 as v1_dot_rules_dot_delivery__method__pb2
-from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1cv1/rules/delivery_time.proto\x12\'pro.omni.oms.api.v1.rules.delivery_time\x1a\x11\x63ommon/base.proto\x1a\x1ev1/rules/delivery_method.proto\x1a\x18v1/rules/warehouse.proto"\xb6\x03\n\x0c\x44\x65liveryTime\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12V\n\x13\x64\x65livery_method_ids\x18\x03 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.rules.delivery_method.DeliveryMethod\x12\x45\n\rwarehouse_ids\x18\x04 \x03(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x1d\n\x15locality_available_id\x18\x05 \x01(\t\x12\x44\n\ttime_type\x18\x06 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.delivery_time.TimeType\x12\x11\n\tvalue_min\x18\x07 \x01(\t\x12\x11\n\tvalue_max\x18\x08 \x01(\t\x12\x11\n\tinversely\x18\t \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xff\x01\n\x19\x44\x65liveryTimeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1d\n\x15locality_available_id\x18\x02 \x01(\t\x12\x44\n\ttime_type\x18\x03 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.delivery_time.TimeType\x12\x11\n\tvalue_min\x18\x04 \x01(\t\x12\x11\n\tvalue_max\x18\x05 \x01(\t\x12\x11\n\tinversely\x18\x06 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1a\x44\x65liveryTimeCreateResponse\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17\x44\x65liveryTimeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18\x44\x65liveryTimeReadResponse\x12M\n\x0e\x64\x65livery_times\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa1\x01\n\x19\x44\x65liveryTimeUpdateRequest\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1a\x44\x65liveryTimeUpdateResponse\x12L\n\rdelivery_time\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTime\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19\x44\x65liveryTimeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"g\n\x1a\x44\x65liveryTimeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*9\n\x08TimeType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07MINUTES\x10\x01\x12\t\n\x05HOURS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x32\x97\x05\n\x13\x44\x65liveryTimeService\x12\x9f\x01\n\x12\x44\x65liveryTimeCreate\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeCreateRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeCreateResponse"\x00\x12\x99\x01\n\x10\x44\x65liveryTimeRead\x12@.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeReadRequest\x1a\x41.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeReadResponse"\x00\x12\x9f\x01\n\x12\x44\x65liveryTimeUpdate\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeUpdateRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeUpdateResponse"\x00\x12\x9f\x01\n\x12\x44\x65liveryTimeDelete\x12\x42.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeDeleteRequest\x1a\x43.pro.omni.oms.api.v1.rules.delivery_time.DeliveryTimeDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1ev1/sales/delivery_method.proto\x12)pro.omni.oms.api.v1.sales.delivery.method\x1a\x11\x63ommon/base.proto"\x89\x01\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"q\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc5\x05\n\x15\x44\x65liveryMethodService\x12\xaa\x01\n\x15\x44\x65liveryServiceCreate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryServiceRead\x12\x44.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceUpdate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceDelete\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_time_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.delivery_method_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TIMETYPE"]._serialized_start = 2201
-    _globals["_TIMETYPE"]._serialized_end = 2258
-    _globals["_DELIVERYTIME"]._serialized_start = 151
-    _globals["_DELIVERYTIME"]._serialized_end = 589
-    _globals["_DELIVERYTIMECREATEREQUEST"]._serialized_start = 592
-    _globals["_DELIVERYTIMECREATEREQUEST"]._serialized_end = 847
-    _globals["_DELIVERYTIMECREATERESPONSE"]._serialized_start = 850
-    _globals["_DELIVERYTIMECREATERESPONSE"]._serialized_end = 1031
-    _globals["_DELIVERYTIMEREADREQUEST"]._serialized_start = 1034
-    _globals["_DELIVERYTIMEREADREQUEST"]._serialized_end = 1407
-    _globals["_DELIVERYTIMEREADRESPONSE"]._serialized_start = 1410
-    _globals["_DELIVERYTIMEREADRESPONSE"]._serialized_end = 1649
-    _globals["_DELIVERYTIMEUPDATEREQUEST"]._serialized_start = 1652
-    _globals["_DELIVERYTIMEUPDATEREQUEST"]._serialized_end = 1813
-    _globals["_DELIVERYTIMEUPDATERESPONSE"]._serialized_start = 1816
-    _globals["_DELIVERYTIMEUPDATERESPONSE"]._serialized_end = 1997
-    _globals["_DELIVERYTIMEDELETEREQUEST"]._serialized_start = 1999
-    _globals["_DELIVERYTIMEDELETEREQUEST"]._serialized_end = 2094
-    _globals["_DELIVERYTIMEDELETERESPONSE"]._serialized_start = 2096
-    _globals["_DELIVERYTIMEDELETERESPONSE"]._serialized_end = 2199
-    _globals["_DELIVERYTIMESERVICE"]._serialized_start = 2261
-    _globals["_DELIVERYTIMESERVICE"]._serialized_end = 2924
+    _globals["_DELIVERYMETHOD"]._serialized_start = 97
+    _globals["_DELIVERYMETHOD"]._serialized_end = 234
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 236
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 349
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 352
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 541
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 544
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 919
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 922
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 1169
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 1172
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 1341
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 1344
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 1533
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 1535
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 1632
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 1634
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 1739
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 1742
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 2451
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_time_warehouse.proto
+# source: v1/rules/delviery_shipper_warehouse.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n&v1/rules/delivery_time_warehouse.proto\x12\x31pro.omni.oms.api.v1.rules.delivery_time_warehouse\x1a\x11\x63ommon/base.proto"\xa4\x01\n\x15\x44\x65liveryTimeWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x18\n\x10\x64\x65livery_time_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8c\x01\n"DeliveryTimeWarehouseCreateRequest\x12\x18\n\x10\x64\x65livery_time_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n#DeliveryTimeWarehouseCreateResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfe\x02\n DeliveryTimeWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x94\x02\n!DeliveryTimeWarehouseReadResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x03(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xc7\x01\n"DeliveryTimeWarehouseUpdateRequest\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n#DeliveryTimeWarehouseUpdateResponse\x12i\n\x17\x64\x65livery_time_warehouse\x18\x01 \x01(\x0b\x32H.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"h\n"DeliveryTimeWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"p\n#DeliveryTimeWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xdc\x06\n\x1c\x44\x65liveryTimeWarehouseService\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseCreate\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseCreateRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseCreateResponse"\x00\x12\xc8\x01\n\x19\x44\x65liveryTimeWarehouseRead\x12S.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseReadRequest\x1aT.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseReadResponse"\x00\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseUpdate\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseUpdateRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseUpdateResponse"\x00\x12\xce\x01\n\x1b\x44\x65liveryTimeWarehouseDelete\x12U.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseDeleteRequest\x1aV.pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n)v1/rules/delviery_shipper_warehouse.proto\x12\x34pro.omni.oms.api.v1.rules.delivery_shipper_warehouse\x1a\x11\x63ommon/base.proto"\xaa\x01\n\x18\x44\x65liveryShipperWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1b\n\x13\x64\x65livery_shipper_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x92\x01\n%DeliveryShipperWarehouseCreateRequest\x12\x1b\n\x13\x64\x65livery_shipper_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe7\x01\n&DeliveryShipperWarehouseCreateResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x81\x03\n#DeliveryShipperWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa0\x02\n$DeliveryShipperWarehouseReadResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x03(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xd3\x01\n%DeliveryShipperWarehouseUpdateRequest\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe7\x01\n&DeliveryShipperWarehouseUpdateResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"k\n%DeliveryShipperWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"s\n&DeliveryShipperWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x9b\x07\n\x1f\x44\x65liveryShipperWarehouseService\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseCreate\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseCreateRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseCreateResponse"\x00\x12\xd7\x01\n\x1c\x44\x65liveryShipperWarehouseRead\x12Y.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseReadRequest\x1aZ.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseReadResponse"\x00\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseUpdate\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseUpdateRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseUpdateResponse"\x00\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseDelete\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseDeleteRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_time_warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delviery_shipper_warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYTIMEWAREHOUSE"]._serialized_start = 113
-    _globals["_DELIVERYTIMEWAREHOUSE"]._serialized_end = 277
-    _globals["_DELIVERYTIMEWAREHOUSECREATEREQUEST"]._serialized_start = 280
-    _globals["_DELIVERYTIMEWAREHOUSECREATEREQUEST"]._serialized_end = 420
-    _globals["_DELIVERYTIMEWAREHOUSECREATERESPONSE"]._serialized_start = 423
-    _globals["_DELIVERYTIMEWAREHOUSECREATERESPONSE"]._serialized_end = 642
-    _globals["_DELIVERYTIMEWAREHOUSEREADREQUEST"]._serialized_start = 645
-    _globals["_DELIVERYTIMEWAREHOUSEREADREQUEST"]._serialized_end = 1027
-    _globals["_DELIVERYTIMEWAREHOUSEREADRESPONSE"]._serialized_start = 1030
-    _globals["_DELIVERYTIMEWAREHOUSEREADRESPONSE"]._serialized_end = 1306
-    _globals["_DELIVERYTIMEWAREHOUSEUPDATEREQUEST"]._serialized_start = 1309
-    _globals["_DELIVERYTIMEWAREHOUSEUPDATEREQUEST"]._serialized_end = 1508
-    _globals["_DELIVERYTIMEWAREHOUSEUPDATERESPONSE"]._serialized_start = 1511
-    _globals["_DELIVERYTIMEWAREHOUSEUPDATERESPONSE"]._serialized_end = 1730
-    _globals["_DELIVERYTIMEWAREHOUSEDELETEREQUEST"]._serialized_start = 1732
-    _globals["_DELIVERYTIMEWAREHOUSEDELETEREQUEST"]._serialized_end = 1836
-    _globals["_DELIVERYTIMEWAREHOUSEDELETERESPONSE"]._serialized_start = 1838
-    _globals["_DELIVERYTIMEWAREHOUSEDELETERESPONSE"]._serialized_end = 1950
-    _globals["_DELIVERYTIMEWAREHOUSESERVICE"]._serialized_start = 1953
-    _globals["_DELIVERYTIMEWAREHOUSESERVICE"]._serialized_end = 2813
+    _globals["_DELIVERYSHIPPERWAREHOUSE"]._serialized_start = 119
+    _globals["_DELIVERYSHIPPERWAREHOUSE"]._serialized_end = 289
+    _globals["_DELIVERYSHIPPERWAREHOUSECREATEREQUEST"]._serialized_start = 292
+    _globals["_DELIVERYSHIPPERWAREHOUSECREATEREQUEST"]._serialized_end = 438
+    _globals["_DELIVERYSHIPPERWAREHOUSECREATERESPONSE"]._serialized_start = 441
+    _globals["_DELIVERYSHIPPERWAREHOUSECREATERESPONSE"]._serialized_end = 672
+    _globals["_DELIVERYSHIPPERWAREHOUSEREADREQUEST"]._serialized_start = 675
+    _globals["_DELIVERYSHIPPERWAREHOUSEREADREQUEST"]._serialized_end = 1060
+    _globals["_DELIVERYSHIPPERWAREHOUSEREADRESPONSE"]._serialized_start = 1063
+    _globals["_DELIVERYSHIPPERWAREHOUSEREADRESPONSE"]._serialized_end = 1351
+    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATEREQUEST"]._serialized_start = 1354
+    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATEREQUEST"]._serialized_end = 1565
+    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATERESPONSE"]._serialized_start = 1568
+    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATERESPONSE"]._serialized_end = 1799
+    _globals["_DELIVERYSHIPPERWAREHOUSEDELETEREQUEST"]._serialized_start = 1801
+    _globals["_DELIVERYSHIPPERWAREHOUSEDELETEREQUEST"]._serialized_end = 1908
+    _globals["_DELIVERYSHIPPERWAREHOUSEDELETERESPONSE"]._serialized_start = 1910
+    _globals["_DELIVERYSHIPPERWAREHOUSEDELETERESPONSE"]._serialized_end = 2025
+    _globals["_DELIVERYSHIPPERWAREHOUSESERVICE"]._serialized_start = 2028
+    _globals["_DELIVERYSHIPPERWAREHOUSESERVICE"]._serialized_end = 2951
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -7,136 +7,139 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryTimeWarehouse(_message.Message):
-    __slots__ = ["id", "delivery_time_id", "warehouse_id", "active", "object_audit"]
+class Warehouse(_message.Message):
+    __slots__ = ["id", "name", "code", "warehouse_sql_id", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_TIME_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    delivery_time_id: int
-    warehouse_id: int
-    active: bool
+    id: str
+    name: str
+    code: str
+    warehouse_sql_id: str
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        delivery_time_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        active: bool = ...,
+        id: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        warehouse_sql_id: _Optional[str] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseCreateRequest(_message.Message):
-    __slots__ = ["delivery_time_id", "warehouse_id", "context"]
-    DELIVERY_TIME_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+class WarehouseCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "warehouse_sql_id", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_time_id: int
-    warehouse_id: int
+    name: str
+    code: str
+    warehouse_sql_id: str
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_time_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        warehouse_sql_id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseCreateResponse(_message.Message):
-    __slots__ = ["delivery_time_warehouse", "response_standard"]
-    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseCreateResponse(_message.Message):
+    __slots__ = ["warehouse", "response_standard"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_time_warehouse: DeliveryTimeWarehouse
+    warehouse: Warehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseReadRequest(_message.Message):
+class WarehouseReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseReadResponse(_message.Message):
-    __slots__ = ["delivery_time_warehouse", "meta_data", "response_standard"]
-    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseReadResponse(_message.Message):
+    __slots__ = ["warehouses", "meta_data", "response_standard"]
+    WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_time_warehouse: _containers.RepeatedCompositeFieldContainer[DeliveryTimeWarehouse]
+    warehouses: _containers.RepeatedCompositeFieldContainer[Warehouse]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_time_warehouse: _Optional[_Iterable[_Union[DeliveryTimeWarehouse, _Mapping]]] = ...,
+        warehouses: _Optional[_Iterable[_Union[Warehouse, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseUpdateRequest(_message.Message):
-    __slots__ = ["delivery_time_warehouse", "context"]
-    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseUpdateRequest(_message.Message):
+    __slots__ = ["warehouse", "context"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_time_warehouse: DeliveryTimeWarehouse
+    warehouse: Warehouse
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseUpdateResponse(_message.Message):
-    __slots__ = ["delivery_time_warehouse", "response_standard"]
-    DELIVERY_TIME_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseUpdateResponse(_message.Message):
+    __slots__ = ["warehouse", "response_standard"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_time_warehouse: DeliveryTimeWarehouse
+    warehouse: Warehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_time_warehouse: _Optional[_Union[DeliveryTimeWarehouse, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryTimeWarehouseDeleteRequest(_message.Message):
+class WarehouseDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryTimeWarehouseDeleteResponse(_message.Message):
+class WarehouseDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.rules import delivery_time_warehouse_pb2 as v1_dot_rules_dot_delivery__time__warehouse__pb2
+from omni.pro.protos.v1.rules import delivery_warehouse_pb2 as v1_dot_rules_dot_delivery__warehouse__pb2
 
 
-class DeliveryTimeWarehouseServiceStub(object):
+class DeliveryWarehouseServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.DeliveryTimeWarehouseCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseCreate",
-            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.FromString,
+        self.DeliveryWarehouseCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseCreate",
+            request_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateResponse.FromString,
         )
-        self.DeliveryTimeWarehouseRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseRead",
-            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.FromString,
+        self.DeliveryWarehouseRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseRead",
+            request_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadResponse.FromString,
         )
-        self.DeliveryTimeWarehouseUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseUpdate",
-            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.FromString,
+        self.DeliveryWarehouseUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseUpdate",
+            request_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateResponse.FromString,
         )
-        self.DeliveryTimeWarehouseDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseDelete",
-            request_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.FromString,
+        self.DeliveryWarehouseDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseDelete",
+            request_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteResponse.FromString,
         )
 
 
-class DeliveryTimeWarehouseServiceServicer(object):
+class DeliveryWarehouseServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def DeliveryTimeWarehouseCreate(self, request, context):
+    def DeliveryWarehouseCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryTimeWarehouseRead(self, request, context):
+    def DeliveryWarehouseRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryTimeWarehouseUpdate(self, request, context):
+    def DeliveryWarehouseUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryTimeWarehouseDelete(self, request, context):
+    def DeliveryWarehouseDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_DeliveryTimeWarehouseServiceServicer_to_server(servicer, server):
+def add_DeliveryWarehouseServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "DeliveryTimeWarehouseCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryTimeWarehouseCreate,
-            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.SerializeToString,
+        "DeliveryWarehouseCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryWarehouseCreate,
+            request_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateResponse.SerializeToString,
         ),
-        "DeliveryTimeWarehouseRead": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryTimeWarehouseRead,
-            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.SerializeToString,
+        "DeliveryWarehouseRead": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryWarehouseRead,
+            request_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadResponse.SerializeToString,
         ),
-        "DeliveryTimeWarehouseUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryTimeWarehouseUpdate,
-            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.SerializeToString,
+        "DeliveryWarehouseUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryWarehouseUpdate,
+            request_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateResponse.SerializeToString,
         ),
-        "DeliveryTimeWarehouseDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryTimeWarehouseDelete,
-            request_deserializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.SerializeToString,
+        "DeliveryWarehouseDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.DeliveryWarehouseDelete,
+            request_deserializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteRequest.FromString,
+            response_serializer=v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService", rpc_method_handlers
+        "pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class DeliveryTimeWarehouseService(object):
+class DeliveryWarehouseService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def DeliveryTimeWarehouseCreate(
+    def DeliveryWarehouseCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseCreate",
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseCreate",
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryTimeWarehouseRead(
+    def DeliveryWarehouseRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseRead",
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseReadResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseRead",
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryTimeWarehouseUpdate(
+    def DeliveryWarehouseUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseUpdate",
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseUpdate",
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryTimeWarehouseDelete(
+    def DeliveryWarehouseDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_time_warehouse.DeliveryTimeWarehouseService/DeliveryTimeWarehouseDelete",
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__time__warehouse__pb2.DeliveryTimeWarehouseDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseService/DeliveryWarehouseDelete",
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteRequest.SerializeToString,
+            v1_dot_rules_dot_delivery__warehouse__pb2.DeliveryWarehouseDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delivery_warehouse_ref.proto
+# source: v1/rules/delivery_warehouse.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
+from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as v1_dot_rules_dot_warehouse__hierarchy__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n%v1/rules/delivery_warehouse_ref.proto\x12\x33pro.omni.oms.api.v1.rules.delivery_method_warehouse\x1a\x11\x63ommon/base.proto"\xa5\x01\n\x14\x44\x65liveryWarehouseRef\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8d\x01\n!DeliveryWarehouseRefCreateRequest\x12\x1a\n\x12\x64\x65livery_method_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n"DeliveryWarehouseRefCreateResponse\x12l\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32I.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRef\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfd\x02\n\x1f\x44\x65liveryWarehouseRefReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x96\x02\n DeliveryWarehouseRefReadResponse\x12l\n\x19\x64\x65livery_method_warehouse\x18\x01 \x03(\x0b\x32I.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRef\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xc9\x01\n!DeliveryWarehouseRefUpdateRequest\x12l\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32I.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRef\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n"DeliveryWarehouseRefUpdateResponse\x12l\n\x19\x64\x65livery_method_warehouse\x18\x01 \x01(\x0b\x32I.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRef\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"g\n!DeliveryWarehouseRefDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"o\n"DeliveryWarehouseRefDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xdf\x06\n\x1b\x44\x65liveryWarehouseRefService\x12\xcf\x01\n\x1a\x44\x65liveryWarehouseRefCreate\x12V.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefCreateRequest\x1aW.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefCreateResponse"\x00\x12\xc9\x01\n\x18\x44\x65liveryWarehouseRefRead\x12T.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefReadRequest\x1aU.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefReadResponse"\x00\x12\xcf\x01\n\x1a\x44\x65liveryWarehouseRefUpdate\x12V.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefUpdateRequest\x1aW.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefUpdateResponse"\x00\x12\xcf\x01\n\x1a\x44\x65liveryWarehouseRefDelete\x12V.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefDeleteRequest\x1aW.pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefDeleteResponse"\x00\x62\x06proto3'
+    b'\n!v1/rules/delivery_warehouse.proto\x12,pro.omni.oms.api.v1.rules.delivery_warehouse\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a"v1/rules/warehouse_hierarchy.proto"\xd5\x02\n\x11\x44\x65liveryWarehouse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12Y\n\x1bhierarchi_warehouse_sort_by\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_warehouse.SortBy\x12^\n\x13transfer_warehouses\x18\x04 \x03(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe1\x01\n\x1e\x44\x65liveryWarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x16transfer_warehouse_ids\x18\x02 \x03(\t\x12Y\n\x1bhierarchi_warehouse_sort_by\x18\x03 \x01(\x0e\x32\x34.pro.omni.oms.api.v1.rules.delivery_warehouse.SortBy\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc9\x01\n\x1f\x44\x65liveryWarehouseCreateResponse\x12[\n\x12\x64\x65livery_warehouse\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfa\x02\n\x1c\x44\x65liveryWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x83\x02\n\x1d\x44\x65liveryWarehouseReadResponse\x12\\\n\x13\x64\x65livery_warehouses\x18\x01 \x03(\x0b\x32?.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb5\x01\n\x1e\x44\x65liveryWarehouseUpdateRequest\x12[\n\x12\x64\x65livery_warehouse\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc9\x01\n\x1f\x44\x65liveryWarehouseUpdateResponse\x12[\n\x12\x64\x65livery_warehouse\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"d\n\x1e\x44\x65liveryWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"l\n\x1f\x44\x65liveryWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*\x1b\n\x06SortBy\x12\x07\n\x03\x41SC\x10\x00\x12\x08\n\x04\x44\x45SC\x10\x01\x32\x80\x06\n\x18\x44\x65liveryWarehouseService\x12\xb8\x01\n\x17\x44\x65liveryWarehouseCreate\x12L.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseCreateRequest\x1aM.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseCreateResponse"\x00\x12\xb2\x01\n\x15\x44\x65liveryWarehouseRead\x12J.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseReadRequest\x1aK.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseReadResponse"\x00\x12\xb8\x01\n\x17\x44\x65liveryWarehouseUpdate\x12L.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseUpdateRequest\x1aM.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseUpdateResponse"\x00\x12\xb8\x01\n\x17\x44\x65liveryWarehouseDelete\x12L.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseDeleteRequest\x1aM.pro.omni.oms.api.v1.rules.delivery_warehouse.DeliveryWarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_warehouse_ref_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delivery_warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYWAREHOUSEREF"]._serialized_start = 114
-    _globals["_DELIVERYWAREHOUSEREF"]._serialized_end = 279
-    _globals["_DELIVERYWAREHOUSEREFCREATEREQUEST"]._serialized_start = 282
-    _globals["_DELIVERYWAREHOUSEREFCREATEREQUEST"]._serialized_end = 423
-    _globals["_DELIVERYWAREHOUSEREFCREATERESPONSE"]._serialized_start = 426
-    _globals["_DELIVERYWAREHOUSEREFCREATERESPONSE"]._serialized_end = 647
-    _globals["_DELIVERYWAREHOUSEREFREADREQUEST"]._serialized_start = 650
-    _globals["_DELIVERYWAREHOUSEREFREADREQUEST"]._serialized_end = 1031
-    _globals["_DELIVERYWAREHOUSEREFREADRESPONSE"]._serialized_start = 1034
-    _globals["_DELIVERYWAREHOUSEREFREADRESPONSE"]._serialized_end = 1312
-    _globals["_DELIVERYWAREHOUSEREFUPDATEREQUEST"]._serialized_start = 1315
-    _globals["_DELIVERYWAREHOUSEREFUPDATEREQUEST"]._serialized_end = 1516
-    _globals["_DELIVERYWAREHOUSEREFUPDATERESPONSE"]._serialized_start = 1519
-    _globals["_DELIVERYWAREHOUSEREFUPDATERESPONSE"]._serialized_end = 1740
-    _globals["_DELIVERYWAREHOUSEREFDELETEREQUEST"]._serialized_start = 1742
-    _globals["_DELIVERYWAREHOUSEREFDELETEREQUEST"]._serialized_end = 1845
-    _globals["_DELIVERYWAREHOUSEREFDELETERESPONSE"]._serialized_start = 1847
-    _globals["_DELIVERYWAREHOUSEREFDELETERESPONSE"]._serialized_end = 1958
-    _globals["_DELIVERYWAREHOUSEREFSERVICE"]._serialized_start = 1961
-    _globals["_DELIVERYWAREHOUSEREFSERVICE"]._serialized_end = 2824
+    _globals["_SORTBY"]._serialized_start = 2189
+    _globals["_SORTBY"]._serialized_end = 2216
+    _globals["_DELIVERYWAREHOUSE"]._serialized_start = 171
+    _globals["_DELIVERYWAREHOUSE"]._serialized_end = 512
+    _globals["_DELIVERYWAREHOUSECREATEREQUEST"]._serialized_start = 515
+    _globals["_DELIVERYWAREHOUSECREATEREQUEST"]._serialized_end = 740
+    _globals["_DELIVERYWAREHOUSECREATERESPONSE"]._serialized_start = 743
+    _globals["_DELIVERYWAREHOUSECREATERESPONSE"]._serialized_end = 944
+    _globals["_DELIVERYWAREHOUSEREADREQUEST"]._serialized_start = 947
+    _globals["_DELIVERYWAREHOUSEREADREQUEST"]._serialized_end = 1325
+    _globals["_DELIVERYWAREHOUSEREADRESPONSE"]._serialized_start = 1328
+    _globals["_DELIVERYWAREHOUSEREADRESPONSE"]._serialized_end = 1587
+    _globals["_DELIVERYWAREHOUSEUPDATEREQUEST"]._serialized_start = 1590
+    _globals["_DELIVERYWAREHOUSEUPDATEREQUEST"]._serialized_end = 1771
+    _globals["_DELIVERYWAREHOUSEUPDATERESPONSE"]._serialized_start = 1774
+    _globals["_DELIVERYWAREHOUSEUPDATERESPONSE"]._serialized_end = 1975
+    _globals["_DELIVERYWAREHOUSEDELETEREQUEST"]._serialized_start = 1977
+    _globals["_DELIVERYWAREHOUSEDELETEREQUEST"]._serialized_end = 2077
+    _globals["_DELIVERYWAREHOUSEDELETERESPONSE"]._serialized_start = 2079
+    _globals["_DELIVERYWAREHOUSEDELETERESPONSE"]._serialized_end = 2187
+    _globals["_DELIVERYWAREHOUSESERVICE"]._serialized_start = 2219
+    _globals["_DELIVERYWAREHOUSESERVICE"]._serialized_end = 2987
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -7,63 +7,66 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryWarehouseRef(_message.Message):
-    __slots__ = ["id", "delivery_method_id", "warehouse_id", "active", "object_audit"]
+class Warehouse(_message.Message):
+    __slots__ = ["id", "name", "code", "warehouse_sql_id", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    delivery_method_id: int
-    warehouse_id: int
-    active: bool
+    name: str
+    code: str
+    warehouse_sql_id: int
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        active: bool = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        warehouse_sql_id: _Optional[int] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefCreateRequest(_message.Message):
-    __slots__ = ["delivery_method_id", "warehouse_id", "context"]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+class WarehouseCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "warehouse_sql_id", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_id: int
-    warehouse_id: int
+    name: str
+    code: str
+    warehouse_sql_id: int
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_method_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        warehouse_sql_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefCreateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseCreateResponse(_message.Message):
+    __slots__ = ["warehouse", "response_standard"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryWarehouseRef
+    warehouse: Warehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryWarehouseRef, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefReadRequest(_message.Message):
+class WarehouseReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -82,61 +85,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefReadResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "meta_data", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseReadResponse(_message.Message):
+    __slots__ = ["warehouses", "meta_data", "response_standard"]
+    WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: _containers.RepeatedCompositeFieldContainer[DeliveryWarehouseRef]
+    warehouses: _containers.RepeatedCompositeFieldContainer[Warehouse]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Iterable[_Union[DeliveryWarehouseRef, _Mapping]]] = ...,
+        warehouses: _Optional[_Iterable[_Union[Warehouse, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefUpdateRequest(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "context"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseUpdateRequest(_message.Message):
+    __slots__ = ["warehouse", "context"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryWarehouseRef
+    warehouse: Warehouse
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryWarehouseRef, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefUpdateResponse(_message.Message):
-    __slots__ = ["delivery_method_warehouse", "response_standard"]
-    DELIVERY_METHOD_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class WarehouseUpdateResponse(_message.Message):
+    __slots__ = ["warehouse", "response_standard"]
+    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_method_warehouse: DeliveryWarehouseRef
+    warehouse: Warehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_method_warehouse: _Optional[_Union[DeliveryWarehouseRef, _Mapping]] = ...,
+        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryWarehouseRefDeleteRequest(_message.Message):
+class WarehouseDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryWarehouseRefDeleteResponse(_message.Message):
+class WarehouseDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.rules import delivery_warehouse_ref_pb2 as v1_dot_rules_dot_delivery__warehouse__ref__pb2
+from omni.pro.protos.v1.sales import warehouse_pb2 as v1_dot_sales_dot_warehouse__pb2
 
 
-class DeliveryWarehouseRefServiceStub(object):
+class WarehouseServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.DeliveryWarehouseRefCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefCreate",
-            request_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateResponse.FromString,
+        self.WarehouseCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseCreate",
+            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
         )
-        self.DeliveryWarehouseRefRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefRead",
-            request_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadResponse.FromString,
+        self.WarehouseRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseRead",
+            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
+            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.FromString,
         )
-        self.DeliveryWarehouseRefUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefUpdate",
-            request_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateResponse.FromString,
+        self.WarehouseUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseUpdate",
+            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
         )
-        self.DeliveryWarehouseRefDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefDelete",
-            request_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteResponse.FromString,
+        self.WarehouseDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseDelete",
+            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
         )
 
 
-class DeliveryWarehouseRefServiceServicer(object):
+class WarehouseServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def DeliveryWarehouseRefCreate(self, request, context):
+    def WarehouseCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryWarehouseRefRead(self, request, context):
+    def WarehouseRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryWarehouseRefUpdate(self, request, context):
+    def WarehouseUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def DeliveryWarehouseRefDelete(self, request, context):
+    def WarehouseDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_DeliveryWarehouseRefServiceServicer_to_server(servicer, server):
+def add_WarehouseServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "DeliveryWarehouseRefCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryWarehouseRefCreate,
-            request_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateResponse.SerializeToString,
+        "WarehouseCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseCreate,
+            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.FromString,
+            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.SerializeToString,
         ),
-        "DeliveryWarehouseRefRead": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryWarehouseRefRead,
-            request_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadResponse.SerializeToString,
+        "WarehouseRead": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseRead,
+            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.FromString,
+            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.SerializeToString,
         ),
-        "DeliveryWarehouseRefUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryWarehouseRefUpdate,
-            request_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateResponse.SerializeToString,
+        "WarehouseUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseUpdate,
+            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.FromString,
+            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.SerializeToString,
         ),
-        "DeliveryWarehouseRefDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.DeliveryWarehouseRefDelete,
-            request_deserializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteRequest.FromString,
-            response_serializer=v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteResponse.SerializeToString,
+        "WarehouseDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseDelete,
+            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.FromString,
+            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService", rpc_method_handlers
+        "pro.omni.oms.api.v1.sales.warehouse.WarehouseService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class DeliveryWarehouseRefService(object):
+class WarehouseService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def DeliveryWarehouseRefCreate(
+    def WarehouseCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefCreate",
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseCreate",
+            v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
+            v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryWarehouseRefRead(
+    def WarehouseRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefRead",
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefReadResponse.FromString,
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseRead",
+            v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
+            v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryWarehouseRefUpdate(
+    def WarehouseUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefUpdate",
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseUpdate",
+            v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
+            v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def DeliveryWarehouseRefDelete(
+    def WarehouseDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.delivery_method_warehouse.DeliveryWarehouseRefService/DeliveryWarehouseRefDelete",
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteRequest.SerializeToString,
-            v1_dot_rules_dot_delivery__warehouse__ref__pb2.DeliveryWarehouseRefDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseDelete",
+            v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
+            v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/delviery_shipper_warehouse.proto
+# source: v1/utilities/payment_method.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n)v1/rules/delviery_shipper_warehouse.proto\x12\x34pro.omni.oms.api.v1.rules.delivery_shipper_warehouse\x1a\x11\x63ommon/base.proto"\xaa\x01\n\x18\x44\x65liveryShipperWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x1b\n\x13\x64\x65livery_shipper_id\x18\x02 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x92\x01\n%DeliveryShipperWarehouseCreateRequest\x12\x1b\n\x13\x64\x65livery_shipper_id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe7\x01\n&DeliveryShipperWarehouseCreateResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x81\x03\n#DeliveryShipperWarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa0\x02\n$DeliveryShipperWarehouseReadResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x03(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xd3\x01\n%DeliveryShipperWarehouseUpdateRequest\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe7\x01\n&DeliveryShipperWarehouseUpdateResponse\x12r\n\x1a\x64\x65livery_shipper_warehouse\x18\x01 \x01(\x0b\x32N.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"k\n%DeliveryShipperWarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"s\n&DeliveryShipperWarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x9b\x07\n\x1f\x44\x65liveryShipperWarehouseService\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseCreate\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseCreateRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseCreateResponse"\x00\x12\xd7\x01\n\x1c\x44\x65liveryShipperWarehouseRead\x12Y.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseReadRequest\x1aZ.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseReadResponse"\x00\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseUpdate\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseUpdateRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseUpdateResponse"\x00\x12\xdd\x01\n\x1e\x44\x65liveryShipperWarehouseDelete\x12[.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseDeleteRequest\x1a\\.pro.omni.oms.api.v1.rules.delivery_shipper_warehouse.DeliveryShipperWarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n!v1/utilities/payment_method.proto\x12,pro.omni.oms.api.v1.utilities.payment_method\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb9\x01\n\rPaymentMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x92\x01\n\x17PaymentMethodAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xba\x01\n\x18PaymentMethodAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12S\n\x0epayment_method\x18\x02 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"\xf6\x02\n\x18PaymentMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x19PaymentMethodReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12T\n\x0fpayment_methods\x18\x03 \x03(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"\xa9\x01\n\x1aPaymentMethodUpdateRequest\x12S\n\x0epayment_method\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1bPaymentMethodUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12S\n\x0epayment_method\x18\x02 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"`\n\x1aPaymentMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bPaymentMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc3\x05\n\x14PaymentMethodService\x12\xa3\x01\n\x10PaymentMethodAdd\x12\x45.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodAddRequest\x1a\x46.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodAddResponse"\x00\x12\xa6\x01\n\x11PaymentMethodRead\x12\x46.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodReadRequest\x1aG.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodReadResponse"\x00\x12\xac\x01\n\x13PaymentMethodUpdate\x12H.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodUpdateRequest\x1aI.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodUpdateResponse"\x00\x12\xac\x01\n\x13PaymentMethodDelete\x12H.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodDeleteRequest\x1aI.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.delviery_shipper_warehouse_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.payment_method_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYSHIPPERWAREHOUSE"]._serialized_start = 119
-    _globals["_DELIVERYSHIPPERWAREHOUSE"]._serialized_end = 289
-    _globals["_DELIVERYSHIPPERWAREHOUSECREATEREQUEST"]._serialized_start = 292
-    _globals["_DELIVERYSHIPPERWAREHOUSECREATEREQUEST"]._serialized_end = 438
-    _globals["_DELIVERYSHIPPERWAREHOUSECREATERESPONSE"]._serialized_start = 441
-    _globals["_DELIVERYSHIPPERWAREHOUSECREATERESPONSE"]._serialized_end = 672
-    _globals["_DELIVERYSHIPPERWAREHOUSEREADREQUEST"]._serialized_start = 675
-    _globals["_DELIVERYSHIPPERWAREHOUSEREADREQUEST"]._serialized_end = 1060
-    _globals["_DELIVERYSHIPPERWAREHOUSEREADRESPONSE"]._serialized_start = 1063
-    _globals["_DELIVERYSHIPPERWAREHOUSEREADRESPONSE"]._serialized_end = 1351
-    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATEREQUEST"]._serialized_start = 1354
-    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATEREQUEST"]._serialized_end = 1565
-    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATERESPONSE"]._serialized_start = 1568
-    _globals["_DELIVERYSHIPPERWAREHOUSEUPDATERESPONSE"]._serialized_end = 1799
-    _globals["_DELIVERYSHIPPERWAREHOUSEDELETEREQUEST"]._serialized_start = 1801
-    _globals["_DELIVERYSHIPPERWAREHOUSEDELETEREQUEST"]._serialized_end = 1908
-    _globals["_DELIVERYSHIPPERWAREHOUSEDELETERESPONSE"]._serialized_start = 1910
-    _globals["_DELIVERYSHIPPERWAREHOUSEDELETERESPONSE"]._serialized_end = 2025
-    _globals["_DELIVERYSHIPPERWAREHOUSESERVICE"]._serialized_start = 2028
-    _globals["_DELIVERYSHIPPERWAREHOUSESERVICE"]._serialized_end = 2951
+    _globals["_PAYMENTMETHOD"]._serialized_start = 135
+    _globals["_PAYMENTMETHOD"]._serialized_end = 320
+    _globals["_PAYMENTMETHODADDREQUEST"]._serialized_start = 323
+    _globals["_PAYMENTMETHODADDREQUEST"]._serialized_end = 469
+    _globals["_PAYMENTMETHODADDRESPONSE"]._serialized_start = 472
+    _globals["_PAYMENTMETHODADDRESPONSE"]._serialized_end = 658
+    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_start = 661
+    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_end = 1035
+    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_start = 1038
+    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_end = 1285
+    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_start = 1288
+    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_end = 1457
+    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_start = 1460
+    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_end = 1649
+    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_start = 1651
+    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_end = 1747
+    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_start = 1749
+    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_end = 1853
+    _globals["_PAYMENTMETHODSERVICE"]._serialized_start = 1856
+    _globals["_PAYMENTMETHODSERVICE"]._serialized_end = 2563
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,141 +2,158 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
+from omni.pro.protos.v1.rules import warehouse_hierarchy_pb2 as _warehouse_hierarchy_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DeliveryShipperWarehouse(_message.Message):
-    __slots__ = ["id", "delivery_shipper_id", "warehouse_id", "active", "object_audit"]
+class SortBy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    ASC: _ClassVar[SortBy]
+    DESC: _ClassVar[SortBy]
+
+ASC: SortBy
+DESC: SortBy
+
+class DeliveryWarehouse(_message.Message):
+    __slots__ = ["id", "name", "hierarchi_warehouse_sort_by", "transfer_warehouses", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_SHIPPER_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    HIERARCHI_WAREHOUSE_SORT_BY_FIELD_NUMBER: _ClassVar[int]
+    TRANSFER_WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    delivery_shipper_id: int
-    warehouse_id: int
-    active: bool
+    id: str
+    name: str
+    hierarchi_warehouse_sort_by: SortBy
+    transfer_warehouses: _containers.RepeatedCompositeFieldContainer[_warehouse_hierarchy_pb2.WarehouseHierarchy]
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        delivery_shipper_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        active: bool = ...,
+        id: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        hierarchi_warehouse_sort_by: _Optional[_Union[SortBy, str]] = ...,
+        transfer_warehouses: _Optional[_Iterable[_Union[_warehouse_hierarchy_pb2.WarehouseHierarchy, _Mapping]]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseCreateRequest(_message.Message):
-    __slots__ = ["delivery_shipper_id", "warehouse_id", "context"]
-    DELIVERY_SHIPPER_ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+class DeliveryWarehouseCreateRequest(_message.Message):
+    __slots__ = ["name", "transfer_warehouse_ids", "hierarchi_warehouse_sort_by", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TRANSFER_WAREHOUSE_IDS_FIELD_NUMBER: _ClassVar[int]
+    HIERARCHI_WAREHOUSE_SORT_BY_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_shipper_id: int
-    warehouse_id: int
+    name: str
+    transfer_warehouse_ids: _containers.RepeatedScalarFieldContainer[str]
+    hierarchi_warehouse_sort_by: SortBy
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_shipper_id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        transfer_warehouse_ids: _Optional[_Iterable[str]] = ...,
+        hierarchi_warehouse_sort_by: _Optional[_Union[SortBy, str]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseCreateResponse(_message.Message):
-    __slots__ = ["delivery_shipper_warehouse", "response_standard"]
-    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryWarehouseCreateResponse(_message.Message):
+    __slots__ = ["delivery_warehouse", "response_standard"]
+    DELIVERY_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_shipper_warehouse: DeliveryShipperWarehouse
+    delivery_warehouse: DeliveryWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
+        delivery_warehouse: _Optional[_Union[DeliveryWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseReadRequest(_message.Message):
+class DeliveryWarehouseReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseReadResponse(_message.Message):
-    __slots__ = ["delivery_shipper_warehouse", "meta_data", "response_standard"]
-    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryWarehouseReadResponse(_message.Message):
+    __slots__ = ["delivery_warehouses", "meta_data", "response_standard"]
+    DELIVERY_WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_shipper_warehouse: _containers.RepeatedCompositeFieldContainer[DeliveryShipperWarehouse]
+    delivery_warehouses: _containers.RepeatedCompositeFieldContainer[DeliveryWarehouse]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_shipper_warehouse: _Optional[_Iterable[_Union[DeliveryShipperWarehouse, _Mapping]]] = ...,
+        delivery_warehouses: _Optional[_Iterable[_Union[DeliveryWarehouse, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseUpdateRequest(_message.Message):
-    __slots__ = ["delivery_shipper_warehouse", "context"]
-    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryWarehouseUpdateRequest(_message.Message):
+    __slots__ = ["delivery_warehouse", "context"]
+    DELIVERY_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    delivery_shipper_warehouse: DeliveryShipperWarehouse
+    delivery_warehouse: DeliveryWarehouse
     context: _base_pb2.Context
     def __init__(
         self,
-        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
+        delivery_warehouse: _Optional[_Union[DeliveryWarehouse, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseUpdateResponse(_message.Message):
-    __slots__ = ["delivery_shipper_warehouse", "response_standard"]
-    DELIVERY_SHIPPER_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class DeliveryWarehouseUpdateResponse(_message.Message):
+    __slots__ = ["delivery_warehouse", "response_standard"]
+    DELIVERY_WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    delivery_shipper_warehouse: DeliveryShipperWarehouse
+    delivery_warehouse: DeliveryWarehouse
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        delivery_shipper_warehouse: _Optional[_Union[DeliveryShipperWarehouse, _Mapping]] = ...,
+        delivery_warehouse: _Optional[_Union[DeliveryWarehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class DeliveryShipperWarehouseDeleteRequest(_message.Message):
+class DeliveryWarehouseDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class DeliveryShipperWarehouseDeleteResponse(_message.Message):
+class DeliveryWarehouseDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17v1/rules/location.proto\x12"pro.omni.oms.api.v1.rules.location\x1a\x11\x63ommon/base.proto"\x83\x01\n\x08Location\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"]\n\x15LocationCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationCreateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13LocationReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14LocationReadResponse\x12?\n\tLocations\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15LocationUpdateRequest\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationUpdateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15LocationDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16LocationDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0fLocationService\x12\x89\x01\n\x0eLocationCreate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationCreateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationCreateResponse"\x00\x12\x83\x01\n\x0cLocationRead\x12\x37.pro.omni.oms.api.v1.rules.location.LocationReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.location.LocationReadResponse"\x00\x12\x89\x01\n\x0eLocationUpdate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationUpdateResponse"\x00\x12\x89\x01\n\x0eLocationDelete\x12\x39.pro.omni.oms.api.v1.rules.location.LocationDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/rules/location.proto\x12"pro.omni.oms.api.v1.rules.location\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb8\x01\n\x08Location\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0flocation_sql_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"]\n\x15LocationCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationCreateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13LocationReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14LocationReadResponse\x12?\n\tLocations\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15LocationUpdateRequest\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationUpdateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15LocationDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16LocationDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0fLocationService\x12\x89\x01\n\x0eLocationCreate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationCreateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationCreateResponse"\x00\x12\x83\x01\n\x0cLocationRead\x12\x37.pro.omni.oms.api.v1.rules.location.LocationReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.location.LocationReadResponse"\x00\x12\x89\x01\n\x0eLocationUpdate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationUpdateResponse"\x00\x12\x89\x01\n\x0eLocationDelete\x12\x39.pro.omni.oms.api.v1.rules.location.LocationDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.location_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_LOCATION"]._serialized_start = 83
-    _globals["_LOCATION"]._serialized_end = 214
-    _globals["_LOCATIONCREATEREQUEST"]._serialized_start = 216
-    _globals["_LOCATIONCREATEREQUEST"]._serialized_end = 309
-    _globals["_LOCATIONCREATERESPONSE"]._serialized_start = 312
-    _globals["_LOCATIONCREATERESPONSE"]._serialized_end = 475
-    _globals["_LOCATIONREADREQUEST"]._serialized_start = 478
-    _globals["_LOCATIONREADREQUEST"]._serialized_end = 847
-    _globals["_LOCATIONREADRESPONSE"]._serialized_start = 850
-    _globals["_LOCATIONREADRESPONSE"]._serialized_end = 1071
-    _globals["_LOCATIONUPDATEREQUEST"]._serialized_start = 1074
-    _globals["_LOCATIONUPDATEREQUEST"]._serialized_end = 1217
-    _globals["_LOCATIONUPDATERESPONSE"]._serialized_start = 1220
-    _globals["_LOCATIONUPDATERESPONSE"]._serialized_end = 1383
-    _globals["_LOCATIONDELETEREQUEST"]._serialized_start = 1385
-    _globals["_LOCATIONDELETEREQUEST"]._serialized_end = 1476
-    _globals["_LOCATIONDELETERESPONSE"]._serialized_start = 1478
-    _globals["_LOCATIONDELETERESPONSE"]._serialized_end = 1577
-    _globals["_LOCATIONSERVICE"]._serialized_start = 1580
-    _globals["_LOCATIONSERVICE"]._serialized_end = 2151
+    _globals["_LOCATION"]._serialized_start = 115
+    _globals["_LOCATION"]._serialized_end = 299
+    _globals["_LOCATIONCREATEREQUEST"]._serialized_start = 301
+    _globals["_LOCATIONCREATEREQUEST"]._serialized_end = 394
+    _globals["_LOCATIONCREATERESPONSE"]._serialized_start = 397
+    _globals["_LOCATIONCREATERESPONSE"]._serialized_end = 560
+    _globals["_LOCATIONREADREQUEST"]._serialized_start = 563
+    _globals["_LOCATIONREADREQUEST"]._serialized_end = 932
+    _globals["_LOCATIONREADRESPONSE"]._serialized_start = 935
+    _globals["_LOCATIONREADRESPONSE"]._serialized_end = 1156
+    _globals["_LOCATIONUPDATEREQUEST"]._serialized_start = 1159
+    _globals["_LOCATIONUPDATEREQUEST"]._serialized_end = 1302
+    _globals["_LOCATIONUPDATERESPONSE"]._serialized_start = 1305
+    _globals["_LOCATIONUPDATERESPONSE"]._serialized_end = 1468
+    _globals["_LOCATIONDELETEREQUEST"]._serialized_start = 1470
+    _globals["_LOCATIONDELETEREQUEST"]._serialized_end = 1561
+    _globals["_LOCATIONDELETERESPONSE"]._serialized_start = 1563
+    _globals["_LOCATIONDELETERESPONSE"]._serialized_end = 1662
+    _globals["_LOCATIONSERVICE"]._serialized_start = 1665
+    _globals["_LOCATIONSERVICE"]._serialized_end = 2236
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Location(_message.Message):
-    __slots__ = ["id", "name", "code", "active", "object_audit"]
+    __slots__ = ["id", "name", "code", "location_sql_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    active: bool
+    location_sql_id: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        active: bool = ...,
+        location_sql_id: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationCreateRequest(_message.Message):
     __slots__ = ["name", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/location_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,41 +9,42 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n!v1/rules/schedule_work_line.proto\x12,pro.omni.oms.api.v1.rules.schedule_work_line\x1a\x11\x63ommon/base.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\x93\x02\n\x10ScheduleWorkLine\x12\n\n\x02id\x18\x01 \x01(\t\x12>\n\x03\x64\x61y\x18\x02 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.schedule_work_line.Day\x12\x30\n\x0copening_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63losing_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xfb\x01\n\x1dScheduleWorkLineCreateRequest\x12>\n\x03\x64\x61y\x18\x01 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.schedule_work_line.Day\x12\x30\n\x0copening_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63losing_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1eScheduleWorkLineCreateResponse\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1bScheduleWorkLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x81\x02\n\x1cScheduleWorkLineReadResponse\x12[\n\x13schedule_work_lines\x18\x01 \x03(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb3\x01\n\x1dScheduleWorkLineUpdateRequest\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1eScheduleWorkLineUpdateResponse\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1dScheduleWorkLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1eScheduleWorkLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*a\n\x03\x44\x61y\x12\n\n\x06MONDAY\x10\x00\x12\x0b\n\x07TUESDAY\x10\x01\x12\r\n\tWEDNESDAY\x10\x02\x12\x0c\n\x08THURSDAY\x10\x03\x12\n\n\x06\x46RIDAY\x10\x04\x12\x0c\n\x08SATURDAY\x10\x05\x12\n\n\x06SUNDAY\x10\x06\x32\xf3\x05\n\x17ScheduleWorkLineService\x12\xb5\x01\n\x16ScheduleWorkLineCreate\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineCreateRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineCreateResponse"\x00\x12\xaf\x01\n\x14ScheduleWorkLineRead\x12I.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineReadRequest\x1aJ.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineReadResponse"\x00\x12\xb5\x01\n\x16ScheduleWorkLineUpdate\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineUpdateRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineUpdateResponse"\x00\x12\xb5\x01\n\x16ScheduleWorkLineDelete\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineDeleteRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineDeleteResponse"\x00\x62\x06proto3'
+    b'\n!v1/rules/schedule_work_line.proto\x12,pro.omni.oms.api.v1.rules.schedule_work_line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xaf\x02\n\x10ScheduleWorkLine\x12\n\n\x02id\x18\x01 \x01(\t\x12>\n\x03\x64\x61y\x18\x02 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.schedule_work_line.Day\x12\x30\n\x0copening_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63losing_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xfb\x01\n\x1dScheduleWorkLineCreateRequest\x12>\n\x03\x64\x61y\x18\x01 \x01(\x0e\x32\x31.pro.omni.oms.api.v1.rules.schedule_work_line.Day\x12\x30\n\x0copening_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63losing_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1eScheduleWorkLineCreateResponse\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf9\x02\n\x1bScheduleWorkLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x81\x02\n\x1cScheduleWorkLineReadResponse\x12[\n\x13schedule_work_lines\x18\x01 \x03(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb3\x01\n\x1dScheduleWorkLineUpdateRequest\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1eScheduleWorkLineUpdateResponse\x12Z\n\x12schedule_work_line\x18\x01 \x01(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"c\n\x1dScheduleWorkLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"k\n\x1eScheduleWorkLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard*a\n\x03\x44\x61y\x12\n\n\x06MONDAY\x10\x00\x12\x0b\n\x07TUESDAY\x10\x01\x12\r\n\tWEDNESDAY\x10\x02\x12\x0c\n\x08THURSDAY\x10\x03\x12\n\n\x06\x46RIDAY\x10\x04\x12\x0c\n\x08SATURDAY\x10\x05\x12\n\n\x06SUNDAY\x10\x06\x32\xf3\x05\n\x17ScheduleWorkLineService\x12\xb5\x01\n\x16ScheduleWorkLineCreate\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineCreateRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineCreateResponse"\x00\x12\xaf\x01\n\x14ScheduleWorkLineRead\x12I.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineReadRequest\x1aJ.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineReadResponse"\x00\x12\xb5\x01\n\x16ScheduleWorkLineUpdate\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineUpdateRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineUpdateResponse"\x00\x12\xb5\x01\n\x16ScheduleWorkLineDelete\x12K.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineDeleteRequest\x1aL.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLineDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.schedule_work_line_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DAY"]._serialized_start = 2103
-    _globals["_DAY"]._serialized_end = 2200
-    _globals["_SCHEDULEWORKLINE"]._serialized_start = 136
-    _globals["_SCHEDULEWORKLINE"]._serialized_end = 411
-    _globals["_SCHEDULEWORKLINECREATEREQUEST"]._serialized_start = 414
-    _globals["_SCHEDULEWORKLINECREATEREQUEST"]._serialized_end = 665
-    _globals["_SCHEDULEWORKLINECREATERESPONSE"]._serialized_start = 668
-    _globals["_SCHEDULEWORKLINECREATERESPONSE"]._serialized_end = 867
-    _globals["_SCHEDULEWORKLINEREADREQUEST"]._serialized_start = 870
-    _globals["_SCHEDULEWORKLINEREADREQUEST"]._serialized_end = 1247
-    _globals["_SCHEDULEWORKLINEREADRESPONSE"]._serialized_start = 1250
-    _globals["_SCHEDULEWORKLINEREADRESPONSE"]._serialized_end = 1507
-    _globals["_SCHEDULEWORKLINEUPDATEREQUEST"]._serialized_start = 1510
-    _globals["_SCHEDULEWORKLINEUPDATEREQUEST"]._serialized_end = 1689
-    _globals["_SCHEDULEWORKLINEUPDATERESPONSE"]._serialized_start = 1692
-    _globals["_SCHEDULEWORKLINEUPDATERESPONSE"]._serialized_end = 1891
-    _globals["_SCHEDULEWORKLINEDELETEREQUEST"]._serialized_start = 1893
-    _globals["_SCHEDULEWORKLINEDELETEREQUEST"]._serialized_end = 1992
-    _globals["_SCHEDULEWORKLINEDELETERESPONSE"]._serialized_start = 1994
-    _globals["_SCHEDULEWORKLINEDELETERESPONSE"]._serialized_end = 2101
-    _globals["_SCHEDULEWORKLINESERVICE"]._serialized_start = 2203
-    _globals["_SCHEDULEWORKLINESERVICE"]._serialized_end = 2958
+    _globals["_DAY"]._serialized_start = 2163
+    _globals["_DAY"]._serialized_end = 2260
+    _globals["_SCHEDULEWORKLINE"]._serialized_start = 168
+    _globals["_SCHEDULEWORKLINE"]._serialized_end = 471
+    _globals["_SCHEDULEWORKLINECREATEREQUEST"]._serialized_start = 474
+    _globals["_SCHEDULEWORKLINECREATEREQUEST"]._serialized_end = 725
+    _globals["_SCHEDULEWORKLINECREATERESPONSE"]._serialized_start = 728
+    _globals["_SCHEDULEWORKLINECREATERESPONSE"]._serialized_end = 927
+    _globals["_SCHEDULEWORKLINEREADREQUEST"]._serialized_start = 930
+    _globals["_SCHEDULEWORKLINEREADREQUEST"]._serialized_end = 1307
+    _globals["_SCHEDULEWORKLINEREADRESPONSE"]._serialized_start = 1310
+    _globals["_SCHEDULEWORKLINEREADRESPONSE"]._serialized_end = 1567
+    _globals["_SCHEDULEWORKLINEUPDATEREQUEST"]._serialized_start = 1570
+    _globals["_SCHEDULEWORKLINEUPDATEREQUEST"]._serialized_end = 1749
+    _globals["_SCHEDULEWORKLINEUPDATERESPONSE"]._serialized_start = 1752
+    _globals["_SCHEDULEWORKLINEUPDATERESPONSE"]._serialized_end = 1951
+    _globals["_SCHEDULEWORKLINEDELETEREQUEST"]._serialized_start = 1953
+    _globals["_SCHEDULEWORKLINEDELETEREQUEST"]._serialized_end = 2052
+    _globals["_SCHEDULEWORKLINEDELETERESPONSE"]._serialized_start = 2054
+    _globals["_SCHEDULEWORKLINEDELETERESPONSE"]._serialized_end = 2161
+    _globals["_SCHEDULEWORKLINESERVICE"]._serialized_start = 2263
+    _globals["_SCHEDULEWORKLINESERVICE"]._serialized_end = 3018
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Day(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
@@ -39,23 +40,23 @@
     CLOSING_TIME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     day: Day
     opening_time: _timestamp_pb2.Timestamp
     closing_time: _timestamp_pb2.Timestamp
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         day: _Optional[_Union[Day, str]] = ...,
         opening_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         closing_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class ScheduleWorkLineCreateRequest(_message.Message):
     __slots__ = ["day", "opening_time", "closing_time", "context"]
     DAY_FIELD_NUMBER: _ClassVar[int]
     OPENING_TIME_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,42 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.rules import calendar_pb2 as v1_dot_rules_dot_calendar__pb2
 from omni.pro.protos.v1.rules import schedule_work_line_pb2 as v1_dot_rules_dot_schedule__work__line__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1cv1/rules/schedule_work.proto\x12\'pro.omni.oms.api.v1.rules.schedule_work\x1a\x11\x63ommon/base.proto\x1a!v1/rules/schedule_work_line.proto\x1a\x17v1/rules/calendar.proto"\x9c\x02\n\x0cScheduleWork\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x41\n\x0b\x63\x61lendar_id\x18\x03 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12^\n\x16schedule_work_line_ids\x18\x04 \x03(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x96\x01\n\x19ScheduleWorkCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63\x61lendar_id\x18\x02 \x01(\t\x12\x1e\n\x16schedule_work_line_ids\x18\x03 \x03(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aScheduleWorkCreateResponse\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17ScheduleWorkReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18ScheduleWorkReadResponse\x12M\n\x0eschedules_work\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa1\x01\n\x19ScheduleWorkUpdateRequest\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aScheduleWorkUpdateResponse\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19ScheduleWorkDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"g\n\x1aScheduleWorkDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x97\x05\n\x13ScheduleWorkService\x12\x9f\x01\n\x12ScheduleWorkCreate\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkCreateRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkCreateResponse"\x00\x12\x99\x01\n\x10ScheduleWorkRead\x12@.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkReadRequest\x1a\x41.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkReadResponse"\x00\x12\x9f\x01\n\x12ScheduleWorkUpdate\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkUpdateRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkUpdateResponse"\x00\x12\x9f\x01\n\x12ScheduleWorkDelete\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkDeleteRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1cv1/rules/schedule_work.proto\x12\'pro.omni.oms.api.v1.rules.schedule_work\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a!v1/rules/schedule_work_line.proto\x1a\x17v1/rules/calendar.proto"\xb5\x02\n\x0cScheduleWork\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x41\n\x0b\x63\x61lendar_id\x18\x03 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.calendar.Calendar\x12[\n\x13schedule_work_lines\x18\x04 \x03(\x0b\x32>.pro.omni.oms.api.v1.rules.schedule_work_line.ScheduleWorkLine\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x96\x01\n\x19ScheduleWorkCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63\x61lendar_id\x18\x02 \x01(\t\x12\x1e\n\x16schedule_work_line_ids\x18\x03 \x03(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aScheduleWorkCreateResponse\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17ScheduleWorkReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18ScheduleWorkReadResponse\x12M\n\x0eschedules_work\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa1\x01\n\x19ScheduleWorkUpdateRequest\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aScheduleWorkUpdateResponse\x12L\n\rschedule_work\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWork\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19ScheduleWorkDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"g\n\x1aScheduleWorkDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x97\x05\n\x13ScheduleWorkService\x12\x9f\x01\n\x12ScheduleWorkCreate\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkCreateRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkCreateResponse"\x00\x12\x99\x01\n\x10ScheduleWorkRead\x12@.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkReadRequest\x1a\x41.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkReadResponse"\x00\x12\x9f\x01\n\x12ScheduleWorkUpdate\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkUpdateRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkUpdateResponse"\x00\x12\x9f\x01\n\x12ScheduleWorkDelete\x12\x42.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkDeleteRequest\x1a\x43.pro.omni.oms.api.v1.rules.schedule_work.ScheduleWorkDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.schedule_work_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_SCHEDULEWORK"]._serialized_start = 153
-    _globals["_SCHEDULEWORK"]._serialized_end = 437
-    _globals["_SCHEDULEWORKCREATEREQUEST"]._serialized_start = 440
-    _globals["_SCHEDULEWORKCREATEREQUEST"]._serialized_end = 590
-    _globals["_SCHEDULEWORKCREATERESPONSE"]._serialized_start = 593
-    _globals["_SCHEDULEWORKCREATERESPONSE"]._serialized_end = 774
-    _globals["_SCHEDULEWORKREADREQUEST"]._serialized_start = 777
-    _globals["_SCHEDULEWORKREADREQUEST"]._serialized_end = 1150
-    _globals["_SCHEDULEWORKREADRESPONSE"]._serialized_start = 1153
-    _globals["_SCHEDULEWORKREADRESPONSE"]._serialized_end = 1392
-    _globals["_SCHEDULEWORKUPDATEREQUEST"]._serialized_start = 1395
-    _globals["_SCHEDULEWORKUPDATEREQUEST"]._serialized_end = 1556
-    _globals["_SCHEDULEWORKUPDATERESPONSE"]._serialized_start = 1559
-    _globals["_SCHEDULEWORKUPDATERESPONSE"]._serialized_end = 1740
-    _globals["_SCHEDULEWORKDELETEREQUEST"]._serialized_start = 1742
-    _globals["_SCHEDULEWORKDELETEREQUEST"]._serialized_end = 1837
-    _globals["_SCHEDULEWORKDELETERESPONSE"]._serialized_start = 1839
-    _globals["_SCHEDULEWORKDELETERESPONSE"]._serialized_end = 1942
-    _globals["_SCHEDULEWORKSERVICE"]._serialized_start = 1945
-    _globals["_SCHEDULEWORKSERVICE"]._serialized_end = 2608
+    _globals["_SCHEDULEWORK"]._serialized_start = 185
+    _globals["_SCHEDULEWORK"]._serialized_end = 494
+    _globals["_SCHEDULEWORKCREATEREQUEST"]._serialized_start = 497
+    _globals["_SCHEDULEWORKCREATEREQUEST"]._serialized_end = 647
+    _globals["_SCHEDULEWORKCREATERESPONSE"]._serialized_start = 650
+    _globals["_SCHEDULEWORKCREATERESPONSE"]._serialized_end = 831
+    _globals["_SCHEDULEWORKREADREQUEST"]._serialized_start = 834
+    _globals["_SCHEDULEWORKREADREQUEST"]._serialized_end = 1207
+    _globals["_SCHEDULEWORKREADRESPONSE"]._serialized_start = 1210
+    _globals["_SCHEDULEWORKREADRESPONSE"]._serialized_end = 1449
+    _globals["_SCHEDULEWORKUPDATEREQUEST"]._serialized_start = 1452
+    _globals["_SCHEDULEWORKUPDATEREQUEST"]._serialized_end = 1613
+    _globals["_SCHEDULEWORKUPDATERESPONSE"]._serialized_start = 1616
+    _globals["_SCHEDULEWORKUPDATERESPONSE"]._serialized_end = 1797
+    _globals["_SCHEDULEWORKDELETEREQUEST"]._serialized_start = 1799
+    _globals["_SCHEDULEWORKDELETEREQUEST"]._serialized_end = 1894
+    _globals["_SCHEDULEWORKDELETERESPONSE"]._serialized_start = 1896
+    _globals["_SCHEDULEWORKDELETERESPONSE"]._serialized_end = 1999
+    _globals["_SCHEDULEWORKSERVICE"]._serialized_start = 2002
+    _globals["_SCHEDULEWORKSERVICE"]._serialized_end = 2665
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 from omni.pro.protos.v1.rules import calendar_pb2 as _calendar_pb2
 from omni.pro.protos.v1.rules import schedule_work_line_pb2 as _schedule_work_line_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ScheduleWork(_message.Message):
-    __slots__ = ["id", "name", "calendar_id", "schedule_work_line_ids", "active", "object_audit"]
+    __slots__ = ["id", "name", "calendar_id", "schedule_work_lines", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CALENDAR_ID_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_WORK_LINE_IDS_FIELD_NUMBER: _ClassVar[int]
+    SCHEDULE_WORK_LINES_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     calendar_id: _calendar_pb2.Calendar
-    schedule_work_line_ids: _containers.RepeatedCompositeFieldContainer[_schedule_work_line_pb2.ScheduleWorkLine]
-    active: bool
+    schedule_work_lines: _containers.RepeatedCompositeFieldContainer[_schedule_work_line_pb2.ScheduleWorkLine]
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         calendar_id: _Optional[_Union[_calendar_pb2.Calendar, _Mapping]] = ...,
-        schedule_work_line_ids: _Optional[_Iterable[_Union[_schedule_work_line_pb2.ScheduleWorkLine, _Mapping]]] = ...,
-        active: bool = ...,
+        schedule_work_lines: _Optional[_Iterable[_Union[_schedule_work_line_pb2.ScheduleWorkLine, _Mapping]]] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class ScheduleWorkCreateRequest(_message.Message):
     __slots__ = ["name", "calendar_id", "schedule_work_line_ids", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CALENDAR_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -2,141 +2,164 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class ScheduleWorkScheduleWorkLine(_message.Message):
-    __slots__ = ["id", "schedule_work_id", "schedule_work_line_id", "active", "object_audit"]
+class Tax(_message.Message):
+    __slots__ = ["id", "name", "code", "rate", "rounding", "decimal_places", "position", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_WORK_ID_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_WORK_LINE_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    schedule_work_id: int
-    schedule_work_line_id: int
-    active: bool
+    id: str
+    name: str
+    code: str
+    rate: float
+    rounding: float
+    decimal_places: int
+    position: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        schedule_work_id: _Optional[int] = ...,
-        schedule_work_line_id: _Optional[int] = ...,
-        active: bool = ...,
+        id: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        rate: _Optional[float] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        position: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineCreateRequest(_message.Message):
-    __slots__ = ["schedule_work_id", "schedule_work_line_id", "context"]
-    SCHEDULE_WORK_ID_FIELD_NUMBER: _ClassVar[int]
-    SCHEDULE_WORK_LINE_ID_FIELD_NUMBER: _ClassVar[int]
+class TaxAddRequest(_message.Message):
+    __slots__ = ["name", "code", "rate", "rounding", "decimal_places", "position", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    schedule_work_id: int
-    schedule_work_line_id: int
+    name: str
+    code: str
+    rate: float
+    rounding: float
+    decimal_places: int
+    position: str
     context: _base_pb2.Context
     def __init__(
         self,
-        schedule_work_id: _Optional[int] = ...,
-        schedule_work_line_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        rate: _Optional[float] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        position: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineCreateResponse(_message.Message):
-    __slots__ = ["schedule_work_schedule_work_line", "response_standard"]
-    SCHEDULE_WORK_SCHEDULE_WORK_LINE_FIELD_NUMBER: _ClassVar[int]
+class TaxAddResponse(_message.Message):
+    __slots__ = ["response_standard", "tax"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    schedule_work_schedule_work_line: ScheduleWorkScheduleWorkLine
+    TAX_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    tax: Tax
     def __init__(
         self,
-        schedule_work_schedule_work_line: _Optional[_Union[ScheduleWorkScheduleWorkLine, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineReadRequest(_message.Message):
+class TaxReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineReadResponse(_message.Message):
-    __slots__ = ["schedule_work_schedule_work_line", "meta_data", "response_standard"]
-    SCHEDULE_WORK_SCHEDULE_WORK_LINE_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+class TaxReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "taxes"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    schedule_work_schedule_work_line: _containers.RepeatedCompositeFieldContainer[ScheduleWorkScheduleWorkLine]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    TAXES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    taxes: _containers.RepeatedCompositeFieldContainer[Tax]
     def __init__(
         self,
-        schedule_work_schedule_work_line: _Optional[_Iterable[_Union[ScheduleWorkScheduleWorkLine, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        taxes: _Optional[_Iterable[_Union[Tax, _Mapping]]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineUpdateRequest(_message.Message):
-    __slots__ = ["schedule_work_schedule_work_line", "context"]
-    SCHEDULE_WORK_SCHEDULE_WORK_LINE_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateRequest(_message.Message):
+    __slots__ = ["tax", "context"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    schedule_work_schedule_work_line: ScheduleWorkScheduleWorkLine
+    tax: Tax
     context: _base_pb2.Context
     def __init__(
-        self,
-        schedule_work_schedule_work_line: _Optional[_Union[ScheduleWorkScheduleWorkLine, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, tax: _Optional[_Union[Tax, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineUpdateResponse(_message.Message):
-    __slots__ = ["schedule_work_schedule_work_line", "response_standard"]
-    SCHEDULE_WORK_SCHEDULE_WORK_LINE_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "tax"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    schedule_work_schedule_work_line: ScheduleWorkScheduleWorkLine
+    TAX_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    tax: Tax
     def __init__(
         self,
-        schedule_work_schedule_work_line: _Optional[_Union[ScheduleWorkScheduleWorkLine, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineDeleteRequest(_message.Message):
+class TaxDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ScheduleWorkScheduleWorkLineDeleteResponse(_message.Message):
+class TaxDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/warehouse_delivery_method.proto
+# source: v1/sales/picking.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n(v1/rules/warehouse_delivery_method.proto\x12\x33pro.omni.oms.api.v1.rules.warehouse_delivery_method\x1a\x11\x63ommon/base.proto"\xa8\x01\n\x17WarehouseDeliveryMethod\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x02 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x90\x01\n$WarehouseDeliveryMethodCreateRequest\x12\x14\n\x0cwarehouse_id\x18\x01 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n%WarehouseDeliveryMethodCreateResponse\x12o\n\x19warehouse_delivery_method\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x80\x03\n"WarehouseDeliveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9c\x02\n#WarehouseDeliveryMethodReadResponse\x12o\n\x19warehouse_delivery_method\x18\x01 \x03(\x0b\x32L.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xcf\x01\n$WarehouseDeliveryMethodUpdateRequest\x12o\n\x19warehouse_delivery_method\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n%WarehouseDeliveryMethodUpdateResponse\x12o\n\x19warehouse_delivery_method\x18\x01 \x01(\x0b\x32L.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"j\n$WarehouseDeliveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"r\n%WarehouseDeliveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x86\x07\n\x1eWarehouseDeliveryMethodService\x12\xd8\x01\n\x1dWarehouseDeliveryMethodCreate\x12Y.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodCreateRequest\x1aZ.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodCreateResponse"\x00\x12\xd2\x01\n\x1bWarehouseDeliveryMethodRead\x12W.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodReadRequest\x1aX.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodReadResponse"\x00\x12\xd8\x01\n\x1dWarehouseDeliveryMethodUpdate\x12Y.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodUpdateRequest\x1aZ.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodUpdateResponse"\x00\x12\xd8\x01\n\x1dWarehouseDeliveryMethodDelete\x12Y.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodDeleteRequest\x1aZ.pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/picking.proto\x12!pro.omni.oms.api.v1.sales.picking\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x11\x63ommon/base.proto"\xd3\x04\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x14 \x01(\x08\x12?\n\x0cobject_audit\x18\x15 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12-\n\tdate_done\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0b \x01(\x02\x12\x15\n\rtime_assigned\x18\x0c \x01(\x02\x12\x12\n\ncarrier_id\x18\r \x01(\x05\x12\x31\n\rdate_delivery\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x0f \x01(\t\x12\x10\n\x08group_id\x18\x10 \x01(\x05\x12\x0e\n\x06weight\x18\x11 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x12 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x13 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.sales.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.warehouse_delivery_method_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.picking_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_WAREHOUSEDELIVERYMETHOD"]._serialized_start = 117
-    _globals["_WAREHOUSEDELIVERYMETHOD"]._serialized_end = 285
-    _globals["_WAREHOUSEDELIVERYMETHODCREATEREQUEST"]._serialized_start = 288
-    _globals["_WAREHOUSEDELIVERYMETHODCREATEREQUEST"]._serialized_end = 432
-    _globals["_WAREHOUSEDELIVERYMETHODCREATERESPONSE"]._serialized_start = 435
-    _globals["_WAREHOUSEDELIVERYMETHODCREATERESPONSE"]._serialized_end = 662
-    _globals["_WAREHOUSEDELIVERYMETHODREADREQUEST"]._serialized_start = 665
-    _globals["_WAREHOUSEDELIVERYMETHODREADREQUEST"]._serialized_end = 1049
-    _globals["_WAREHOUSEDELIVERYMETHODREADRESPONSE"]._serialized_start = 1052
-    _globals["_WAREHOUSEDELIVERYMETHODREADRESPONSE"]._serialized_end = 1336
-    _globals["_WAREHOUSEDELIVERYMETHODUPDATEREQUEST"]._serialized_start = 1339
-    _globals["_WAREHOUSEDELIVERYMETHODUPDATEREQUEST"]._serialized_end = 1546
-    _globals["_WAREHOUSEDELIVERYMETHODUPDATERESPONSE"]._serialized_start = 1549
-    _globals["_WAREHOUSEDELIVERYMETHODUPDATERESPONSE"]._serialized_end = 1776
-    _globals["_WAREHOUSEDELIVERYMETHODDELETEREQUEST"]._serialized_start = 1778
-    _globals["_WAREHOUSEDELIVERYMETHODDELETEREQUEST"]._serialized_end = 1884
-    _globals["_WAREHOUSEDELIVERYMETHODDELETERESPONSE"]._serialized_start = 1886
-    _globals["_WAREHOUSEDELIVERYMETHODDELETERESPONSE"]._serialized_end = 2000
-    _globals["_WAREHOUSEDELIVERYMETHODSERVICE"]._serialized_start = 2003
-    _globals["_WAREHOUSEDELIVERYMETHODSERVICE"]._serialized_end = 2905
+    _globals["_PICKING"]._serialized_start = 114
+    _globals["_PICKING"]._serialized_end = 709
+    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 712
+    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1283
+    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1286
+    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1445
+    _globals["_PICKINGREADREQUEST"]._serialized_start = 1448
+    _globals["_PICKINGREADREQUEST"]._serialized_end = 1816
+    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1819
+    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2036
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2039
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2178
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2181
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2340
+    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2342
+    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2432
+    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2434
+    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2532
+    _globals["_PICKINGSERVICE"]._serialized_start = 2535
+    _globals["_PICKINGSERVICE"]._serialized_end = 3084
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,68 +2,70 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class WarehouseDeliveryMethod(_message.Message):
-    __slots__ = ["id", "warehouse_id", "delivery_method_id", "active", "object_audit"]
+class ProcurementGroup(_message.Message):
+    __slots__ = ["id", "name", "move_type", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    MOVE_TYPE_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    warehouse_id: int
-    delivery_method_id: int
-    active: bool
+    name: str
+    move_type: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        warehouse_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        active: bool = ...,
+        name: _Optional[str] = ...,
+        move_type: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodCreateRequest(_message.Message):
-    __slots__ = ["warehouse_id", "delivery_method_id", "context"]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
+class ProcurementGroupCreateRequest(_message.Message):
+    __slots__ = ["name", "move_type", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    MOVE_TYPE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse_id: int
-    delivery_method_id: int
+    name: str
+    move_type: str
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
+        name: _Optional[str] = ...,
+        move_type: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodCreateResponse(_message.Message):
-    __slots__ = ["warehouse_delivery_method", "response_standard"]
-    WAREHOUSE_DELIVERY_METHOD_FIELD_NUMBER: _ClassVar[int]
+class ProcurementGroupCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "procurement_group"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse_delivery_method: WarehouseDeliveryMethod
+    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    procurement_group: ProcurementGroup
     def __init__(
         self,
-        warehouse_delivery_method: _Optional[_Union[WarehouseDeliveryMethod, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodReadRequest(_message.Message):
+class ProcurementGroupReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -82,61 +84,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodReadResponse(_message.Message):
-    __slots__ = ["warehouse_delivery_method", "meta_data", "response_standard"]
-    WAREHOUSE_DELIVERY_METHOD_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+class ProcurementGroupReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "procurement_groups"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse_delivery_method: _containers.RepeatedCompositeFieldContainer[WarehouseDeliveryMethod]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    PROCUREMENT_GROUPS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    procurement_groups: _containers.RepeatedCompositeFieldContainer[ProcurementGroup]
     def __init__(
         self,
-        warehouse_delivery_method: _Optional[_Iterable[_Union[WarehouseDeliveryMethod, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        procurement_groups: _Optional[_Iterable[_Union[ProcurementGroup, _Mapping]]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodUpdateRequest(_message.Message):
-    __slots__ = ["warehouse_delivery_method", "context"]
-    WAREHOUSE_DELIVERY_METHOD_FIELD_NUMBER: _ClassVar[int]
+class ProcurementGroupUpdateRequest(_message.Message):
+    __slots__ = ["procurement_group", "context"]
+    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse_delivery_method: WarehouseDeliveryMethod
+    procurement_group: ProcurementGroup
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse_delivery_method: _Optional[_Union[WarehouseDeliveryMethod, _Mapping]] = ...,
+        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodUpdateResponse(_message.Message):
-    __slots__ = ["warehouse_delivery_method", "response_standard"]
-    WAREHOUSE_DELIVERY_METHOD_FIELD_NUMBER: _ClassVar[int]
+class ProcurementGroupUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "procurement_group"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse_delivery_method: WarehouseDeliveryMethod
+    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    procurement_group: ProcurementGroup
     def __init__(
         self,
-        warehouse_delivery_method: _Optional[_Union[WarehouseDeliveryMethod, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeliveryMethodDeleteRequest(_message.Message):
+class ProcurementGroupDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class WarehouseDeliveryMethodDeleteResponse(_message.Message):
+class ProcurementGroupDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.rules import warehouse_delivery_method_pb2 as v1_dot_rules_dot_warehouse__delivery__method__pb2
+from omni.pro.protos.v1.stock import warehouse_pb2 as v1_dot_stock_dot_warehouse__pb2
 
 
-class WarehouseDeliveryMethodServiceStub(object):
+class WarehouseServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.WarehouseDeliveryMethodCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodCreate",
-            request_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateResponse.FromString,
+        self.WarehouseCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseCreate",
+            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
         )
-        self.WarehouseDeliveryMethodRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodRead",
-            request_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadResponse.FromString,
+        self.WarehouseRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseRead",
+            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.FromString,
         )
-        self.WarehouseDeliveryMethodUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodUpdate",
-            request_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateResponse.FromString,
+        self.WarehouseUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseUpdate",
+            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
         )
-        self.WarehouseDeliveryMethodDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodDelete",
-            request_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteResponse.FromString,
+        self.WarehouseDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseDelete",
+            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
         )
 
 
-class WarehouseDeliveryMethodServiceServicer(object):
+class WarehouseServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def WarehouseDeliveryMethodCreate(self, request, context):
+    def WarehouseCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseDeliveryMethodRead(self, request, context):
+    def WarehouseRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseDeliveryMethodUpdate(self, request, context):
+    def WarehouseUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseDeliveryMethodDelete(self, request, context):
+    def WarehouseDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_WarehouseDeliveryMethodServiceServicer_to_server(servicer, server):
+def add_WarehouseServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "WarehouseDeliveryMethodCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDeliveryMethodCreate,
-            request_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateResponse.SerializeToString,
+        "WarehouseCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseCreate,
+            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.FromString,
+            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.SerializeToString,
         ),
-        "WarehouseDeliveryMethodRead": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDeliveryMethodRead,
-            request_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadRequest.FromString,
-            response_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadResponse.SerializeToString,
+        "WarehouseRead": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseRead,
+            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.FromString,
+            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.SerializeToString,
         ),
-        "WarehouseDeliveryMethodUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDeliveryMethodUpdate,
-            request_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateRequest.FromString,
-            response_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateResponse.SerializeToString,
+        "WarehouseUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseUpdate,
+            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.FromString,
+            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.SerializeToString,
         ),
-        "WarehouseDeliveryMethodDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDeliveryMethodDelete,
-            request_deserializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteRequest.FromString,
-            response_serializer=v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteResponse.SerializeToString,
+        "WarehouseDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.WarehouseDelete,
+            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.FromString,
+            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService", rpc_method_handlers
+        "pro.omni.oms.api.v1.stock.warehouse.WarehouseService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class WarehouseDeliveryMethodService(object):
+class WarehouseService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def WarehouseDeliveryMethodCreate(
+    def WarehouseCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodCreate",
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateRequest.SerializeToString,
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseCreate",
+            v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
+            v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseDeliveryMethodRead(
+    def WarehouseRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodRead",
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadRequest.SerializeToString,
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodReadResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseRead",
+            v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
+            v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseDeliveryMethodUpdate(
+    def WarehouseUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodUpdate",
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateRequest.SerializeToString,
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseUpdate",
+            v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
+            v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseDeliveryMethodDelete(
+    def WarehouseDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.rules.warehouse_delivery_method.WarehouseDeliveryMethodService/WarehouseDeliveryMethodDelete",
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteRequest.SerializeToString,
-            v1_dot_rules_dot_warehouse__delivery__method__pb2.WarehouseDeliveryMethodDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseDelete",
+            v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
+            v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/rules/warehouse_hierarchy.proto
+# source: v1/stock/rule.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
-from omni.pro.protos.v1.rules import location_pb2 as v1_dot_rules_dot_location__pb2
-from omni.pro.protos.v1.rules import warehouse_pb2 as v1_dot_rules_dot_warehouse__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n"v1/rules/warehouse_hierarchy.proto\x12-pro.omni.oms.api.v1.rules.warehouse_hierarchy\x1a\x11\x63ommon/base.proto\x1a\x18v1/rules/warehouse.proto\x1a\x17v1/rules/location.proto"\xbf\x02\n\x12WarehouseHierarchy\x12\n\n\x02id\x18\x01 \x01(\t\x12\x44\n\x0cwarehouse_id\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.v1.rules.warehouse.Warehouse\x12\x41\n\x0blocation_id\x18\t \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x19\n\x11quantity_security\x18\x04 \x01(\x02\x12\x10\n\x08sequence\x18\x05 \x01(\x05\x12\x16\n\x0esequence_order\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc9\x01\n\x1fWarehouseHierarchyCreateRequest\x12\x14\n\x0cwarehouse_id\x18\x01 \x01(\t\x12\x13\n\x0blocation_id\x18\x02 \x01(\t\x12\x19\n\x11quantity_security\x18\x03 \x01(\x02\x12\x10\n\x08sequence\x18\x04 \x01(\x05\x12\x16\n\x0esequence_order\x18\x05 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n WarehouseHierarchyCreateResponse\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xfb\x02\n\x1dWarehouseHierarchyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x87\x02\n\x1eWarehouseHierarchyReadResponse\x12_\n\x14warehouses_hierarchy\x18\x01 \x03(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xb9\x01\n\x1fWarehouseHierarchyUpdateRequest\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n WarehouseHierarchyUpdateResponse\x12^\n\x13warehouse_hierarchy\x18\x01 \x01(\x0b\x32\x41.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchy\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"e\n\x1fWarehouseHierarchyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"m\n WarehouseHierarchyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x95\x06\n\x19WarehouseHierarchyService\x12\xbd\x01\n\x18WarehouseHierarchyCreate\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyCreateRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyCreateResponse"\x00\x12\xb7\x01\n\x16WarehouseHierarchyRead\x12L.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyReadRequest\x1aM.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyReadResponse"\x00\x12\xbd\x01\n\x18WarehouseHierarchyUpdate\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyUpdateRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyUpdateResponse"\x00\x12\xbd\x01\n\x18WarehouseHierarchyDelete\x12N.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyDeleteRequest\x1aO.pro.omni.oms.api.v1.rules.warehouse_hierarchy.WarehouseHierarchyDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x13v1/stock/rule.proto\x12\x18pro.omni.oms.api.v1.rule\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x02\n\x04Rule\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x04 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x05 \x01(\x05\x12\x13\n\x0blocation_id\x18\x06 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x07 \x01(\t\x12\x10\n\x08route_id\x18\x08 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\t \x01(\x05\x12\x10\n\x08sequence\x18\n \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x82\x02\n\x11RuleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x04 \x01(\x05\x12\x13\n\x0blocation_id\x18\x05 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x06 \x01(\t\x12\x10\n\x08route_id\x18\x07 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x08 \x01(\x05\x12\x10\n\x08sequence\x18\t \x01(\x05\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"\xed\x02\n\x0fRuleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x10RuleReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12-\n\x05rules\x18\x03 \x03(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"y\n\x11RuleUpdateRequest\x12,\n\x04rule\x18\x01 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"W\n\x11RuleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12RuleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xb3\x03\n\x0bRuleService\x12i\n\nRuleCreate\x12+.pro.omni.oms.api.v1.rule.RuleCreateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleCreateResponse"\x00\x12\x63\n\x08RuleRead\x12).pro.omni.oms.api.v1.rule.RuleReadRequest\x1a*.pro.omni.oms.api.v1.rule.RuleReadResponse"\x00\x12i\n\nRuleUpdate\x12+.pro.omni.oms.api.v1.rule.RuleUpdateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleUpdateResponse"\x00\x12i\n\nRuleDelete\x12+.pro.omni.oms.api.v1.rule.RuleDeleteRequest\x1a,.pro.omni.oms.api.v1.rule.RuleDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.warehouse_hierarchy_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.rule_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_WAREHOUSEHIERARCHY"]._serialized_start = 156
-    _globals["_WAREHOUSEHIERARCHY"]._serialized_end = 475
-    _globals["_WAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_start = 478
-    _globals["_WAREHOUSEHIERARCHYCREATEREQUEST"]._serialized_end = 679
-    _globals["_WAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_start = 682
-    _globals["_WAREHOUSEHIERARCHYCREATERESPONSE"]._serialized_end = 887
-    _globals["_WAREHOUSEHIERARCHYREADREQUEST"]._serialized_start = 890
-    _globals["_WAREHOUSEHIERARCHYREADREQUEST"]._serialized_end = 1269
-    _globals["_WAREHOUSEHIERARCHYREADRESPONSE"]._serialized_start = 1272
-    _globals["_WAREHOUSEHIERARCHYREADRESPONSE"]._serialized_end = 1535
-    _globals["_WAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_start = 1538
-    _globals["_WAREHOUSEHIERARCHYUPDATEREQUEST"]._serialized_end = 1723
-    _globals["_WAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_start = 1726
-    _globals["_WAREHOUSEHIERARCHYUPDATERESPONSE"]._serialized_end = 1931
-    _globals["_WAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_start = 1933
-    _globals["_WAREHOUSEHIERARCHYDELETEREQUEST"]._serialized_end = 2034
-    _globals["_WAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_start = 2036
-    _globals["_WAREHOUSEHIERARCHYDELETERESPONSE"]._serialized_end = 2145
-    _globals["_WAREHOUSEHIERARCHYSERVICE"]._serialized_start = 2148
-    _globals["_WAREHOUSEHIERARCHYSERVICE"]._serialized_end = 2937
+    _globals["_RULE"]._serialized_start = 131
+    _globals["_RULE"]._serialized_end = 441
+    _globals["_RULECREATEREQUEST"]._serialized_start = 444
+    _globals["_RULECREATEREQUEST"]._serialized_end = 702
+    _globals["_RULECREATERESPONSE"]._serialized_start = 705
+    _globals["_RULECREATERESPONSE"]._serialized_end = 846
+    _globals["_RULEREADREQUEST"]._serialized_start = 849
+    _globals["_RULEREADREQUEST"]._serialized_end = 1214
+    _globals["_RULEREADRESPONSE"]._serialized_start = 1217
+    _globals["_RULEREADRESPONSE"]._serialized_end = 1416
+    _globals["_RULEUPDATEREQUEST"]._serialized_start = 1418
+    _globals["_RULEUPDATEREQUEST"]._serialized_end = 1539
+    _globals["_RULEUPDATERESPONSE"]._serialized_start = 1542
+    _globals["_RULEUPDATERESPONSE"]._serialized_end = 1683
+    _globals["_RULEDELETEREQUEST"]._serialized_start = 1685
+    _globals["_RULEDELETEREQUEST"]._serialized_end = 1772
+    _globals["_RULEDELETERESPONSE"]._serialized_start = 1774
+    _globals["_RULEDELETERESPONSE"]._serialized_end = 1869
+    _globals["_RULESERVICE"]._serialized_start = 1872
+    _globals["_RULESERVICE"]._serialized_end = 2307
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,170 +2,200 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
-from omni.pro.protos.v1.rules import location_pb2 as _location_pb2
-from omni.pro.protos.v1.rules import warehouse_pb2 as _warehouse_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class WarehouseHierarchy(_message.Message):
+class Sequence(_message.Message):
     __slots__ = [
         "id",
-        "warehouse_id",
-        "location_id",
-        "quantity_security",
-        "sequence",
-        "sequence_order",
+        "name",
+        "code",
+        "implementation",
+        "prefix",
+        "suffix",
+        "padding",
+        "number_increment",
+        "number_next_actual",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
-    QUANTITY_SECURITY_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_ORDER_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
+    PREFIX_FIELD_NUMBER: _ClassVar[int]
+    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    PADDING_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
-    warehouse_id: _warehouse_pb2.Warehouse
-    location_id: _location_pb2.Location
-    quantity_security: float
-    sequence: int
-    sequence_order: bool
-    active: bool
+    name: str
+    code: str
+    implementation: str
+    prefix: str
+    suffix: str
+    padding: float
+    number_increment: int
+    number_next_actual: int
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
-        warehouse_id: _Optional[_Union[_warehouse_pb2.Warehouse, _Mapping]] = ...,
-        location_id: _Optional[_Union[_location_pb2.Location, _Mapping]] = ...,
-        quantity_security: _Optional[float] = ...,
-        sequence: _Optional[int] = ...,
-        sequence_order: bool = ...,
-        active: bool = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        implementation: _Optional[str] = ...,
+        prefix: _Optional[str] = ...,
+        suffix: _Optional[str] = ...,
+        padding: _Optional[float] = ...,
+        number_increment: _Optional[int] = ...,
+        number_next_actual: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyCreateRequest(_message.Message):
-    __slots__ = ["warehouse_id", "location_id", "quantity_security", "sequence", "sequence_order", "context"]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
-    QUANTITY_SECURITY_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_ORDER_FIELD_NUMBER: _ClassVar[int]
+class SequenceCreateRequest(_message.Message):
+    __slots__ = [
+        "name",
+        "code",
+        "implementation",
+        "prefix",
+        "suffix",
+        "padding",
+        "number_increment",
+        "number_next_actual",
+        "context",
+    ]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
+    PREFIX_FIELD_NUMBER: _ClassVar[int]
+    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    PADDING_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse_id: str
-    location_id: str
-    quantity_security: float
-    sequence: int
-    sequence_order: bool
+    name: str
+    code: str
+    implementation: str
+    prefix: str
+    suffix: str
+    padding: float
+    number_increment: int
+    number_next_actual: int
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse_id: _Optional[str] = ...,
-        location_id: _Optional[str] = ...,
-        quantity_security: _Optional[float] = ...,
-        sequence: _Optional[int] = ...,
-        sequence_order: bool = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        implementation: _Optional[str] = ...,
+        prefix: _Optional[str] = ...,
+        suffix: _Optional[str] = ...,
+        padding: _Optional[float] = ...,
+        number_increment: _Optional[int] = ...,
+        number_next_actual: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyCreateResponse(_message.Message):
-    __slots__ = ["warehouse_hierarchy", "response_standard"]
-    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class SequenceCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "sequence"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse_hierarchy: WarehouseHierarchy
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    sequence: Sequence
     def __init__(
         self,
-        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyReadRequest(_message.Message):
+class SequenceReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyReadResponse(_message.Message):
-    __slots__ = ["warehouses_hierarchy", "meta_data", "response_standard"]
-    WAREHOUSES_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+class SequenceReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "sequences"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouses_hierarchy: _containers.RepeatedCompositeFieldContainer[WarehouseHierarchy]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    sequences: _containers.RepeatedCompositeFieldContainer[Sequence]
     def __init__(
         self,
-        warehouses_hierarchy: _Optional[_Iterable[_Union[WarehouseHierarchy, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        sequences: _Optional[_Iterable[_Union[Sequence, _Mapping]]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyUpdateRequest(_message.Message):
-    __slots__ = ["warehouse_hierarchy", "context"]
-    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class SequenceUpdateRequest(_message.Message):
+    __slots__ = ["sequence", "context"]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse_hierarchy: WarehouseHierarchy
+    sequence: Sequence
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyUpdateResponse(_message.Message):
-    __slots__ = ["warehouse_hierarchy", "response_standard"]
-    WAREHOUSE_HIERARCHY_FIELD_NUMBER: _ClassVar[int]
+class SequenceUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "sequence"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse_hierarchy: WarehouseHierarchy
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    sequence: Sequence
     def __init__(
         self,
-        warehouse_hierarchy: _Optional[_Union[WarehouseHierarchy, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseHierarchyDeleteRequest(_message.Message):
+class SequenceDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class WarehouseHierarchyDeleteResponse(_message.Message):
+class SequenceDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,71 +2,72 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Warehouse(_message.Message):
-    __slots__ = ["id", "name", "code", "warehouse_sql_id", "object_audit"]
+class Model(_message.Message):
+    __slots__ = ["id", "name", "model", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
-    code: str
-    warehouse_sql_id: str
+    model: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        code: _Optional[str] = ...,
-        warehouse_sql_id: _Optional[str] = ...,
+        model: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "warehouse_sql_id", "context"]
+class ModelCreateRequest(_message.Message):
+    __slots__ = ["name", "model", "active", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    code: str
-    warehouse_sql_id: str
+    model: str
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        code: _Optional[str] = ...,
-        warehouse_sql_id: _Optional[str] = ...,
+        model: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateResponse(_message.Message):
-    __slots__ = ["warehouse", "response_standard"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class ModelCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "model"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    model: Model
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadRequest(_message.Message):
+class ModelReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -85,61 +86,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadResponse(_message.Message):
-    __slots__ = ["warehouses", "meta_data", "response_standard"]
-    WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+class ModelReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "models"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouses: _containers.RepeatedCompositeFieldContainer[Warehouse]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    MODELS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    models: _containers.RepeatedCompositeFieldContainer[Model]
     def __init__(
         self,
-        warehouses: _Optional[_Iterable[_Union[Warehouse, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        models: _Optional[_Iterable[_Union[Model, _Mapping]]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateRequest(_message.Message):
-    __slots__ = ["warehouse", "context"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class ModelUpdateRequest(_message.Message):
+    __slots__ = ["model", "context"]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    model: Model
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateResponse(_message.Message):
-    __slots__ = ["warehouse", "response_standard"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class ModelUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "model"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    model: Model
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeleteRequest(_message.Message):
+class ModelDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class WarehouseDeleteResponse(_message.Message):
+class ModelDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/address_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/carrier_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/channel_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/client_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/country_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/currency_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/sales/delivery_method.proto
+# source: v1/utilities/tax.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1ev1/sales/delivery_method.proto\x12)pro.omni.oms.api.v1.sales.delivery.method\x1a\x11\x63ommon/base.proto"\x89\x01\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"q\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc5\x05\n\x15\x44\x65liveryMethodService\x12\xaa\x01\n\x15\x44\x65liveryServiceCreate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryServiceRead\x12\x44.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceUpdate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceDelete\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/tax.proto\x12!pro.omni.oms.api.v1.utilities.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xe4\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04rate\x18\x04 \x01(\x02\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x06 \x01(\x05\x12\x10\n\x08position\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\t \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xad\x01\n\rTaxAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04rate\x18\x03 \x01(\x02\x12\x10\n\x08rounding\x18\x04 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x05 \x01(\x05\x12\x10\n\x08position\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x90\x01\n\x0eTaxAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xce\x01\n\x0fTaxReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x35\n\x05taxes\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"\x7f\n\x10TaxUpdateRequest\x12\x33\n\x03tax\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11TaxUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03tax\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.tax.Tax"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe5\x03\n\nTaxService\x12o\n\x06TaxAdd\x12\x30.pro.omni.oms.api.v1.utilities.tax.TaxAddRequest\x1a\x31.pro.omni.oms.api.v1.utilities.tax.TaxAddResponse"\x00\x12r\n\x07TaxRead\x12\x31.pro.omni.oms.api.v1.utilities.tax.TaxReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.tax.TaxReadResponse"\x00\x12x\n\tTaxUpdate\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxUpdateResponse"\x00\x12x\n\tTaxDelete\x12\x33.pro.omni.oms.api.v1.utilities.tax.TaxDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.tax.TaxDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.delivery_method_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.tax_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYMETHOD"]._serialized_start = 97
-    _globals["_DELIVERYMETHOD"]._serialized_end = 234
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 236
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 349
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 352
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 541
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 544
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 919
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 922
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 1169
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 1172
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 1341
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 1344
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 1533
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 1535
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 1632
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 1634
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 1739
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 1742
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 2451
+    _globals["_TAX"]._serialized_start = 113
+    _globals["_TAX"]._serialized_end = 341
+    _globals["_TAXADDREQUEST"]._serialized_start = 344
+    _globals["_TAXADDREQUEST"]._serialized_end = 517
+    _globals["_TAXADDRESPONSE"]._serialized_start = 520
+    _globals["_TAXADDRESPONSE"]._serialized_end = 664
+    _globals["_TAXREADREQUEST"]._serialized_start = 667
+    _globals["_TAXREADREQUEST"]._serialized_end = 1031
+    _globals["_TAXREADRESPONSE"]._serialized_start = 1034
+    _globals["_TAXREADRESPONSE"]._serialized_end = 1240
+    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1242
+    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1369
+    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1372
+    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1519
+    _globals["_TAXDELETEREQUEST"]._serialized_start = 1521
+    _globals["_TAXDELETEREQUEST"]._serialized_end = 1607
+    _globals["_TAXDELETERESPONSE"]._serialized_start = 1609
+    _globals["_TAXDELETERESPONSE"]._serialized_end = 1703
+    _globals["_TAXSERVICE"]._serialized_start = 1706
+    _globals["_TAXSERVICE"]._serialized_end = 2191
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_line_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,134 +2,119 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Order(_message.Message):
+class StockMove(_message.Message):
     __slots__ = [
         "id",
-        "name",
-        "sale_id",
-        "ship_address_id",
-        "delivery_method_id",
-        "carrier_id",
-        "payment_method_id",
-        "tax_total",
-        "subtotal",
-        "total",
+        "picking_id",
+        "state",
+        "product_id",
+        "product_uom_qty",
+        "quantity_done",
+        "product_uom_id",
+        "description_picking",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SALE_ID_FIELD_NUMBER: _ClassVar[int]
-    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
-    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    PICKING_ID_FIELD_NUMBER: _ClassVar[int]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_UOM_QTY_FIELD_NUMBER: _ClassVar[int]
+    QUANTITY_DONE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_UOM_ID_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_PICKING_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    name: str
-    sale_id: int
-    ship_address_id: int
-    delivery_method_id: int
-    carrier_id: int
-    payment_method_id: int
-    tax_total: float
-    subtotal: float
-    total: float
-    active: bool
+    picking_id: int
+    state: str
+    product_id: int
+    product_uom_qty: float
+    quantity_done: float
+    product_uom_id: int
+    description_picking: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        name: _Optional[str] = ...,
-        sale_id: _Optional[int] = ...,
-        ship_address_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        carrier_id: _Optional[int] = ...,
-        payment_method_id: _Optional[int] = ...,
-        tax_total: _Optional[float] = ...,
-        subtotal: _Optional[float] = ...,
-        total: _Optional[float] = ...,
-        active: bool = ...,
+        picking_id: _Optional[int] = ...,
+        state: _Optional[str] = ...,
+        product_id: _Optional[int] = ...,
+        product_uom_qty: _Optional[float] = ...,
+        quantity_done: _Optional[float] = ...,
+        product_uom_id: _Optional[int] = ...,
+        description_picking: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderCreateRequest(_message.Message):
+class StockMoveCreateRequest(_message.Message):
     __slots__ = [
-        "name",
-        "sale_id",
-        "ship_address_id",
-        "delivery_method_id",
-        "carrier_id",
-        "payment_method_id",
-        "tax_total",
-        "subtotal",
-        "total",
+        "picking_id",
+        "state",
+        "product_id",
+        "product_uom_qty",
+        "quantity_done",
+        "product_uom_id",
+        "description_picking",
         "context",
     ]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SALE_ID_FIELD_NUMBER: _ClassVar[int]
-    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
-    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    PICKING_ID_FIELD_NUMBER: _ClassVar[int]
+    STATE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_UOM_QTY_FIELD_NUMBER: _ClassVar[int]
+    QUANTITY_DONE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_UOM_ID_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_PICKING_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    sale_id: int
-    ship_address_id: int
-    delivery_method_id: int
-    carrier_id: int
-    payment_method_id: int
-    tax_total: float
-    subtotal: float
-    total: float
+    picking_id: int
+    state: str
+    product_id: int
+    product_uom_qty: float
+    quantity_done: float
+    product_uom_id: int
+    description_picking: str
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
-        sale_id: _Optional[int] = ...,
-        ship_address_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        carrier_id: _Optional[int] = ...,
-        payment_method_id: _Optional[int] = ...,
-        tax_total: _Optional[float] = ...,
-        subtotal: _Optional[float] = ...,
-        total: _Optional[float] = ...,
+        picking_id: _Optional[int] = ...,
+        state: _Optional[str] = ...,
+        product_id: _Optional[int] = ...,
+        product_uom_qty: _Optional[float] = ...,
+        quantity_done: _Optional[float] = ...,
+        product_uom_id: _Optional[int] = ...,
+        description_picking: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderCreateResponse(_message.Message):
-    __slots__ = ["order", "response_standard"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class StockMoveCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "stock_move"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    stock_move: StockMove
     def __init__(
         self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderReadRequest(_message.Message):
+class StockMoveReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -148,61 +133,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderReadResponse(_message.Message):
-    __slots__ = ["order", "response_standard", "meta_data"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class StockMoveReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "stock_moves"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    order: _containers.RepeatedCompositeFieldContainer[Order]
+    STOCK_MOVES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
+    stock_moves: _containers.RepeatedCompositeFieldContainer[StockMove]
     def __init__(
         self,
-        order: _Optional[_Iterable[_Union[Order, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        stock_moves: _Optional[_Iterable[_Union[StockMove, _Mapping]]] = ...,
     ) -> None: ...
 
-class OrderUpdateRequest(_message.Message):
-    __slots__ = ["order", "context"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class StockMoveUpdateRequest(_message.Message):
+    __slots__ = ["stock_move", "context"]
+    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    stock_move: StockMove
     context: _base_pb2.Context
     def __init__(
         self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
+        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderUpdateResponse(_message.Message):
-    __slots__ = ["order", "response_standard"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class StockMoveUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "stock_move"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    stock_move: StockMove
     def __init__(
         self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderDeleteRequest(_message.Message):
+class StockMoveDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class OrderDeleteResponse(_message.Message):
+class StockMoveDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/order_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/sales/picking.proto
+# source: v1/stock/picking.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/picking.proto\x12!pro.omni.oms.api.v1.sales.picking\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x11\x63ommon/base.proto"\xd3\x04\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x14 \x01(\x08\x12?\n\x0cobject_audit\x18\x15 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12-\n\tdate_done\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0b \x01(\x02\x12\x15\n\rtime_assigned\x18\x0c \x01(\x02\x12\x12\n\ncarrier_id\x18\r \x01(\x05\x12\x31\n\rdate_delivery\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x0f \x01(\t\x12\x10\n\x08group_id\x18\x10 \x01(\x05\x12\x0e\n\x06weight\x18\x11 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x12 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x13 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.sales.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/stock/picking.proto\x12!pro.omni.oms.api.v1.stock.picking\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xab\x05\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12:\n\x16\x64\x61te_start_preparation\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tdate_done\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\r \x01(\x02\x12\x15\n\rtime_assigned\x18\x0e \x01(\x02\x12\x12\n\ncarrier_id\x18\x0f \x01(\x05\x12\x31\n\rdate_delivery\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x11 \x01(\t\x12\x10\n\x08group_id\x18\x12 \x01(\x05\x12\x0e\n\x06weight\x18\x13 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x14 \x01(\x02\x12*\n\x06\x61\x63tive\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x16 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xf7\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12:\n\x16\x64\x61te_start_preparation\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x14 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.stock.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.stock.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.picking_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.picking_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PICKING"]._serialized_start = 114
-    _globals["_PICKING"]._serialized_end = 709
-    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 712
-    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1283
-    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1286
-    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1445
-    _globals["_PICKINGREADREQUEST"]._serialized_start = 1448
-    _globals["_PICKINGREADREQUEST"]._serialized_end = 1816
-    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1819
-    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2036
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2039
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2178
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2181
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2340
-    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2342
-    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2432
-    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2434
-    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2532
-    _globals["_PICKINGSERVICE"]._serialized_start = 2535
-    _globals["_PICKINGSERVICE"]._serialized_end = 3084
+    _globals["_PICKING"]._serialized_start = 146
+    _globals["_PICKING"]._serialized_end = 829
+    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 832
+    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1463
+    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1466
+    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1625
+    _globals["_PICKINGREADREQUEST"]._serialized_start = 1628
+    _globals["_PICKINGREADREQUEST"]._serialized_end = 1996
+    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1999
+    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2216
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2219
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2358
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2361
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2520
+    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2522
+    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2612
+    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2614
+    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2712
+    _globals["_PICKINGSERVICE"]._serialized_start = 2715
+    _globals["_PICKINGSERVICE"]._serialized_end = 3264
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/picking_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/product_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/sale_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/sale_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/tax_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/uom_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/user_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/sales/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,144 +2,148 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Warehouse(_message.Message):
-    __slots__ = ["id", "name", "code", "warehouse_sql_id", "object_audit"]
+class Country(_message.Message):
+    __slots__ = ["id", "name", "code", "country_doc_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    COUNTRY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
     code: str
-    warehouse_sql_id: int
+    country_doc_id: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        warehouse_sql_id: _Optional[int] = ...,
+        country_doc_id: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "warehouse_sql_id", "context"]
+class CountryCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "category_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    CATEGORY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    warehouse_sql_id: int
+    category_doc_id: str
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        warehouse_sql_id: _Optional[int] = ...,
+        category_doc_id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseCreateResponse(_message.Message):
-    __slots__ = ["warehouse", "response_standard"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class CountryCreateResponse(_message.Message):
+    __slots__ = ["country", "response_standard"]
+    COUNTRY_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    country: Country
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        country: _Optional[_Union[Country, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadRequest(_message.Message):
+class CountryReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseReadResponse(_message.Message):
-    __slots__ = ["warehouses", "meta_data", "response_standard"]
-    WAREHOUSES_FIELD_NUMBER: _ClassVar[int]
+class CountryReadResponse(_message.Message):
+    __slots__ = ["countries", "meta_data", "response_standard"]
+    COUNTRIES_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouses: _containers.RepeatedCompositeFieldContainer[Warehouse]
+    countries: _containers.RepeatedCompositeFieldContainer[Country]
     meta_data: _base_pb2.MetaData
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        warehouses: _Optional[_Iterable[_Union[Warehouse, _Mapping]]] = ...,
+        countries: _Optional[_Iterable[_Union[Country, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateRequest(_message.Message):
-    __slots__ = ["warehouse", "context"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class CountryUpdateRequest(_message.Message):
+    __slots__ = ["country", "context"]
+    COUNTRY_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    country: Country
     context: _base_pb2.Context
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        country: _Optional[_Union[Country, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseUpdateResponse(_message.Message):
-    __slots__ = ["warehouse", "response_standard"]
-    WAREHOUSE_FIELD_NUMBER: _ClassVar[int]
+class CountryUpdateResponse(_message.Message):
+    __slots__ = ["country", "response_standard"]
+    COUNTRY_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    warehouse: Warehouse
+    country: Country
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        warehouse: _Optional[_Union[Warehouse, _Mapping]] = ...,
+        country: _Optional[_Union[Country, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class WarehouseDeleteRequest(_message.Message):
+class CountryDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class WarehouseDeleteResponse(_message.Message):
+class CountryDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.sales import warehouse_pb2 as v1_dot_sales_dot_warehouse__pb2
+from omni.pro.protos.v1.utilities import sequence_pb2 as v1_dot_utilities_dot_sequence__pb2
 
 
-class WarehouseServiceStub(object):
+class SequenceServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.WarehouseCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseCreate",
-            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
+        self.SequenceCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceCreate",
+            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.FromString,
         )
-        self.WarehouseRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseRead",
-            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
-            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.FromString,
+        self.SequenceRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceRead",
+            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.FromString,
         )
-        self.WarehouseUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseUpdate",
-            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
+        self.SequenceUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceUpdate",
+            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.FromString,
         )
-        self.WarehouseDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseDelete",
-            request_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
+        self.SequenceDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceDelete",
+            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.FromString,
         )
 
 
-class WarehouseServiceServicer(object):
+class SequenceServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def WarehouseCreate(self, request, context):
+    def SequenceCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseRead(self, request, context):
+    def SequenceRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseUpdate(self, request, context):
+    def SequenceUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseDelete(self, request, context):
+    def SequenceDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_WarehouseServiceServicer_to_server(servicer, server):
+def add_SequenceServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "WarehouseCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseCreate,
-            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.FromString,
-            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.SerializeToString,
+        "SequenceCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.SequenceCreate,
+            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.SerializeToString,
         ),
-        "WarehouseRead": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseRead,
-            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.FromString,
-            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.SerializeToString,
+        "SequenceRead": grpc.unary_unary_rpc_method_handler(
+            servicer.SequenceRead,
+            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.SerializeToString,
         ),
-        "WarehouseUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseUpdate,
-            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.FromString,
-            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.SerializeToString,
+        "SequenceUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.SequenceUpdate,
+            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.SerializeToString,
         ),
-        "WarehouseDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDelete,
-            request_deserializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.FromString,
-            response_serializer=v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.SerializeToString,
+        "SequenceDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.SequenceDelete,
+            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.sales.warehouse.WarehouseService", rpc_method_handlers
+        "pro.omni.oms.api.v1.utilities.sequence.SequenceService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class WarehouseService(object):
+class SequenceService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def WarehouseCreate(
+    def SequenceCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseCreate",
-            v1_dot_sales_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
-            v1_dot_sales_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceCreate",
+            v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.SerializeToString,
+            v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseRead(
+    def SequenceRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseRead",
-            v1_dot_sales_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
-            v1_dot_sales_dot_warehouse__pb2.WarehouseReadResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceRead",
+            v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.SerializeToString,
+            v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseUpdate(
+    def SequenceUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseUpdate",
-            v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
-            v1_dot_sales_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceUpdate",
+            v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.SerializeToString,
+            v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseDelete(
+    def SequenceDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.sales.warehouse.WarehouseService/WarehouseDelete",
-            v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
-            v1_dot_sales_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceDelete",
+            v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.SerializeToString,
+            v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/attachment_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/carrier_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/country_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/location_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/picking.proto
+# source: v1/stock/picking_type.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
+from omni.pro.protos.v1.stock import sequence_pb2 as v1_dot_stock_dot_sequence__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/stock/picking.proto\x12!pro.omni.oms.api.v1.stock.picking\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xab\x05\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12:\n\x16\x64\x61te_start_preparation\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tdate_done\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\r \x01(\x02\x12\x15\n\rtime_assigned\x18\x0e \x01(\x02\x12\x12\n\ncarrier_id\x18\x0f \x01(\x05\x12\x31\n\rdate_delivery\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x11 \x01(\t\x12\x10\n\x08group_id\x18\x12 \x01(\x05\x12\x0e\n\x06weight\x18\x13 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x14 \x01(\x02\x12*\n\x06\x61\x63tive\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x16 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xf7\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12:\n\x16\x64\x61te_start_preparation\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x14 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.stock.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.stock.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.stock.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.stock.picking.PickingDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1bv1/stock/picking_type.proto\x12&pro.omni.oms.api.v1.stock.picking_type\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17v1/stock/sequence.proto"\x9d\x04\n\x0bPickingType\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rsequence_code\x18\x03 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x04 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x06 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\t \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\n \x01(\x05\x12\x41\n\x0bsequence_id\x18\x0b \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.sequence.Sequence\x12\x0f\n\x07\x62\x61rcode\x18\x0c \x01(\t\x12\x1a\n\x12reservation_method\x18\r \x01(\t\x12\x11\n\ttype_code\x18\x0e \x01(\t\x12*\n\x06\x61\x63tive\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x10 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x03\n\x18PickingTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rsequence_code\x18\x02 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x05 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\x08 \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\t \x01(\x05\x12\x0f\n\x07\x62\x61rcode\x18\n \x01(\t\x12\x1a\n\x12reservation_method\x18\x0b \x01(\t\x12\x11\n\ttype_code\x18\x0c \x01(\t\x12\x13\n\x0bsequence_id\x18\r \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0e \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\xf4\x02\n\x16PickingTypeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xeb\x01\n\x17PickingTypeReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12J\n\rpicking_types\x18\x03 \x03(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\x9d\x01\n\x18PickingTypeUpdateRequest\x12I\n\x0cpicking_type\x18\x01 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"^\n\x18PickingTypeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"f\n\x19PickingTypeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x82\x05\n\x12PickingTypeService\x12\x9a\x01\n\x11PickingTypeCreate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateResponse"\x00\x12\x94\x01\n\x0fPickingTypeRead\x12>.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadRequest\x1a?.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadResponse"\x00\x12\x9a\x01\n\x11PickingTypeUpdate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateResponse"\x00\x12\x9a\x01\n\x11PickingTypeDelete\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.picking_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.picking_type_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PICKING"]._serialized_start = 146
-    _globals["_PICKING"]._serialized_end = 829
-    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 832
-    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1463
-    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1466
-    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1625
-    _globals["_PICKINGREADREQUEST"]._serialized_start = 1628
-    _globals["_PICKINGREADREQUEST"]._serialized_end = 1996
-    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1999
-    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2216
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2219
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2358
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2361
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2520
-    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2522
-    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2612
-    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2614
-    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2712
-    _globals["_PICKINGSERVICE"]._serialized_start = 2715
-    _globals["_PICKINGSERVICE"]._serialized_end = 3264
+    _globals["_PICKINGTYPE"]._serialized_start = 148
+    _globals["_PICKINGTYPE"]._serialized_end = 689
+    _globals["_PICKINGTYPECREATEREQUEST"]._serialized_start = 692
+    _globals["_PICKINGTYPECREATEREQUEST"]._serialized_end = 1135
+    _globals["_PICKINGTYPECREATERESPONSE"]._serialized_start = 1138
+    _globals["_PICKINGTYPECREATERESPONSE"]._serialized_end = 1315
+    _globals["_PICKINGTYPEREADREQUEST"]._serialized_start = 1318
+    _globals["_PICKINGTYPEREADREQUEST"]._serialized_end = 1690
+    _globals["_PICKINGTYPEREADRESPONSE"]._serialized_start = 1693
+    _globals["_PICKINGTYPEREADRESPONSE"]._serialized_end = 1928
+    _globals["_PICKINGTYPEUPDATEREQUEST"]._serialized_start = 1931
+    _globals["_PICKINGTYPEUPDATEREQUEST"]._serialized_end = 2088
+    _globals["_PICKINGTYPEUPDATERESPONSE"]._serialized_start = 2091
+    _globals["_PICKINGTYPEUPDATERESPONSE"]._serialized_end = 2268
+    _globals["_PICKINGTYPEDELETEREQUEST"]._serialized_start = 2270
+    _globals["_PICKINGTYPEDELETEREQUEST"]._serialized_end = 2364
+    _globals["_PICKINGTYPEDELETERESPONSE"]._serialized_start = 2366
+    _globals["_PICKINGTYPEDELETERESPONSE"]._serialized_end = 2468
+    _globals["_PICKINGTYPESERVICE"]._serialized_start = 2471
+    _globals["_PICKINGTYPESERVICE"]._serialized_end = 3113
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/picking_type.proto
+# source: v1/utilities/currency.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bv1/stock/picking_type.proto\x12&pro.omni.oms.api.v1.stock.picking_type\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x9a\x03\n\x0bPickingType\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rsequence_code\x18\x03 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x04 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x05 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x06 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\t \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\n \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe6\x02\n\x18PickingTypeCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rsequence_code\x18\x02 \x01(\t\x12\x14\n\x0cwarehouse_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x1e\n\x16return_picking_type_id\x18\x05 \x01(\x05\x12\x33\n\x0fshow_operations\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x31\n\rshow_reserved\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x1f\n\x17\x64\x65\x66\x61ult_location_src_id\x18\x08 \x01(\x05\x12 \n\x18\x64\x65\x66\x61ult_location_dest_id\x18\t \x01(\x05\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\xf4\x02\n\x16PickingTypeReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xeb\x01\n\x17PickingTypeReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12J\n\rpicking_types\x18\x03 \x03(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"\x9d\x01\n\x18PickingTypeUpdateRequest\x12I\n\x0cpicking_type\x18\x01 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb1\x01\n\x19PickingTypeUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12I\n\x0cpicking_type\x18\x02 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType"^\n\x18PickingTypeDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"f\n\x19PickingTypeDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x82\x05\n\x12PickingTypeService\x12\x9a\x01\n\x11PickingTypeCreate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeCreateResponse"\x00\x12\x94\x01\n\x0fPickingTypeRead\x12>.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadRequest\x1a?.pro.omni.oms.api.v1.stock.picking_type.PickingTypeReadResponse"\x00\x12\x9a\x01\n\x11PickingTypeUpdate\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeUpdateResponse"\x00\x12\x9a\x01\n\x11PickingTypeDelete\x12@.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteRequest\x1a\x41.pro.omni.oms.api.v1.stock.picking_type.PickingTypeDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1bv1/utilities/currency.proto\x12&pro.omni.oms.api.v1.utilities.currency\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x02\n\x08\x43urrency\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x1b\n\x13\x63urrency_unit_label\x18\x04 \x01(\t\x12\x1e\n\x16\x63urrency_subunit_label\x18\x05 \x01(\t\x12\x0c\n\x04rate\x18\x06 \x01(\x05\x12\x10\n\x08rounding\x18\x07 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x08 \x01(\x05\x12\x0e\n\x06symbol\x18\t \x01(\t\x12\x10\n\x08position\x18\n \x01(\t\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xab\x02\n\x12\x43urrencyAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrency_unit_label\x18\x03 \x01(\t\x12\x1e\n\x16\x63urrency_subunit_label\x18\x04 \x01(\t\x12\x0c\n\x04rate\x18\x05 \x01(\x05\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x07 \x01(\x05\x12\x0e\n\x06symbol\x18\x08 \x01(\t\x12\x10\n\x08position\x18\t \x01(\t\x12*\n\x06\x61\x63tive\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x0b \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa4\x01\n\x13\x43urrencyAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08\x63urrency\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"\xf1\x02\n\x13\x43urrencyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe2\x01\n\x14\x43urrencyReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\ncurrencies\x18\x03 \x03(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"\x93\x01\n\x15\x43urrencyUpdateRequest\x12\x42\n\x08\x63urrency\x18\x01 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x16\x43urrencyUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08\x63urrency\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"[\n\x15\x43urrencyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43urrencyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd2\x04\n\x0f\x43urrencyService\x12\x88\x01\n\x0b\x43urrencyAdd\x12:.pro.omni.oms.api.v1.utilities.currency.CurrencyAddRequest\x1a;.pro.omni.oms.api.v1.utilities.currency.CurrencyAddResponse"\x00\x12\x8b\x01\n\x0c\x43urrencyRead\x12;.pro.omni.oms.api.v1.utilities.currency.CurrencyReadRequest\x1a<.pro.omni.oms.api.v1.utilities.currency.CurrencyReadResponse"\x00\x12\x91\x01\n\x0e\x43urrencyUpdate\x12=.pro.omni.oms.api.v1.utilities.currency.CurrencyUpdateRequest\x1a>.pro.omni.oms.api.v1.utilities.currency.CurrencyUpdateResponse"\x00\x12\x91\x01\n\x0e\x43urrencyDelete\x12=.pro.omni.oms.api.v1.utilities.currency.CurrencyDeleteRequest\x1a>.pro.omni.oms.api.v1.utilities.currency.CurrencyDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.picking_type_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.currency_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PICKINGTYPE"]._serialized_start = 123
-    _globals["_PICKINGTYPE"]._serialized_end = 533
-    _globals["_PICKINGTYPECREATEREQUEST"]._serialized_start = 536
-    _globals["_PICKINGTYPECREATEREQUEST"]._serialized_end = 894
-    _globals["_PICKINGTYPECREATERESPONSE"]._serialized_start = 897
-    _globals["_PICKINGTYPECREATERESPONSE"]._serialized_end = 1074
-    _globals["_PICKINGTYPEREADREQUEST"]._serialized_start = 1077
-    _globals["_PICKINGTYPEREADREQUEST"]._serialized_end = 1449
-    _globals["_PICKINGTYPEREADRESPONSE"]._serialized_start = 1452
-    _globals["_PICKINGTYPEREADRESPONSE"]._serialized_end = 1687
-    _globals["_PICKINGTYPEUPDATEREQUEST"]._serialized_start = 1690
-    _globals["_PICKINGTYPEUPDATEREQUEST"]._serialized_end = 1847
-    _globals["_PICKINGTYPEUPDATERESPONSE"]._serialized_start = 1850
-    _globals["_PICKINGTYPEUPDATERESPONSE"]._serialized_end = 2027
-    _globals["_PICKINGTYPEDELETEREQUEST"]._serialized_start = 2029
-    _globals["_PICKINGTYPEDELETEREQUEST"]._serialized_end = 2123
-    _globals["_PICKINGTYPEDELETERESPONSE"]._serialized_start = 2125
-    _globals["_PICKINGTYPEDELETERESPONSE"]._serialized_end = 2227
-    _globals["_PICKINGTYPESERVICE"]._serialized_start = 2230
-    _globals["_PICKINGTYPESERVICE"]._serialized_end = 2872
+    _globals["_CURRENCY"]._serialized_start = 123
+    _globals["_CURRENCY"]._serialized_end = 433
+    _globals["_CURRENCYADDREQUEST"]._serialized_start = 436
+    _globals["_CURRENCYADDREQUEST"]._serialized_end = 735
+    _globals["_CURRENCYADDRESPONSE"]._serialized_start = 738
+    _globals["_CURRENCYADDRESPONSE"]._serialized_end = 902
+    _globals["_CURRENCYREADREQUEST"]._serialized_start = 905
+    _globals["_CURRENCYREADREQUEST"]._serialized_end = 1274
+    _globals["_CURRENCYREADRESPONSE"]._serialized_start = 1277
+    _globals["_CURRENCYREADRESPONSE"]._serialized_end = 1503
+    _globals["_CURRENCYUPDATEREQUEST"]._serialized_start = 1506
+    _globals["_CURRENCYUPDATEREQUEST"]._serialized_end = 1653
+    _globals["_CURRENCYUPDATERESPONSE"]._serialized_start = 1656
+    _globals["_CURRENCYUPDATERESPONSE"]._serialized_end = 1823
+    _globals["_CURRENCYDELETEREQUEST"]._serialized_start = 1825
+    _globals["_CURRENCYDELETEREQUEST"]._serialized_end = 1916
+    _globals["_CURRENCYDELETERESPONSE"]._serialized_start = 1918
+    _globals["_CURRENCYDELETERESPONSE"]._serialized_end = 2017
+    _globals["_CURRENCYSERVICE"]._serialized_start = 2020
+    _globals["_CURRENCYSERVICE"]._serialized_end = 2614
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
+from omni.pro.protos.v1.stock import sequence_pb2 as _sequence_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PickingType(_message.Message):
     __slots__ = [
         "id",
         "name",
@@ -20,53 +21,69 @@
         "warehouse_id",
         "code",
         "return_picking_type_id",
         "show_operations",
         "show_reserved",
         "default_location_src_id",
         "default_location_dest_id",
+        "sequence_id",
+        "barcode",
+        "reservation_method",
+        "type_code",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SEQUENCE_CODE_FIELD_NUMBER: _ClassVar[int]
     WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     RETURN_PICKING_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     SHOW_OPERATIONS_FIELD_NUMBER: _ClassVar[int]
     SHOW_RESERVED_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_LOCATION_SRC_ID_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_LOCATION_DEST_ID_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_ID_FIELD_NUMBER: _ClassVar[int]
+    BARCODE_FIELD_NUMBER: _ClassVar[int]
+    RESERVATION_METHOD_FIELD_NUMBER: _ClassVar[int]
+    TYPE_CODE_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     sequence_code: str
     warehouse_id: int
     code: str
     return_picking_type_id: int
     show_operations: _wrappers_pb2.BoolValue
     show_reserved: _wrappers_pb2.BoolValue
     default_location_src_id: int
     default_location_dest_id: int
+    sequence_id: _sequence_pb2.Sequence
+    barcode: str
+    reservation_method: str
+    type_code: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         sequence_code: _Optional[str] = ...,
         warehouse_id: _Optional[int] = ...,
         code: _Optional[str] = ...,
         return_picking_type_id: _Optional[int] = ...,
         show_operations: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         show_reserved: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         default_location_src_id: _Optional[int] = ...,
         default_location_dest_id: _Optional[int] = ...,
+        sequence_id: _Optional[_Union[_sequence_pb2.Sequence, _Mapping]] = ...,
+        barcode: _Optional[str] = ...,
+        reservation_method: _Optional[str] = ...,
+        type_code: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class PickingTypeCreateRequest(_message.Message):
     __slots__ = [
         "name",
@@ -74,47 +91,63 @@
         "warehouse_id",
         "code",
         "return_picking_type_id",
         "show_operations",
         "show_reserved",
         "default_location_src_id",
         "default_location_dest_id",
+        "barcode",
+        "reservation_method",
+        "type_code",
+        "sequence_id",
         "context",
     ]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SEQUENCE_CODE_FIELD_NUMBER: _ClassVar[int]
     WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     RETURN_PICKING_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     SHOW_OPERATIONS_FIELD_NUMBER: _ClassVar[int]
     SHOW_RESERVED_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_LOCATION_SRC_ID_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_LOCATION_DEST_ID_FIELD_NUMBER: _ClassVar[int]
+    BARCODE_FIELD_NUMBER: _ClassVar[int]
+    RESERVATION_METHOD_FIELD_NUMBER: _ClassVar[int]
+    TYPE_CODE_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     sequence_code: str
     warehouse_id: int
     code: str
     return_picking_type_id: int
     show_operations: _wrappers_pb2.BoolValue
     show_reserved: _wrappers_pb2.BoolValue
     default_location_src_id: int
     default_location_dest_id: int
+    barcode: str
+    reservation_method: str
+    type_code: str
+    sequence_id: int
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         sequence_code: _Optional[str] = ...,
         warehouse_id: _Optional[int] = ...,
         code: _Optional[str] = ...,
         return_picking_type_id: _Optional[int] = ...,
         show_operations: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         show_reserved: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         default_location_src_id: _Optional[int] = ...,
         default_location_dest_id: _Optional[int] = ...,
+        barcode: _Optional[str] = ...,
+        reservation_method: _Optional[str] = ...,
+        type_code: _Optional[str] = ...,
+        sequence_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class PickingTypeCreateResponse(_message.Message):
     __slots__ = ["response_standard", "picking_type"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     PICKING_TYPE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,143 +2,151 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class ProcurementGroup(_message.Message):
-    __slots__ = ["id", "name", "move_type", "active", "object_audit"]
+class PaymentMethod(_message.Message):
+    __slots__ = ["id", "name", "code", "description", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    MOVE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
-    move_type: str
+    code: str
+    description: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        move_type: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        description: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupCreateRequest(_message.Message):
-    __slots__ = ["name", "move_type", "context"]
+class PaymentMethodAddRequest(_message.Message):
+    __slots__ = ["name", "code", "description", "active", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    MOVE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    move_type: str
+    code: str
+    description: str
+    active: bool
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        move_type: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        description: _Optional[str] = ...,
+        active: bool = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "procurement_group"]
+class PaymentMethodAddResponse(_message.Message):
+    __slots__ = ["response_standard", "payment_method"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    procurement_group: ProcurementGroup
+    payment_method: PaymentMethod
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupReadRequest(_message.Message):
+class PaymentMethodReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "procurement_groups"]
+class PaymentMethodReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "payment_methods"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    PROCUREMENT_GROUPS_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHODS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    procurement_groups: _containers.RepeatedCompositeFieldContainer[ProcurementGroup]
+    payment_methods: _containers.RepeatedCompositeFieldContainer[PaymentMethod]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        procurement_groups: _Optional[_Iterable[_Union[ProcurementGroup, _Mapping]]] = ...,
+        payment_methods: _Optional[_Iterable[_Union[PaymentMethod, _Mapping]]] = ...,
     ) -> None: ...
 
-class ProcurementGroupUpdateRequest(_message.Message):
-    __slots__ = ["procurement_group", "context"]
-    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
+class PaymentMethodUpdateRequest(_message.Message):
+    __slots__ = ["payment_method", "context"]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    procurement_group: ProcurementGroup
+    payment_method: PaymentMethod
     context: _base_pb2.Context
     def __init__(
         self,
-        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "procurement_group"]
+class PaymentMethodUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "payment_method"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    PROCUREMENT_GROUP_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    procurement_group: ProcurementGroup
+    payment_method: PaymentMethod
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        procurement_group: _Optional[_Union[ProcurementGroup, _Mapping]] = ...,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
     ) -> None: ...
 
-class ProcurementGroupDeleteRequest(_message.Message):
+class PaymentMethodDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ProcurementGroupDeleteResponse(_message.Message):
+class PaymentMethodDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/product_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/quant_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/quant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/route_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/route_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/rule.proto
+# source: v1/stock/stock_move_line.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x13v1/stock/rule.proto\x12\x18pro.omni.oms.api.v1.rule\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x02\n\x04Rule\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x04 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x05 \x01(\x05\x12\x13\n\x0blocation_id\x18\x06 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x07 \x01(\t\x12\x10\n\x08route_id\x18\x08 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\t \x01(\x05\x12\x10\n\x08sequence\x18\n \x01(\x05\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x82\x02\n\x11RuleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x17\n\x0flocation_src_id\x18\x04 \x01(\x05\x12\x13\n\x0blocation_id\x18\x05 \x01(\x05\x12\x16\n\x0eprocure_method\x18\x06 \x01(\t\x12\x10\n\x08route_id\x18\x07 \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x08 \x01(\x05\x12\x10\n\x08sequence\x18\t \x01(\x05\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"\xed\x02\n\x0fRuleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x10RuleReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12-\n\x05rules\x18\x03 \x03(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"y\n\x11RuleUpdateRequest\x12,\n\x04rule\x18\x01 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8d\x01\n\x12RuleUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12,\n\x04rule\x18\x02 \x01(\x0b\x32\x1e.pro.omni.oms.api.v1.rule.Rule"W\n\x11RuleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12RuleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xb3\x03\n\x0bRuleService\x12i\n\nRuleCreate\x12+.pro.omni.oms.api.v1.rule.RuleCreateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleCreateResponse"\x00\x12\x63\n\x08RuleRead\x12).pro.omni.oms.api.v1.rule.RuleReadRequest\x1a*.pro.omni.oms.api.v1.rule.RuleReadResponse"\x00\x12i\n\nRuleUpdate\x12+.pro.omni.oms.api.v1.rule.RuleUpdateRequest\x1a,.pro.omni.oms.api.v1.rule.RuleUpdateResponse"\x00\x12i\n\nRuleDelete\x12+.pro.omni.oms.api.v1.rule.RuleDeleteRequest\x1a,.pro.omni.oms.api.v1.rule.RuleDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1ev1/stock/stock_move_line.proto\x12)pro.omni.oms.api.v1.stock.stock_move_line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xfd\x02\n\rStockMoveLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x15\n\rstock_move_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\treference\x18\x05 \x01(\t\x12(\n\x04\x64\x61te\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x12\n\nproduct_id\x18\x08 \x01(\x05\x12\x13\n\x0blocation_id\x18\t \x01(\x05\x12\x18\n\x10location_dest_id\x18\n \x01(\x05\x12\x10\n\x08qty_done\x18\x0b \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0c \x01(\x05\x12*\n\x06\x61\x63tive\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc9\x02\n\x1aStockMoveLineCreateRequest\x12\x15\n\rstock_move_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x11\n\treference\x18\x04 \x01(\t\x12(\n\x04\x64\x61te\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x06 \x01(\t\x12\x12\n\nproduct_id\x18\x07 \x01(\x05\x12\x13\n\x0blocation_id\x18\x08 \x01(\x05\x12\x18\n\x10location_dest_id\x18\t \x01(\x05\x12\x10\n\x08qty_done\x18\n \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0b \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xf6\x02\n\x18StockMoveLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf5\x01\n\x19StockMoveLineReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12R\n\x10stock_move_lines\x18\x03 \x03(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xa7\x01\n\x1aStockMoveLineUpdateRequest\x12Q\n\x0fstock_move_line\x18\x01 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"`\n\x1aStockMoveLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bStockMoveLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xac\x05\n\x14StockMoveLineService\x12\xa4\x01\n\x13StockMoveLineCreate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateResponse\x12\x9e\x01\n\x11StockMoveLineRead\x12\x43.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadRequest\x1a\x44.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadResponse\x12\xa4\x01\n\x13StockMoveLineUpdate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateResponse\x12\xa4\x01\n\x13StockMoveLineDelete\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteResponseb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.rule_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_line_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_RULE"]._serialized_start = 131
-    _globals["_RULE"]._serialized_end = 441
-    _globals["_RULECREATEREQUEST"]._serialized_start = 444
-    _globals["_RULECREATEREQUEST"]._serialized_end = 702
-    _globals["_RULECREATERESPONSE"]._serialized_start = 705
-    _globals["_RULECREATERESPONSE"]._serialized_end = 846
-    _globals["_RULEREADREQUEST"]._serialized_start = 849
-    _globals["_RULEREADREQUEST"]._serialized_end = 1214
-    _globals["_RULEREADRESPONSE"]._serialized_start = 1217
-    _globals["_RULEREADRESPONSE"]._serialized_end = 1416
-    _globals["_RULEUPDATEREQUEST"]._serialized_start = 1418
-    _globals["_RULEUPDATEREQUEST"]._serialized_end = 1539
-    _globals["_RULEUPDATERESPONSE"]._serialized_start = 1542
-    _globals["_RULEUPDATERESPONSE"]._serialized_end = 1683
-    _globals["_RULEDELETEREQUEST"]._serialized_start = 1685
-    _globals["_RULEDELETEREQUEST"]._serialized_end = 1772
-    _globals["_RULEDELETERESPONSE"]._serialized_start = 1774
-    _globals["_RULEDELETERESPONSE"]._serialized_end = 1869
-    _globals["_RULESERVICE"]._serialized_start = 1872
-    _globals["_RULESERVICE"]._serialized_end = 2307
+    _globals["_STOCKMOVELINE"]._serialized_start = 162
+    _globals["_STOCKMOVELINE"]._serialized_end = 543
+    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_start = 546
+    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_end = 875
+    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_start = 878
+    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_end = 1065
+    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_start = 1068
+    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_end = 1442
+    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_start = 1445
+    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_end = 1690
+    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_start = 1693
+    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_end = 1860
+    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_start = 1863
+    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_end = 2050
+    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_start = 2052
+    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_end = 2148
+    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_start = 2150
+    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_end = 2254
+    _globals["_STOCKMOVELINESERVICE"]._serialized_start = 2257
+    _globals["_STOCKMOVELINESERVICE"]._serialized_end = 2941
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/rule_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/sequence_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/sequence_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/stock_move_line.proto
+# source: v1/stock/stock_move.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1ev1/stock/stock_move_line.proto\x12)pro.omni.oms.api.v1.stock.stock_move_line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xfd\x02\n\rStockMoveLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x15\n\rstock_move_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\treference\x18\x05 \x01(\t\x12(\n\x04\x64\x61te\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x12\n\nproduct_id\x18\x08 \x01(\x05\x12\x13\n\x0blocation_id\x18\t \x01(\x05\x12\x18\n\x10location_dest_id\x18\n \x01(\x05\x12\x10\n\x08qty_done\x18\x0b \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0c \x01(\x05\x12*\n\x06\x61\x63tive\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc9\x02\n\x1aStockMoveLineCreateRequest\x12\x15\n\rstock_move_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x11\n\treference\x18\x04 \x01(\t\x12(\n\x04\x64\x61te\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x06 \x01(\t\x12\x12\n\nproduct_id\x18\x07 \x01(\x05\x12\x13\n\x0blocation_id\x18\x08 \x01(\x05\x12\x18\n\x10location_dest_id\x18\t \x01(\x05\x12\x10\n\x08qty_done\x18\n \x01(\x05\x12\x16\n\x0eproduct_uom_id\x18\x0b \x01(\x05\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xf6\x02\n\x18StockMoveLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf5\x01\n\x19StockMoveLineReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12R\n\x10stock_move_lines\x18\x03 \x03(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"\xa7\x01\n\x1aStockMoveLineUpdateRequest\x12Q\n\x0fstock_move_line\x18\x01 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbb\x01\n\x1bStockMoveLineUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12Q\n\x0fstock_move_line\x18\x02 \x01(\x0b\x32\x38.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLine"`\n\x1aStockMoveLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bStockMoveLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xac\x05\n\x14StockMoveLineService\x12\xa4\x01\n\x13StockMoveLineCreate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineCreateResponse\x12\x9e\x01\n\x11StockMoveLineRead\x12\x43.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadRequest\x1a\x44.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineReadResponse\x12\xa4\x01\n\x13StockMoveLineUpdate\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineUpdateResponse\x12\xa4\x01\n\x13StockMoveLineDelete\x12\x45.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteRequest\x1a\x46.pro.omni.oms.api.v1.stock.stock_move_line.StockMoveLineDeleteResponseb\x06proto3'
+    b'\n\x19v1/stock/stock_move.proto\x12$pro.omni.oms.api.v1.stock.stock_move\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa0\x02\n\tStockMove\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\r\n\x05state\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x05 \x01(\x02\x12\x15\n\rquantity_done\x18\x06 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x07 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x08 \x01(\t\x12*\n\x06\x61\x63tive\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\n \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xec\x01\n\x16StockMoveCreateRequest\x12\x12\n\npicking_id\x18\x01 \x01(\x05\x12\r\n\x05state\x18\x02 \x01(\t\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x04 \x01(\x02\x12\x15\n\rquantity_done\x18\x05 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x07 \x01(\t\x12\x36\n\x07\x63ontext\x18\x08 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\xf2\x02\n\x14StockMoveReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15StockMoveReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\x0bstock_moves\x18\x03 \x03(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\x95\x01\n\x16StockMoveUpdateRequest\x12\x43\n\nstock_move\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\\\n\x16StockMoveDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17StockMoveDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10StockMoveService\x12\x90\x01\n\x0fStockMoveCreate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateResponse"\x00\x12\x8a\x01\n\rStockMoveRead\x12:.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadRequest\x1a;.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadResponse"\x00\x12\x90\x01\n\x0fStockMoveUpdate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateResponse"\x00\x12\x90\x01\n\x0fStockMoveDelete\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_line_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_STOCKMOVELINE"]._serialized_start = 162
-    _globals["_STOCKMOVELINE"]._serialized_end = 543
-    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_start = 546
-    _globals["_STOCKMOVELINECREATEREQUEST"]._serialized_end = 875
-    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_start = 878
-    _globals["_STOCKMOVELINECREATERESPONSE"]._serialized_end = 1065
-    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_start = 1068
-    _globals["_STOCKMOVELINEREADREQUEST"]._serialized_end = 1442
-    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_start = 1445
-    _globals["_STOCKMOVELINEREADRESPONSE"]._serialized_end = 1690
-    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_start = 1693
-    _globals["_STOCKMOVELINEUPDATEREQUEST"]._serialized_end = 1860
-    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_start = 1863
-    _globals["_STOCKMOVELINEUPDATERESPONSE"]._serialized_end = 2050
-    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_start = 2052
-    _globals["_STOCKMOVELINEDELETEREQUEST"]._serialized_end = 2148
-    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_start = 2150
-    _globals["_STOCKMOVELINEDELETERESPONSE"]._serialized_end = 2254
-    _globals["_STOCKMOVELINESERVICE"]._serialized_start = 2257
-    _globals["_STOCKMOVELINESERVICE"]._serialized_end = 2941
+    _globals["_STOCKMOVE"]._serialized_start = 119
+    _globals["_STOCKMOVE"]._serialized_end = 407
+    _globals["_STOCKMOVECREATEREQUEST"]._serialized_start = 410
+    _globals["_STOCKMOVECREATEREQUEST"]._serialized_end = 646
+    _globals["_STOCKMOVECREATERESPONSE"]._serialized_start = 649
+    _globals["_STOCKMOVECREATERESPONSE"]._serialized_end = 818
+    _globals["_STOCKMOVEREADREQUEST"]._serialized_start = 821
+    _globals["_STOCKMOVEREADREQUEST"]._serialized_end = 1191
+    _globals["_STOCKMOVEREADRESPONSE"]._serialized_start = 1194
+    _globals["_STOCKMOVEREADRESPONSE"]._serialized_end = 1421
+    _globals["_STOCKMOVEUPDATEREQUEST"]._serialized_start = 1424
+    _globals["_STOCKMOVEUPDATEREQUEST"]._serialized_end = 1573
+    _globals["_STOCKMOVEUPDATERESPONSE"]._serialized_start = 1576
+    _globals["_STOCKMOVEUPDATERESPONSE"]._serialized_end = 1745
+    _globals["_STOCKMOVEDELETEREQUEST"]._serialized_start = 1747
+    _globals["_STOCKMOVEDELETEREQUEST"]._serialized_end = 1839
+    _globals["_STOCKMOVEDELETERESPONSE"]._serialized_start = 1841
+    _globals["_STOCKMOVEDELETERESPONSE"]._serialized_end = 1941
+    _globals["_STOCKMOVESERVICE"]._serialized_start = 1944
+    _globals["_STOCKMOVESERVICE"]._serialized_end = 2544
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/stock/stock_move.proto
+# source: v1/utilities/timezone.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x19v1/stock/stock_move.proto\x12$pro.omni.oms.api.v1.stock.stock_move\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa0\x02\n\tStockMove\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\r\n\x05state\x18\x03 \x01(\t\x12\x12\n\nproduct_id\x18\x04 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x05 \x01(\x02\x12\x15\n\rquantity_done\x18\x06 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x07 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x08 \x01(\t\x12*\n\x06\x61\x63tive\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\n \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xec\x01\n\x16StockMoveCreateRequest\x12\x12\n\npicking_id\x18\x01 \x01(\x05\x12\r\n\x05state\x18\x02 \x01(\t\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x17\n\x0fproduct_uom_qty\x18\x04 \x01(\x02\x12\x15\n\rquantity_done\x18\x05 \x01(\x02\x12\x16\n\x0eproduct_uom_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x64\x65scription_picking\x18\x07 \x01(\t\x12\x36\n\x07\x63ontext\x18\x08 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\xf2\x02\n\x14StockMoveReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15StockMoveReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\x0bstock_moves\x18\x03 \x03(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\x95\x01\n\x16StockMoveUpdateRequest\x12\x43\n\nstock_move\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17StockMoveUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x43\n\nstock_move\x18\x02 \x01(\x0b\x32/.pro.omni.oms.api.v1.stock.stock_move.StockMove"\\\n\x16StockMoveDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17StockMoveDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10StockMoveService\x12\x90\x01\n\x0fStockMoveCreate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveCreateResponse"\x00\x12\x8a\x01\n\rStockMoveRead\x12:.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadRequest\x1a;.pro.omni.oms.api.v1.stock.stock_move.StockMoveReadResponse"\x00\x12\x90\x01\n\x0fStockMoveUpdate\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveUpdateResponse"\x00\x12\x90\x01\n\x0fStockMoveDelete\x12<.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteRequest\x1a=.pro.omni.oms.api.v1.stock.stock_move.StockMoveDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1bv1/utilities/timezone.proto\x12&pro.omni.oms.api.v1.utilities.timezone\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xc3\x01\n\x08Timezone\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\x12\n\noffset_dst\x18\x05 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xb8\x01\n\x12TimezoneAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x05\x12\x12\n\noffset_dst\x18\x04 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa4\x01\n\x13TimezoneAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08timezone\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.timezone.Timezone"\xf1\x02\n\x13TimezoneReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x14TimezoneReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x43\n\ttimezones\x18\x03 \x03(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.timezone.Timezone"\x93\x01\n\x15TimezoneUpdateRequest\x12\x42\n\x08timezone\x18\x01 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.timezone.Timezone\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x16TimezoneUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08timezone\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.timezone.Timezone"[\n\x15TimezoneDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16TimezoneDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd2\x04\n\x0fTimezoneService\x12\x88\x01\n\x0bTimezoneAdd\x12:.pro.omni.oms.api.v1.utilities.timezone.TimezoneAddRequest\x1a;.pro.omni.oms.api.v1.utilities.timezone.TimezoneAddResponse"\x00\x12\x8b\x01\n\x0cTimezoneRead\x12;.pro.omni.oms.api.v1.utilities.timezone.TimezoneReadRequest\x1a<.pro.omni.oms.api.v1.utilities.timezone.TimezoneReadResponse"\x00\x12\x91\x01\n\x0eTimezoneUpdate\x12=.pro.omni.oms.api.v1.utilities.timezone.TimezoneUpdateRequest\x1a>.pro.omni.oms.api.v1.utilities.timezone.TimezoneUpdateResponse"\x00\x12\x91\x01\n\x0eTimezoneDelete\x12=.pro.omni.oms.api.v1.utilities.timezone.TimezoneDeleteRequest\x1a>.pro.omni.oms.api.v1.utilities.timezone.TimezoneDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.stock_move_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.timezone_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_STOCKMOVE"]._serialized_start = 119
-    _globals["_STOCKMOVE"]._serialized_end = 407
-    _globals["_STOCKMOVECREATEREQUEST"]._serialized_start = 410
-    _globals["_STOCKMOVECREATEREQUEST"]._serialized_end = 646
-    _globals["_STOCKMOVECREATERESPONSE"]._serialized_start = 649
-    _globals["_STOCKMOVECREATERESPONSE"]._serialized_end = 818
-    _globals["_STOCKMOVEREADREQUEST"]._serialized_start = 821
-    _globals["_STOCKMOVEREADREQUEST"]._serialized_end = 1191
-    _globals["_STOCKMOVEREADRESPONSE"]._serialized_start = 1194
-    _globals["_STOCKMOVEREADRESPONSE"]._serialized_end = 1421
-    _globals["_STOCKMOVEUPDATEREQUEST"]._serialized_start = 1424
-    _globals["_STOCKMOVEUPDATEREQUEST"]._serialized_end = 1573
-    _globals["_STOCKMOVEUPDATERESPONSE"]._serialized_start = 1576
-    _globals["_STOCKMOVEUPDATERESPONSE"]._serialized_end = 1745
-    _globals["_STOCKMOVEDELETEREQUEST"]._serialized_start = 1747
-    _globals["_STOCKMOVEDELETEREQUEST"]._serialized_end = 1839
-    _globals["_STOCKMOVEDELETERESPONSE"]._serialized_start = 1841
-    _globals["_STOCKMOVEDELETERESPONSE"]._serialized_end = 1941
-    _globals["_STOCKMOVESERVICE"]._serialized_start = 1944
-    _globals["_STOCKMOVESERVICE"]._serialized_end = 2544
+    _globals["_TIMEZONE"]._serialized_start = 123
+    _globals["_TIMEZONE"]._serialized_end = 318
+    _globals["_TIMEZONEADDREQUEST"]._serialized_start = 321
+    _globals["_TIMEZONEADDREQUEST"]._serialized_end = 505
+    _globals["_TIMEZONEADDRESPONSE"]._serialized_start = 508
+    _globals["_TIMEZONEADDRESPONSE"]._serialized_end = 672
+    _globals["_TIMEZONEREADREQUEST"]._serialized_start = 675
+    _globals["_TIMEZONEREADREQUEST"]._serialized_end = 1044
+    _globals["_TIMEZONEREADRESPONSE"]._serialized_start = 1047
+    _globals["_TIMEZONEREADRESPONSE"]._serialized_end = 1272
+    _globals["_TIMEZONEUPDATEREQUEST"]._serialized_start = 1275
+    _globals["_TIMEZONEUPDATEREQUEST"]._serialized_end = 1422
+    _globals["_TIMEZONEUPDATERESPONSE"]._serialized_start = 1425
+    _globals["_TIMEZONEUPDATERESPONSE"]._serialized_end = 1592
+    _globals["_TIMEZONEDELETEREQUEST"]._serialized_start = 1594
+    _globals["_TIMEZONEDELETEREQUEST"]._serialized_end = 1685
+    _globals["_TIMEZONEDELETERESPONSE"]._serialized_start = 1687
+    _globals["_TIMEZONEDELETERESPONSE"]._serialized_end = 1786
+    _globals["_TIMEZONESERVICE"]._serialized_start = 1789
+    _globals["_TIMEZONESERVICE"]._serialized_end = 2383
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -8,186 +8,151 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class StockMove(_message.Message):
-    __slots__ = [
-        "id",
-        "picking_id",
-        "state",
-        "product_id",
-        "product_uom_qty",
-        "quantity_done",
-        "product_uom_id",
-        "description_picking",
-        "active",
-        "object_audit",
-    ]
+class Timezone(_message.Message):
+    __slots__ = ["id", "name", "code", "offset", "offset_dst", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    PICKING_ID_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_UOM_QTY_FIELD_NUMBER: _ClassVar[int]
-    QUANTITY_DONE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_UOM_ID_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_PICKING_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    picking_id: int
-    state: str
-    product_id: int
-    product_uom_qty: float
-    quantity_done: float
-    product_uom_id: int
-    description_picking: str
+    id: str
+    name: str
+    code: str
+    offset: int
+    offset_dst: int
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        picking_id: _Optional[int] = ...,
-        state: _Optional[str] = ...,
-        product_id: _Optional[int] = ...,
-        product_uom_qty: _Optional[float] = ...,
-        quantity_done: _Optional[float] = ...,
-        product_uom_id: _Optional[int] = ...,
-        description_picking: _Optional[str] = ...,
+        id: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveCreateRequest(_message.Message):
-    __slots__ = [
-        "picking_id",
-        "state",
-        "product_id",
-        "product_uom_qty",
-        "quantity_done",
-        "product_uom_id",
-        "description_picking",
-        "context",
-    ]
-    PICKING_ID_FIELD_NUMBER: _ClassVar[int]
-    STATE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_UOM_QTY_FIELD_NUMBER: _ClassVar[int]
-    QUANTITY_DONE_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_UOM_ID_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_PICKING_FIELD_NUMBER: _ClassVar[int]
+class TimezoneAddRequest(_message.Message):
+    __slots__ = ["name", "code", "offset", "offset_dst", "active", "context"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    picking_id: int
-    state: str
-    product_id: int
-    product_uom_qty: float
-    quantity_done: float
-    product_uom_id: int
-    description_picking: str
+    name: str
+    code: str
+    offset: int
+    offset_dst: int
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
-        picking_id: _Optional[int] = ...,
-        state: _Optional[str] = ...,
-        product_id: _Optional[int] = ...,
-        product_uom_qty: _Optional[float] = ...,
-        quantity_done: _Optional[float] = ...,
-        product_uom_id: _Optional[int] = ...,
-        description_picking: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "stock_move"]
+class TimezoneAddResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    stock_move: StockMove
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveReadRequest(_message.Message):
+class TimezoneReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "stock_moves"]
+class TimezoneReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "timezones"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    STOCK_MOVES_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    stock_moves: _containers.RepeatedCompositeFieldContainer[StockMove]
+    timezones: _containers.RepeatedCompositeFieldContainer[Timezone]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        stock_moves: _Optional[_Iterable[_Union[StockMove, _Mapping]]] = ...,
+        timezones: _Optional[_Iterable[_Union[Timezone, _Mapping]]] = ...,
     ) -> None: ...
 
-class StockMoveUpdateRequest(_message.Message):
-    __slots__ = ["stock_move", "context"]
-    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
+class TimezoneUpdateRequest(_message.Message):
+    __slots__ = ["timezone", "context"]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    stock_move: StockMove
+    timezone: Timezone
     context: _base_pb2.Context
     def __init__(
         self,
-        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "stock_move"]
+class TimezoneUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    STOCK_MOVE_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    stock_move: StockMove
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        stock_move: _Optional[_Union[StockMove, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class StockMoveDeleteRequest(_message.Message):
+class TimezoneDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class StockMoveDeleteResponse(_message.Message):
+class TimezoneDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/uom_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/user_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 from omni.pro.protos.v1.stock import country_pb2 as v1_dot_stock_dot_country__pb2
 from omni.pro.protos.v1.stock import location_pb2 as v1_dot_stock_dot_location__pb2
 from omni.pro.protos.v1.stock import picking_type_pb2 as v1_dot_stock_dot_picking__type__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x18v1/stock/warehouse.proto\x12#pro.omni.oms.api.v1.stock.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17v1/stock/location.proto\x1a\x1bv1/stock/picking_type.proto\x1a\x16v1/stock/country.proto"\xa0\t\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12>\n\ncountry_id\x18\x04 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.country.Country\x12\x37\n\x16territory_matrix_value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x12\n\ncomplement\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x16\n\x0e\x64\x65livery_steps\x18\t \x01(\t\x12\x18\n\x10receptions_steps\x18\n \x01(\t\x12\x46\n\x10view_location_id\x18\x0b \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12\x42\n\x0clot_stock_id\x18\x0c \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12K\n\x15wh_input_stock_loc_id\x18\r \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12H\n\x12wh_qc_stock_loc_id\x18\x0e \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12J\n\x14wh_pack_stock_loc_id\x18\x0f \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12L\n\x16wh_output_stock_loc_id\x18\x10 \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12G\n\nin_type_id\x18\x11 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12H\n\x0bint_type_id\x18\x12 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12I\n\x0cpick_type_id\x18\x13 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12I\n\x0cpack_type_id\x18\x14 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12H\n\x0bout_type_id\x18\x15 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12?\n\x0cobject_audit\x18\x16 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xa3\x04\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x12\n\ncountry_id\x18\x03 \x01(\x05\x12\x37\n\x16territory_matrix_value\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x05 \x01(\t\x12\x12\n\ncomplement\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65livery_steps\x18\x07 \x01(\t\x12\x18\n\x10receptions_steps\x18\x08 \x01(\t\x12\x18\n\x10view_location_id\x18\t \x01(\x05\x12\x14\n\x0clot_stock_id\x18\n \x01(\x05\x12\x1d\n\x15wh_input_stock_loc_id\x18\x0b \x01(\x05\x12\x1a\n\x12wh_qc_stock_loc_id\x18\x0c \x01(\x05\x12\x1c\n\x14wh_pack_stock_loc_id\x18\r \x01(\x05\x12\x1e\n\x16wh_output_stock_loc_id\x18\x0e \x01(\x05\x12\x12\n\nin_type_id\x18\x0f \x01(\x05\x12\x13\n\x0bint_type_id\x18\x10 \x01(\x05\x12\x14\n\x0cpick_type_id\x18\x11 \x01(\x05\x12\x14\n\x0cpack_type_id\x18\x12 \x01(\x05\x12\x13\n\x0bout_type_id\x18\x13 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x14 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x42\n\nwarehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x18v1/stock/warehouse.proto\x12#pro.omni.oms.api.v1.stock.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17v1/stock/location.proto\x1a\x1bv1/stock/picking_type.proto\x1a\x16v1/stock/country.proto"\x9d\t\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12;\n\x07\x63ountry\x18\x04 \x01(\x0b\x32*.pro.omni.oms.api.v1.stock.country.Country\x12\x37\n\x16territory_matrix_value\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x06 \x01(\t\x12\x12\n\ncomplement\x18\x07 \x01(\t\x12*\n\x06\x61\x63tive\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x16\n\x0e\x64\x65livery_steps\x18\t \x01(\t\x12\x18\n\x10receptions_steps\x18\n \x01(\t\x12\x46\n\x10view_location_id\x18\x0b \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12\x42\n\x0clot_stock_id\x18\x0c \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12K\n\x15wh_input_stock_loc_id\x18\r \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12H\n\x12wh_qc_stock_loc_id\x18\x0e \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12J\n\x14wh_pack_stock_loc_id\x18\x0f \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12L\n\x16wh_output_stock_loc_id\x18\x10 \x01(\x0b\x32,.pro.omni.oms.api.v1.stock.location.Location\x12G\n\nin_type_id\x18\x11 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12H\n\x0bint_type_id\x18\x12 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12I\n\x0cpick_type_id\x18\x13 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12I\n\x0cpack_type_id\x18\x14 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12H\n\x0bout_type_id\x18\x15 \x01(\x0b\x32\x33.pro.omni.oms.api.v1.stock.picking_type.PickingType\x12?\n\x0cobject_audit\x18\x16 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xa5\x04\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x14\n\x0c\x63ountry_code\x18\x03 \x01(\t\x12\x37\n\x16territory_matrix_value\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x0f\n\x07\x61\x64\x64ress\x18\x05 \x01(\t\x12\x12\n\ncomplement\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65livery_steps\x18\x07 \x01(\t\x12\x18\n\x10receptions_steps\x18\x08 \x01(\t\x12\x18\n\x10view_location_id\x18\t \x01(\x05\x12\x14\n\x0clot_stock_id\x18\n \x01(\x05\x12\x1d\n\x15wh_input_stock_loc_id\x18\x0b \x01(\x05\x12\x1a\n\x12wh_qc_stock_loc_id\x18\x0c \x01(\x05\x12\x1c\n\x14wh_pack_stock_loc_id\x18\r \x01(\x05\x12\x1e\n\x16wh_output_stock_loc_id\x18\x0e \x01(\x05\x12\x12\n\nin_type_id\x18\x0f \x01(\x05\x12\x13\n\x0bint_type_id\x18\x10 \x01(\x05\x12\x14\n\x0cpick_type_id\x18\x11 \x01(\x05\x12\x14\n\x0cpack_type_id\x18\x12 \x01(\x05\x12\x13\n\x0bout_type_id\x18\x13 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x14 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x42\n\nwarehouses\x18\x03 \x03(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x41\n\twarehouse\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.v1.stock.warehouse.Warehouse"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.stock.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.stock.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.stock.warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     _globals["_WAREHOUSE"]._serialized_start = 225
-    _globals["_WAREHOUSE"]._serialized_end = 1409
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 1412
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 1959
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 1962
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 2129
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 2132
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 2502
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 2505
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 2730
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 2733
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 2880
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 2883
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 3050
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 3052
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 3144
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 3146
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 3246
-    _globals["_WAREHOUSESERVICE"]._serialized_start = 3249
-    _globals["_WAREHOUSESERVICE"]._serialized_end = 3841
+    _globals["_WAREHOUSE"]._serialized_end = 1406
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 1409
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 1958
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 1961
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 2128
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 2131
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 2501
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 2504
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 2729
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 2732
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 2879
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 2882
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 3049
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 3051
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 3143
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 3145
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 3245
+    _globals["_WAREHOUSESERVICE"]._serialized_start = 3248
+    _globals["_WAREHOUSESERVICE"]._serialized_end = 3840
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/stock/warehouse_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Warehouse(_message.Message):
     __slots__ = [
         "id",
         "name",
         "code",
-        "country_id",
+        "country",
         "territory_matrix_value",
         "address",
         "complement",
         "active",
         "delivery_steps",
         "receptions_steps",
         "view_location_id",
@@ -40,15 +40,15 @@
         "pack_type_id",
         "out_type_id",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
+    COUNTRY_FIELD_NUMBER: _ClassVar[int]
     TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
     ADDRESS_FIELD_NUMBER: _ClassVar[int]
     COMPLEMENT_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     DELIVERY_STEPS_FIELD_NUMBER: _ClassVar[int]
     RECEPTIONS_STEPS_FIELD_NUMBER: _ClassVar[int]
     VIEW_LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
@@ -62,15 +62,15 @@
     PICK_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     PACK_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     OUT_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     code: str
-    country_id: _country_pb2.Country
+    country: _country_pb2.Country
     territory_matrix_value: _struct_pb2.Struct
     address: str
     complement: str
     active: _wrappers_pb2.BoolValue
     delivery_steps: str
     receptions_steps: str
     view_location_id: _location_pb2.Location
@@ -86,15 +86,15 @@
     out_type_id: _picking_type_pb2.PickingType
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        country_id: _Optional[_Union[_country_pb2.Country, _Mapping]] = ...,
+        country: _Optional[_Union[_country_pb2.Country, _Mapping]] = ...,
         territory_matrix_value: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
         address: _Optional[str] = ...,
         complement: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         delivery_steps: _Optional[str] = ...,
         receptions_steps: _Optional[str] = ...,
         view_location_id: _Optional[_Union[_location_pb2.Location, _Mapping]] = ...,
@@ -111,15 +111,15 @@
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class WarehouseCreateRequest(_message.Message):
     __slots__ = [
         "name",
         "code",
-        "country_id",
+        "country_code",
         "territory_matrix_value",
         "address",
         "complement",
         "delivery_steps",
         "receptions_steps",
         "view_location_id",
         "lot_stock_id",
@@ -132,15 +132,15 @@
         "pick_type_id",
         "pack_type_id",
         "out_type_id",
         "context",
     ]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
+    COUNTRY_CODE_FIELD_NUMBER: _ClassVar[int]
     TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
     ADDRESS_FIELD_NUMBER: _ClassVar[int]
     COMPLEMENT_FIELD_NUMBER: _ClassVar[int]
     DELIVERY_STEPS_FIELD_NUMBER: _ClassVar[int]
     RECEPTIONS_STEPS_FIELD_NUMBER: _ClassVar[int]
     VIEW_LOCATION_ID_FIELD_NUMBER: _ClassVar[int]
     LOT_STOCK_ID_FIELD_NUMBER: _ClassVar[int]
@@ -152,15 +152,15 @@
     INT_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     PICK_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     PACK_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     OUT_TYPE_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    country_id: int
+    country_code: str
     territory_matrix_value: _struct_pb2.Struct
     address: str
     complement: str
     delivery_steps: str
     receptions_steps: str
     view_location_id: int
     lot_stock_id: int
@@ -174,15 +174,15 @@
     pack_type_id: int
     out_type_id: int
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        country_id: _Optional[int] = ...,
+        country_code: _Optional[str] = ...,
         territory_matrix_value: _Optional[_Union[_struct_pb2.Struct, _Mapping]] = ...,
         address: _Optional[str] = ...,
         complement: _Optional[str] = ...,
         delivery_steps: _Optional[str] = ...,
         receptions_steps: _Optional[str] = ...,
         view_location_id: _Optional[int] = ...,
         lot_stock_id: _Optional[int] = ...,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.stock import warehouse_pb2 as v1_dot_stock_dot_warehouse__pb2
+from omni.pro.protos.v1.utilities import payment_method_pb2 as v1_dot_utilities_dot_payment__method__pb2
 
 
-class WarehouseServiceStub(object):
+class PaymentMethodServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.WarehouseCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseCreate",
-            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
+        self.PaymentMethodAdd = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodAdd",
+            request_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddResponse.FromString,
         )
-        self.WarehouseRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseRead",
-            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.FromString,
+        self.PaymentMethodRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodRead",
+            request_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadResponse.FromString,
         )
-        self.WarehouseUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseUpdate",
-            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
+        self.PaymentMethodUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodUpdate",
+            request_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateResponse.FromString,
         )
-        self.WarehouseDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseDelete",
-            request_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
+        self.PaymentMethodDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodDelete",
+            request_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteResponse.FromString,
         )
 
 
-class WarehouseServiceServicer(object):
+class PaymentMethodServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def WarehouseCreate(self, request, context):
+    def PaymentMethodAdd(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseRead(self, request, context):
+    def PaymentMethodRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseUpdate(self, request, context):
+    def PaymentMethodUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def WarehouseDelete(self, request, context):
+    def PaymentMethodDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_WarehouseServiceServicer_to_server(servicer, server):
+def add_PaymentMethodServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "WarehouseCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseCreate,
-            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.SerializeToString,
+        "PaymentMethodAdd": grpc.unary_unary_rpc_method_handler(
+            servicer.PaymentMethodAdd,
+            request_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddResponse.SerializeToString,
         ),
-        "WarehouseRead": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseRead,
-            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.FromString,
-            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.SerializeToString,
+        "PaymentMethodRead": grpc.unary_unary_rpc_method_handler(
+            servicer.PaymentMethodRead,
+            request_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadResponse.SerializeToString,
         ),
-        "WarehouseUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseUpdate,
-            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.FromString,
-            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.SerializeToString,
+        "PaymentMethodUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.PaymentMethodUpdate,
+            request_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateResponse.SerializeToString,
         ),
-        "WarehouseDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.WarehouseDelete,
-            request_deserializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.FromString,
-            response_serializer=v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.SerializeToString,
+        "PaymentMethodDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.PaymentMethodDelete,
+            request_deserializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.stock.warehouse.WarehouseService", rpc_method_handlers
+        "pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class WarehouseService(object):
+class PaymentMethodService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def WarehouseCreate(
+    def PaymentMethodAdd(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseCreate",
-            v1_dot_stock_dot_warehouse__pb2.WarehouseCreateRequest.SerializeToString,
-            v1_dot_stock_dot_warehouse__pb2.WarehouseCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodAdd",
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddRequest.SerializeToString,
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodAddResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseRead(
+    def PaymentMethodRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseRead",
-            v1_dot_stock_dot_warehouse__pb2.WarehouseReadRequest.SerializeToString,
-            v1_dot_stock_dot_warehouse__pb2.WarehouseReadResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodRead",
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadRequest.SerializeToString,
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseUpdate(
+    def PaymentMethodUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseUpdate",
-            v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateRequest.SerializeToString,
-            v1_dot_stock_dot_warehouse__pb2.WarehouseUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodUpdate",
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateRequest.SerializeToString,
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def WarehouseDelete(
+    def PaymentMethodDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.stock.warehouse.WarehouseService/WarehouseDelete",
-            v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteRequest.SerializeToString,
-            v1_dot_stock_dot_warehouse__pb2.WarehouseDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodService/PaymentMethodDelete",
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteRequest.SerializeToString,
+            v1_dot_utilities_dot_payment__method__pb2.PaymentMethodDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/users/user_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/users/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/country_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/currency.proto
+# source: v1/rules/country.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1bv1/utilities/currency.proto\x12&pro.omni.oms.api.v1.utilities.currency\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x02\n\x08\x43urrency\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x1b\n\x13\x63urrency_unit_label\x18\x04 \x01(\t\x12\x1e\n\x16\x63urrency_subunit_label\x18\x05 \x01(\t\x12\x0c\n\x04rate\x18\x06 \x01(\x05\x12\x10\n\x08rounding\x18\x07 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x08 \x01(\x05\x12\x0e\n\x06symbol\x18\t \x01(\t\x12\x10\n\x08position\x18\n \x01(\t\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xab\x02\n\x12\x43urrencyAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrency_unit_label\x18\x03 \x01(\t\x12\x1e\n\x16\x63urrency_subunit_label\x18\x04 \x01(\t\x12\x0c\n\x04rate\x18\x05 \x01(\x05\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12\x16\n\x0e\x64\x65\x63imal_places\x18\x07 \x01(\x05\x12\x0e\n\x06symbol\x18\x08 \x01(\t\x12\x10\n\x08position\x18\t \x01(\t\x12*\n\x06\x61\x63tive\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x0b \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa4\x01\n\x13\x43urrencyAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08\x63urrency\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"\xf1\x02\n\x13\x43urrencyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe2\x01\n\x14\x43urrencyReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x44\n\ncurrencies\x18\x03 \x03(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"\x93\x01\n\x15\x43urrencyUpdateRequest\x12\x42\n\x08\x63urrency\x18\x01 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x16\x43urrencyUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x42\n\x08\x63urrency\x18\x02 \x01(\x0b\x32\x30.pro.omni.oms.api.v1.utilities.currency.Currency"[\n\x15\x43urrencyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43urrencyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd2\x04\n\x0f\x43urrencyService\x12\x88\x01\n\x0b\x43urrencyAdd\x12:.pro.omni.oms.api.v1.utilities.currency.CurrencyAddRequest\x1a;.pro.omni.oms.api.v1.utilities.currency.CurrencyAddResponse"\x00\x12\x8b\x01\n\x0c\x43urrencyRead\x12;.pro.omni.oms.api.v1.utilities.currency.CurrencyReadRequest\x1a<.pro.omni.oms.api.v1.utilities.currency.CurrencyReadResponse"\x00\x12\x91\x01\n\x0e\x43urrencyUpdate\x12=.pro.omni.oms.api.v1.utilities.currency.CurrencyUpdateRequest\x1a>.pro.omni.oms.api.v1.utilities.currency.CurrencyUpdateResponse"\x00\x12\x91\x01\n\x0e\x43urrencyDelete\x12=.pro.omni.oms.api.v1.utilities.currency.CurrencyDeleteRequest\x1a>.pro.omni.oms.api.v1.utilities.currency.CurrencyDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/rules/country.proto\x12!pro.omni.oms.api.v1.rules.country\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x01\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x16\n\x0e\x63ountry_doc_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x83\x01\n\x14\x43ountryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0f\x63\x61tegory_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryCreateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.rules.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xda\x01\n\x13\x43ountryReadResponse\x12=\n\tcountries\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.rules.country.Country\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x01\n\x14\x43ountryUpdateRequest\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.rules.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryUpdateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.rules.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x43ountryService\x12\x84\x01\n\rCountryCreate\x12\x37.pro.omni.oms.api.v1.rules.country.CountryCreateRequest\x1a\x38.pro.omni.oms.api.v1.rules.country.CountryCreateResponse"\x00\x12~\n\x0b\x43ountryRead\x12\x35.pro.omni.oms.api.v1.rules.country.CountryReadRequest\x1a\x36.pro.omni.oms.api.v1.rules.country.CountryReadResponse"\x00\x12\x84\x01\n\rCountryUpdate\x12\x37.pro.omni.oms.api.v1.rules.country.CountryUpdateRequest\x1a\x38.pro.omni.oms.api.v1.rules.country.CountryUpdateResponse"\x00\x12\x84\x01\n\rCountryDelete\x12\x37.pro.omni.oms.api.v1.rules.country.CountryDeleteRequest\x1a\x38.pro.omni.oms.api.v1.rules.country.CountryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.currency_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.country_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CURRENCY"]._serialized_start = 123
-    _globals["_CURRENCY"]._serialized_end = 433
-    _globals["_CURRENCYADDREQUEST"]._serialized_start = 436
-    _globals["_CURRENCYADDREQUEST"]._serialized_end = 735
-    _globals["_CURRENCYADDRESPONSE"]._serialized_start = 738
-    _globals["_CURRENCYADDRESPONSE"]._serialized_end = 902
-    _globals["_CURRENCYREADREQUEST"]._serialized_start = 905
-    _globals["_CURRENCYREADREQUEST"]._serialized_end = 1274
-    _globals["_CURRENCYREADRESPONSE"]._serialized_start = 1277
-    _globals["_CURRENCYREADRESPONSE"]._serialized_end = 1503
-    _globals["_CURRENCYUPDATEREQUEST"]._serialized_start = 1506
-    _globals["_CURRENCYUPDATEREQUEST"]._serialized_end = 1653
-    _globals["_CURRENCYUPDATERESPONSE"]._serialized_start = 1656
-    _globals["_CURRENCYUPDATERESPONSE"]._serialized_end = 1823
-    _globals["_CURRENCYDELETEREQUEST"]._serialized_start = 1825
-    _globals["_CURRENCYDELETEREQUEST"]._serialized_end = 1916
-    _globals["_CURRENCYDELETERESPONSE"]._serialized_start = 1918
-    _globals["_CURRENCYDELETERESPONSE"]._serialized_end = 2017
-    _globals["_CURRENCYSERVICE"]._serialized_start = 2020
-    _globals["_CURRENCYSERVICE"]._serialized_end = 2614
+    _globals["_COUNTRY"]._serialized_start = 113
+    _globals["_COUNTRY"]._serialized_end = 295
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 298
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 429
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 432
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 591
+    _globals["_COUNTRYREADREQUEST"]._serialized_start = 594
+    _globals["_COUNTRYREADREQUEST"]._serialized_end = 962
+    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 965
+    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 1183
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 1186
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 1325
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 1328
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 1487
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 1489
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 1579
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 1581
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 1679
+    _globals["_COUNTRYSERVICE"]._serialized_start = 1682
+    _globals["_COUNTRYSERVICE"]._serialized_end = 2231
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/currency_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/language_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/language_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,72 +2,73 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Model(_message.Message):
-    __slots__ = ["id", "name", "model", "active", "object_audit"]
+class TerritoryMatrixValue(_message.Message):
+    __slots__ = ["id", "territory_matrixes", "data", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
-    name: str
-    model: str
+    territory_matrixes: _struct_pb2.ListValue
+    data: _struct_pb2.ListValue
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
-        name: _Optional[str] = ...,
-        model: _Optional[str] = ...,
+        territory_matrixes: _Optional[_Union[_struct_pb2.ListValue, _Mapping]] = ...,
+        data: _Optional[_Union[_struct_pb2.ListValue, _Mapping]] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelCreateRequest(_message.Message):
-    __slots__ = ["name", "model", "active", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+class TerritoryMatrixValueAddRequest(_message.Message):
+    __slots__ = ["territory_matrixes", "data", "active", "context"]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
+    DATA_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    model: str
+    territory_matrixes: _struct_pb2.ListValue
+    data: _struct_pb2.ListValue
     active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
-        model: _Optional[str] = ...,
+        territory_matrixes: _Optional[_Union[_struct_pb2.ListValue, _Mapping]] = ...,
+        data: _Optional[_Union[_struct_pb2.ListValue, _Mapping]] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "model"]
+class TerritoryMatrixValueAddResponse(_message.Message):
+    __slots__ = ["response_standard", "territory_matrix_value"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    model: Model
+    territory_matrix_value: TerritoryMatrixValue
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
+        territory_matrix_value: _Optional[_Union[TerritoryMatrixValue, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelReadRequest(_message.Message):
+class TerritoryMatrixValueReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -86,61 +87,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "models"]
+class TerritoryMatrixValueReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "territory_matrixes_values"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    MODELS_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_VALUES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    models: _containers.RepeatedCompositeFieldContainer[Model]
+    territory_matrixes_values: _containers.RepeatedCompositeFieldContainer[TerritoryMatrixValue]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        models: _Optional[_Iterable[_Union[Model, _Mapping]]] = ...,
+        territory_matrixes_values: _Optional[_Iterable[_Union[TerritoryMatrixValue, _Mapping]]] = ...,
     ) -> None: ...
 
-class ModelUpdateRequest(_message.Message):
-    __slots__ = ["model", "context"]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+class TerritoryMatrixValueUpdateRequest(_message.Message):
+    __slots__ = ["territory_matrix_value", "context"]
+    TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    model: Model
+    territory_matrix_value: TerritoryMatrixValue
     context: _base_pb2.Context
     def __init__(
         self,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
+        territory_matrix_value: _Optional[_Union[TerritoryMatrixValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "model"]
+class TerritoryMatrixValueUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "territory_matrix_value"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIX_VALUE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    model: Model
+    territory_matrix_value: TerritoryMatrixValue
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
+        territory_matrix_value: _Optional[_Union[TerritoryMatrixValue, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelDeleteRequest(_message.Message):
+class TerritoryMatrixValueDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ModelDeleteResponse(_message.Message):
+class TerritoryMatrixValueDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/model_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/payment_method_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/payment_method.proto
+# source: v1/utilities/uom.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n!v1/utilities/payment_method.proto\x12,pro.omni.oms.api.v1.utilities.payment_method\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb9\x01\n\rPaymentMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x92\x01\n\x17PaymentMethodAddRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xba\x01\n\x18PaymentMethodAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12S\n\x0epayment_method\x18\x02 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"\xf6\x02\n\x18PaymentMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x19PaymentMethodReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12T\n\x0fpayment_methods\x18\x03 \x03(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"\xa9\x01\n\x1aPaymentMethodUpdateRequest\x12S\n\x0epayment_method\x18\x01 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1bPaymentMethodUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12S\n\x0epayment_method\x18\x02 \x01(\x0b\x32;.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethod"`\n\x1aPaymentMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bPaymentMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc3\x05\n\x14PaymentMethodService\x12\xa3\x01\n\x10PaymentMethodAdd\x12\x45.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodAddRequest\x1a\x46.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodAddResponse"\x00\x12\xa6\x01\n\x11PaymentMethodRead\x12\x46.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodReadRequest\x1aG.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodReadResponse"\x00\x12\xac\x01\n\x13PaymentMethodUpdate\x12H.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodUpdateRequest\x1aI.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodUpdateResponse"\x00\x12\xac\x01\n\x13PaymentMethodDelete\x12H.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodDeleteRequest\x1aI.pro.omni.oms.api.v1.utilities.payment_method.PaymentMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/utilities/uom.proto\x12!pro.omni.oms.api.v1.utilities.uom\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xcc\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x10\n\x08rounding\x18\x06 \x01(\x01\x12*\n\x06\x61\x63tive\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x08 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x98\x01\n\x10UomCreateRequest\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08rounding\x18\x05 \x01(\x01\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcd\x01\n\x0fUomReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12\x34\n\x04uoms\x18\x03 \x03(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"\x7f\n\x10UomUpdateRequest\x12\x33\n\x03uom\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x11UomUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x33\n\x03uom\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.v1.utilities.uom.Uom"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xee\x03\n\nUomService\x12x\n\tUomCreate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomCreateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomCreateResponse"\x00\x12r\n\x07UomRead\x12\x31.pro.omni.oms.api.v1.utilities.uom.UomReadRequest\x1a\x32.pro.omni.oms.api.v1.utilities.uom.UomReadResponse"\x00\x12x\n\tUomUpdate\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomUpdateRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomUpdateResponse"\x00\x12x\n\tUomDelete\x12\x33.pro.omni.oms.api.v1.utilities.uom.UomDeleteRequest\x1a\x34.pro.omni.oms.api.v1.utilities.uom.UomDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.payment_method_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.uom_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PAYMENTMETHOD"]._serialized_start = 135
-    _globals["_PAYMENTMETHOD"]._serialized_end = 320
-    _globals["_PAYMENTMETHODADDREQUEST"]._serialized_start = 323
-    _globals["_PAYMENTMETHODADDREQUEST"]._serialized_end = 469
-    _globals["_PAYMENTMETHODADDRESPONSE"]._serialized_start = 472
-    _globals["_PAYMENTMETHODADDRESPONSE"]._serialized_end = 658
-    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_start = 661
-    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_end = 1035
-    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_start = 1038
-    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_end = 1285
-    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_start = 1288
-    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_end = 1457
-    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_start = 1460
-    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_end = 1649
-    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_start = 1651
-    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_end = 1747
-    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_start = 1749
-    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_end = 1853
-    _globals["_PAYMENTMETHODSERVICE"]._serialized_start = 1856
-    _globals["_PAYMENTMETHODSERVICE"]._serialized_end = 2563
+    _globals["_UOM"]._serialized_start = 113
+    _globals["_UOM"]._serialized_end = 317
+    _globals["_UOMCREATEREQUEST"]._serialized_start = 320
+    _globals["_UOMCREATEREQUEST"]._serialized_end = 472
+    _globals["_UOMCREATERESPONSE"]._serialized_start = 475
+    _globals["_UOMCREATERESPONSE"]._serialized_end = 622
+    _globals["_UOMREADREQUEST"]._serialized_start = 625
+    _globals["_UOMREADREQUEST"]._serialized_end = 989
+    _globals["_UOMREADRESPONSE"]._serialized_start = 992
+    _globals["_UOMREADRESPONSE"]._serialized_end = 1197
+    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1199
+    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1326
+    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1329
+    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1476
+    _globals["_UOMDELETEREQUEST"]._serialized_start = 1478
+    _globals["_UOMDELETEREQUEST"]._serialized_end = 1564
+    _globals["_UOMDELETERESPONSE"]._serialized_start = 1566
+    _globals["_UOMDELETERESPONSE"]._serialized_end = 1660
+    _globals["_UOMSERVICE"]._serialized_start = 1663
+    _globals["_UOMSERVICE"]._serialized_end = 2157
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/payment_method_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,145 +8,152 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class PaymentMethod(_message.Message):
-    __slots__ = ["id", "name", "code", "description", "active", "object_audit"]
+class Uom(_message.Message):
+    __slots__ = ["id", "category", "code", "name", "type", "rounding", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
-    name: str
+    category: str
     code: str
-    description: str
+    name: str
+    type: str
+    rounding: float
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
-        name: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        description: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodAddRequest(_message.Message):
-    __slots__ = ["name", "code", "description", "active", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class UomCreateRequest(_message.Message):
+    __slots__ = ["category", "code", "name", "type", "rounding", "context"]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
+    category: str
     code: str
-    description: str
-    active: bool
+    name: str
+    type: str
+    rounding: float
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        description: _Optional[str] = ...,
-        active: bool = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodAddResponse(_message.Message):
-    __slots__ = ["response_standard", "payment_method"]
+class UomCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    payment_method: PaymentMethod
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodReadRequest(_message.Message):
+class UomReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "payment_methods"]
+class UomReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "uoms"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHODS_FIELD_NUMBER: _ClassVar[int]
+    UOMS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    payment_methods: _containers.RepeatedCompositeFieldContainer[PaymentMethod]
+    uoms: _containers.RepeatedCompositeFieldContainer[Uom]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        payment_methods: _Optional[_Iterable[_Union[PaymentMethod, _Mapping]]] = ...,
+        uoms: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
     ) -> None: ...
 
-class PaymentMethodUpdateRequest(_message.Message):
-    __slots__ = ["payment_method", "context"]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+class UomUpdateRequest(_message.Message):
+    __slots__ = ["uom", "context"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    payment_method: PaymentMethod
+    uom: Uom
     context: _base_pb2.Context
     def __init__(
-        self,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class PaymentMethodUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "payment_method"]
+class UomUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    payment_method: PaymentMethod
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodDeleteRequest(_message.Message):
+class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class PaymentMethodDeleteResponse(_message.Message):
+class UomDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/sequence_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2.pyi` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,200 +2,206 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import struct_pb2 as _struct_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Sequence(_message.Message):
-    __slots__ = [
-        "id",
-        "name",
-        "code",
-        "implementation",
-        "prefix",
-        "suffix",
-        "padding",
-        "number_increment",
-        "number_next_actual",
-        "active",
-        "object_audit",
-    ]
+class TerritoryMatrix(_message.Message):
+    __slots__ = ["id", "sequence", "name", "code", "active", "country_id", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
-    PREFIX_FIELD_NUMBER: _ClassVar[int]
-    SUFFIX_FIELD_NUMBER: _ClassVar[int]
-    PADDING_FIELD_NUMBER: _ClassVar[int]
-    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
-    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
+    sequence: int
     name: str
     code: str
-    implementation: str
-    prefix: str
-    suffix: str
-    padding: float
-    number_increment: int
-    number_next_actual: int
     active: _wrappers_pb2.BoolValue
+    country_id: str
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
+        sequence: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        implementation: _Optional[str] = ...,
-        prefix: _Optional[str] = ...,
-        suffix: _Optional[str] = ...,
-        padding: _Optional[float] = ...,
-        number_increment: _Optional[int] = ...,
-        number_next_actual: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+        country_id: _Optional[str] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceCreateRequest(_message.Message):
-    __slots__ = [
-        "name",
-        "code",
-        "implementation",
-        "prefix",
-        "suffix",
-        "padding",
-        "number_increment",
-        "number_next_actual",
-        "context",
-    ]
+class TerritoryMatrixAddRequest(_message.Message):
+    __slots__ = ["country_id", "sequence", "name", "code", "active", "context"]
+    COUNTRY_ID_FIELD_NUMBER: _ClassVar[int]
+    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    IMPLEMENTATION_FIELD_NUMBER: _ClassVar[int]
-    PREFIX_FIELD_NUMBER: _ClassVar[int]
-    SUFFIX_FIELD_NUMBER: _ClassVar[int]
-    PADDING_FIELD_NUMBER: _ClassVar[int]
-    NUMBER_INCREMENT_FIELD_NUMBER: _ClassVar[int]
-    NUMBER_NEXT_ACTUAL_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    country_id: str
+    sequence: int
     name: str
     code: str
-    implementation: str
-    prefix: str
-    suffix: str
-    padding: float
-    number_increment: int
-    number_next_actual: int
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
+        country_id: _Optional[str] = ...,
+        sequence: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        implementation: _Optional[str] = ...,
-        prefix: _Optional[str] = ...,
-        suffix: _Optional[str] = ...,
-        padding: _Optional[float] = ...,
-        number_increment: _Optional[int] = ...,
-        number_next_actual: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "sequence"]
+class TerritoryMatrixAddResponse(_message.Message):
+    __slots__ = ["response_standard", "territory_matrixes"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    sequence: Sequence
+    territory_matrixes: TerritoryMatrix
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
+        territory_matrixes: _Optional[_Union[TerritoryMatrix, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceReadRequest(_message.Message):
+class TerritoryMatrixReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "sequences"]
+class TerritoryMatrixReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "territory_matrixes"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCES_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    sequences: _containers.RepeatedCompositeFieldContainer[Sequence]
+    territory_matrixes: _containers.RepeatedCompositeFieldContainer[TerritoryMatrix]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        sequences: _Optional[_Iterable[_Union[Sequence, _Mapping]]] = ...,
+        territory_matrixes: _Optional[_Iterable[_Union[TerritoryMatrix, _Mapping]]] = ...,
     ) -> None: ...
 
-class SequenceUpdateRequest(_message.Message):
-    __slots__ = ["sequence", "context"]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+class TerritoryMatrixUpdateRequest(_message.Message):
+    __slots__ = ["territory_matrix", "context"]
+    TERRITORY_MATRIX_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    sequence: Sequence
+    territory_matrix: TerritoryMatrix
     context: _base_pb2.Context
     def __init__(
         self,
-        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
+        territory_matrix: _Optional[_Union[TerritoryMatrix, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "sequence"]
+class TerritoryMatrixUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "territory_matrixes"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    SEQUENCE_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    sequence: Sequence
+    territory_matrixes: TerritoryMatrix
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        sequence: _Optional[_Union[Sequence, _Mapping]] = ...,
+        territory_matrixes: _Optional[_Union[TerritoryMatrix, _Mapping]] = ...,
     ) -> None: ...
 
-class SequenceDeleteRequest(_message.Message):
+class TerritoryMatrixDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class SequenceDeleteResponse(_message.Message):
+class TerritoryMatrixDeleteResponse(_message.Message):
+    __slots__ = ["response_standard"]
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    response_standard: _base_pb2.ResponseStandard
+    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
+
+class TerritoryMatrixLoadRequest(_message.Message):
+    __slots__ = ["country_code", "csv_name", "context"]
+    COUNTRY_CODE_FIELD_NUMBER: _ClassVar[int]
+    CSV_NAME_FIELD_NUMBER: _ClassVar[int]
+    CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    country_code: str
+    csv_name: str
+    context: _base_pb2.Context
+    def __init__(
+        self,
+        country_code: _Optional[str] = ...,
+        csv_name: _Optional[str] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
+
+class TerritoryMatrixLoadResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
+
+class TerritoryMatrixStructureRequest(_message.Message):
+    __slots__ = ["territorymatrix", "parent_code", "context"]
+    TERRITORYMATRIX_FIELD_NUMBER: _ClassVar[int]
+    PARENT_CODE_FIELD_NUMBER: _ClassVar[int]
+    CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    territorymatrix: TerritoryMatrix
+    parent_code: str
+    context: _base_pb2.Context
+    def __init__(
+        self,
+        territorymatrix: _Optional[_Union[TerritoryMatrix, _Mapping]] = ...,
+        parent_code: _Optional[str] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+    ) -> None: ...
+
+class TerritoryMatrixStructureResponse(_message.Message):
+    __slots__ = ["response_standard", "territory_matrixes"]
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    TERRITORY_MATRIXES_FIELD_NUMBER: _ClassVar[int]
+    response_standard: _base_pb2.ResponseStandard
+    territory_matrixes: _struct_pb2.ListValue
+    def __init__(
+        self,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        territory_matrixes: _Optional[_Union[_struct_pb2.ListValue, _Mapping]] = ...,
+    ) -> None: ...
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/uom_pb2_grpc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.utilities import sequence_pb2 as v1_dot_utilities_dot_sequence__pb2
+from omni.pro.protos.v1.utilities import uom_pb2 as v1_dot_utilities_dot_uom__pb2
 
 
-class SequenceServiceStub(object):
+class UomServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.SequenceCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceCreate",
-            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.FromString,
+        self.UomCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
         )
-        self.SequenceRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceRead",
-            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.FromString,
+        self.UomRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
         )
-        self.SequenceUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceUpdate",
-            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.FromString,
+        self.UomUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
         )
-        self.SequenceDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceDelete",
-            request_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.FromString,
+        self.UomDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
+            request_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
         )
 
 
-class SequenceServiceServicer(object):
+class UomServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def SequenceCreate(self, request, context):
+    def UomCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SequenceRead(self, request, context):
+    def UomRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SequenceUpdate(self, request, context):
+    def UomUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def SequenceDelete(self, request, context):
+    def UomDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_SequenceServiceServicer_to_server(servicer, server):
+def add_UomServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "SequenceCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.SequenceCreate,
-            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.SerializeToString,
+        "UomCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.UomCreate,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.SerializeToString,
         ),
-        "SequenceRead": grpc.unary_unary_rpc_method_handler(
-            servicer.SequenceRead,
-            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.SerializeToString,
+        "UomRead": grpc.unary_unary_rpc_method_handler(
+            servicer.UomRead,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.SerializeToString,
         ),
-        "SequenceUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.SequenceUpdate,
-            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.SerializeToString,
+        "UomUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.UomUpdate,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.SerializeToString,
         ),
-        "SequenceDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.SequenceDelete,
-            request_deserializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.SerializeToString,
+        "UomDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.UomDelete,
+            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.utilities.sequence.SequenceService", rpc_method_handlers
+        "pro.omni.oms.api.v1.utilities.uom.UomService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class SequenceService(object):
+class UomService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def SequenceCreate(
+    def UomCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceCreate",
-            v1_dot_utilities_dot_sequence__pb2.SequenceCreateRequest.SerializeToString,
-            v1_dot_utilities_dot_sequence__pb2.SequenceCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
+            v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SequenceRead(
+    def UomRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceRead",
-            v1_dot_utilities_dot_sequence__pb2.SequenceReadRequest.SerializeToString,
-            v1_dot_utilities_dot_sequence__pb2.SequenceReadResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
+            v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SequenceUpdate(
+    def UomUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceUpdate",
-            v1_dot_utilities_dot_sequence__pb2.SequenceUpdateRequest.SerializeToString,
-            v1_dot_utilities_dot_sequence__pb2.SequenceUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
+            v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def SequenceDelete(
+    def UomDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.sequence.SequenceService/SequenceDelete",
-            v1_dot_utilities_dot_sequence__pb2.SequenceDeleteRequest.SerializeToString,
-            v1_dot_utilities_dot_sequence__pb2.SequenceDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
+            v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
+            v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/tax_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/territory_matrix.proto
+# source: v1/utilities/territory_matrix_value.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n#v1/utilities/territory_matrix.proto\x12.pro.omni.oms.api.v1.utilities.territory_matrix\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xcc\x01\n\x0fTerritoryMatrix\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08sequence\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x12\n\ncountry_id\x18\x06 \x01(\t\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc1\x01\n\x19TerritoryMatrixAddRequest\x12\x12\n\ncountry_id\x18\x01 \x01(\t\x12\x10\n\x08sequence\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc4\x01\n\x1aTerritoryMatrixAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12[\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"\xf8\x02\n\x1aTerritoryMatrixReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1bTerritoryMatrixReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12[\n\x12territory_matrixes\x18\x03 \x03(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"\xb1\x01\n\x1cTerritoryMatrixUpdateRequest\x12Y\n\x10territory_matrix\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1dTerritoryMatrixUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12[\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"b\n\x1cTerritoryMatrixDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1dTerritoryMatrixDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xed\x05\n\x16TerritoryMatrixService\x12\xad\x01\n\x12TerritoryMatrixAdd\x12I.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixAddRequest\x1aJ.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixAddResponse"\x00\x12\xb0\x01\n\x13TerritoryMatrixRead\x12J.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixReadRequest\x1aK.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixReadResponse"\x00\x12\xb6\x01\n\x15TerritoryMatrixUpdate\x12L.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixUpdateRequest\x1aM.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixUpdateResponse"\x00\x12\xb6\x01\n\x15TerritoryMatrixDelete\x12L.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixDeleteRequest\x1aM.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixDeleteResponse"\x00\x62\x06proto3'
+    b'\n)v1/utilities/territory_matrix_value.proto\x12\x34pro.omni.oms.api.v1.utilities.territory_matrix_value\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xf1\x01\n\x14TerritoryMatrixValue\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12(\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe6\x01\n\x1eTerritoryMatrixValueAddRequest\x12\x36\n\x12territory_matrixes\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\x06\x61\x63tive\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd8\x01\n\x1fTerritoryMatrixValueAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12j\n\x16territory_matrix_value\x18\x02 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"\xfd\x02\n\x1fTerritoryMatrixValueReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x02\n TerritoryMatrixValueReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12m\n\x19territory_matrixes_values\x18\x03 \x03(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"\xc7\x01\n!TerritoryMatrixValueUpdateRequest\x12j\n\x16territory_matrix_value\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n"TerritoryMatrixValueUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12j\n\x16territory_matrix_value\x18\x02 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"g\n!TerritoryMatrixValueDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"o\n"TerritoryMatrixValueDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xde\x06\n\x1bTerritoryMatrixValueService\x12\xc8\x01\n\x17TerritoryMatrixValueAdd\x12T.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueAddRequest\x1aU.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueAddResponse"\x00\x12\xcb\x01\n\x18TerritoryMatrixValueRead\x12U.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueReadRequest\x1aV.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueReadResponse"\x00\x12\xd1\x01\n\x1aTerritoryMatrixValueUpdate\x12W.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueUpdateRequest\x1aX.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueUpdateResponse"\x00\x12\xd1\x01\n\x1aTerritoryMatrixValueDelete\x12W.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueDeleteRequest\x1aX.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.territory_matrix_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.territory_matrix_value_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TERRITORYMATRIX"]._serialized_start = 139
-    _globals["_TERRITORYMATRIX"]._serialized_end = 343
-    _globals["_TERRITORYMATRIXADDREQUEST"]._serialized_start = 346
-    _globals["_TERRITORYMATRIXADDREQUEST"]._serialized_end = 539
-    _globals["_TERRITORYMATRIXADDRESPONSE"]._serialized_start = 542
-    _globals["_TERRITORYMATRIXADDRESPONSE"]._serialized_end = 738
-    _globals["_TERRITORYMATRIXREADREQUEST"]._serialized_start = 741
-    _globals["_TERRITORYMATRIXREADREQUEST"]._serialized_end = 1117
-    _globals["_TERRITORYMATRIXREADRESPONSE"]._serialized_start = 1120
-    _globals["_TERRITORYMATRIXREADRESPONSE"]._serialized_end = 1376
-    _globals["_TERRITORYMATRIXUPDATEREQUEST"]._serialized_start = 1379
-    _globals["_TERRITORYMATRIXUPDATEREQUEST"]._serialized_end = 1556
-    _globals["_TERRITORYMATRIXUPDATERESPONSE"]._serialized_start = 1559
-    _globals["_TERRITORYMATRIXUPDATERESPONSE"]._serialized_end = 1758
-    _globals["_TERRITORYMATRIXDELETEREQUEST"]._serialized_start = 1760
-    _globals["_TERRITORYMATRIXDELETEREQUEST"]._serialized_end = 1858
-    _globals["_TERRITORYMATRIXDELETERESPONSE"]._serialized_start = 1860
-    _globals["_TERRITORYMATRIXDELETERESPONSE"]._serialized_end = 1966
-    _globals["_TERRITORYMATRIXSERVICE"]._serialized_start = 1969
-    _globals["_TERRITORYMATRIXSERVICE"]._serialized_end = 2718
+    _globals["_TERRITORYMATRIXVALUE"]._serialized_start = 181
+    _globals["_TERRITORYMATRIXVALUE"]._serialized_end = 422
+    _globals["_TERRITORYMATRIXVALUEADDREQUEST"]._serialized_start = 425
+    _globals["_TERRITORYMATRIXVALUEADDREQUEST"]._serialized_end = 655
+    _globals["_TERRITORYMATRIXVALUEADDRESPONSE"]._serialized_start = 658
+    _globals["_TERRITORYMATRIXVALUEADDRESPONSE"]._serialized_end = 874
+    _globals["_TERRITORYMATRIXVALUEREADREQUEST"]._serialized_start = 877
+    _globals["_TERRITORYMATRIXVALUEREADREQUEST"]._serialized_end = 1258
+    _globals["_TERRITORYMATRIXVALUEREADRESPONSE"]._serialized_start = 1261
+    _globals["_TERRITORYMATRIXVALUEREADRESPONSE"]._serialized_end = 1540
+    _globals["_TERRITORYMATRIXVALUEUPDATEREQUEST"]._serialized_start = 1543
+    _globals["_TERRITORYMATRIXVALUEUPDATEREQUEST"]._serialized_end = 1742
+    _globals["_TERRITORYMATRIXVALUEUPDATERESPONSE"]._serialized_start = 1745
+    _globals["_TERRITORYMATRIXVALUEUPDATERESPONSE"]._serialized_end = 1964
+    _globals["_TERRITORYMATRIXVALUEDELETEREQUEST"]._serialized_start = 1966
+    _globals["_TERRITORYMATRIXVALUEDELETEREQUEST"]._serialized_end = 2069
+    _globals["_TERRITORYMATRIXVALUEDELETERESPONSE"]._serialized_start = 2071
+    _globals["_TERRITORYMATRIXVALUEDELETERESPONSE"]._serialized_end = 2182
+    _globals["_TERRITORYMATRIXVALUESERVICE"]._serialized_start = 2185
+    _globals["_TERRITORYMATRIXVALUESERVICE"]._serialized_end = 3047
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,24 @@
             response_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixUpdateResponse.FromString,
         )
         self.TerritoryMatrixDelete = channel.unary_unary(
             "/pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService/TerritoryMatrixDelete",
             request_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixDeleteResponse.FromString,
         )
+        self.TerritoryMatrixLoad = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService/TerritoryMatrixLoad",
+            request_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadResponse.FromString,
+        )
+        self.TerritoryMatrixStructure = channel.unary_unary(
+            "/pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService/TerritoryMatrixStructure",
+            request_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureRequest.SerializeToString,
+            response_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureResponse.FromString,
+        )
 
 
 class TerritoryMatrixServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def TerritoryMatrixAdd(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -58,14 +68,26 @@
 
     def TerritoryMatrixDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def TerritoryMatrixLoad(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def TerritoryMatrixStructure(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
 
 def add_TerritoryMatrixServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "TerritoryMatrixAdd": grpc.unary_unary_rpc_method_handler(
             servicer.TerritoryMatrixAdd,
             request_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixAddRequest.FromString,
             response_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixAddResponse.SerializeToString,
@@ -81,14 +103,24 @@
             response_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixUpdateResponse.SerializeToString,
         ),
         "TerritoryMatrixDelete": grpc.unary_unary_rpc_method_handler(
             servicer.TerritoryMatrixDelete,
             request_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixDeleteRequest.FromString,
             response_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixDeleteResponse.SerializeToString,
         ),
+        "TerritoryMatrixLoad": grpc.unary_unary_rpc_method_handler(
+            servicer.TerritoryMatrixLoad,
+            request_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadResponse.SerializeToString,
+        ),
+        "TerritoryMatrixStructure": grpc.unary_unary_rpc_method_handler(
+            servicer.TerritoryMatrixStructure,
+            request_deserializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureRequest.FromString,
+            response_serializer=v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -205,9 +237,67 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def TerritoryMatrixLoad(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService/TerritoryMatrixLoad",
+            v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadRequest.SerializeToString,
+            v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixLoadResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def TerritoryMatrixStructure(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixService/TerritoryMatrixStructure",
+            v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureRequest.SerializeToString,
+            v1_dot_utilities_dot_territory__matrix__pb2.TerritoryMatrixStructureResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: v1/utilities/territory_matrix_value.proto
+# source: v1/utilities/territory_matrix.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
@@ -13,36 +13,44 @@
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n)v1/utilities/territory_matrix_value.proto\x12\x34pro.omni.oms.api.v1.utilities.territory_matrix_value\x1a\x11\x63ommon/base.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xf1\x01\n\x14TerritoryMatrixValue\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12(\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe6\x01\n\x1eTerritoryMatrixValueAddRequest\x12\x36\n\x12territory_matrixes\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12*\n\x06\x61\x63tive\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd8\x01\n\x1fTerritoryMatrixValueAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12j\n\x16territory_matrix_value\x18\x02 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"\xfd\x02\n\x1fTerritoryMatrixValueReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x02\n TerritoryMatrixValueReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12m\n\x19territory_matrixes_values\x18\x03 \x03(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"\xc7\x01\n!TerritoryMatrixValueUpdateRequest\x12j\n\x16territory_matrix_value\x18\x01 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdb\x01\n"TerritoryMatrixValueUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12j\n\x16territory_matrix_value\x18\x02 \x01(\x0b\x32J.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValue"g\n!TerritoryMatrixValueDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"o\n"TerritoryMatrixValueDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xde\x06\n\x1bTerritoryMatrixValueService\x12\xc8\x01\n\x17TerritoryMatrixValueAdd\x12T.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueAddRequest\x1aU.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueAddResponse"\x00\x12\xcb\x01\n\x18TerritoryMatrixValueRead\x12U.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueReadRequest\x1aV.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueReadResponse"\x00\x12\xd1\x01\n\x1aTerritoryMatrixValueUpdate\x12W.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueUpdateRequest\x1aX.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueUpdateResponse"\x00\x12\xd1\x01\n\x1aTerritoryMatrixValueDelete\x12W.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueDeleteRequest\x1aX.pro.omni.oms.api.v1.utilities.territory_matrix_value.TerritoryMatrixValueDeleteResponse"\x00\x62\x06proto3'
+    b'\n#v1/utilities/territory_matrix.proto\x12.pro.omni.oms.api.v1.utilities.territory_matrix\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1cgoogle/protobuf/struct.proto"\xcc\x01\n\x0fTerritoryMatrix\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08sequence\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x12\n\ncountry_id\x18\x06 \x01(\t\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xc1\x01\n\x19TerritoryMatrixAddRequest\x12\x12\n\ncountry_id\x18\x01 \x01(\t\x12\x10\n\x08sequence\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x07\x63ontext\x18\x06 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc4\x01\n\x1aTerritoryMatrixAddResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12[\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"\xf8\x02\n\x1aTerritoryMatrixReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x80\x02\n\x1bTerritoryMatrixReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12[\n\x12territory_matrixes\x18\x03 \x03(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"\xb1\x01\n\x1cTerritoryMatrixUpdateRequest\x12Y\n\x10territory_matrix\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc7\x01\n\x1dTerritoryMatrixUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12[\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix"b\n\x1cTerritoryMatrixDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"j\n\x1dTerritoryMatrixDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"|\n\x1aTerritoryMatrixLoadRequest\x12\x14\n\x0c\x63ountry_code\x18\x01 \x01(\t\x12\x10\n\x08\x63sv_name\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bTerritoryMatrixLoadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xc8\x01\n\x1fTerritoryMatrixStructureRequest\x12X\n\x0fterritorymatrix\x18\x01 \x01(\x0b\x32?.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrix\x12\x13\n\x0bparent_code\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa5\x01\n TerritoryMatrixStructureResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x36\n\x12territory_matrixes\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.ListValue2\xe2\x08\n\x16TerritoryMatrixService\x12\xad\x01\n\x12TerritoryMatrixAdd\x12I.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixAddRequest\x1aJ.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixAddResponse"\x00\x12\xb0\x01\n\x13TerritoryMatrixRead\x12J.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixReadRequest\x1aK.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixReadResponse"\x00\x12\xb6\x01\n\x15TerritoryMatrixUpdate\x12L.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixUpdateRequest\x1aM.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixUpdateResponse"\x00\x12\xb6\x01\n\x15TerritoryMatrixDelete\x12L.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixDeleteRequest\x1aM.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixDeleteResponse"\x00\x12\xb0\x01\n\x13TerritoryMatrixLoad\x12J.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixLoadRequest\x1aK.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixLoadResponse"\x00\x12\xbf\x01\n\x18TerritoryMatrixStructure\x12O.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixStructureRequest\x1aP.pro.omni.oms.api.v1.utilities.territory_matrix.TerritoryMatrixStructureResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.territory_matrix_value_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.utilities.territory_matrix_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TERRITORYMATRIXVALUE"]._serialized_start = 181
-    _globals["_TERRITORYMATRIXVALUE"]._serialized_end = 422
-    _globals["_TERRITORYMATRIXVALUEADDREQUEST"]._serialized_start = 425
-    _globals["_TERRITORYMATRIXVALUEADDREQUEST"]._serialized_end = 655
-    _globals["_TERRITORYMATRIXVALUEADDRESPONSE"]._serialized_start = 658
-    _globals["_TERRITORYMATRIXVALUEADDRESPONSE"]._serialized_end = 874
-    _globals["_TERRITORYMATRIXVALUEREADREQUEST"]._serialized_start = 877
-    _globals["_TERRITORYMATRIXVALUEREADREQUEST"]._serialized_end = 1258
-    _globals["_TERRITORYMATRIXVALUEREADRESPONSE"]._serialized_start = 1261
-    _globals["_TERRITORYMATRIXVALUEREADRESPONSE"]._serialized_end = 1540
-    _globals["_TERRITORYMATRIXVALUEUPDATEREQUEST"]._serialized_start = 1543
-    _globals["_TERRITORYMATRIXVALUEUPDATEREQUEST"]._serialized_end = 1742
-    _globals["_TERRITORYMATRIXVALUEUPDATERESPONSE"]._serialized_start = 1745
-    _globals["_TERRITORYMATRIXVALUEUPDATERESPONSE"]._serialized_end = 1964
-    _globals["_TERRITORYMATRIXVALUEDELETEREQUEST"]._serialized_start = 1966
-    _globals["_TERRITORYMATRIXVALUEDELETEREQUEST"]._serialized_end = 2069
-    _globals["_TERRITORYMATRIXVALUEDELETERESPONSE"]._serialized_start = 2071
-    _globals["_TERRITORYMATRIXVALUEDELETERESPONSE"]._serialized_end = 2182
-    _globals["_TERRITORYMATRIXVALUESERVICE"]._serialized_start = 2185
-    _globals["_TERRITORYMATRIXVALUESERVICE"]._serialized_end = 3047
+    _globals["_TERRITORYMATRIX"]._serialized_start = 169
+    _globals["_TERRITORYMATRIX"]._serialized_end = 373
+    _globals["_TERRITORYMATRIXADDREQUEST"]._serialized_start = 376
+    _globals["_TERRITORYMATRIXADDREQUEST"]._serialized_end = 569
+    _globals["_TERRITORYMATRIXADDRESPONSE"]._serialized_start = 572
+    _globals["_TERRITORYMATRIXADDRESPONSE"]._serialized_end = 768
+    _globals["_TERRITORYMATRIXREADREQUEST"]._serialized_start = 771
+    _globals["_TERRITORYMATRIXREADREQUEST"]._serialized_end = 1147
+    _globals["_TERRITORYMATRIXREADRESPONSE"]._serialized_start = 1150
+    _globals["_TERRITORYMATRIXREADRESPONSE"]._serialized_end = 1406
+    _globals["_TERRITORYMATRIXUPDATEREQUEST"]._serialized_start = 1409
+    _globals["_TERRITORYMATRIXUPDATEREQUEST"]._serialized_end = 1586
+    _globals["_TERRITORYMATRIXUPDATERESPONSE"]._serialized_start = 1589
+    _globals["_TERRITORYMATRIXUPDATERESPONSE"]._serialized_end = 1788
+    _globals["_TERRITORYMATRIXDELETEREQUEST"]._serialized_start = 1790
+    _globals["_TERRITORYMATRIXDELETEREQUEST"]._serialized_end = 1888
+    _globals["_TERRITORYMATRIXDELETERESPONSE"]._serialized_start = 1890
+    _globals["_TERRITORYMATRIXDELETERESPONSE"]._serialized_end = 1996
+    _globals["_TERRITORYMATRIXLOADREQUEST"]._serialized_start = 1998
+    _globals["_TERRITORYMATRIXLOADREQUEST"]._serialized_end = 2122
+    _globals["_TERRITORYMATRIXLOADRESPONSE"]._serialized_start = 2124
+    _globals["_TERRITORYMATRIXLOADRESPONSE"]._serialized_end = 2228
+    _globals["_TERRITORYMATRIXSTRUCTUREREQUEST"]._serialized_start = 2231
+    _globals["_TERRITORYMATRIXSTRUCTUREREQUEST"]._serialized_end = 2431
+    _globals["_TERRITORYMATRIXSTRUCTURERESPONSE"]._serialized_start = 2434
+    _globals["_TERRITORYMATRIXSTRUCTURERESPONSE"]._serialized_end = 2599
+    _globals["_TERRITORYMATRIXSERVICE"]._serialized_start = 2602
+    _globals["_TERRITORYMATRIXSERVICE"]._serialized_end = 3724
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/protos/v1/utilities/uom_pb2_grpc.py` & `omni-pro-0.1.28/omni/pro/protos/v1/rules/country_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-from omni.pro.protos.v1.utilities import uom_pb2 as v1_dot_utilities_dot_uom__pb2
+from omni.pro.protos.v1.rules import country_pb2 as v1_dot_rules_dot_country__pb2
 
 
-class UomServiceStub(object):
+class CountryServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.UomCreate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
-            request_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
+        self.CountryCreate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryCreate",
+            request_serializer=v1_dot_rules_dot_country__pb2.CountryCreateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_country__pb2.CountryCreateResponse.FromString,
         )
-        self.UomRead = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
-            request_serializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
+        self.CountryRead = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryRead",
+            request_serializer=v1_dot_rules_dot_country__pb2.CountryReadRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_country__pb2.CountryReadResponse.FromString,
         )
-        self.UomUpdate = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
-            request_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
+        self.CountryUpdate = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryUpdate",
+            request_serializer=v1_dot_rules_dot_country__pb2.CountryUpdateRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_country__pb2.CountryUpdateResponse.FromString,
         )
-        self.UomDelete = channel.unary_unary(
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
-            request_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
-            response_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
+        self.CountryDelete = channel.unary_unary(
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryDelete",
+            request_serializer=v1_dot_rules_dot_country__pb2.CountryDeleteRequest.SerializeToString,
+            response_deserializer=v1_dot_rules_dot_country__pb2.CountryDeleteResponse.FromString,
         )
 
 
-class UomServiceServicer(object):
+class CountryServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def UomCreate(self, request, context):
+    def CountryCreate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def UomRead(self, request, context):
+    def CountryRead(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def UomUpdate(self, request, context):
+    def CountryUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
-    def UomDelete(self, request, context):
+    def CountryDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
-def add_UomServiceServicer_to_server(servicer, server):
+def add_CountryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "UomCreate": grpc.unary_unary_rpc_method_handler(
-            servicer.UomCreate,
-            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomCreateRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_uom__pb2.UomCreateResponse.SerializeToString,
+        "CountryCreate": grpc.unary_unary_rpc_method_handler(
+            servicer.CountryCreate,
+            request_deserializer=v1_dot_rules_dot_country__pb2.CountryCreateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_country__pb2.CountryCreateResponse.SerializeToString,
         ),
-        "UomRead": grpc.unary_unary_rpc_method_handler(
-            servicer.UomRead,
-            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomReadRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_uom__pb2.UomReadResponse.SerializeToString,
+        "CountryRead": grpc.unary_unary_rpc_method_handler(
+            servicer.CountryRead,
+            request_deserializer=v1_dot_rules_dot_country__pb2.CountryReadRequest.FromString,
+            response_serializer=v1_dot_rules_dot_country__pb2.CountryReadResponse.SerializeToString,
         ),
-        "UomUpdate": grpc.unary_unary_rpc_method_handler(
-            servicer.UomUpdate,
-            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.SerializeToString,
+        "CountryUpdate": grpc.unary_unary_rpc_method_handler(
+            servicer.CountryUpdate,
+            request_deserializer=v1_dot_rules_dot_country__pb2.CountryUpdateRequest.FromString,
+            response_serializer=v1_dot_rules_dot_country__pb2.CountryUpdateResponse.SerializeToString,
         ),
-        "UomDelete": grpc.unary_unary_rpc_method_handler(
-            servicer.UomDelete,
-            request_deserializer=v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.FromString,
-            response_serializer=v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.SerializeToString,
+        "CountryDelete": grpc.unary_unary_rpc_method_handler(
+            servicer.CountryDelete,
+            request_deserializer=v1_dot_rules_dot_country__pb2.CountryDeleteRequest.FromString,
+            response_serializer=v1_dot_rules_dot_country__pb2.CountryDeleteResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "pro.omni.oms.api.v1.utilities.uom.UomService", rpc_method_handlers
+        "pro.omni.oms.api.v1.rules.country.CountryService", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
-class UomService(object):
+class CountryService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def UomCreate(
+    def CountryCreate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomCreate",
-            v1_dot_utilities_dot_uom__pb2.UomCreateRequest.SerializeToString,
-            v1_dot_utilities_dot_uom__pb2.UomCreateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryCreate",
+            v1_dot_rules_dot_country__pb2.CountryCreateRequest.SerializeToString,
+            v1_dot_rules_dot_country__pb2.CountryCreateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def UomRead(
+    def CountryRead(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomRead",
-            v1_dot_utilities_dot_uom__pb2.UomReadRequest.SerializeToString,
-            v1_dot_utilities_dot_uom__pb2.UomReadResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryRead",
+            v1_dot_rules_dot_country__pb2.CountryReadRequest.SerializeToString,
+            v1_dot_rules_dot_country__pb2.CountryReadResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def UomUpdate(
+    def CountryUpdate(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomUpdate",
-            v1_dot_utilities_dot_uom__pb2.UomUpdateRequest.SerializeToString,
-            v1_dot_utilities_dot_uom__pb2.UomUpdateResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryUpdate",
+            v1_dot_rules_dot_country__pb2.CountryUpdateRequest.SerializeToString,
+            v1_dot_rules_dot_country__pb2.CountryUpdateResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
             metadata,
         )
 
     @staticmethod
-    def UomDelete(
+    def CountryDelete(
         request,
         target,
         options=(),
         channel_credentials=None,
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
-            "/pro.omni.oms.api.v1.utilities.uom.UomService/UomDelete",
-            v1_dot_utilities_dot_uom__pb2.UomDeleteRequest.SerializeToString,
-            v1_dot_utilities_dot_uom__pb2.UomDeleteResponse.FromString,
+            "/pro.omni.oms.api.v1.rules.country.CountryService/CountryDelete",
+            v1_dot_rules_dot_country__pb2.CountryDeleteRequest.SerializeToString,
+            v1_dot_rules_dot_country__pb2.CountryDeleteResponse.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `omni-pro-0.1.27/omni/pro/stack.py` & `omni-pro-0.1.28/omni/pro/stack.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni/pro/user/access.py` & `omni-pro-0.1.28/omni/pro/user/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     CAN_READ_GROUP = "CAN_READ_GROUP"
     CAN_UPDATE_GROUP = "CAN_UPDATE_GROUP"
     CAN_DELETE_GROUP = "CAN_DELETE_GROUP"
     CAN_CREATE_USER = "CAN_CREATE_USER"
     CAN_UPDATE_USER = "CAN_UPDATE_USER"
     CAN_READ_USER = "CAN_READ_USER"
     CAN_DELETE_USER = "CAN_DELETE_USER"
-    CAN_CHANGE_PASSWORD_USER = "CAN_CHAMGE_PASSWORD_USER"
+    CAN_CHANGE_PASSWORD_USER = "CAN_CHANGE_PASSWORD_USER"
     CAN_CHANGE_EMAIL_USER = "CAN_CHANGE_EMAIL_USER"
     CAN_ACCESS_TO_GROUP = "CAN_ACCESS_TO_GROUP"
     CAN_REMOVE_ACCESS_FROM_GROUP = "CAN_REMOVE_ACCESS_FROM_GROUP"
     CAN_GROUP_TO_USER = "CAN_GROUP_TO_USER"
     CAN_REMOVE_GROUP_FROM_USER = "CAN_REMOVE_GROUP_FROM_USER"
```

### Comparing `omni-pro-0.1.27/omni/pro/util.py` & `omni-pro-0.1.28/omni/pro/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import secrets
 import string
+import unicodedata
 from functools import reduce
 
 DEFAULT_RECORD_LIMIT = 10000
 
 
 def generate_strong_password(length=12):
     if length < 8:
@@ -110,14 +111,18 @@
 
 
 def to_camel_case(text: str):
     # Divide el texto por guiones bajos y une cada palabra con la primera letra en mayúsculas
     return "".join(word.capitalize() for word in text.split("_"))
 
 
+def normalize(value):
+    return unicodedata.normalize("NFKD", str(value).strip()).encode("ascii", "ignore").decode("UTF-8")
+
+
 class HTTPStatus(object):
     OK = 200
     CREATED = 201
     ACCEPTED = 202
     NO_CONTENT = 204
     BAD_REQUEST = 400
     UNAUTHORIZED = 401
```

### Comparing `omni-pro-0.1.27/omni/pro/validators.py` & `omni-pro-0.1.28/omni/pro/validators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.27/omni_pro.egg-info/PKG-INFO` & `omni-pro-0.1.28/omni_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.27
+Version: 0.1.28
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.27/omni_pro.egg-info/SOURCES.txt` & `omni-pro-0.1.28/omni_pro.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -74,50 +74,41 @@
 omni/pro/protos/v1/rules/__init__.py
 omni/pro/protos/v1/rules/calendar_pb2.py
 omni/pro/protos/v1/rules/calendar_pb2.pyi
 omni/pro/protos/v1/rules/calendar_pb2_grpc.py
 omni/pro/protos/v1/rules/category_pb2.py
 omni/pro/protos/v1/rules/category_pb2.pyi
 omni/pro/protos/v1/rules/category_pb2_grpc.py
-omni/pro/protos/v1/rules/delivery_category_category_pb2.py
-omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
-omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
+omni/pro/protos/v1/rules/country_pb2.py
+omni/pro/protos/v1/rules/country_pb2.pyi
+omni/pro/protos/v1/rules/country_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_category_pb2.py
 omni/pro/protos/v1/rules/delivery_category_pb2.pyi
 omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
 omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
 omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_locality_pb2.py
 omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
 omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_method_pb2.py
 omni/pro/protos/v1/rules/delivery_method_pb2.pyi
 omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
-omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
-omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
-omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
-omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
-omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
-omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
 omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
 omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_price_pb2.py
 omni/pro/protos/v1/rules/delivery_price_pb2.pyi
 omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
 omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
 omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_schedule_pb2.py
 omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
 omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
-omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
-omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
-omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
 omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
 omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_shipper_pb2.py
 omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
 omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
@@ -125,35 +116,29 @@
 omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_time_pb2.py
 omni/pro/protos/v1/rules/delivery_time_pb2.pyi
 omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
 omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
 omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
 omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
-omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
-omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
-omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
+omni/pro/protos/v1/rules/delivery_warehouse_pb2.py
+omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi
+omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py
 omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
 omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
 omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
 omni/pro/protos/v1/rules/location_pb2.py
 omni/pro/protos/v1/rules/location_pb2.pyi
 omni/pro/protos/v1/rules/location_pb2_grpc.py
 omni/pro/protos/v1/rules/schedule_work_line_pb2.py
 omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
 omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
 omni/pro/protos/v1/rules/schedule_work_pb2.py
 omni/pro/protos/v1/rules/schedule_work_pb2.pyi
 omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
-omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
-omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
-omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
-omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
-omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
-omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
 omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
 omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
 omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
 omni/pro/protos/v1/rules/warehouse_pb2.py
 omni/pro/protos/v1/rules/warehouse_pb2.pyi
 omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
 omni/pro/protos/v1/sales/__init__.py
```

### Comparing `omni-pro-0.1.27/setup.py` & `omni-pro-0.1.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 DESCRIPTION = "Python library designed to be a utility for OMS microservices"
-VERSION = "0.1.27"
+VERSION = "0.1.28"
 PACKAGE_NAME = "omni-pro"
 AUTHOR = "OMNI.PRO"
 AUTHOR_EMAIL = "development@omni.pro"
 URL = "https://github.com/Omnipro-Solutions/saas-ms-library"
 
 INSTALL_REQUIRES = [
     "protobuf==4.23.4",
```

