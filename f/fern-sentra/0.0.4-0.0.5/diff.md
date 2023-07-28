# Comparing `tmp/fern_sentra-0.0.4.tar.gz` & `tmp/fern_sentra-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_sentra-0.0.4.tar", max compression
+gzip compressed data, was "fern_sentra-0.0.5.tar", max compression
```

## Comparing `fern_sentra-0.0.4.tar` & `fern_sentra-0.0.5.tar`

### file list

```diff
@@ -1,266 +1,267 @@
--rw-r--r--   0        0        0     2693 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/README.md
--rw-r--r--   0        0        0      390 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    15065 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/__init__.py
--rw-r--r--   0        0        0     5264 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/client.py
--rw-r--r--   0        0        0      519 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/api_error.py
--rw-r--r--   0        0        0      629 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      230 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/errors/not_found_error.py
--rw-r--r--   0        0        0      313 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/py.typed
--rw-r--r--   0        0        0      618 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/alerts/__init__.py
--rw-r--r--   0        0        0    34052 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/alerts/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/api_keys/__init__.py
--rw-r--r--   0        0        0    14362 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/api_keys/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/audit_log/__init__.py
--rw-r--r--   0        0        0     9216 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/audit_log/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/connectors/__init__.py
--rw-r--r--   0        0        0    23046 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/connectors/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/context_labels/__init__.py
--rw-r--r--   0        0        0     5350 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/context_labels/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/dashboard/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/dashboard/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.468992 fern_sentra-0.0.4/src/sentra/resources/data_access/__init__.py
--rw-r--r--   0        0        0    55803 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_access/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_assets/__init__.py
--rw-r--r--   0        0        0    22416 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_assets/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_classes/__init__.py
--rw-r--r--   0        0        0    20576 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_classes/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_stores/__init__.py
--rw-r--r--   0        0        0    30920 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/data_stores/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/export/__init__.py
--rw-r--r--   0        0        0     9569 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/export/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/integrations/__init__.py
--rw-r--r--   0        0        0    13480 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/integrations/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/policies/__init__.py
--rw-r--r--   0        0        0    30702 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/policies/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/roles/__init__.py
--rw-r--r--   0        0        0     5355 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/roles/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/sensitivity/__init__.py
--rw-r--r--   0        0        0     3629 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/sensitivity/client.py
--rw-r--r--   0        0        0       65 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/users/__init__.py
--rw-r--r--   0        0        0    13257 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/resources/users/client.py
--rw-r--r--   0        0        0    21428 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/__init__.py
--rw-r--r--   0        0        0     1081 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/access_data_store.py
--rw-r--r--   0        0        0     1078 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/access_method_accessible_entities_flowchart.py
--rw-r--r--   0        0        0      897 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/access_permissions.py
--rw-r--r--   0        0        0      957 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/accessible_entities_flowchart_identity_node.py
--rw-r--r--   0        0        0     1009 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/accessible_entities_flowchart_store_node.py
--rw-r--r--   0        0        0     1177 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/account_type.py
--rw-r--r--   0        0        0      881 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_comment_schema.py
--rw-r--r--   0        0        0      847 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_entity_type.py
--rw-r--r--   0        0        0     1483 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_response_schema.py
--rw-r--r--   0        0        0     1901 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_response_schema_content.py
--rw-r--r--   0        0        0      782 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_stats_by_date.py
--rw-r--r--   0        0        0      676 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_status.py
--rw-r--r--   0        0        0     1201 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_status_reason.py
--rw-r--r--   0        0        0     1171 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/alert_type.py
--rw-r--r--   0        0        0      858 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/amazon_security_lake_integration.py
--rw-r--r--   0        0        0      938 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/amazon_security_lake_item.py
--rw-r--r--   0        0        0      952 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/app_schemas_assets_public_access_level.py
--rw-r--r--   0        0        0      952 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/app_schemas_stores_public_access_level.py
--rw-r--r--   0        0        0      960 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/asset_class_user_request.py
--rw-r--r--   0        0        0      886 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/asset_classes_props.py
--rw-r--r--   0        0        0      931 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/asset_type.py
--rw-r--r--   0        0        0      945 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/auth_token_row.py
--rw-r--r--   0        0        0      910 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/auth_token_schema.py
--rw-r--r--   0        0        0     1452 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/aws_connector_args.py
--rw-r--r--   0        0        0      523 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/aws_installation_mode.py
--rw-r--r--   0        0        0      829 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/azure_boards_integration.py
--rw-r--r--   0        0        0      946 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/azure_boards_item.py
--rw-r--r--   0        0        0     1348 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/azure_connector_args.py
--rw-r--r--   0        0        0      807 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/choice_filter_data.py
--rw-r--r--   0        0        0     1027 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/class_categories.py
--rw-r--r--   0        0        0      784 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/class_config.py
--rw-r--r--   0        0        0      494 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/class_source.py
--rw-r--r--   0        0        0      909 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/classification_result_example.py
--rw-r--r--   0        0        0      518 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/classifier_type.py
--rw-r--r--   0        0        0      545 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/compute_connectivity_type.py
--rw-r--r--   0        0        0     1105 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_aws.py
--rw-r--r--   0        0        0      929 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_azure.py
--rw-r--r--   0        0        0      909 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_gcp.py
--rw-r--r--   0        0        0     1511 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_display.py
--rw-r--r--   0        0        0      510 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_display_args.py
--rw-r--r--   0        0        0     1213 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_display_compute_properties.py
--rw-r--r--   0        0        0     1287 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_input.py
--rw-r--r--   0        0        0      508 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_input_args.py
--rw-r--r--   0        0        0     1190 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_input_compute_properties.py
--rw-r--r--   0        0        0     1476 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_schema.py
--rw-r--r--   0        0        0      509 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_schema_args.py
--rw-r--r--   0        0        0     1197 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/connector_schema_compute_properties.py
--rw-r--r--   0        0        0      844 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/context_label_schema.py
--rw-r--r--   0        0        0      218 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/create_api_v_2_connectors_post_request.py
--rw-r--r--   0        0        0      228 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/create_api_v_2_integrations_post_request.py
--rw-r--r--   0        0        0      897 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/current_user_data.py
--rw-r--r--   0        0        0      802 2023-07-28 05:36:38.472992 fern_sentra-0.0.4/src/sentra/types/dashboard_data.py
--rw-r--r--   0        0        0      956 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_at_risk.py
--rw-r--r--   0        0        0      527 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_class_user_operation.py
--rw-r--r--   0        0        0     2714 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_extended.py
--rw-r--r--   0        0        0     1012 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_object.py
--rw-r--r--   0        0        0     1457 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_props.py
--rw-r--r--   0        0        0     2123 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_row.py
--rw-r--r--   0        0        0     1969 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_asset_schema.py
--rw-r--r--   0        0        0     1538 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_class_config_schema.py
--rw-r--r--   0        0        0     1579 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_class_config_with_user_schema.py
--rw-r--r--   0        0        0     1131 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_class_item.py
--rw-r--r--   0        0        0     1492 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_class_schema.py
--rw-r--r--   0        0        0      848 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_dog_integration.py
--rw-r--r--   0        0        0      972 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_dog_item.py
--rw-r--r--   0        0        0      763 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_dog_region.py
--rw-r--r--   0        0        0     1515 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_hub_fabric.py
--rw-r--r--   0        0        0      813 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_hub_integration.py
--rw-r--r--   0        0        0      999 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_hub_item.py
--rw-r--r--   0        0        0      835 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_access_metadata.py
--rw-r--r--   0        0        0     2481 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_extended.py
--rw-r--r--   0        0        0      999 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_identity.py
--rw-r--r--   0        0        0     2404 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_props.py
--rw-r--r--   0        0        0      878 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_risk_aggregation.py
--rw-r--r--   0        0        0     2110 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/data_store_row.py
--rw-r--r--   0        0        0     1877 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema.py
--rw-r--r--   0        0        0     1901 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_content.py
--rw-r--r--   0        0        0     2025 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_with_comment.py
--rw-r--r--   0        0        0     2022 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_with_comment_content.py
--rw-r--r--   0        0        0     1201 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_iam_group_schema.py
--rw-r--r--   0        0        0     1280 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/detailed_iam_role_schema.py
--rw-r--r--   0        0        0      937 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/email_input_item.py
--rw-r--r--   0        0        0      858 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/email_integration.py
--rw-r--r--   0        0        0      860 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/email_integration_input.py
--rw-r--r--   0        0        0      926 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/email_output_item.py
--rw-r--r--   0        0        0     5757 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/event_log_action.py
--rw-r--r--   0        0        0     1687 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/event_log_entity_type.py
--rw-r--r--   0        0        0     1129 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/event_log_row.py
--rw-r--r--   0        0        0     2149 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/external_classifier_config.py
--rw-r--r--   0        0        0      899 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_item.py
--rw-r--r--   0        0        0      224 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_item_value.py
--rw-r--r--   0        0        0     1316 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_specs.py
--rw-r--r--   0        0        0      214 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_specs_and_item.py
--rw-r--r--   0        0        0      214 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_specs_not_item.py
--rw-r--r--   0        0        0      213 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/filter_specs_or_item.py
--rw-r--r--   0        0        0      510 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/format_type.py
--rw-r--r--   0        0        0     1138 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/gcp_connector_args.py
--rw-r--r--   0        0        0      284 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_alerts_get_response.py
--rw-r--r--   0        0        0      303 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_audit_log_get_response.py
--rw-r--r--   0        0        0      353 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_classes_get_response.py
--rw-r--r--   0        0        0      332 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_connectors_get_response.py
--rw-r--r--   0        0        0      320 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_data_access_identities_get_response.py
--rw-r--r--   0        0        0      298 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_data_assets_get_response.py
--rw-r--r--   0        0        0      302 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_policies_get_response.py
--rw-r--r--   0        0        0      290 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_roles_get_response.py
--rw-r--r--   0        0        0      290 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_api_v_2_users_get_response.py
--rw-r--r--   0        0        0      319 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_all_external_api_v_2_data_stores_get_response.py
--rw-r--r--   0        0        0      282 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_alerts_filter_name_get_response.py
--rw-r--r--   0        0        0      283 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_classes_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_data_access_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_data_assets_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_data_stores_filter_name_get_response.py
--rw-r--r--   0        0        0      284 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/get_filter_api_v_2_policies_filter_name_get_response.py
--rw-r--r--   0        0        0      853 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/group_item.py
--rw-r--r--   0        0        0      947 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/grouped_data_table_result.py
--rw-r--r--   0        0        0      843 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/http_validation_error.py
--rw-r--r--   0        0        0      888 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/iam_access_key_schema.py
--rw-r--r--   0        0        0      885 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/iam_group_data_classes.py
--rw-r--r--   0        0        0      951 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/iam_group_schema.py
--rw-r--r--   0        0        0      884 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/iam_role_data_classes.py
--rw-r--r--   0        0        0     1030 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/iam_role_schema.py
--rw-r--r--   0        0        0     1262 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart.py
--rw-r--r--   0        0        0      937 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py
--rw-r--r--   0        0        0      945 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_group.py
--rw-r--r--   0        0        0      943 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_role.py
--rw-r--r--   0        0        0      523 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_origin.py
--rw-r--r--   0        0        0     1623 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/identity_schema.py
--rw-r--r--   0        0        0     1117 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_display.py
--rw-r--r--   0        0        0     1080 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_display_properties.py
--rw-r--r--   0        0        0      981 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_input.py
--rw-r--r--   0        0        0     1126 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_input_properties.py
--rw-r--r--   0        0        0     1110 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_output_schema.py
--rw-r--r--   0        0        0     1085 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_output_schema_properties.py
--rw-r--r--   0        0        0     1085 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_schema.py
--rw-r--r--   0        0        0     1127 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_schema_properties.py
--rw-r--r--   0        0        0     2067 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/integration_type.py
--rw-r--r--   0        0        0      835 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/jira_integration.py
--rw-r--r--   0        0        0      946 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/jira_item.py
--rw-r--r--   0        0        0      764 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/keyword_requirement.py
--rw-r--r--   0        0        0      974 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_alerts_response.py
--rw-r--r--   0        0        0      956 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_assets_response.py
--rw-r--r--   0        0        0      960 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_auth_tokens_response.py
--rw-r--r--   0        0        0      978 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_connector_displays_response.py
--rw-r--r--   0        0        0      980 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_context_label_response.py
--rw-r--r--   0        0        0     1028 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_data_class_config_with_users_response.py
--rw-r--r--   0        0        0      960 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_data_stores_response.py
--rw-r--r--   0        0        0      955 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_event_log_response.py
--rw-r--r--   0        0        0      965 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_identities_response.py
--rw-r--r--   0        0        0      957 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_policies_response.py
--rw-r--r--   0        0        0      948 2023-07-28 05:36:38.476992 fern_sentra-0.0.4/src/sentra/types/list_all_roles_response.py
--rw-r--r--   0        0        0      948 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/list_all_users_response.py
--rw-r--r--   0        0        0      979 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/list_similar_assets_pair_response.py
--rw-r--r--   0        0        0      978 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/list_similar_assets_response.py
--rw-r--r--   0        0        0      980 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/list_violated_data_assets_response.py
--rw-r--r--   0        0        0      967 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/list_violated_objects_response.py
--rw-r--r--   0        0        0     1133 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/microsoft_365_connector_args.py
--rw-r--r--   0        0        0      843 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/monday_integration.py
--rw-r--r--   0        0        0      973 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/monday_item.py
--rw-r--r--   0        0        0      842 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/new_auth_token_response.py
--rw-r--r--   0        0        0      775 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/object_class.py
--rw-r--r--   0        0        0      830 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/open_alerts_aggregation.py
--rw-r--r--   0        0        0      821 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/pager_duty_integration.py
--rw-r--r--   0        0        0      932 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/pager_duty_item.py
--rw-r--r--   0        0        0     7556 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/permissions.py
--rw-r--r--   0        0        0     1061 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_rule.py
--rw-r--r--   0        0        0     1169 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_rule_entity.py
--rw-r--r--   0        0        0      503 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_rule_type.py
--rw-r--r--   0        0        0     1738 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_schema.py
--rw-r--r--   0        0        0      797 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_severity.py
--rw-r--r--   0        0        0      512 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_status.py
--rw-r--r--   0        0        0      536 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_triggering_type.py
--rw-r--r--   0        0        0      682 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_type.py
--rw-r--r--   0        0        0      874 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/policy_update_response.py
--rw-r--r--   0        0        0      835 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/provider_minimal_metadata.py
--rw-r--r--   0        0        0      955 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/provider_schema.py
--rw-r--r--   0        0        0     1604 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/provider_types.py
--rw-r--r--   0        0        0      795 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/range_filter_data.py
--rw-r--r--   0        0        0      533 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/resolved_alert_source.py
--rw-r--r--   0        0        0     1897 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/risk_type.py
--rw-r--r--   0        0        0     1173 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/role_identity.py
--rw-r--r--   0        0        0      877 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/role_schema.py
--rw-r--r--   0        0        0     1229 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/runtime_properties.py
--rw-r--r--   0        0        0      911 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/schedule_properties.py
--rw-r--r--   0        0        0      828 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/seemplicity_integration.py
--rw-r--r--   0        0        0      902 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/seemplicity_item.py
--rw-r--r--   0        0        0      859 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/sensitivity_levels.py
--rw-r--r--   0        0        0       83 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/session_type.py
--rw-r--r--   0        0        0     2982 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_asset_schema.py
--rw-r--r--   0        0        0      812 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_assets_alert_content.py
--rw-r--r--   0        0        0     1037 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_assets_pair.py
--rw-r--r--   0        0        0     1065 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_assets_pair_schema.py
--rw-r--r--   0        0        0      789 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_assets_props.py
--rw-r--r--   0        0        0      914 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similar_store.py
--rw-r--r--   0        0        0      523 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/similarity_type.py
--rw-r--r--   0        0        0      846 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/slack_integration.py
--rw-r--r--   0        0        0      848 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/slack_integration_input.py
--rw-r--r--   0        0        0     1113 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/slack_web_hook_input_item.py
--rw-r--r--   0        0        0     1102 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/slack_web_hook_output_item.py
--rw-r--r--   0        0        0     1106 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/snowflake_connector_args.py
--rw-r--r--   0        0        0      811 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/sort.py
--rw-r--r--   0        0        0      463 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/sort_order.py
--rw-r--r--   0        0        0      823 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/teams_integration.py
--rw-r--r--   0        0        0      896 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/teams_output_item.py
--rw-r--r--   0        0        0      775 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/test_connection_result.py
--rw-r--r--   0        0        0      872 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/user_schema.py
--rw-r--r--   0        0        0      506 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/user_status.py
--rw-r--r--   0        0        0      788 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/validation_error.py
--rw-r--r--   0        0        0     2436 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_data_asset.py
--rw-r--r--   0        0        0      747 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_iam_group_alert_content.py
--rw-r--r--   0        0        0      746 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_iam_role_alert_content.py
--rw-r--r--   0        0        0      747 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_identity_alert_content.py
--rw-r--r--   0        0        0      963 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_object.py
--rw-r--r--   0        0        0      786 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/violated_store_alert_content.py
--rw-r--r--   0        0        0      945 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/web_hook_input_item.py
--rw-r--r--   0        0        0      832 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/web_hook_integration.py
--rw-r--r--   0        0        0      834 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/web_hook_integration_input.py
--rw-r--r--   0        0        0      934 2023-07-28 05:36:38.480992 fern_sentra-0.0.4/src/sentra/types/web_hook_output_item.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 fern_sentra-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2693 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/README.md
+-rw-r--r--   0        0        0      390 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    16435 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/client.py
+-rw-r--r--   0        0        0      519 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/api_error.py
+-rw-r--r--   0        0        0      765 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      156 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/environment.py
+-rw-r--r--   0        0        0      230 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/not_found_error.py
+-rw-r--r--   0        0        0      313 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/py.typed
+-rw-r--r--   0        0        0      618 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/alerts/__init__.py
+-rw-r--r--   0        0        0    34335 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/alerts/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/api_keys/__init__.py
+-rw-r--r--   0        0        0    14573 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/api_keys/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/audit_log/__init__.py
+-rw-r--r--   0        0        0    12862 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/audit_log/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/connectors/__init__.py
+-rw-r--r--   0        0        0    23305 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/connectors/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/context_labels/__init__.py
+-rw-r--r--   0        0        0     5525 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/context_labels/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/dashboard/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/dashboard/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_access/__init__.py
+-rw-r--r--   0        0        0    56254 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_access/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_assets/__init__.py
+-rw-r--r--   0        0        0    22663 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_assets/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_classes/__init__.py
+-rw-r--r--   0        0        0    25370 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_classes/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_stores/__init__.py
+-rw-r--r--   0        0        0    31203 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_stores/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/export/__init__.py
+-rw-r--r--   0        0        0     9780 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/export/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/integrations/__init__.py
+-rw-r--r--   0        0        0    13703 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/integrations/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/policies/__init__.py
+-rw-r--r--   0        0        0    30961 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/policies/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/roles/__init__.py
+-rw-r--r--   0        0        0     5530 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/roles/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/sensitivity/__init__.py
+-rw-r--r--   0        0        0     3804 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/sensitivity/client.py
+-rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/users/__init__.py
+-rw-r--r--   0        0        0    13468 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/users/client.py
+-rw-r--r--   0        0        0    23027 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_data_store.py
+-rw-r--r--   0        0        0     1078 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_method_accessible_entities_flowchart.py
+-rw-r--r--   0        0        0      897 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_permissions.py
+-rw-r--r--   0        0        0      957 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_identity_node.py
+-rw-r--r--   0        0        0     1009 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_store_node.py
+-rw-r--r--   0        0        0     1177 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/account_type.py
+-rw-r--r--   0        0        0      881 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_comment_schema.py
+-rw-r--r--   0        0        0      847 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_entity_type.py
+-rw-r--r--   0        0        0     1483 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_response_schema.py
+-rw-r--r--   0        0        0     1901 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_response_schema_content.py
+-rw-r--r--   0        0        0      782 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_stats_by_date.py
+-rw-r--r--   0        0        0      676 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_status.py
+-rw-r--r--   0        0        0     1201 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_status_reason.py
+-rw-r--r--   0        0        0     1171 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_type.py
+-rw-r--r--   0        0        0      858 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_integration.py
+-rw-r--r--   0        0        0      938 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_item.py
+-rw-r--r--   0        0        0      952 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/app_schemas_assets_public_access_level.py
+-rw-r--r--   0        0        0      952 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/app_schemas_stores_public_access_level.py
+-rw-r--r--   0        0        0      960 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_class_user_request.py
+-rw-r--r--   0        0        0      886 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_classes_props.py
+-rw-r--r--   0        0        0      931 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_type.py
+-rw-r--r--   0        0        0      945 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/auth_token_row.py
+-rw-r--r--   0        0        0      910 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/auth_token_schema.py
+-rw-r--r--   0        0        0     1452 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/aws_connector_args.py
+-rw-r--r--   0        0        0      523 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/aws_installation_mode.py
+-rw-r--r--   0        0        0      829 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_boards_integration.py
+-rw-r--r--   0        0        0      946 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_boards_item.py
+-rw-r--r--   0        0        0     1348 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_connector_args.py
+-rw-r--r--   0        0        0      807 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/choice_filter_data.py
+-rw-r--r--   0        0        0     1394 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema.py
+-rw-r--r--   0        0        0     1301 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema_classifier_config.py
+-rw-r--r--   0        0        0     1027 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_categories.py
+-rw-r--r--   0        0        0      494 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_source.py
+-rw-r--r--   0        0        0      909 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/classification_result_example.py
+-rw-r--r--   0        0        0      545 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connectivity_type.py
+-rw-r--r--   0        0        0     1105 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_aws.py
+-rw-r--r--   0        0        0      929 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_azure.py
+-rw-r--r--   0        0        0      909 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_gcp.py
+-rw-r--r--   0        0        0     1511 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display.py
+-rw-r--r--   0        0        0      510 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display_args.py
+-rw-r--r--   0        0        0     1213 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display_compute_properties.py
+-rw-r--r--   0        0        0     1287 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input.py
+-rw-r--r--   0        0        0      508 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input_args.py
+-rw-r--r--   0        0        0     1190 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input_compute_properties.py
+-rw-r--r--   0        0        0     1476 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema.py
+-rw-r--r--   0        0        0      509 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema_args.py
+-rw-r--r--   0        0        0     1197 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema_compute_properties.py
+-rw-r--r--   0        0        0      844 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/context_label_schema.py
+-rw-r--r--   0        0        0      218 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_api_v_2_connectors_post_request.py
+-rw-r--r--   0        0        0      228 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_api_v_2_integrations_post_request.py
+-rw-r--r--   0        0        0      954 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_class_request_schema_classifier_schema.py
+-rw-r--r--   0        0        0     1010 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/create_dictionary_classifier_request_schema.py
+-rw-r--r--   0        0        0     1066 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/create_regex_classifier_request_schema.py
+-rw-r--r--   0        0        0      897 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/current_user_data.py
+-rw-r--r--   0        0        0      802 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/dashboard_data.py
+-rw-r--r--   0        0        0      956 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_at_risk.py
+-rw-r--r--   0        0        0      527 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_class_user_operation.py
+-rw-r--r--   0        0        0     2714 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_extended.py
+-rw-r--r--   0        0        0     1012 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_object.py
+-rw-r--r--   0        0        0     1457 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_props.py
+-rw-r--r--   0        0        0     2163 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_row.py
+-rw-r--r--   0        0        0     1969 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_schema.py
+-rw-r--r--   0        0        0     1283 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_class_config_with_user_schema.py
+-rw-r--r--   0        0        0     1131 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_class_item.py
+-rw-r--r--   0        0        0      848 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_integration.py
+-rw-r--r--   0        0        0      972 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_item.py
+-rw-r--r--   0        0        0      763 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_region.py
+-rw-r--r--   0        0        0     1515 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_fabric.py
+-rw-r--r--   0        0        0      813 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_integration.py
+-rw-r--r--   0        0        0      999 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_item.py
+-rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_access_metadata.py
+-rw-r--r--   0        0        0     2481 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_extended.py
+-rw-r--r--   0        0        0      999 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_identity.py
+-rw-r--r--   0        0        0     2404 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_props.py
+-rw-r--r--   0        0        0      878 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_risk_aggregation.py
+-rw-r--r--   0        0        0     2110 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_row.py
+-rw-r--r--   0        0        0     1877 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema.py
+-rw-r--r--   0        0        0     1901 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_content.py
+-rw-r--r--   0        0        0     2025 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment.py
+-rw-r--r--   0        0        0     2022 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment_content.py
+-rw-r--r--   0        0        0     1201 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_iam_group_schema.py
+-rw-r--r--   0        0        0     1280 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_iam_role_schema.py
+-rw-r--r--   0        0        0      927 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/dictionary_classifier_response.py
+-rw-r--r--   0        0        0      920 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_input_item.py
+-rw-r--r--   0        0        0      858 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_integration.py
+-rw-r--r--   0        0        0      860 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_integration_input.py
+-rw-r--r--   0        0        0      926 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_output_item.py
+-rw-r--r--   0        0        0     5757 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_action.py
+-rw-r--r--   0        0        0     1687 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_entity_type.py
+-rw-r--r--   0        0        0     1129 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_row.py
+-rw-r--r--   0        0        0     1138 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/gcp_connector_args.py
+-rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_alerts_get_response.py
+-rw-r--r--   0        0        0      303 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_audit_log_get_response.py
+-rw-r--r--   0        0        0      353 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_classes_get_response.py
+-rw-r--r--   0        0        0      332 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_connectors_get_response.py
+-rw-r--r--   0        0        0      320 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_data_access_identities_get_response.py
+-rw-r--r--   0        0        0      298 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_data_assets_get_response.py
+-rw-r--r--   0        0        0      302 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_policies_get_response.py
+-rw-r--r--   0        0        0      290 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_roles_get_response.py
+-rw-r--r--   0        0        0      290 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_users_get_response.py
+-rw-r--r--   0        0        0      319 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_external_api_v_2_data_stores_get_response.py
+-rw-r--r--   0        0        0      282 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_alerts_filter_name_get_response.py
+-rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_audit_log_filter_name_get_response.py
+-rw-r--r--   0        0        0      283 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_classes_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_access_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_assets_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_stores_filter_name_get_response.py
+-rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_policies_filter_name_get_response.py
+-rw-r--r--   0        0        0      853 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/group_item.py
+-rw-r--r--   0        0        0      947 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/grouped_data_table_result.py
+-rw-r--r--   0        0        0      843 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/http_validation_error.py
+-rw-r--r--   0        0        0      888 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_access_key_schema.py
+-rw-r--r--   0        0        0      885 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_group_data_classes.py
+-rw-r--r--   0        0        0      951 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_group_schema.py
+-rw-r--r--   0        0        0      884 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_role_data_classes.py
+-rw-r--r--   0        0        0     1030 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_role_schema.py
+-rw-r--r--   0        0        0     1262 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart.py
+-rw-r--r--   0        0        0      937 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py
+-rw-r--r--   0        0        0      945 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_group.py
+-rw-r--r--   0        0        0      943 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_role.py
+-rw-r--r--   0        0        0      523 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_origin.py
+-rw-r--r--   0        0        0     1623 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_schema.py
+-rw-r--r--   0        0        0     1117 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_display.py
+-rw-r--r--   0        0        0     1080 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_display_properties.py
+-rw-r--r--   0        0        0      981 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_input.py
+-rw-r--r--   0        0        0     1126 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_input_properties.py
+-rw-r--r--   0        0        0     1110 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_output_schema.py
+-rw-r--r--   0        0        0     1085 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_output_schema_properties.py
+-rw-r--r--   0        0        0     1085 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_schema.py
+-rw-r--r--   0        0        0     1127 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_schema_properties.py
+-rw-r--r--   0        0        0     2067 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_type.py
+-rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/jira_integration.py
+-rw-r--r--   0        0        0      946 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/jira_item.py
+-rw-r--r--   0        0        0      764 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/keyword_requirement.py
+-rw-r--r--   0        0        0      974 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_alerts_response.py
+-rw-r--r--   0        0        0      956 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_assets_response.py
+-rw-r--r--   0        0        0      960 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_auth_tokens_response.py
+-rw-r--r--   0        0        0      978 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_connector_displays_response.py
+-rw-r--r--   0        0        0      980 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_context_label_response.py
+-rw-r--r--   0        0        0     1028 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_data_class_config_with_users_response.py
+-rw-r--r--   0        0        0      960 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_data_stores_response.py
+-rw-r--r--   0        0        0      955 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_event_log_response.py
+-rw-r--r--   0        0        0      965 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_identities_response.py
+-rw-r--r--   0        0        0      957 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_policies_response.py
+-rw-r--r--   0        0        0      948 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_roles_response.py
+-rw-r--r--   0        0        0      948 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_users_response.py
+-rw-r--r--   0        0        0      979 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_similar_assets_pair_response.py
+-rw-r--r--   0        0        0      978 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_similar_assets_response.py
+-rw-r--r--   0        0        0      980 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_violated_data_assets_response.py
+-rw-r--r--   0        0        0      967 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_violated_objects_response.py
+-rw-r--r--   0        0        0     1133 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/microsoft_365_connector_args.py
+-rw-r--r--   0        0        0      843 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/monday_integration.py
+-rw-r--r--   0        0        0      973 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/monday_item.py
+-rw-r--r--   0        0        0      842 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/new_auth_token_response.py
+-rw-r--r--   0        0        0      775 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/object_class.py
+-rw-r--r--   0        0        0      830 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/open_alerts_aggregation.py
+-rw-r--r--   0        0        0      821 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/pager_duty_integration.py
+-rw-r--r--   0        0        0      932 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/pager_duty_item.py
+-rw-r--r--   0        0        0     7556 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/permissions.py
+-rw-r--r--   0        0        0     1061 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule.py
+-rw-r--r--   0        0        0     1169 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule_entity.py
+-rw-r--r--   0        0        0      503 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule_type.py
+-rw-r--r--   0        0        0     1698 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_schema.py
+-rw-r--r--   0        0        0      797 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_severity.py
+-rw-r--r--   0        0        0      512 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_status.py
+-rw-r--r--   0        0        0      536 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_triggering_type.py
+-rw-r--r--   0        0        0      682 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_type.py
+-rw-r--r--   0        0        0      874 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_update_response.py
+-rw-r--r--   0        0        0      836 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/proprietary_classifier_response.py
+-rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_minimal_metadata.py
+-rw-r--r--   0        0        0      955 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_schema.py
+-rw-r--r--   0        0        0     1604 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_types.py
+-rw-r--r--   0        0        0      795 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/range_filter_data.py
+-rw-r--r--   0        0        0      891 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/regex_classifier_response.py
+-rw-r--r--   0        0        0      533 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/resolved_alert_source.py
+-rw-r--r--   0        0        0     1897 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/risk_type.py
+-rw-r--r--   0        0        0     1173 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/role_identity.py
+-rw-r--r--   0        0        0      877 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/role_schema.py
+-rw-r--r--   0        0        0     1229 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/runtime_properties.py
+-rw-r--r--   0        0        0      911 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/schedule_properties.py
+-rw-r--r--   0        0        0      828 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/seemplicity_integration.py
+-rw-r--r--   0        0        0      902 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/seemplicity_item.py
+-rw-r--r--   0        0        0      859 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sensitivity_levels.py
+-rw-r--r--   0        0        0       83 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/session_type.py
+-rw-r--r--   0        0        0     2982 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_asset_schema.py
+-rw-r--r--   0        0        0      812 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_alert_content.py
+-rw-r--r--   0        0        0     1037 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_pair.py
+-rw-r--r--   0        0        0     1065 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_pair_schema.py
+-rw-r--r--   0        0        0      789 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_props.py
+-rw-r--r--   0        0        0      914 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_store.py
+-rw-r--r--   0        0        0      523 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similarity_type.py
+-rw-r--r--   0        0        0      846 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_integration.py
+-rw-r--r--   0        0        0      848 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_integration_input.py
+-rw-r--r--   0        0        0     1096 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_web_hook_input_item.py
+-rw-r--r--   0        0        0     1102 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_web_hook_output_item.py
+-rw-r--r--   0        0        0     1106 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/snowflake_connector_args.py
+-rw-r--r--   0        0        0      811 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sort.py
+-rw-r--r--   0        0        0      463 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sort_order.py
+-rw-r--r--   0        0        0      823 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/teams_integration.py
+-rw-r--r--   0        0        0      896 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/teams_output_item.py
+-rw-r--r--   0        0        0      775 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/test_connection_result.py
+-rw-r--r--   0        0        0      954 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_class_request_schema_classifier_schema.py
+-rw-r--r--   0        0        0     1010 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_dictionary_classifier_request_schema.py
+-rw-r--r--   0        0        0     1083 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_regex_classifier_request_schema.py
+-rw-r--r--   0        0        0      872 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/user_schema.py
+-rw-r--r--   0        0        0      506 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/user_status.py
+-rw-r--r--   0        0        0      788 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/validation_error.py
+-rw-r--r--   0        0        0     2436 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_data_asset.py
+-rw-r--r--   0        0        0      747 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_iam_group_alert_content.py
+-rw-r--r--   0        0        0      746 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_iam_role_alert_content.py
+-rw-r--r--   0        0        0      747 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_identity_alert_content.py
+-rw-r--r--   0        0        0      963 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_object.py
+-rw-r--r--   0        0        0      786 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_store_alert_content.py
+-rw-r--r--   0        0        0      928 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_input_item.py
+-rw-r--r--   0        0        0      832 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_integration.py
+-rw-r--r--   0        0        0      834 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_integration_input.py
+-rw-r--r--   0        0        0      934 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_output_item.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 fern_sentra-0.0.5/PKG-INFO
```

### Comparing `fern_sentra-0.0.4/README.md` & `fern_sentra-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/__init__.py` & `fern_sentra-0.0.5/src/sentra/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,19 +31,22 @@
     AuthTokenSchema,
     AwsConnectorArgs,
     AwsInstallationMode,
     AzureBoardsIntegration,
     AzureBoardsItem,
     AzureConnectorArgs,
     ChoiceFilterData,
+    ClassAndClassifierConfigSchema,
+    ClassAndClassifierConfigSchemaClassifierConfig,
+    ClassAndClassifierConfigSchemaClassifierConfig_Dictionary,
+    ClassAndClassifierConfigSchemaClassifierConfig_Proprietary,
+    ClassAndClassifierConfigSchemaClassifierConfig_Regex,
     ClassCategories,
-    ClassConfig,
     ClassSource,
     ClassificationResultExample,
-    ClassifierType,
     ComputeConnectivityType,
     ComputeConnectorPropertiesAws,
     ComputeConnectorPropertiesAzure,
     ComputeConnectorPropertiesGcp,
     ConnectorDisplay,
     ConnectorDisplayArgs,
     ConnectorDisplayComputeProperties,
@@ -61,27 +64,30 @@
     ConnectorSchemaComputeProperties,
     ConnectorSchemaComputeProperties_Aws,
     ConnectorSchemaComputeProperties_Azure,
     ConnectorSchemaComputeProperties_Gcp,
     ContextLabelSchema,
     CreateApiV2ConnectorsPostRequest,
     CreateApiV2IntegrationsPostRequest,
+    CreateClassRequestSchemaClassifierSchema,
+    CreateClassRequestSchemaClassifierSchema_Dictionary,
+    CreateClassRequestSchemaClassifierSchema_Regex,
+    CreateDictionaryClassifierRequestSchema,
+    CreateRegexClassifierRequestSchema,
     CurrentUserData,
     DashboardData,
     DataAssetAtRisk,
     DataAssetClassUserOperation,
     DataAssetExtended,
     DataAssetObject,
     DataAssetProps,
     DataAssetRow,
     DataAssetSchema,
-    DataClassConfigSchema,
     DataClassConfigWithUserSchema,
     DataClassItem,
-    DataClassSchema,
     DataDogIntegration,
     DataDogItem,
     DataDogRegion,
     DataHubFabric,
     DataHubIntegration,
     DataHubItem,
     DataStoreAccessMetadata,
@@ -102,41 +108,35 @@
     DetailedAlertSchemaWithCommentContent_SimilarAssets,
     DetailedAlertSchemaWithCommentContent_ViolatedIamGroup,
     DetailedAlertSchemaWithCommentContent_ViolatedIamRole,
     DetailedAlertSchemaWithCommentContent_ViolatedIdentity,
     DetailedAlertSchemaWithCommentContent_ViolatedStore,
     DetailedIamGroupSchema,
     DetailedIamRoleSchema,
+    DictionaryClassifierResponse,
     EmailInputItem,
     EmailIntegration,
     EmailIntegrationInput,
     EmailOutputItem,
     EventLogAction,
     EventLogEntityType,
     EventLogRow,
-    ExternalClassifierConfig,
-    FilterItem,
-    FilterItemValue,
-    FilterSpecs,
-    FilterSpecsAndItem,
-    FilterSpecsNotItem,
-    FilterSpecsOrItem,
-    FormatType,
     GcpConnectorArgs,
     GetAllApiV2AlertsGetResponse,
     GetAllApiV2AuditLogGetResponse,
     GetAllApiV2ClassesGetResponse,
     GetAllApiV2ConnectorsGetResponse,
     GetAllApiV2DataAccessIdentitiesGetResponse,
     GetAllApiV2DataAssetsGetResponse,
     GetAllApiV2PoliciesGetResponse,
     GetAllApiV2RolesGetResponse,
     GetAllApiV2UsersGetResponse,
     GetAllExternalApiV2DataStoresGetResponse,
     GetFilterApiV2AlertsFilterNameGetResponse,
+    GetFilterApiV2AuditLogFilterNameGetResponse,
     GetFilterApiV2ClassesFilterNameGetResponse,
     GetFilterApiV2DataAccessFilterNameGetResponse,
     GetFilterApiV2DataAssetsFilterNameGetResponse,
     GetFilterApiV2DataStoresFilterNameGetResponse,
     GetFilterApiV2PoliciesFilterNameGetResponse,
     GroupItem,
     GroupedDataTableResult,
@@ -194,18 +194,20 @@
     PolicyRuleType,
     PolicySchema,
     PolicySeverity,
     PolicyStatus,
     PolicyTriggeringType,
     PolicyType,
     PolicyUpdateResponse,
+    ProprietaryClassifierResponse,
     ProviderMinimalMetadata,
     ProviderSchema,
     ProviderTypes,
     RangeFilterData,
+    RegexClassifierResponse,
     ResolvedAlertSource,
     RiskType,
     RoleIdentity,
     RoleSchema,
     RuntimeProperties,
     ScheduleProperties,
     SeemplicityIntegration,
@@ -225,14 +227,19 @@
     SlackWebHookOutputItem,
     SnowflakeConnectorArgs,
     Sort,
     SortOrder,
     TeamsIntegration,
     TeamsOutputItem,
     TestConnectionResult,
+    UpdateClassRequestSchemaClassifierSchema,
+    UpdateClassRequestSchemaClassifierSchema_Dictionary,
+    UpdateClassRequestSchemaClassifierSchema_Regex,
+    UpdateDictionaryClassifierRequestSchema,
+    UpdateRegexClassifierRequestSchema,
     UserSchema,
     UserStatus,
     ValidationError,
     ViolatedDataAsset,
     ViolatedIamGroupAlertContent,
     ViolatedIamRoleAlertContent,
     ViolatedIdentityAlertContent,
@@ -258,14 +265,15 @@
     export,
     integrations,
     policies,
     roles,
     sensitivity,
     users,
 )
+from .environment import SentraEnvironment
 
 __all__ = [
     "AccessDataStore",
     "AccessMethodAccessibleEntitiesFlowchart",
     "AccessPermissions",
     "AccessibleEntitiesFlowchartIdentityNode",
     "AccessibleEntitiesFlowchartStoreNode",
@@ -294,19 +302,22 @@
     "AuthTokenSchema",
     "AwsConnectorArgs",
     "AwsInstallationMode",
     "AzureBoardsIntegration",
     "AzureBoardsItem",
     "AzureConnectorArgs",
     "ChoiceFilterData",
+    "ClassAndClassifierConfigSchema",
+    "ClassAndClassifierConfigSchemaClassifierConfig",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Dictionary",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Proprietary",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Regex",
     "ClassCategories",
-    "ClassConfig",
     "ClassSource",
     "ClassificationResultExample",
-    "ClassifierType",
     "ComputeConnectivityType",
     "ComputeConnectorPropertiesAws",
     "ComputeConnectorPropertiesAzure",
     "ComputeConnectorPropertiesGcp",
     "ConnectorDisplay",
     "ConnectorDisplayArgs",
     "ConnectorDisplayComputeProperties",
@@ -324,27 +335,30 @@
     "ConnectorSchemaComputeProperties",
     "ConnectorSchemaComputeProperties_Aws",
     "ConnectorSchemaComputeProperties_Azure",
     "ConnectorSchemaComputeProperties_Gcp",
     "ContextLabelSchema",
     "CreateApiV2ConnectorsPostRequest",
     "CreateApiV2IntegrationsPostRequest",
+    "CreateClassRequestSchemaClassifierSchema",
+    "CreateClassRequestSchemaClassifierSchema_Dictionary",
+    "CreateClassRequestSchemaClassifierSchema_Regex",
+    "CreateDictionaryClassifierRequestSchema",
+    "CreateRegexClassifierRequestSchema",
     "CurrentUserData",
     "DashboardData",
     "DataAssetAtRisk",
     "DataAssetClassUserOperation",
     "DataAssetExtended",
     "DataAssetObject",
     "DataAssetProps",
     "DataAssetRow",
     "DataAssetSchema",
-    "DataClassConfigSchema",
     "DataClassConfigWithUserSchema",
     "DataClassItem",
-    "DataClassSchema",
     "DataDogIntegration",
     "DataDogItem",
     "DataDogRegion",
     "DataHubFabric",
     "DataHubIntegration",
     "DataHubItem",
     "DataStoreAccessMetadata",
@@ -365,41 +379,35 @@
     "DetailedAlertSchemaWithCommentContent_SimilarAssets",
     "DetailedAlertSchemaWithCommentContent_ViolatedIamGroup",
     "DetailedAlertSchemaWithCommentContent_ViolatedIamRole",
     "DetailedAlertSchemaWithCommentContent_ViolatedIdentity",
     "DetailedAlertSchemaWithCommentContent_ViolatedStore",
     "DetailedIamGroupSchema",
     "DetailedIamRoleSchema",
+    "DictionaryClassifierResponse",
     "EmailInputItem",
     "EmailIntegration",
     "EmailIntegrationInput",
     "EmailOutputItem",
     "EventLogAction",
     "EventLogEntityType",
     "EventLogRow",
-    "ExternalClassifierConfig",
-    "FilterItem",
-    "FilterItemValue",
-    "FilterSpecs",
-    "FilterSpecsAndItem",
-    "FilterSpecsNotItem",
-    "FilterSpecsOrItem",
-    "FormatType",
     "GcpConnectorArgs",
     "GetAllApiV2AlertsGetResponse",
     "GetAllApiV2AuditLogGetResponse",
     "GetAllApiV2ClassesGetResponse",
     "GetAllApiV2ConnectorsGetResponse",
     "GetAllApiV2DataAccessIdentitiesGetResponse",
     "GetAllApiV2DataAssetsGetResponse",
     "GetAllApiV2PoliciesGetResponse",
     "GetAllApiV2RolesGetResponse",
     "GetAllApiV2UsersGetResponse",
     "GetAllExternalApiV2DataStoresGetResponse",
     "GetFilterApiV2AlertsFilterNameGetResponse",
+    "GetFilterApiV2AuditLogFilterNameGetResponse",
     "GetFilterApiV2ClassesFilterNameGetResponse",
     "GetFilterApiV2DataAccessFilterNameGetResponse",
     "GetFilterApiV2DataAssetsFilterNameGetResponse",
     "GetFilterApiV2DataStoresFilterNameGetResponse",
     "GetFilterApiV2PoliciesFilterNameGetResponse",
     "GroupItem",
     "GroupedDataTableResult",
@@ -458,27 +466,30 @@
     "PolicyRuleType",
     "PolicySchema",
     "PolicySeverity",
     "PolicyStatus",
     "PolicyTriggeringType",
     "PolicyType",
     "PolicyUpdateResponse",
+    "ProprietaryClassifierResponse",
     "ProviderMinimalMetadata",
     "ProviderSchema",
     "ProviderTypes",
     "RangeFilterData",
+    "RegexClassifierResponse",
     "ResolvedAlertSource",
     "RiskType",
     "RoleIdentity",
     "RoleSchema",
     "RuntimeProperties",
     "ScheduleProperties",
     "SeemplicityIntegration",
     "SeemplicityItem",
     "SensitivityLevels",
+    "SentraEnvironment",
     "SessionType",
     "SimilarAssetSchema",
     "SimilarAssetsAlertContent",
     "SimilarAssetsPair",
     "SimilarAssetsPairSchema",
     "SimilarAssetsProps",
     "SimilarStore",
@@ -490,14 +501,19 @@
     "SnowflakeConnectorArgs",
     "Sort",
     "SortOrder",
     "TeamsIntegration",
     "TeamsOutputItem",
     "TestConnectionResult",
     "UnprocessableEntityError",
+    "UpdateClassRequestSchemaClassifierSchema",
+    "UpdateClassRequestSchemaClassifierSchema_Dictionary",
+    "UpdateClassRequestSchemaClassifierSchema_Regex",
+    "UpdateDictionaryClassifierRequestSchema",
+    "UpdateRegexClassifierRequestSchema",
     "UserSchema",
     "UserStatus",
     "ValidationError",
     "ViolatedDataAsset",
     "ViolatedIamGroupAlertContent",
     "ViolatedIamRoleAlertContent",
     "ViolatedIdentityAlertContent",
```

### Comparing `fern_sentra-0.0.4/src/sentra/client.py` & `fern_sentra-0.0.5/src/sentra/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 import httpx
 
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .environment import SentraEnvironment
 from .resources.alerts.client import AlertsClient, AsyncAlertsClient
 from .resources.api_keys.client import ApiKeysClient, AsyncApiKeysClient
 from .resources.audit_log.client import AsyncAuditLogClient, AuditLogClient
 from .resources.connectors.client import AsyncConnectorsClient, ConnectorsClient
 from .resources.context_labels.client import AsyncContextLabelsClient, ContextLabelsClient
 from .resources.dashboard.client import AsyncDashboardClient, DashboardClient
 from .resources.data_access.client import AsyncDataAccessClient, DataAccessClient
@@ -20,17 +21,23 @@
 from .resources.policies.client import AsyncPoliciesClient, PoliciesClient
 from .resources.roles.client import AsyncRolesClient, RolesClient
 from .resources.sensitivity.client import AsyncSensitivityClient, SensitivityClient
 from .resources.users.client import AsyncUsersClient, UsersClient
 
 
 class Sentra:
-    def __init__(self, *, environment: str, timeout: typing.Optional[float] = 60):
+    def __init__(
+        self,
+        *,
+        environment: SentraEnvironment = SentraEnvironment.PRODUCTION,
+        api_key: str,
+        timeout: typing.Optional[float] = 60
+    ):
         self._environment = environment
-        self._client_wrapper = SyncClientWrapper(httpx_client=httpx.Client(timeout=timeout))
+        self._client_wrapper = SyncClientWrapper(api_key=api_key, httpx_client=httpx.Client(timeout=timeout))
         self.connectors = ConnectorsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.alerts = AlertsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.policies = PoliciesClient(environment=environment, client_wrapper=self._client_wrapper)
         self.data_stores = DataStoresClient(environment=environment, client_wrapper=self._client_wrapper)
         self.data_assets = DataAssetsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.dashboard = DashboardClient(environment=environment, client_wrapper=self._client_wrapper)
         self.sensitivity = SensitivityClient(environment=environment, client_wrapper=self._client_wrapper)
@@ -42,17 +49,23 @@
         self.audit_log = AuditLogClient(environment=environment, client_wrapper=self._client_wrapper)
         self.context_labels = ContextLabelsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.roles = RolesClient(environment=environment, client_wrapper=self._client_wrapper)
         self.api_keys = ApiKeysClient(environment=environment, client_wrapper=self._client_wrapper)
 
 
 class AsyncSentra:
-    def __init__(self, *, environment: str, timeout: typing.Optional[float] = 60):
+    def __init__(
+        self,
+        *,
+        environment: SentraEnvironment = SentraEnvironment.PRODUCTION,
+        api_key: str,
+        timeout: typing.Optional[float] = 60
+    ):
         self._environment = environment
-        self._client_wrapper = AsyncClientWrapper(httpx_client=httpx.AsyncClient(timeout=timeout))
+        self._client_wrapper = AsyncClientWrapper(api_key=api_key, httpx_client=httpx.AsyncClient(timeout=timeout))
         self.connectors = AsyncConnectorsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.alerts = AsyncAlertsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.policies = AsyncPoliciesClient(environment=environment, client_wrapper=self._client_wrapper)
         self.data_stores = AsyncDataStoresClient(environment=environment, client_wrapper=self._client_wrapper)
         self.data_assets = AsyncDataAssetsClient(environment=environment, client_wrapper=self._client_wrapper)
         self.dashboard = AsyncDashboardClient(environment=environment, client_wrapper=self._client_wrapper)
         self.sensitivity = AsyncSensitivityClient(environment=environment, client_wrapper=self._client_wrapper)
```

### Comparing `fern_sentra-0.0.4/src/sentra/core/__init__.py` & `fern_sentra-0.0.5/src/sentra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/core/client_wrapper.py` & `fern_sentra-0.0.5/src/sentra/core/client_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import typing
 
 import httpx
 
 
 class BaseClientWrapper:
-    def __init__(self) -> None:
-        pass
+    def __init__(self, *, api_key: str):
+        self.api_key = api_key
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {}
+        headers["X-Sentra-API-Key"] = self.api_key
         return headers
 
 
 class SyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, httpx_client: httpx.Client):
-        super().__init__()
+    def __init__(self, *, api_key: str, httpx_client: httpx.Client):
+        super().__init__(api_key=api_key)
         self.httpx_client = httpx_client
 
 
 class AsyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, httpx_client: httpx.AsyncClient):
-        super().__init__()
+    def __init__(self, *, api_key: str, httpx_client: httpx.AsyncClient):
+        super().__init__(api_key=api_key)
         self.httpx_client = httpx_client
```

### Comparing `fern_sentra-0.0.4/src/sentra/core/datetime_utils.py` & `fern_sentra-0.0.5/src/sentra/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/core/jsonable_encoder.py` & `fern_sentra-0.0.5/src/sentra/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/resources/__init__.py` & `fern_sentra-0.0.5/src/sentra/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/resources/alerts/client.py` & `fern_sentra-0.0.5/src/sentra/resources/alerts/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.alert_response_schema import AlertResponseSchema
 from ...types.alert_stats_by_date import AlertStatsByDate
 from ...types.alert_status import AlertStatus
 from ...types.alert_status_reason import AlertStatusReason
 from ...types.detailed_alert_schema_with_comment import DetailedAlertSchemaWithComment
@@ -27,15 +28,17 @@
 from ...types.resolved_alert_source import ResolvedAlertSource
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AlertsClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_filter(
         self, name: str, *, values: typing.Optional[str] = None, filters: typing.Optional[str] = None
     ) -> GetFilterApiV2AlertsFilterNameGetResponse:
         """
@@ -46,15 +49,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2AlertsFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -72,15 +75,15 @@
         Gets all data assets of a corresponding alert which are related to the violation.
 
         Parameters:
             - alert_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/data-assets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/data-assets"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedDataAssetsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -105,15 +108,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/violated_objects"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/violated_objects"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -133,15 +136,15 @@
         This endpoint is only relevant to alerts which are triggered on assets of type `OBJECT_GROUP`.
 
         Parameters:
             - alert_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/violated_objects_csv"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/violated_objects_csv"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -179,15 +182,15 @@
         _request: typing.Dict[str, typing.Any] = {"status": status, "reason": reason}
         if resolved_alert_source is not OMIT:
             _request["resolved_alert_source"] = resolved_alert_source
         if transitioned_at is not OMIT:
             _request["transitioned_at"] = transitioned_at
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/transition/{alert_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/transition/{alert_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AlertResponseSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -222,15 +225,15 @@
 
             - interval: typing.Optional[float].
 
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts/trends"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts/trends"),
             params=remove_none_from_dict(
                 {
                     "from_date": from_date,
                     "severity": severity,
                     "to_date": to_date,
                     "interval": interval,
                     "connector_id": connector_id,
@@ -267,15 +270,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if comment is not OMIT:
             _request["comment"] = comment
         if comment_id is not OMIT:
             _request["comment_id"] = comment_id
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/comment/{alert_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/comment/{alert_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -295,15 +298,15 @@
         Get a summary of the number of open alerts per severity.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts/aggregation/open"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts/aggregation/open"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[OpenAlertsAggregation], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -321,15 +324,15 @@
         Get information about a specific alert by ID.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedAlertSchemaWithComment, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -368,15 +371,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -397,15 +400,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAlertsClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_filter(
         self, name: str, *, values: typing.Optional[str] = None, filters: typing.Optional[str] = None
     ) -> GetFilterApiV2AlertsFilterNameGetResponse:
         """
@@ -416,15 +421,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2AlertsFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -442,15 +447,15 @@
         Gets all data assets of a corresponding alert which are related to the violation.
 
         Parameters:
             - alert_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/data-assets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/data-assets"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedDataAssetsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -475,15 +480,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/violated_objects"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/violated_objects"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -503,15 +508,15 @@
         This endpoint is only relevant to alerts which are triggered on assets of type `OBJECT_GROUP`.
 
         Parameters:
             - alert_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{alert_id}/violated_objects_csv"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{alert_id}/violated_objects_csv"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListViolatedObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -549,15 +554,15 @@
         _request: typing.Dict[str, typing.Any] = {"status": status, "reason": reason}
         if resolved_alert_source is not OMIT:
             _request["resolved_alert_source"] = resolved_alert_source
         if transitioned_at is not OMIT:
             _request["transitioned_at"] = transitioned_at
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/transition/{alert_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/transition/{alert_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AlertResponseSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -592,15 +597,15 @@
 
             - interval: typing.Optional[float].
 
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts/trends"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts/trends"),
             params=remove_none_from_dict(
                 {
                     "from_date": from_date,
                     "severity": severity,
                     "to_date": to_date,
                     "interval": interval,
                     "connector_id": connector_id,
@@ -637,15 +642,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if comment is not OMIT:
             _request["comment"] = comment
         if comment_id is not OMIT:
             _request["comment_id"] = comment_id
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/comment/{alert_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/comment/{alert_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -665,15 +670,15 @@
         Get a summary of the number of open alerts per severity.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts/aggregation/open"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts/aggregation/open"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[OpenAlertsAggregation], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -691,15 +696,15 @@
         Get information about a specific alert by ID.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/alerts/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/alerts/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedAlertSchemaWithComment, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -738,15 +743,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/alerts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/alerts"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/api_keys/client.py` & `fern_sentra-0.0.5/src/sentra/resources/api_keys/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.auth_token_schema import AuthTokenSchema
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_all_auth_tokens_response import ListAllAuthTokensResponse
 from ...types.new_auth_token_response import NewAuthTokenResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ApiKeysClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -53,15 +56,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/tokens"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/tokens"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -96,15 +99,15 @@
 
             - role_id: int.
 
             - expiration_days: int.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/tokens"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/tokens"),
             json=jsonable_encoder({"name": name, "role_id": role_id, "expiration_days": expiration_days}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(NewAuthTokenResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -133,15 +136,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         if expiration_days is not OMIT:
             _request["expiration_days"] = expiration_days
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/tokens/{auth_token_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/tokens/{auth_token_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AuthTokenSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -159,15 +162,15 @@
         Delete an API key by ID.
 
         Parameters:
             - auth_token_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/tokens/{auth_token_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/tokens/{auth_token_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -177,15 +180,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncApiKeysClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -212,15 +217,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/tokens"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/tokens"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -255,15 +260,15 @@
 
             - role_id: int.
 
             - expiration_days: int.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/tokens"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/tokens"),
             json=jsonable_encoder({"name": name, "role_id": role_id, "expiration_days": expiration_days}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(NewAuthTokenResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -292,15 +297,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         if expiration_days is not OMIT:
             _request["expiration_days"] = expiration_days
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/tokens/{auth_token_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/tokens/{auth_token_id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AuthTokenSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -318,15 +323,15 @@
         Delete an API key by ID.
 
         Parameters:
             - auth_token_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/tokens/{auth_token_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/tokens/{auth_token_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/audit_log/client.py` & `fern_sentra-0.0.5/src/sentra/resources/audit_log/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,70 +6,74 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.event_log_action import EventLogAction
 from ...types.event_log_entity_type import EventLogEntityType
 from ...types.get_all_api_v_2_audit_log_get_response import GetAllApiV2AuditLogGetResponse
+from ...types.get_filter_api_v_2_audit_log_filter_name_get_response import GetFilterApiV2AuditLogFilterNameGetResponse
 from ...types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AuditLogClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
-        group_by: typing.Optional[str] = None,
-        sort_by: typing.Optional[str] = None,
-        filters: typing.Optional[str] = None,
         offset: typing.Optional[int] = None,
         limit: typing.Optional[int] = None,
         count_only: typing.Optional[bool] = None,
+        group_by: typing.Optional[str] = None,
+        sort_by: typing.Optional[str] = None,
+        filters: typing.Optional[str] = None,
         with_entities: typing.Optional[str] = None,
     ) -> GetAllApiV2AuditLogGetResponse:
         """
         List all audit log events.
 
         Parameters:
-            - group_by: typing.Optional[str].
-
-            - sort_by: typing.Optional[str].
-
-            - filters: typing.Optional[str].
-
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
 
             - count_only: typing.Optional[bool].
 
+            - group_by: typing.Optional[str].
+
+            - sort_by: typing.Optional[str].
+
+            - filters: typing.Optional[str].
+
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/audit-log"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/audit-log"),
             params=remove_none_from_dict(
                 {
-                    "group_by": group_by,
-                    "sort_by": sort_by,
-                    "filters": filters,
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
+                    "group_by": group_by,
+                    "sort_by": sort_by,
+                    "filters": filters,
                     "with_entities": with_entities,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -109,15 +113,15 @@
             "action": action,
             "properties": properties,
         }
         if entity_id is not OMIT:
             _request["entity_id"] = entity_id
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/audit-log"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/audit-log"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(bool, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -126,60 +130,101 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def get_filter(
+        self,
+        name: str,
+        *,
+        values: typing.Optional[str] = None,
+        filters: typing.Optional[str] = None,
+        with_entities: typing.Optional[str] = None,
+    ) -> GetFilterApiV2AuditLogFilterNameGetResponse:
+        """
+        Get all available filtering options for filtering on audit log events.
+
+        Parameters:
+            - name: str.
+
+            - values: typing.Optional[str].
+
+            - filters: typing.Optional[str].
+
+            - with_entities: typing.Optional[str].
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/audit-log/filter/{name}"),
+            params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(GetFilterApiV2AuditLogFilterNameGetResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncAuditLogClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
-        group_by: typing.Optional[str] = None,
-        sort_by: typing.Optional[str] = None,
-        filters: typing.Optional[str] = None,
         offset: typing.Optional[int] = None,
         limit: typing.Optional[int] = None,
         count_only: typing.Optional[bool] = None,
+        group_by: typing.Optional[str] = None,
+        sort_by: typing.Optional[str] = None,
+        filters: typing.Optional[str] = None,
         with_entities: typing.Optional[str] = None,
     ) -> GetAllApiV2AuditLogGetResponse:
         """
         List all audit log events.
 
         Parameters:
-            - group_by: typing.Optional[str].
-
-            - sort_by: typing.Optional[str].
-
-            - filters: typing.Optional[str].
-
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
 
             - count_only: typing.Optional[bool].
 
+            - group_by: typing.Optional[str].
+
+            - sort_by: typing.Optional[str].
+
+            - filters: typing.Optional[str].
+
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/audit-log"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/audit-log"),
             params=remove_none_from_dict(
                 {
-                    "group_by": group_by,
-                    "sort_by": sort_by,
-                    "filters": filters,
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
+                    "group_by": group_by,
+                    "sort_by": sort_by,
+                    "filters": filters,
                     "with_entities": with_entities,
                 }
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -219,23 +264,62 @@
             "action": action,
             "properties": properties,
         }
         if entity_id is not OMIT:
             _request["entity_id"] = entity_id
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/audit-log"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/audit-log"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(bool, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_filter(
+        self,
+        name: str,
+        *,
+        values: typing.Optional[str] = None,
+        filters: typing.Optional[str] = None,
+        with_entities: typing.Optional[str] = None,
+    ) -> GetFilterApiV2AuditLogFilterNameGetResponse:
+        """
+        Get all available filtering options for filtering on audit log events.
+
+        Parameters:
+            - name: str.
+
+            - values: typing.Optional[str].
+
+            - filters: typing.Optional[str].
+
+            - with_entities: typing.Optional[str].
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/audit-log/filter/{name}"),
+            params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(GetFilterApiV2AuditLogFilterNameGetResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/connectors/client.py` & `fern_sentra-0.0.5/src/sentra/resources/connectors/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.connector_input import ConnectorInput
 from ...types.connector_schema import ConnectorSchema
 from ...types.create_api_v_2_connectors_post_request import CreateApiV2ConnectorsPostRequest
 from ...types.get_all_api_v_2_connectors_get_response import GetAllApiV2ConnectorsGetResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.test_connection_result import TestConnectionResult
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ConnectorsClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -55,15 +58,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -91,15 +94,15 @@
         Create a new account.
 
         Parameters:
             - request: CreateApiV2ConnectorsPostRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ConnectorSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -114,15 +117,15 @@
 
     def get_scanner_accounts(self) -> typing.Any:
         """
         List all scanner accounts.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors/scanners"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors/scanners"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -141,15 +144,15 @@
         Parameters:
             - id: int.
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -169,15 +172,15 @@
         Parameters:
             - id: int.
 
             - request: ConnectorInput.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -195,15 +198,15 @@
         Delete an account.
 
         Parameters:
             - id: int.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -225,15 +228,15 @@
             - enabled: typing.Optional[bool].
         """
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/status/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/status/{id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -251,15 +254,15 @@
         Test the connection of an account to see if it was configured correctly.
 
         Parameters:
             - request: ConnectorInput.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors/test_connection"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors/test_connection"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TestConnectionResult, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -270,15 +273,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncConnectorsClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -305,15 +310,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -341,15 +346,15 @@
         Create a new account.
 
         Parameters:
             - request: CreateApiV2ConnectorsPostRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ConnectorSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -364,15 +369,15 @@
 
     async def get_scanner_accounts(self) -> typing.Any:
         """
         List all scanner accounts.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors/scanners"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors/scanners"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -391,15 +396,15 @@
         Parameters:
             - id: int.
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -419,15 +424,15 @@
         Parameters:
             - id: int.
 
             - request: ConnectorInput.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -445,15 +450,15 @@
         Delete an account.
 
         Parameters:
             - id: int.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -475,15 +480,15 @@
             - enabled: typing.Optional[bool].
         """
         _request: typing.Dict[str, typing.Any] = {}
         if enabled is not OMIT:
             _request["enabled"] = enabled
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/connectors/status/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/connectors/status/{id}"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConnectorSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -501,15 +506,15 @@
         Test the connection of an account to see if it was configured correctly.
 
         Parameters:
             - request: ConnectorInput.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/connectors/test_connection"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/connectors/test_connection"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TestConnectionResult, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/context_labels/client.py` & `fern_sentra-0.0.5/src/sentra/resources/context_labels/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_all_context_label_response import ListAllContextLabelResponse
 
 
 class ContextLabelsClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -47,15 +50,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/context_labels"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/context_labels"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -76,15 +79,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncContextLabelsClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -111,15 +116,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/context_labels"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/context_labels"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/dashboard/client.py` & `fern_sentra-0.0.5/src/sentra/resources/dashboard/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.dashboard_data import DashboardData
 from ...types.http_validation_error import HttpValidationError
 
 
 class DashboardClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_dashboard_summary_data(self, *, connector_id: typing.Optional[int] = None) -> DashboardData:
         """
         Get a high level overview of an account.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/dashboard"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/dashboard"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DashboardData, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -44,28 +47,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDashboardClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_dashboard_summary_data(self, *, connector_id: typing.Optional[int] = None) -> DashboardData:
         """
         Get a high level overview of an account.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/dashboard"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/dashboard"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DashboardData, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/data_access/client.py` & `fern_sentra-0.0.5/src/sentra/resources/data_access/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.access_data_store import AccessDataStore
 from ...types.access_method_accessible_entities_flowchart import AccessMethodAccessibleEntitiesFlowchart
 from ...types.detailed_iam_group_schema import DetailedIamGroupSchema
 from ...types.detailed_iam_role_schema import DetailedIamRoleSchema
 from ...types.get_all_api_v_2_data_access_identities_get_response import GetAllApiV2DataAccessIdentitiesGetResponse
@@ -26,28 +27,30 @@
 from ...types.iam_role_schema import IamRoleSchema
 from ...types.identity_accessible_entities_flowchart import IdentityAccessibleEntitiesFlowchart
 from ...types.identity_schema import IdentitySchema
 from ...types.role_identity import RoleIdentity
 
 
 class DataAccessClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list_iam_groups(self, *, ids: typing.Union[typing.Optional[str], typing.List[str]]) -> typing.List[typing.Any]:
         """
         List identity groups of a set of given identities.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/groups/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/groups/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -65,15 +68,15 @@
         Get an identity group by ID.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedIamGroupSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -90,15 +93,15 @@
         Get all data classes related to a specific identity group.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}/data-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/data-classes"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IamGroupDataClasses, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -128,15 +131,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/data-stores"),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -155,15 +158,15 @@
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/groups/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccessMethodAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -182,15 +185,15 @@
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/roles/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccessMethodAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -221,15 +224,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/data-stores"),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -247,15 +250,15 @@
         List identity roles of a set of given identities.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/roles/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/roles/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -273,15 +276,15 @@
         Get an identity role by ID.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedIamRoleSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -298,15 +301,15 @@
         Get all data classes related to a specific identity role.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/data-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/data-classes"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IamRoleDataClasses, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -336,15 +339,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/identities"),
             params=remove_none_from_dict({"identity_name": identity_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RoleIdentity], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -384,15 +387,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/identities"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -426,15 +429,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataAccessFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -452,15 +455,15 @@
         List access identities by a list of IDs.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/identities/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/identities/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -478,15 +481,15 @@
         Get all information about a specific access identity by ID.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IdentitySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -509,15 +512,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}/groups"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/groups"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IamGroupSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -541,15 +544,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}/roles"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/roles"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IamRoleSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -580,15 +583,17 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{identity_id}/data-stores"),
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"api/v2/data-access/identities/{identity_id}/data-stores"
+            ),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -608,15 +613,15 @@
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/identities/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IdentityAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -627,30 +632,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDataAccessClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list_iam_groups(
         self, *, ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> typing.List[typing.Any]:
         """
         List identity groups of a set of given identities.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/groups/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/groups/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -668,15 +675,15 @@
         Get an identity group by ID.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedIamGroupSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -693,15 +700,15 @@
         Get all data classes related to a specific identity group.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}/data-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/data-classes"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IamGroupDataClasses, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -731,15 +738,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/groups/{id}/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/data-stores"),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -758,15 +765,15 @@
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/groups/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/groups/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccessMethodAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -785,15 +792,15 @@
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/roles/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AccessMethodAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -824,15 +831,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/data-stores"),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -852,15 +859,15 @@
         List identity roles of a set of given identities.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/roles/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/roles/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -878,15 +885,15 @@
         Get an identity role by ID.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DetailedIamRoleSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -903,15 +910,15 @@
         Get all data classes related to a specific identity role.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/data-classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/data-classes"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IamRoleDataClasses, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -941,15 +948,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/roles/{id}/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/roles/{id}/identities"),
             params=remove_none_from_dict({"identity_name": identity_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[RoleIdentity], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -989,15 +996,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/identities"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -1031,15 +1038,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataAccessFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -1059,15 +1066,15 @@
         List access identities by a list of IDs.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-access/identities/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-access/identities/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -1085,15 +1092,15 @@
         Get all information about a specific access identity by ID.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IdentitySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -1116,15 +1123,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}/groups"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/groups"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IamGroupSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -1148,15 +1155,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{id}/roles"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/roles"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IamRoleSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -1187,15 +1194,17 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-access/identities/{identity_id}/data-stores"),
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"api/v2/data-access/identities/{identity_id}/data-stores"
+            ),
             params=remove_none_from_dict({"store_name": store_name, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[AccessDataStore], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -1215,15 +1224,15 @@
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-access/identities/{id}/accessible_entities_flowchart"
+                f"{self._environment.value}/", f"api/v2/data-access/identities/{id}/accessible_entities_flowchart"
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IdentityAccessibleEntitiesFlowchart, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/data_assets/client.py` & `fern_sentra-0.0.5/src/sentra/resources/data_assets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.asset_class_user_request import AssetClassUserRequest
 from ...types.data_asset_at_risk import DataAssetAtRisk
 from ...types.data_asset_extended import DataAssetExtended
 from ...types.get_all_api_v_2_data_assets_get_response import GetAllApiV2DataAssetsGetResponse
 from ...types.get_filter_api_v_2_data_assets_filter_name_get_response import (
@@ -24,15 +25,17 @@
 from ...types.similar_assets_pair_schema import SimilarAssetsPairSchema
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class DataAssetsClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_filter(
         self, name: str, *, values: typing.Optional[str] = None, filters: typing.Optional[str] = None
     ) -> GetFilterApiV2DataAssetsFilterNameGetResponse:
         """
@@ -43,15 +46,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataAssetsFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -73,15 +76,15 @@
         Parameters:
             - limit: typing.Optional[int].
 
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/at-risk"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/at-risk"),
             params=remove_none_from_dict({"limit": limit, "connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataAssetAtRisk], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -115,15 +118,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/similar"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/similar"),
             params=remove_none_from_dict(
                 {"asset_id": asset_id, "filters": filters, "sort_by": sort_by, "offset": offset, "limit": limit}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -143,15 +146,15 @@
         Get information about a similarity between two assets using its pair ID.
 
         Parameters:
             - pair_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/similar/{pair_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/similar/{pair_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SimilarAssetsPairSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -169,15 +172,15 @@
         the data class was found.
 
         Parameters:
             - request: typing.List[AssetClassUserRequest].
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/classes"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[int], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -211,15 +214,15 @@
 
             - filters: typing.Optional[str].
 
             - group_by: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets"),
             params=remove_none_from_dict(
                 {"offset": offset, "limit": limit, "sort_by": sort_by, "filters": filters, "group_by": group_by}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -241,15 +244,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataAssetExtended, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -260,15 +263,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDataAssetsClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_filter(
         self, name: str, *, values: typing.Optional[str] = None, filters: typing.Optional[str] = None
     ) -> GetFilterApiV2DataAssetsFilterNameGetResponse:
         """
@@ -279,15 +284,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataAssetsFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -309,15 +314,15 @@
         Parameters:
             - limit: typing.Optional[int].
 
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/at-risk"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/at-risk"),
             params=remove_none_from_dict({"limit": limit, "connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataAssetAtRisk], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -351,15 +356,15 @@
 
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/similar"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/similar"),
             params=remove_none_from_dict(
                 {"asset_id": asset_id, "filters": filters, "sort_by": sort_by, "offset": offset, "limit": limit}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -379,15 +384,15 @@
         Get information about a similarity between two assets using its pair ID.
 
         Parameters:
             - pair_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/similar/{pair_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/similar/{pair_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SimilarAssetsPairSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -405,15 +410,15 @@
         the data class was found.
 
         Parameters:
             - request: typing.List[AssetClassUserRequest].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets/classes"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[int], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -447,15 +452,15 @@
 
             - filters: typing.Optional[str].
 
             - group_by: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-assets"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-assets"),
             params=remove_none_from_dict(
                 {"offset": offset, "limit": limit, "sort_by": sort_by, "filters": filters, "group_by": group_by}
             ),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -477,15 +482,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-assets/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-assets/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataAssetExtended, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/data_classes/client.py` & `fern_sentra-0.0.5/src/sentra/resources/data_classes/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.class_and_classifier_config_schema import ClassAndClassifierConfigSchema
 from ...types.class_categories import ClassCategories
-from ...types.class_source import ClassSource
-from ...types.classifier_type import ClassifierType
-from ...types.data_class_config_schema import DataClassConfigSchema
-from ...types.data_class_schema import DataClassSchema
-from ...types.external_classifier_config import ExternalClassifierConfig
+from ...types.create_class_request_schema_classifier_schema import CreateClassRequestSchemaClassifierSchema
 from ...types.get_all_api_v_2_classes_get_response import GetAllApiV2ClassesGetResponse
 from ...types.get_filter_api_v_2_classes_filter_name_get_response import GetFilterApiV2ClassesFilterNameGetResponse
 from ...types.http_validation_error import HttpValidationError
+from ...types.update_class_request_schema_classifier_schema import UpdateClassRequestSchemaClassifierSchema
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class DataClassesClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -58,15 +59,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/classes"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -85,64 +86,57 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_class_config(
+    def create_class(
         self,
         *,
         name: str,
         description: typing.Optional[str] = OMIT,
         category: ClassCategories,
+        sensitivity_weight: int,
         enabled: typing.Optional[bool] = OMIT,
-        experimental: typing.Optional[bool] = OMIT,
-        source: typing.Optional[ClassSource] = OMIT,
-        type: ClassifierType,
-        config: ExternalClassifierConfig,
-    ) -> DataClassConfigSchema:
+        classifier_schema: CreateClassRequestSchemaClassifierSchema,
+    ) -> ClassAndClassifierConfigSchema:
         """
-        Create a data class.
-
         Parameters:
             - name: str.
 
-            - description: typing.Optional[str]. <span style="white-space: nowrap">`<= 1024 characters`</span>
+            - description: typing.Optional[str].
 
             - category: ClassCategories.
 
-            - enabled: typing.Optional[bool].
-
-            - experimental: typing.Optional[bool].
+            - sensitivity_weight: int.
 
-            - source: typing.Optional[ClassSource].
-
-            - type: ClassifierType.
+            - enabled: typing.Optional[bool].
 
-            - config: ExternalClassifierConfig.
+            - classifier_schema: CreateClassRequestSchemaClassifierSchema.
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "category": category, "type": type, "config": config}
+        _request: typing.Dict[str, typing.Any] = {
+            "name": name,
+            "category": category,
+            "sensitivity_weight": sensitivity_weight,
+            "classifier_schema": classifier_schema,
+        }
         if description is not OMIT:
             _request["description"] = description
         if enabled is not OMIT:
             _request["enabled"] = enabled
-        if experimental is not OMIT:
-            _request["experimental"] = experimental
-        if source is not OMIT:
-            _request["source"] = source
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/classes"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassConfigSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -160,15 +154,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2ClassesFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -177,77 +171,108 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str) -> DataClassConfigSchema:
+    def get(self, id: str) -> ClassAndClassifierConfigSchema:
         """
         Get all information about a specific data class by ID.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassConfigSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_class_config(self, id: str, *, enabled: bool) -> DataClassSchema:
+    def update_class(
+        self,
+        id: str,
+        *,
+        name: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        category: typing.Optional[ClassCategories] = OMIT,
+        sensitivity_weight: typing.Optional[int] = OMIT,
+        enabled: typing.Optional[bool] = OMIT,
+        classifier_schema: typing.Optional[UpdateClassRequestSchemaClassifierSchema] = OMIT,
+    ) -> ClassAndClassifierConfigSchema:
         """
         Update a data class.
 
         Parameters:
             - id: str.
 
-            - enabled: bool.
+            - name: typing.Optional[str].
+
+            - description: typing.Optional[str].
+
+            - category: typing.Optional[ClassCategories].
+
+            - sensitivity_weight: typing.Optional[int].
+
+            - enabled: typing.Optional[bool].
+
+            - classifier_schema: typing.Optional[UpdateClassRequestSchemaClassifierSchema].
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if description is not OMIT:
+            _request["description"] = description
+        if category is not OMIT:
+            _request["category"] = category
+        if sensitivity_weight is not OMIT:
+            _request["sensitivity_weight"] = sensitivity_weight
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if classifier_schema is not OMIT:
+            _request["classifier_schema"] = classifier_schema
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
-            json=jsonable_encoder({"enabled": enabled}),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
+            json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_data_class_config(self, id: str) -> str:
         """
-        Delete a data class.
-
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -255,17 +280,46 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def update_class_file(self, id: str, *, dictionary_file: typing.IO) -> ClassAndClassifierConfigSchema:
+        """
+        Parameters:
+            - id: str.
+
+            - dictionary_file: typing.IO.
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/dictionary_file/{id}"),
+            data=jsonable_encoder({}),
+            files={"dictionary_file": dictionary_file},
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncDataClassesClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -292,15 +346,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/classes"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -319,64 +373,57 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_class_config(
+    async def create_class(
         self,
         *,
         name: str,
         description: typing.Optional[str] = OMIT,
         category: ClassCategories,
+        sensitivity_weight: int,
         enabled: typing.Optional[bool] = OMIT,
-        experimental: typing.Optional[bool] = OMIT,
-        source: typing.Optional[ClassSource] = OMIT,
-        type: ClassifierType,
-        config: ExternalClassifierConfig,
-    ) -> DataClassConfigSchema:
+        classifier_schema: CreateClassRequestSchemaClassifierSchema,
+    ) -> ClassAndClassifierConfigSchema:
         """
-        Create a data class.
-
         Parameters:
             - name: str.
 
-            - description: typing.Optional[str]. <span style="white-space: nowrap">`<= 1024 characters`</span>
+            - description: typing.Optional[str].
 
             - category: ClassCategories.
 
-            - enabled: typing.Optional[bool].
-
-            - experimental: typing.Optional[bool].
+            - sensitivity_weight: int.
 
-            - source: typing.Optional[ClassSource].
-
-            - type: ClassifierType.
+            - enabled: typing.Optional[bool].
 
-            - config: ExternalClassifierConfig.
+            - classifier_schema: CreateClassRequestSchemaClassifierSchema.
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "category": category, "type": type, "config": config}
+        _request: typing.Dict[str, typing.Any] = {
+            "name": name,
+            "category": category,
+            "sensitivity_weight": sensitivity_weight,
+            "classifier_schema": classifier_schema,
+        }
         if description is not OMIT:
             _request["description"] = description
         if enabled is not OMIT:
             _request["enabled"] = enabled
-        if experimental is not OMIT:
-            _request["experimental"] = experimental
-        if source is not OMIT:
-            _request["source"] = source
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/classes"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/classes"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassConfigSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -394,15 +441,15 @@
 
             - values: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2ClassesFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -411,84 +458,142 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str) -> DataClassConfigSchema:
+    async def get(self, id: str) -> ClassAndClassifierConfigSchema:
         """
         Get all information about a specific data class by ID.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassConfigSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_class_config(self, id: str, *, enabled: bool) -> DataClassSchema:
+    async def update_class(
+        self,
+        id: str,
+        *,
+        name: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        category: typing.Optional[ClassCategories] = OMIT,
+        sensitivity_weight: typing.Optional[int] = OMIT,
+        enabled: typing.Optional[bool] = OMIT,
+        classifier_schema: typing.Optional[UpdateClassRequestSchemaClassifierSchema] = OMIT,
+    ) -> ClassAndClassifierConfigSchema:
         """
         Update a data class.
 
         Parameters:
             - id: str.
 
-            - enabled: bool.
+            - name: typing.Optional[str].
+
+            - description: typing.Optional[str].
+
+            - category: typing.Optional[ClassCategories].
+
+            - sensitivity_weight: typing.Optional[int].
+
+            - enabled: typing.Optional[bool].
+
+            - classifier_schema: typing.Optional[UpdateClassRequestSchemaClassifierSchema].
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if description is not OMIT:
+            _request["description"] = description
+        if category is not OMIT:
+            _request["category"] = category
+        if sensitivity_weight is not OMIT:
+            _request["sensitivity_weight"] = sensitivity_weight
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if classifier_schema is not OMIT:
+            _request["classifier_schema"] = classifier_schema
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
-            json=jsonable_encoder({"enabled": enabled}),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
+            json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DataClassSchema, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_data_class_config(self, id: str) -> str:
         """
-        Delete a data class.
-
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/classes/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def update_class_file(self, id: str, *, dictionary_file: typing.IO) -> ClassAndClassifierConfigSchema:
+        """
+        Parameters:
+            - id: str.
+
+            - dictionary_file: typing.IO.
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/classes/dictionary_file/{id}"),
+            data=jsonable_encoder({}),
+            files={"dictionary_file": dictionary_file},
+            headers=self._client_wrapper.get_headers(),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ClassAndClassifierConfigSchema, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/data_stores/client.py` & `fern_sentra-0.0.5/src/sentra/resources/data_stores/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.data_store_access_metadata import DataStoreAccessMetadata
 from ...types.data_store_extended import DataStoreExtended
 from ...types.data_store_identity import DataStoreIdentity
 from ...types.data_store_risk_aggregation import DataStoreRiskAggregation
 from ...types.get_all_external_api_v_2_data_stores_get_response import GetAllExternalApiV2DataStoresGetResponse
@@ -21,28 +22,30 @@
 )
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_similar_assets_pair_response import ListSimilarAssetsPairResponse
 from ...types.similar_store import SimilarStore
 
 
 class DataStoresClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def list_data_stores(self, *, ids: typing.Union[typing.Optional[str], typing.List[str]]) -> typing.List[typing.Any]:
         """
         List all data stores.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -62,15 +65,15 @@
         Get a summary of number of data stores, aggregated by risk.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores/risk-aggregation"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores/risk-aggregation"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataStoreRiskAggregation], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -88,15 +91,15 @@
         Get a list of all data stores similar to a specific data store.
 
         Parameters:
             - store_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/similar"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/similar"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SimilarStore], _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -115,15 +118,15 @@
         Parameters:
             - store_a: str.
 
             - store_b: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_a}/similar/{store_b}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_a}/similar/{store_b}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SimilarStore, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -160,15 +163,15 @@
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-stores/{base_store_id}/similar/{similar_store_id}/assets"
+                f"{self._environment.value}/", f"api/v2/data-stores/{base_store_id}/similar/{similar_store_id}/assets"
             ),
             params=remove_none_from_dict({"filters": filters, "sort_by": sort_by, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListSimilarAssetsPairResponse, _response.json())  # type: ignore
@@ -187,15 +190,15 @@
         Get a high level overview of the number of access permissions of a specific data store.
 
         Parameters:
             - store_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/access/metadata"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/access/metadata"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataStoreAccessMetadata, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -216,15 +219,15 @@
         Parameters:
             - store_id: str.
 
             - identity_name: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/access/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/access/identities"),
             params=remove_none_from_dict({"identity_name": identity_name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataStoreIdentity], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -261,15 +264,15 @@
 
             - sort_by: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -309,15 +312,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataStoresFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -337,15 +340,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataStoreExtended, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -356,30 +359,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDataStoresClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def list_data_stores(
         self, *, ids: typing.Union[typing.Optional[str], typing.List[str]]
     ) -> typing.List[typing.Any]:
         """
         List all data stores.
 
         Parameters:
             - ids: typing.Union[typing.Optional[str], typing.List[str]].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores/list"),
             params=remove_none_from_dict({"ids": ids}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[typing.Any], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -399,15 +404,15 @@
         Get a summary of number of data stores, aggregated by risk.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores/risk-aggregation"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores/risk-aggregation"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataStoreRiskAggregation], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -425,15 +430,15 @@
         Get a list of all data stores similar to a specific data store.
 
         Parameters:
             - store_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/similar"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/similar"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[SimilarStore], _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -452,15 +457,15 @@
         Parameters:
             - store_a: str.
 
             - store_b: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_a}/similar/{store_b}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_a}/similar/{store_b}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SimilarStore, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -497,15 +502,15 @@
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
-                f"{self._environment}/", f"api/v2/data-stores/{base_store_id}/similar/{similar_store_id}/assets"
+                f"{self._environment.value}/", f"api/v2/data-stores/{base_store_id}/similar/{similar_store_id}/assets"
             ),
             params=remove_none_from_dict({"filters": filters, "sort_by": sort_by, "offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListSimilarAssetsPairResponse, _response.json())  # type: ignore
@@ -524,15 +529,15 @@
         Get a high level overview of the number of access permissions of a specific data store.
 
         Parameters:
             - store_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/access/metadata"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/access/metadata"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataStoreAccessMetadata, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -553,15 +558,15 @@
         Parameters:
             - store_id: str.
 
             - identity_name: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{store_id}/access/identities"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{store_id}/access/identities"),
             params=remove_none_from_dict({"identity_name": identity_name}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DataStoreIdentity], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -598,15 +603,15 @@
 
             - sort_by: typing.Optional[str].
 
             - filters: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/data-stores"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/data-stores"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -646,15 +651,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2DataStoresFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -674,15 +679,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/data-stores/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/data-stores/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DataStoreExtended, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/export/client.py` & `fern_sentra-0.0.5/src/sentra/resources/export/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class ExportClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def export_wiz(self) -> typing.Any:
         """
         Export data file for ingestion with Wiz.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/wiz"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/wiz"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -42,15 +45,15 @@
 
     def export_axonius(self) -> typing.Any:
         """
         Export data file for ingestion with Axonius.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/axonius"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/axonius"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -67,15 +70,15 @@
         Export all objects of an asset.
 
         Parameters:
             - asset_id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/export/s3_group/{asset_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/export/s3_group/{asset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -89,15 +92,15 @@
 
     def export_security_lake(self) -> typing.Any:
         """
         Export data file to security lake format.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/security_lake"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/security_lake"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -107,25 +110,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncExportClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def export_wiz(self) -> typing.Any:
         """
         Export data file for ingestion with Wiz.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/wiz"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/wiz"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -139,15 +144,15 @@
 
     async def export_axonius(self) -> typing.Any:
         """
         Export data file for ingestion with Axonius.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/axonius"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/axonius"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -164,15 +169,15 @@
         Export all objects of an asset.
 
         Parameters:
             - asset_id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/export/s3_group/{asset_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/export/s3_group/{asset_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -186,15 +191,15 @@
 
     async def export_security_lake(self) -> typing.Any:
         """
         Export data file to security lake format.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/export/security_lake"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/export/security_lake"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/integrations/client.py` & `fern_sentra-0.0.5/src/sentra/resources/integrations/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,39 +5,42 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_api_v_2_integrations_post_request import CreateApiV2IntegrationsPostRequest
 from ...types.http_validation_error import HttpValidationError
 from ...types.integration_display import IntegrationDisplay
 from ...types.integration_input import IntegrationInput
 from ...types.integration_output_schema import IntegrationOutputSchema
 from ...types.integration_schema import IntegrationSchema
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class IntegrationsClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(self) -> typing.List[IntegrationDisplay]:
         """
         List all external facing integrations.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/integrations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/integrations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IntegrationDisplay], _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -54,15 +57,15 @@
         Create a new external facing integration.
 
         Parameters:
             - request: CreateApiV2IntegrationsPostRequest.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/integrations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/integrations"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IntegrationSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -82,15 +85,15 @@
         Parameters:
             - id: int.
 
             - request: IntegrationInput.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -108,15 +111,15 @@
         Delete an external facing integration.
 
         Parameters:
             - id: int.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -135,15 +138,15 @@
         Parameters:
             - id: int.
 
             - enabled: bool.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}/toggle_status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}/toggle_status"),
             json=jsonable_encoder({"enabled": enabled}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationOutputSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -154,25 +157,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncIntegrationsClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(self) -> typing.List[IntegrationDisplay]:
         """
         List all external facing integrations.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/integrations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/integrations"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IntegrationDisplay], _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -189,15 +194,15 @@
         Create a new external facing integration.
 
         Parameters:
             - request: CreateApiV2IntegrationsPostRequest.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/integrations"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/integrations"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[IntegrationSchema], _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -217,15 +222,15 @@
         Parameters:
             - id: int.
 
             - request: IntegrationInput.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}"),
             json=jsonable_encoder(request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -243,15 +248,15 @@
         Delete an external facing integration.
 
         Parameters:
             - id: int.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -270,15 +275,15 @@
         Parameters:
             - id: int.
 
             - enabled: bool.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/integrations/{id}/toggle_status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/integrations/{id}/toggle_status"),
             json=jsonable_encoder({"enabled": enabled}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(IntegrationOutputSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/policies/client.py` & `fern_sentra-0.0.5/src/sentra/resources/policies/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.get_all_api_v_2_policies_get_response import GetAllApiV2PoliciesGetResponse
 from ...types.get_filter_api_v_2_policies_filter_name_get_response import GetFilterApiV2PoliciesFilterNameGetResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.policy_rule import PolicyRule
 from ...types.policy_schema import PolicySchema
@@ -25,15 +26,17 @@
 from ...types.risk_type import RiskType
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class PoliciesClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_filter(
         self,
         name: str,
         *,
@@ -51,15 +54,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2PoliciesFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -79,15 +82,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -105,15 +108,15 @@
         Delete a policy and all of its associated alerts.
 
         Parameters:
             - id: str.
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -132,15 +135,15 @@
         Parameters:
             - policy_id: str.
 
             - enabled: bool.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{policy_id}/status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{policy_id}/status"),
             params=remove_none_from_dict({"enabled": enabled}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -233,15 +236,15 @@
             _request["predefined"] = predefined
         if auto_approval is not OMIT:
             _request["auto_approval"] = auto_approval
         if triggering_type is not OMIT:
             _request["triggering_type"] = triggering_type
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{policy_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{policy_id}"),
             params=remove_none_from_dict({"force": force}),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicyUpdateResponse, _response.json())  # type: ignore
@@ -257,15 +260,15 @@
 
     def get_policy_enums(self) -> typing.Any:
         """
         Get available enums for filtering on policies.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies:getEnums"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies:getEnums"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -304,15 +307,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -378,15 +381,15 @@
             _request["risk_type"] = risk_type
         if description is not OMIT:
             _request["description"] = description
         if recommendation is not OMIT:
             _request["recommendation"] = recommendation
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -397,15 +400,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPoliciesClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_filter(
         self,
         name: str,
         *,
@@ -423,15 +428,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/filter/{name}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/filter/{name}"),
             params=remove_none_from_dict({"values": values, "filters": filters, "with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetFilterApiV2PoliciesFilterNameGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -451,15 +456,15 @@
         Parameters:
             - id: str.
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{id}"),
             params=remove_none_from_dict({"with_entities": with_entities}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -477,15 +482,15 @@
         Delete a policy and all of its associated alerts.
 
         Parameters:
             - id: str.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -504,15 +509,15 @@
         Parameters:
             - policy_id: str.
 
             - enabled: bool.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{policy_id}/status"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{policy_id}/status"),
             params=remove_none_from_dict({"enabled": enabled}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -605,15 +610,15 @@
             _request["predefined"] = predefined
         if auto_approval is not OMIT:
             _request["auto_approval"] = auto_approval
         if triggering_type is not OMIT:
             _request["triggering_type"] = triggering_type
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/policies/{policy_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/policies/{policy_id}"),
             params=remove_none_from_dict({"force": force}),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicyUpdateResponse, _response.json())  # type: ignore
@@ -629,15 +634,15 @@
 
     async def get_policy_enums(self) -> typing.Any:
         """
         Get available enums for filtering on policies.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies:getEnums"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies:getEnums"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -676,15 +681,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -750,15 +755,15 @@
             _request["risk_type"] = risk_type
         if description is not OMIT:
             _request["description"] = description
         if recommendation is not OMIT:
             _request["recommendation"] = recommendation
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/policies"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/policies"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PolicySchema, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/roles/client.py` & `fern_sentra-0.0.5/src/sentra/resources/roles/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.get_all_api_v_2_roles_get_response import GetAllApiV2RolesGetResponse
 from ...types.http_validation_error import HttpValidationError
 
 
 class RolesClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -47,15 +50,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/roles"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/roles"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -76,15 +79,17 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncRolesClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_all(
         self,
         *,
         offset: typing.Optional[int] = None,
@@ -111,15 +116,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/roles"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/roles"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/sensitivity/client.py` & `fern_sentra-0.0.5/src/sentra/resources/sensitivity/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 from json.decoder import JSONDecodeError
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.sensitivity_levels import SensitivityLevels
 
 
 class SensitivityClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_sensitivity_summary_data(self, *, connector_id: typing.Optional[int] = None) -> SensitivityLevels:
         """
         Get a summary of the number of data stores, grouped by sensitivity level.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/sensitivity/summary"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/sensitivity/summary"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SensitivityLevels, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -44,28 +47,30 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncSensitivityClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_sensitivity_summary_data(self, *, connector_id: typing.Optional[int] = None) -> SensitivityLevels:
         """
         Get a summary of the number of data stores, grouped by sensitivity level.
 
         Parameters:
             - connector_id: typing.Optional[int].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/sensitivity/summary"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/sensitivity/summary"),
             params=remove_none_from_dict({"connector_id": connector_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SensitivityLevels, _response.json())  # type: ignore
         if _response.status_code == 404:
```

### Comparing `fern_sentra-0.0.4/src/sentra/resources/users/client.py` & `fern_sentra-0.0.5/src/sentra/resources/users/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,38 +6,41 @@
 
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...environment import SentraEnvironment
 from ...errors.not_found_error import NotFoundError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.current_user_data import CurrentUserData
 from ...types.get_all_api_v_2_users_get_response import GetAllApiV2UsersGetResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.user_schema import UserSchema
 from ...types.user_status import UserStatus
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class UsersClient:
-    def __init__(self, *, environment: str, client_wrapper: SyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: SyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     def get_current_details(self) -> CurrentUserData:
         """
         Get information about the current logged in user or service account.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users/current"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users/current"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CurrentUserData, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -76,15 +79,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -123,15 +126,15 @@
         _request: typing.Dict[str, typing.Any] = {"user_id": user_id}
         if role_id is not OMIT:
             _request["role_id"] = role_id
         if status is not OMIT:
             _request["status"] = status
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -149,15 +152,15 @@
         Get all information on a specific user by ID.
 
         Parameters:
             - id: int.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/users/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -167,25 +170,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUsersClient:
-    def __init__(self, *, environment: str, client_wrapper: AsyncClientWrapper):
+    def __init__(
+        self, *, environment: SentraEnvironment = SentraEnvironment.PRODUCTION, client_wrapper: AsyncClientWrapper
+    ):
         self._environment = environment
         self._client_wrapper = client_wrapper
 
     async def get_current_details(self) -> CurrentUserData:
         """
         Get information about the current logged in user or service account.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users/current"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users/current"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CurrentUserData, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -224,15 +229,15 @@
 
             - filters: typing.Optional[str].
 
             - with_entities: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users"),
             params=remove_none_from_dict(
                 {
                     "offset": offset,
                     "limit": limit,
                     "count_only": count_only,
                     "group_by": group_by,
                     "sort_by": sort_by,
@@ -271,15 +276,15 @@
         _request: typing.Dict[str, typing.Any] = {"user_id": user_id}
         if role_id is not OMIT:
             _request["role_id"] = role_id
         if status is not OMIT:
             _request["status"] = status
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment}/", "api/v2/users"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/v2/users"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -297,15 +302,15 @@
         Get all information on a specific user by ID.
 
         Parameters:
             - id: int.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", f"api/v2/users/{id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/v2/users/{id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UserSchema, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/__init__.py` & `fern_sentra-0.0.5/src/sentra/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,24 @@
 from .auth_token_schema import AuthTokenSchema
 from .aws_connector_args import AwsConnectorArgs
 from .aws_installation_mode import AwsInstallationMode
 from .azure_boards_integration import AzureBoardsIntegration
 from .azure_boards_item import AzureBoardsItem
 from .azure_connector_args import AzureConnectorArgs
 from .choice_filter_data import ChoiceFilterData
+from .class_and_classifier_config_schema import ClassAndClassifierConfigSchema
+from .class_and_classifier_config_schema_classifier_config import (
+    ClassAndClassifierConfigSchemaClassifierConfig,
+    ClassAndClassifierConfigSchemaClassifierConfig_Dictionary,
+    ClassAndClassifierConfigSchemaClassifierConfig_Proprietary,
+    ClassAndClassifierConfigSchemaClassifierConfig_Regex,
+)
 from .class_categories import ClassCategories
-from .class_config import ClassConfig
 from .class_source import ClassSource
 from .classification_result_example import ClassificationResultExample
-from .classifier_type import ClassifierType
 from .compute_connectivity_type import ComputeConnectivityType
 from .compute_connector_properties_aws import ComputeConnectorPropertiesAws
 from .compute_connector_properties_azure import ComputeConnectorPropertiesAzure
 from .compute_connector_properties_gcp import ComputeConnectorPropertiesGcp
 from .connector_display import ConnectorDisplay
 from .connector_display_args import ConnectorDisplayArgs
 from .connector_display_compute_properties import (
@@ -68,27 +73,32 @@
     ConnectorSchemaComputeProperties_Aws,
     ConnectorSchemaComputeProperties_Azure,
     ConnectorSchemaComputeProperties_Gcp,
 )
 from .context_label_schema import ContextLabelSchema
 from .create_api_v_2_connectors_post_request import CreateApiV2ConnectorsPostRequest
 from .create_api_v_2_integrations_post_request import CreateApiV2IntegrationsPostRequest
+from .create_class_request_schema_classifier_schema import (
+    CreateClassRequestSchemaClassifierSchema,
+    CreateClassRequestSchemaClassifierSchema_Dictionary,
+    CreateClassRequestSchemaClassifierSchema_Regex,
+)
+from .create_dictionary_classifier_request_schema import CreateDictionaryClassifierRequestSchema
+from .create_regex_classifier_request_schema import CreateRegexClassifierRequestSchema
 from .current_user_data import CurrentUserData
 from .dashboard_data import DashboardData
 from .data_asset_at_risk import DataAssetAtRisk
 from .data_asset_class_user_operation import DataAssetClassUserOperation
 from .data_asset_extended import DataAssetExtended
 from .data_asset_object import DataAssetObject
 from .data_asset_props import DataAssetProps
 from .data_asset_row import DataAssetRow
 from .data_asset_schema import DataAssetSchema
-from .data_class_config_schema import DataClassConfigSchema
 from .data_class_config_with_user_schema import DataClassConfigWithUserSchema
 from .data_class_item import DataClassItem
-from .data_class_schema import DataClassSchema
 from .data_dog_integration import DataDogIntegration
 from .data_dog_item import DataDogItem
 from .data_dog_region import DataDogRegion
 from .data_hub_fabric import DataHubFabric
 from .data_hub_integration import DataHubIntegration
 from .data_hub_item import DataHubItem
 from .data_store_access_metadata import DataStoreAccessMetadata
@@ -113,41 +123,35 @@
     DetailedAlertSchemaWithCommentContent_ViolatedIamGroup,
     DetailedAlertSchemaWithCommentContent_ViolatedIamRole,
     DetailedAlertSchemaWithCommentContent_ViolatedIdentity,
     DetailedAlertSchemaWithCommentContent_ViolatedStore,
 )
 from .detailed_iam_group_schema import DetailedIamGroupSchema
 from .detailed_iam_role_schema import DetailedIamRoleSchema
+from .dictionary_classifier_response import DictionaryClassifierResponse
 from .email_input_item import EmailInputItem
 from .email_integration import EmailIntegration
 from .email_integration_input import EmailIntegrationInput
 from .email_output_item import EmailOutputItem
 from .event_log_action import EventLogAction
 from .event_log_entity_type import EventLogEntityType
 from .event_log_row import EventLogRow
-from .external_classifier_config import ExternalClassifierConfig
-from .filter_item import FilterItem
-from .filter_item_value import FilterItemValue
-from .filter_specs import FilterSpecs
-from .filter_specs_and_item import FilterSpecsAndItem
-from .filter_specs_not_item import FilterSpecsNotItem
-from .filter_specs_or_item import FilterSpecsOrItem
-from .format_type import FormatType
 from .gcp_connector_args import GcpConnectorArgs
 from .get_all_api_v_2_alerts_get_response import GetAllApiV2AlertsGetResponse
 from .get_all_api_v_2_audit_log_get_response import GetAllApiV2AuditLogGetResponse
 from .get_all_api_v_2_classes_get_response import GetAllApiV2ClassesGetResponse
 from .get_all_api_v_2_connectors_get_response import GetAllApiV2ConnectorsGetResponse
 from .get_all_api_v_2_data_access_identities_get_response import GetAllApiV2DataAccessIdentitiesGetResponse
 from .get_all_api_v_2_data_assets_get_response import GetAllApiV2DataAssetsGetResponse
 from .get_all_api_v_2_policies_get_response import GetAllApiV2PoliciesGetResponse
 from .get_all_api_v_2_roles_get_response import GetAllApiV2RolesGetResponse
 from .get_all_api_v_2_users_get_response import GetAllApiV2UsersGetResponse
 from .get_all_external_api_v_2_data_stores_get_response import GetAllExternalApiV2DataStoresGetResponse
 from .get_filter_api_v_2_alerts_filter_name_get_response import GetFilterApiV2AlertsFilterNameGetResponse
+from .get_filter_api_v_2_audit_log_filter_name_get_response import GetFilterApiV2AuditLogFilterNameGetResponse
 from .get_filter_api_v_2_classes_filter_name_get_response import GetFilterApiV2ClassesFilterNameGetResponse
 from .get_filter_api_v_2_data_access_filter_name_get_response import GetFilterApiV2DataAccessFilterNameGetResponse
 from .get_filter_api_v_2_data_assets_filter_name_get_response import GetFilterApiV2DataAssetsFilterNameGetResponse
 from .get_filter_api_v_2_data_stores_filter_name_get_response import GetFilterApiV2DataStoresFilterNameGetResponse
 from .get_filter_api_v_2_policies_filter_name_get_response import GetFilterApiV2PoliciesFilterNameGetResponse
 from .group_item import GroupItem
 from .grouped_data_table_result import GroupedDataTableResult
@@ -205,18 +209,20 @@
 from .policy_rule_type import PolicyRuleType
 from .policy_schema import PolicySchema
 from .policy_severity import PolicySeverity
 from .policy_status import PolicyStatus
 from .policy_triggering_type import PolicyTriggeringType
 from .policy_type import PolicyType
 from .policy_update_response import PolicyUpdateResponse
+from .proprietary_classifier_response import ProprietaryClassifierResponse
 from .provider_minimal_metadata import ProviderMinimalMetadata
 from .provider_schema import ProviderSchema
 from .provider_types import ProviderTypes
 from .range_filter_data import RangeFilterData
+from .regex_classifier_response import RegexClassifierResponse
 from .resolved_alert_source import ResolvedAlertSource
 from .risk_type import RiskType
 from .role_identity import RoleIdentity
 from .role_schema import RoleSchema
 from .runtime_properties import RuntimeProperties
 from .schedule_properties import ScheduleProperties
 from .seemplicity_integration import SeemplicityIntegration
@@ -236,14 +242,21 @@
 from .slack_web_hook_output_item import SlackWebHookOutputItem
 from .snowflake_connector_args import SnowflakeConnectorArgs
 from .sort import Sort
 from .sort_order import SortOrder
 from .teams_integration import TeamsIntegration
 from .teams_output_item import TeamsOutputItem
 from .test_connection_result import TestConnectionResult
+from .update_class_request_schema_classifier_schema import (
+    UpdateClassRequestSchemaClassifierSchema,
+    UpdateClassRequestSchemaClassifierSchema_Dictionary,
+    UpdateClassRequestSchemaClassifierSchema_Regex,
+)
+from .update_dictionary_classifier_request_schema import UpdateDictionaryClassifierRequestSchema
+from .update_regex_classifier_request_schema import UpdateRegexClassifierRequestSchema
 from .user_schema import UserSchema
 from .user_status import UserStatus
 from .validation_error import ValidationError
 from .violated_data_asset import ViolatedDataAsset
 from .violated_iam_group_alert_content import ViolatedIamGroupAlertContent
 from .violated_iam_role_alert_content import ViolatedIamRoleAlertContent
 from .violated_identity_alert_content import ViolatedIdentityAlertContent
@@ -285,19 +298,22 @@
     "AuthTokenSchema",
     "AwsConnectorArgs",
     "AwsInstallationMode",
     "AzureBoardsIntegration",
     "AzureBoardsItem",
     "AzureConnectorArgs",
     "ChoiceFilterData",
+    "ClassAndClassifierConfigSchema",
+    "ClassAndClassifierConfigSchemaClassifierConfig",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Dictionary",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Proprietary",
+    "ClassAndClassifierConfigSchemaClassifierConfig_Regex",
     "ClassCategories",
-    "ClassConfig",
     "ClassSource",
     "ClassificationResultExample",
-    "ClassifierType",
     "ComputeConnectivityType",
     "ComputeConnectorPropertiesAws",
     "ComputeConnectorPropertiesAzure",
     "ComputeConnectorPropertiesGcp",
     "ConnectorDisplay",
     "ConnectorDisplayArgs",
     "ConnectorDisplayComputeProperties",
@@ -315,27 +331,30 @@
     "ConnectorSchemaComputeProperties",
     "ConnectorSchemaComputeProperties_Aws",
     "ConnectorSchemaComputeProperties_Azure",
     "ConnectorSchemaComputeProperties_Gcp",
     "ContextLabelSchema",
     "CreateApiV2ConnectorsPostRequest",
     "CreateApiV2IntegrationsPostRequest",
+    "CreateClassRequestSchemaClassifierSchema",
+    "CreateClassRequestSchemaClassifierSchema_Dictionary",
+    "CreateClassRequestSchemaClassifierSchema_Regex",
+    "CreateDictionaryClassifierRequestSchema",
+    "CreateRegexClassifierRequestSchema",
     "CurrentUserData",
     "DashboardData",
     "DataAssetAtRisk",
     "DataAssetClassUserOperation",
     "DataAssetExtended",
     "DataAssetObject",
     "DataAssetProps",
     "DataAssetRow",
     "DataAssetSchema",
-    "DataClassConfigSchema",
     "DataClassConfigWithUserSchema",
     "DataClassItem",
-    "DataClassSchema",
     "DataDogIntegration",
     "DataDogItem",
     "DataDogRegion",
     "DataHubFabric",
     "DataHubIntegration",
     "DataHubItem",
     "DataStoreAccessMetadata",
@@ -356,41 +375,35 @@
     "DetailedAlertSchemaWithCommentContent_SimilarAssets",
     "DetailedAlertSchemaWithCommentContent_ViolatedIamGroup",
     "DetailedAlertSchemaWithCommentContent_ViolatedIamRole",
     "DetailedAlertSchemaWithCommentContent_ViolatedIdentity",
     "DetailedAlertSchemaWithCommentContent_ViolatedStore",
     "DetailedIamGroupSchema",
     "DetailedIamRoleSchema",
+    "DictionaryClassifierResponse",
     "EmailInputItem",
     "EmailIntegration",
     "EmailIntegrationInput",
     "EmailOutputItem",
     "EventLogAction",
     "EventLogEntityType",
     "EventLogRow",
-    "ExternalClassifierConfig",
-    "FilterItem",
-    "FilterItemValue",
-    "FilterSpecs",
-    "FilterSpecsAndItem",
-    "FilterSpecsNotItem",
-    "FilterSpecsOrItem",
-    "FormatType",
     "GcpConnectorArgs",
     "GetAllApiV2AlertsGetResponse",
     "GetAllApiV2AuditLogGetResponse",
     "GetAllApiV2ClassesGetResponse",
     "GetAllApiV2ConnectorsGetResponse",
     "GetAllApiV2DataAccessIdentitiesGetResponse",
     "GetAllApiV2DataAssetsGetResponse",
     "GetAllApiV2PoliciesGetResponse",
     "GetAllApiV2RolesGetResponse",
     "GetAllApiV2UsersGetResponse",
     "GetAllExternalApiV2DataStoresGetResponse",
     "GetFilterApiV2AlertsFilterNameGetResponse",
+    "GetFilterApiV2AuditLogFilterNameGetResponse",
     "GetFilterApiV2ClassesFilterNameGetResponse",
     "GetFilterApiV2DataAccessFilterNameGetResponse",
     "GetFilterApiV2DataAssetsFilterNameGetResponse",
     "GetFilterApiV2DataStoresFilterNameGetResponse",
     "GetFilterApiV2PoliciesFilterNameGetResponse",
     "GroupItem",
     "GroupedDataTableResult",
@@ -448,18 +461,20 @@
     "PolicyRuleType",
     "PolicySchema",
     "PolicySeverity",
     "PolicyStatus",
     "PolicyTriggeringType",
     "PolicyType",
     "PolicyUpdateResponse",
+    "ProprietaryClassifierResponse",
     "ProviderMinimalMetadata",
     "ProviderSchema",
     "ProviderTypes",
     "RangeFilterData",
+    "RegexClassifierResponse",
     "ResolvedAlertSource",
     "RiskType",
     "RoleIdentity",
     "RoleSchema",
     "RuntimeProperties",
     "ScheduleProperties",
     "SeemplicityIntegration",
@@ -479,14 +494,19 @@
     "SlackWebHookOutputItem",
     "SnowflakeConnectorArgs",
     "Sort",
     "SortOrder",
     "TeamsIntegration",
     "TeamsOutputItem",
     "TestConnectionResult",
+    "UpdateClassRequestSchemaClassifierSchema",
+    "UpdateClassRequestSchemaClassifierSchema_Dictionary",
+    "UpdateClassRequestSchemaClassifierSchema_Regex",
+    "UpdateDictionaryClassifierRequestSchema",
+    "UpdateRegexClassifierRequestSchema",
     "UserSchema",
     "UserStatus",
     "ValidationError",
     "ViolatedDataAsset",
     "ViolatedIamGroupAlertContent",
     "ViolatedIamRoleAlertContent",
     "ViolatedIdentityAlertContent",
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/access_data_store.py` & `fern_sentra-0.0.5/src/sentra/types/access_data_store.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/access_method_accessible_entities_flowchart.py` & `fern_sentra-0.0.5/src/sentra/types/access_method_accessible_entities_flowchart.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/access_permissions.py` & `fern_sentra-0.0.5/src/sentra/types/access_permissions.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/accessible_entities_flowchart_identity_node.py` & `fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_identity_node.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/accessible_entities_flowchart_store_node.py` & `fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_store_node.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/account_type.py` & `fern_sentra-0.0.5/src/sentra/types/account_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_comment_schema.py` & `fern_sentra-0.0.5/src/sentra/types/alert_comment_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_entity_type.py` & `fern_sentra-0.0.5/src/sentra/types/alert_entity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_response_schema.py` & `fern_sentra-0.0.5/src/sentra/types/alert_response_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_response_schema_content.py` & `fern_sentra-0.0.5/src/sentra/types/alert_response_schema_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_stats_by_date.py` & `fern_sentra-0.0.5/src/sentra/types/alert_stats_by_date.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_status.py` & `fern_sentra-0.0.5/src/sentra/types/alert_status.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_status_reason.py` & `fern_sentra-0.0.5/src/sentra/types/alert_status_reason.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/alert_type.py` & `fern_sentra-0.0.5/src/sentra/types/alert_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/amazon_security_lake_integration.py` & `fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/amazon_security_lake_item.py` & `fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/app_schemas_assets_public_access_level.py` & `fern_sentra-0.0.5/src/sentra/types/app_schemas_assets_public_access_level.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/app_schemas_stores_public_access_level.py` & `fern_sentra-0.0.5/src/sentra/types/app_schemas_stores_public_access_level.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/asset_class_user_request.py` & `fern_sentra-0.0.5/src/sentra/types/asset_class_user_request.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/asset_classes_props.py` & `fern_sentra-0.0.5/src/sentra/types/asset_classes_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/asset_type.py` & `fern_sentra-0.0.5/src/sentra/types/asset_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/auth_token_row.py` & `fern_sentra-0.0.5/src/sentra/types/auth_token_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/auth_token_schema.py` & `fern_sentra-0.0.5/src/sentra/types/auth_token_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/aws_connector_args.py` & `fern_sentra-0.0.5/src/sentra/types/aws_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/aws_installation_mode.py` & `fern_sentra-0.0.5/src/sentra/types/aws_installation_mode.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/azure_boards_integration.py` & `fern_sentra-0.0.5/src/sentra/types/azure_boards_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/azure_boards_item.py` & `fern_sentra-0.0.5/src/sentra/types/azure_boards_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/azure_connector_args.py` & `fern_sentra-0.0.5/src/sentra/types/azure_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/choice_filter_data.py` & `fern_sentra-0.0.5/src/sentra/types/choice_filter_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/class_categories.py` & `fern_sentra-0.0.5/src/sentra/types/class_categories.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/class_config.py` & `fern_sentra-0.0.5/src/sentra/types/validation_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ClassConfig(pydantic.BaseModel):
-    class_sensitivity_weight: typing.Optional[float]
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[str]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/classification_result_example.py` & `fern_sentra-0.0.5/src/sentra/types/classification_result_example.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/classifier_type.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_class_user_operation.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class ClassifierType(str, enum.Enum):
+class DataAssetClassUserOperation(str, enum.Enum):
     """
     An enumeration.
     """
 
-    REGEX = "REGEX"
-    DICTIONARY = "DICTIONARY"
+    ADD = "ADD"
+    REMOVE = "REMOVE"
 
-    def visit(self, regex: typing.Callable[[], T_Result], dictionary: typing.Callable[[], T_Result]) -> T_Result:
-        if self is ClassifierType.REGEX:
-            return regex()
-        if self is ClassifierType.DICTIONARY:
-            return dictionary()
+    def visit(self, add: typing.Callable[[], T_Result], remove: typing.Callable[[], T_Result]) -> T_Result:
+        if self is DataAssetClassUserOperation.ADD:
+            return add()
+        if self is DataAssetClassUserOperation.REMOVE:
+            return remove()
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/compute_connectivity_type.py` & `fern_sentra-0.0.5/src/sentra/types/compute_connectivity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_aws.py` & `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_aws.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_azure.py` & `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_azure.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/compute_connector_properties_gcp.py` & `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_gcp.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_display.py` & `fern_sentra-0.0.5/src/sentra/types/connector_display.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_display_compute_properties.py` & `fern_sentra-0.0.5/src/sentra/types/connector_display_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_input.py` & `fern_sentra-0.0.5/src/sentra/types/connector_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_input_compute_properties.py` & `fern_sentra-0.0.5/src/sentra/types/connector_input_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_schema.py` & `fern_sentra-0.0.5/src/sentra/types/connector_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/connector_schema_compute_properties.py` & `fern_sentra-0.0.5/src/sentra/types/connector_schema_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/context_label_schema.py` & `fern_sentra-0.0.5/src/sentra/types/context_label_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/current_user_data.py` & `fern_sentra-0.0.5/src/sentra/types/current_user_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/dashboard_data.py` & `fern_sentra-0.0.5/src/sentra/types/dashboard_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_at_risk.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_at_risk.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_extended.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_extended.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_object.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_object.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_props.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_row.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     sensitivity_level: typing.Optional[int]
     retention: typing.Optional[int]
     object_count: typing.Optional[int]
     row_count: typing.Optional[int]
     public_access_level: typing.Optional[AppSchemasAssetsPublicAccessLevel]
     is_backed_up: typing.Optional[bool]
     findings_count: typing.Optional[int]
+    last_modified: typing.Optional[str]
     connector_name: str = pydantic.Field(alias="Connector__name")
     connector_account_id: str = pydantic.Field(alias="Connector__account_id")
     data_store_name: str = pydantic.Field(alias="DataStore__name")
     data_store_region: typing.Optional[str] = pydantic.Field(alias="DataStore__region")
     database_engine: typing.Optional[str] = pydantic.Field(alias="Database__engine")
     connector_account_type: AccountType = pydantic.Field(alias="Connector__account_type")
     data_classes: typing.Optional[typing.List[DataClassItem]]
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_asset_schema.py` & `fern_sentra-0.0.5/src/sentra/types/data_asset_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_class_config_schema.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_iam_role_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,44 +2,37 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .class_categories import ClassCategories
-from .class_source import ClassSource
-from .external_classifier_config import ExternalClassifierConfig
+from .access_permissions import AccessPermissions
 
 
-class DataClassConfigSchema(pydantic.BaseModel):
-    """
-    Class represents a type of entity such as email, phone number, etc. It's a user facing entity that is also
-    controlled by the user. They can disable it, change its config, etc.
-    A class belongs to one category but has many classifiers
-    """
-
-    id: str
+class DetailedIamRoleSchema(pydantic.BaseModel):
     organization_id: int
+    connector_id: int
     name: str
-    description: typing.Optional[str] = pydantic.Field(
-        description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
-    )
-    source: ClassSource
-    category: ClassCategories
-    created_by: typing.Optional[int]
     created_at: str
-    config: ExternalClassifierConfig
-    enabled: bool
-    experimental: bool
+    last_activity: typing.Optional[str]
+    arn: str
+    access_policies_checksum: typing.Optional[str]
+    assumable_by_users_count: typing.Optional[int]
+    assumable_by_all_users: typing.Optional[int]
+    id: str
+    connector_name: str = pydantic.Field(alias="Connector__name")
+    permissions: typing.List[AccessPermissions]
+    accessible_data_stores: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_class_config_with_user_schema.py` & `fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,41 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .class_and_classifier_config_schema_classifier_config import ClassAndClassifierConfigSchemaClassifierConfig
 from .class_categories import ClassCategories
-from .class_config import ClassConfig
 from .class_source import ClassSource
 
 
-class DataClassConfigWithUserSchema(pydantic.BaseModel):
-    """
-    Class represents a type of entity such as email, phone number, etc. It's a user facing entity that is also
-    controlled by the user. They can disable it, change its config, etc.
-    A class belongs to one category but has many classifiers
-    """
-
+class ClassAndClassifierConfigSchema(pydantic.BaseModel):
     id: str
     organization_id: int
     name: str
     description: typing.Optional[str] = pydantic.Field(
         description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
     )
     source: ClassSource
     category: ClassCategories
     created_by: typing.Optional[int]
     created_at: str
-    config: ClassConfig
+    sensitivity_weight: int
     enabled: bool
     experimental: bool
-    user_name: typing.Optional[str]
-    user_email: typing.Optional[str]
+    classifier_config: ClassAndClassifierConfigSchemaClassifierConfig
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_class_item.py` & `fern_sentra-0.0.5/src/sentra/types/data_class_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_class_schema.py` & `fern_sentra-0.0.5/src/sentra/types/identity_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .class_categories import ClassCategories
-from .class_config import ClassConfig
-from .class_source import ClassSource
+from .access_permissions import AccessPermissions
+from .context_label_schema import ContextLabelSchema
+from .data_class_item import DataClassItem
+from .iam_access_key_schema import IamAccessKeySchema
+from .identity_origin import IdentityOrigin
+from .provider_schema import ProviderSchema
 
 
-class DataClassSchema(pydantic.BaseModel):
-    """
-    Class represents a type of entity such as email, phone number, etc. It's a user facing entity that is also
-    controlled by the user. They can disable it, change its config, etc.
-    A class belongs to one category but has many classifiers
-    """
-
-    id: str
+class IdentitySchema(pydantic.BaseModel):
     organization_id: int
+    connector_id: int
+    id: str
     name: str
-    description: typing.Optional[str] = pydantic.Field(
-        description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
-    )
-    source: ClassSource
-    category: ClassCategories
-    created_by: typing.Optional[int]
-    created_at: str
-    config: ClassConfig
-    enabled: bool
-    experimental: bool
+    origin: IdentityOrigin
+    provider: ProviderSchema
+    roles: int
+    groups: int
+    findings_count: typing.Optional[int]
+    permissions: typing.List[AccessPermissions]
+    data_classes: typing.Optional[typing.List[DataClassItem]]
+    created_at: typing.Optional[str]
+    last_activity: typing.Optional[str]
+    connector_name: str = pydantic.Field(alias="Connector__name")
+    access_keys: typing.List[IamAccessKeySchema]
+    context_labels: typing.List[ContextLabelSchema]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_dog_integration.py` & `fern_sentra-0.0.5/src/sentra/types/data_dog_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_dog_item.py` & `fern_sentra-0.0.5/src/sentra/types/data_dog_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_dog_region.py` & `fern_sentra-0.0.5/src/sentra/types/data_dog_region.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_hub_fabric.py` & `fern_sentra-0.0.5/src/sentra/types/data_hub_fabric.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_hub_integration.py` & `fern_sentra-0.0.5/src/sentra/types/data_hub_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_hub_item.py` & `fern_sentra-0.0.5/src/sentra/types/data_hub_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_access_metadata.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_access_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_extended.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_extended.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_identity.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_identity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_props.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_risk_aggregation.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_risk_aggregation.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/data_store_row.py` & `fern_sentra-0.0.5/src/sentra/types/data_store_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_content.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_with_comment.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_alert_schema_with_comment_content.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_iam_group_schema.py` & `fern_sentra-0.0.5/src/sentra/types/detailed_iam_group_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/detailed_iam_role_schema.py` & `fern_sentra-0.0.5/src/sentra/types/iam_group_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,37 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .access_permissions import AccessPermissions
 
 
-class DetailedIamRoleSchema(pydantic.BaseModel):
+class IamGroupSchema(pydantic.BaseModel):
     organization_id: int
     connector_id: int
     name: str
     created_at: str
-    last_activity: typing.Optional[str]
+    users: int
     arn: str
     access_policies_checksum: typing.Optional[str]
-    assumable_by_users_count: typing.Optional[int]
-    assumable_by_all_users: typing.Optional[int]
     id: str
-    connector_name: str = pydantic.Field(alias="Connector__name")
-    permissions: typing.List[AccessPermissions]
-    accessible_data_stores: int
+    discovered_at: str
+    last_seen_at: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/email_input_item.py` & `fern_sentra-0.0.5/src/sentra/types/email_input_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .policy_severity import PolicySeverity
 
 
 class EmailInputItem(pydantic.BaseModel):
     severities: typing.Optional[typing.List[PolicySeverity]]
     enabled: typing.Optional[bool]
-    accounts: typing.Optional[typing.List[int]]
+    accounts: typing.List[int]
     email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/email_integration.py` & `fern_sentra-0.0.5/src/sentra/types/email_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/email_integration_input.py` & `fern_sentra-0.0.5/src/sentra/types/email_integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/email_output_item.py` & `fern_sentra-0.0.5/src/sentra/types/email_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/event_log_action.py` & `fern_sentra-0.0.5/src/sentra/types/event_log_action.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/event_log_entity_type.py` & `fern_sentra-0.0.5/src/sentra/types/event_log_entity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/event_log_row.py` & `fern_sentra-0.0.5/src/sentra/types/event_log_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/filter_item.py` & `fern_sentra-0.0.5/src/sentra/types/dictionary_classifier_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .filter_item_value import FilterItemValue
 
 
-class FilterItem(pydantic.BaseModel):
-    value: typing.Optional[FilterItemValue]
-    op: typing.Optional[str]
-    negate: typing.Optional[bool]
-    field: str
+class DictionaryClassifierResponse(pydantic.BaseModel):
+    masking_function_name: str
+    match_min_count: int
+    keywords: typing.List[str]
+    dictionary: typing.Optional[typing.List[str]]
+    dictionary_size: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/filter_specs.py` & `fern_sentra-0.0.5/src/sentra/types/jira_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .policy_severity import PolicySeverity
 
 
-class FilterSpecs(pydantic.BaseModel):
-    not_: typing.Optional[typing.List[FilterSpecsNotItem]] = pydantic.Field(alias="not")
-    and_: typing.Optional[typing.List[FilterSpecsAndItem]] = pydantic.Field(alias="and")
-    or_: typing.Optional[typing.List[FilterSpecsOrItem]] = pydantic.Field(alias="or")
+class JiraItem(pydantic.BaseModel):
+    severities: typing.Optional[typing.List[PolicySeverity]]
+    enabled: typing.Optional[bool]
+    project_key: str
+    username: str
+    api_token: str
+    org_domain: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .filter_specs_and_item import FilterSpecsAndItem  # noqa: E402
-from .filter_specs_not_item import FilterSpecsNotItem  # noqa: E402
-from .filter_specs_or_item import FilterSpecsOrItem  # noqa: E402
-
-FilterSpecs.update_forward_refs()
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/gcp_connector_args.py` & `fern_sentra-0.0.5/src/sentra/types/gcp_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/group_item.py` & `fern_sentra-0.0.5/src/sentra/types/group_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/grouped_data_table_result.py` & `fern_sentra-0.0.5/src/sentra/types/grouped_data_table_result.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/http_validation_error.py` & `fern_sentra-0.0.5/src/sentra/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/iam_access_key_schema.py` & `fern_sentra-0.0.5/src/sentra/types/iam_access_key_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/iam_group_data_classes.py` & `fern_sentra-0.0.5/src/sentra/types/iam_group_data_classes.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/iam_group_schema.py` & `fern_sentra-0.0.5/src/sentra/types/user_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .user_status import UserStatus
 
 
-class IamGroupSchema(pydantic.BaseModel):
-    organization_id: int
-    connector_id: int
+class UserSchema(pydantic.BaseModel):
     name: str
-    created_at: str
-    users: int
-    arn: str
-    access_policies_checksum: typing.Optional[str]
-    id: str
-    discovered_at: str
-    last_seen_at: str
+    email: str
+    organization_id: int
+    role_id: int
+    status: UserStatus
+    id: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/iam_role_data_classes.py` & `fern_sentra-0.0.5/src/sentra/types/iam_role_data_classes.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/iam_role_schema.py` & `fern_sentra-0.0.5/src/sentra/types/iam_role_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart.py` & `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py` & `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_group.py` & `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_group.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_accessible_entities_flowchart_role.py` & `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_role.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_origin.py` & `fern_sentra-0.0.5/src/sentra/types/identity_origin.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/identity_schema.py` & `fern_sentra-0.0.5/src/sentra/types/policy_schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .access_permissions import AccessPermissions
-from .context_label_schema import ContextLabelSchema
-from .data_class_item import DataClassItem
-from .iam_access_key_schema import IamAccessKeySchema
-from .identity_origin import IdentityOrigin
-from .provider_schema import ProviderSchema
+from .policy_rule import PolicyRule
+from .policy_severity import PolicySeverity
+from .policy_status import PolicyStatus
+from .policy_triggering_type import PolicyTriggeringType
+from .policy_type import PolicyType
+from .risk_type import RiskType
 
 
-class IdentitySchema(pydantic.BaseModel):
-    organization_id: int
-    connector_id: int
-    id: str
+class PolicySchema(pydantic.BaseModel):
+    canonical: str
+    revision: str
     name: str
-    origin: IdentityOrigin
-    provider: ProviderSchema
-    roles: int
-    groups: int
-    findings_count: typing.Optional[int]
-    permissions: typing.List[AccessPermissions]
-    data_classes: typing.Optional[typing.List[DataClassItem]]
-    created_at: typing.Optional[str]
-    last_activity: typing.Optional[str]
-    connector_name: str = pydantic.Field(alias="Connector__name")
-    access_keys: typing.List[IamAccessKeySchema]
-    context_labels: typing.List[ContextLabelSchema]
+    severity: PolicySeverity
+    risk_type: typing.Optional[RiskType]
+    description: typing.Optional[str] = pydantic.Field(
+        description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
+    )
+    recommendation: typing.Optional[str]
+    status: PolicyStatus
+    predefined: bool
+    type: PolicyType
+    tags: typing.List[str]
+    frameworks: typing.List[str]
+    rules: typing.List[PolicyRule]
+    auto_approval: bool
+    triggering_type: typing.Optional[PolicyTriggeringType]
+    id: str
+    created_at: str
+    created_by: typing.Optional[str]
+    user_id: typing.Optional[int]
+    organization_id: int
+    opened_alerts: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_display.py` & `fern_sentra-0.0.5/src/sentra/types/integration_display.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_display_properties.py` & `fern_sentra-0.0.5/src/sentra/types/integration_display_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_input.py` & `fern_sentra-0.0.5/src/sentra/types/integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_input_properties.py` & `fern_sentra-0.0.5/src/sentra/types/integration_input_properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from .teams_integration import TeamsIntegration
 from .web_hook_integration_input import WebHookIntegrationInput
 
 IntegrationInputProperties = typing.Union[
     SlackIntegrationInput,
     EmailIntegrationInput,
     WebHookIntegrationInput,
+    TeamsIntegration,
     MondayIntegration,
     DataDogIntegration,
-    TeamsIntegration,
     JiraIntegration,
     DataHubIntegration,
     PagerDutyIntegration,
     SeemplicityIntegration,
     AmazonSecurityLakeIntegration,
     AzureBoardsIntegration,
 ]
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_output_schema.py` & `fern_sentra-0.0.5/src/sentra/types/integration_output_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_output_schema_properties.py` & `fern_sentra-0.0.5/src/sentra/types/integration_output_schema_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_schema.py` & `fern_sentra-0.0.5/src/sentra/types/integration_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_schema_properties.py` & `fern_sentra-0.0.5/src/sentra/types/integration_schema_properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from .teams_integration import TeamsIntegration
 from .web_hook_integration_input import WebHookIntegrationInput
 
 IntegrationSchemaProperties = typing.Union[
     SlackIntegrationInput,
     EmailIntegrationInput,
     WebHookIntegrationInput,
+    TeamsIntegration,
     MondayIntegration,
     DataDogIntegration,
-    TeamsIntegration,
     JiraIntegration,
     DataHubIntegration,
     PagerDutyIntegration,
     SeemplicityIntegration,
     AmazonSecurityLakeIntegration,
     AzureBoardsIntegration,
 ]
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/integration_type.py` & `fern_sentra-0.0.5/src/sentra/types/integration_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/jira_integration.py` & `fern_sentra-0.0.5/src/sentra/types/jira_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/jira_item.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_policies_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .policy_severity import PolicySeverity
+from .policy_schema import PolicySchema
+from .sort import Sort
 
 
-class JiraItem(pydantic.BaseModel):
-    severities: typing.Optional[typing.List[PolicySeverity]]
-    enabled: typing.Optional[bool]
-    project_key: str
-    username: str
-    api_token: str
-    org_domain: str
+class ListAllPoliciesResponse(pydantic.BaseModel):
+    grouped_by: typing.Optional[str]
+    sorted_by: typing.Optional[typing.List[Sort]]
+    all_matches_count: int
+    items: typing.List[PolicySchema]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/keyword_requirement.py` & `fern_sentra-0.0.5/src/sentra/types/keyword_requirement.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 class KeywordRequirement(str, enum.Enum):
     """
     An enumeration.
     """
 
     REQUIRED = "REQUIRED"
-    IF_STANDALONE = "IF_STANDALONE"
     NOT_REQUIRED = "NOT_REQUIRED"
+    IF_STANDALONE = "IF_STANDALONE"
 
     def visit(
         self,
         required: typing.Callable[[], T_Result],
-        if_standalone: typing.Callable[[], T_Result],
         not_required: typing.Callable[[], T_Result],
+        if_standalone: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is KeywordRequirement.REQUIRED:
             return required()
-        if self is KeywordRequirement.IF_STANDALONE:
-            return if_standalone()
         if self is KeywordRequirement.NOT_REQUIRED:
             return not_required()
+        if self is KeywordRequirement.IF_STANDALONE:
+            return if_standalone()
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_alerts_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_alerts_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_assets_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_auth_tokens_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_auth_tokens_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_connector_displays_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_connector_displays_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_context_label_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_context_label_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_data_class_config_with_users_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_data_class_config_with_users_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_data_stores_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_data_stores_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_event_log_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_event_log_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_identities_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_identities_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_policies_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_roles_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .policy_schema import PolicySchema
+from .role_schema import RoleSchema
 from .sort import Sort
 
 
-class ListAllPoliciesResponse(pydantic.BaseModel):
+class ListAllRolesResponse(pydantic.BaseModel):
     grouped_by: typing.Optional[str]
     sorted_by: typing.Optional[typing.List[Sort]]
     all_matches_count: int
-    items: typing.List[PolicySchema]
+    items: typing.List[RoleSchema]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_roles_response.py` & `fern_sentra-0.0.5/src/sentra/types/provider_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .role_schema import RoleSchema
-from .sort import Sort
+from .provider_types import ProviderTypes
 
 
-class ListAllRolesResponse(pydantic.BaseModel):
-    grouped_by: typing.Optional[str]
-    sorted_by: typing.Optional[typing.List[Sort]]
-    all_matches_count: int
-    items: typing.List[RoleSchema]
+class ProviderSchema(pydantic.BaseModel):
+    organization_id: int
+    connector_id: int
+    name: str
+    created_at: typing.Optional[str]
+    type: ProviderTypes
+    id: str
+    discovered_at: str
+    last_seen_at: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_all_users_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_all_users_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_similar_assets_pair_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_similar_assets_pair_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_similar_assets_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_similar_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_violated_data_assets_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_violated_data_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/list_violated_objects_response.py` & `fern_sentra-0.0.5/src/sentra/types/list_violated_objects_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/microsoft_365_connector_args.py` & `fern_sentra-0.0.5/src/sentra/types/microsoft_365_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/monday_integration.py` & `fern_sentra-0.0.5/src/sentra/types/monday_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/monday_item.py` & `fern_sentra-0.0.5/src/sentra/types/monday_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/new_auth_token_response.py` & `fern_sentra-0.0.5/src/sentra/types/new_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/object_class.py` & `fern_sentra-0.0.5/src/sentra/types/object_class.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/open_alerts_aggregation.py` & `fern_sentra-0.0.5/src/sentra/types/open_alerts_aggregation.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/pager_duty_integration.py` & `fern_sentra-0.0.5/src/sentra/types/pager_duty_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/pager_duty_item.py` & `fern_sentra-0.0.5/src/sentra/types/pager_duty_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/permissions.py` & `fern_sentra-0.0.5/src/sentra/types/permissions.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_rule.py` & `fern_sentra-0.0.5/src/sentra/types/policy_rule.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_rule_entity.py` & `fern_sentra-0.0.5/src/sentra/types/policy_rule_entity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_schema.py` & `fern_sentra-0.0.5/src/sentra/types/similar_assets_pair.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,47 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .policy_rule import PolicyRule
-from .policy_severity import PolicySeverity
-from .policy_status import PolicyStatus
-from .policy_triggering_type import PolicyTriggeringType
-from .policy_type import PolicyType
-from .risk_type import RiskType
-
-
-class PolicySchema(pydantic.BaseModel):
-    canonical: str
-    revision: str
-    name: str
-    severity: PolicySeverity
-    risk_type: typing.Optional[RiskType]
-    description: typing.Optional[str] = pydantic.Field(
-        description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
-    )
-    recommendation: typing.Optional[str]
-    status: PolicyStatus
-    predefined: bool
-    type: PolicyType
-    tags: typing.List[str]
-    frameworks: typing.List[str]
-    rules: typing.List[PolicyRule]
-    auto_approval: bool
-    triggering_type: typing.Optional[PolicyTriggeringType]
+from .data_asset_schema import DataAssetSchema
+from .similar_assets_props import SimilarAssetsProps
+
+
+class SimilarAssetsPair(pydantic.BaseModel):
     id: str
-    created_at: str
-    created_by: typing.Optional[str]
-    user_id: typing.Optional[int]
-    organization_id: int
-    opened_alerts: typing.Optional[int]
-    last_executed: typing.Optional[str]
+    base_asset: DataAssetSchema
+    similar_asset: DataAssetSchema
+    similarity_rate: float
+    similarity_size: typing.Optional[int]
+    properties: typing.Optional[SimilarAssetsProps]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_severity.py` & `fern_sentra-0.0.5/src/sentra/types/policy_severity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_status.py` & `fern_sentra-0.0.5/src/sentra/types/policy_status.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_triggering_type.py` & `fern_sentra-0.0.5/src/sentra/types/policy_triggering_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_type.py` & `fern_sentra-0.0.5/src/sentra/types/policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/policy_update_response.py` & `fern_sentra-0.0.5/src/sentra/types/policy_update_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/provider_minimal_metadata.py` & `fern_sentra-0.0.5/src/sentra/types/provider_minimal_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/provider_schema.py` & `fern_sentra-0.0.5/src/sentra/types/sort.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .provider_types import ProviderTypes
+from .sort_order import SortOrder
 
 
-class ProviderSchema(pydantic.BaseModel):
-    organization_id: int
-    connector_id: int
-    name: str
-    created_at: typing.Optional[str]
-    type: ProviderTypes
-    id: str
-    discovered_at: str
-    last_seen_at: str
+class Sort(pydantic.BaseModel):
+    field: str
+    order: typing.Optional[SortOrder]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/provider_types.py` & `fern_sentra-0.0.5/src/sentra/types/provider_types.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/range_filter_data.py` & `fern_sentra-0.0.5/src/sentra/types/range_filter_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/resolved_alert_source.py` & `fern_sentra-0.0.5/src/sentra/types/resolved_alert_source.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/risk_type.py` & `fern_sentra-0.0.5/src/sentra/types/risk_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/role_identity.py` & `fern_sentra-0.0.5/src/sentra/types/role_identity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/role_schema.py` & `fern_sentra-0.0.5/src/sentra/types/role_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/runtime_properties.py` & `fern_sentra-0.0.5/src/sentra/types/runtime_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/schedule_properties.py` & `fern_sentra-0.0.5/src/sentra/types/schedule_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/seemplicity_integration.py` & `fern_sentra-0.0.5/src/sentra/types/seemplicity_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/seemplicity_item.py` & `fern_sentra-0.0.5/src/sentra/types/seemplicity_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/sensitivity_levels.py` & `fern_sentra-0.0.5/src/sentra/types/sensitivity_levels.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_asset_schema.py` & `fern_sentra-0.0.5/src/sentra/types/similar_asset_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_assets_alert_content.py` & `fern_sentra-0.0.5/src/sentra/types/similar_assets_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_assets_pair.py` & `fern_sentra-0.0.5/src/sentra/types/similar_assets_pair_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .data_asset_schema import DataAssetSchema
 from .similar_assets_props import SimilarAssetsProps
+from .similarity_type import SimilarityType
 
 
-class SimilarAssetsPair(pydantic.BaseModel):
+class SimilarAssetsPairSchema(pydantic.BaseModel):
     id: str
-    base_asset: DataAssetSchema
-    similar_asset: DataAssetSchema
-    similarity_rate: float
-    similarity_size: typing.Optional[int]
+    organization_id: int
+    asset_a_id: str
+    asset_b_id: str
+    store_a_id: str
+    store_b_id: str
+    similarity_type: SimilarityType
+    created_at: str
     properties: typing.Optional[SimilarAssetsProps]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_assets_pair_schema.py` & `fern_sentra-0.0.5/src/sentra/types/violated_identity_alert_content.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,29 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .similar_assets_props import SimilarAssetsProps
-from .similarity_type import SimilarityType
 
 
-class SimilarAssetsPairSchema(pydantic.BaseModel):
-    id: str
-    organization_id: int
-    asset_a_id: str
-    asset_b_id: str
-    store_a_id: str
-    store_b_id: str
-    similarity_type: SimilarityType
-    created_at: str
-    properties: typing.Optional[SimilarAssetsProps]
-
+class ViolatedIdentityAlertContent(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_assets_props.py` & `fern_sentra-0.0.5/src/sentra/types/similar_assets_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/similar_store.py` & `fern_sentra-0.0.5/src/sentra/types/similar_store.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/similarity_type.py` & `fern_sentra-0.0.5/src/sentra/types/similarity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/slack_integration.py` & `fern_sentra-0.0.5/src/sentra/types/slack_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/slack_integration_input.py` & `fern_sentra-0.0.5/src/sentra/types/slack_integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/slack_web_hook_input_item.py` & `fern_sentra-0.0.5/src/sentra/types/slack_web_hook_input_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .policy_severity import PolicySeverity
 
 
 class SlackWebHookInputItem(pydantic.BaseModel):
     severities: typing.Optional[typing.List[PolicySeverity]]
     enabled: typing.Optional[bool]
-    accounts: typing.Optional[typing.List[int]]
+    accounts: typing.List[int]
     slack_webhook: str = pydantic.Field(
         description='<span style="white-space: nowrap">`non-empty`</span> <span style="white-space: nowrap">`<= 2083 characters`</span>'
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/slack_web_hook_output_item.py` & `fern_sentra-0.0.5/src/sentra/types/slack_web_hook_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/snowflake_connector_args.py` & `fern_sentra-0.0.5/src/sentra/types/snowflake_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/sort.py` & `fern_sentra-0.0.5/src/sentra/types/violated_store_alert_content.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .sort_order import SortOrder
 
 
-class Sort(pydantic.BaseModel):
-    field: str
-    order: typing.Optional[SortOrder]
+class ViolatedStoreAlertContent(pydantic.BaseModel):
+    violated_asset_ids: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/teams_integration.py` & `fern_sentra-0.0.5/src/sentra/types/teams_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/teams_output_item.py` & `fern_sentra-0.0.5/src/sentra/types/teams_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/test_connection_result.py` & `fern_sentra-0.0.5/src/sentra/types/test_connection_result.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/user_schema.py` & `fern_sentra-0.0.5/src/sentra/types/create_regex_classifier_request_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .user_status import UserStatus
+from .keyword_requirement import KeywordRequirement
 
 
-class UserSchema(pydantic.BaseModel):
-    name: str
-    email: str
-    organization_id: int
-    role_id: int
-    status: UserStatus
-    id: int
+class CreateRegexClassifierRequestSchema(pydantic.BaseModel):
+    match_min_count: typing.Optional[int]
+    masking_function_name: typing.Optional[str]
+    keywords: typing.Optional[typing.List[str]]
+    keyword_requirement: typing.Optional[KeywordRequirement]
+    pattern: str
+    exclusion_pattern: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/validation_error.py` & `fern_sentra-0.0.5/src/sentra/types/proprietary_classifier_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[str]
-    msg: str
-    type: str
+class ProprietaryClassifierResponse(pydantic.BaseModel):
+    masking_function_name: str
+    match_min_count: int
+    keywords: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_data_asset.py` & `fern_sentra-0.0.5/src/sentra/types/violated_data_asset.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_iam_group_alert_content.py` & `fern_sentra-0.0.5/src/sentra/types/violated_iam_group_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_iam_role_alert_content.py` & `fern_sentra-0.0.5/src/sentra/types/violated_iam_role_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_identity_alert_content.py` & `fern_sentra-0.0.5/src/sentra/types/web_hook_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .web_hook_output_item import WebHookOutputItem
 
 
-class ViolatedIdentityAlertContent(pydantic.BaseModel):
+class WebHookIntegration(pydantic.BaseModel):
+    items: typing.List[WebHookOutputItem]
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_object.py` & `fern_sentra-0.0.5/src/sentra/types/violated_object.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.4/src/sentra/types/violated_store_alert_content.py` & `fern_sentra-0.0.5/src/sentra/types/regex_classifier_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ViolatedStoreAlertContent(pydantic.BaseModel):
-    violated_asset_ids: typing.List[str]
+class RegexClassifierResponse(pydantic.BaseModel):
+    masking_function_name: str
+    match_min_count: int
+    keywords: typing.List[str]
+    pattern: str
+    exclusion_pattern: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/web_hook_input_item.py` & `fern_sentra-0.0.5/src/sentra/types/web_hook_input_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .policy_severity import PolicySeverity
 
 
 class WebHookInputItem(pydantic.BaseModel):
     severities: typing.Optional[typing.List[PolicySeverity]]
     enabled: typing.Optional[bool]
-    accounts: typing.Optional[typing.List[int]]
+    accounts: typing.List[int]
     webhook_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/web_hook_integration.py` & `fern_sentra-0.0.5/src/sentra/types/web_hook_integration_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .web_hook_output_item import WebHookOutputItem
+from .web_hook_input_item import WebHookInputItem
 
 
-class WebHookIntegration(pydantic.BaseModel):
-    items: typing.List[WebHookOutputItem]
+class WebHookIntegrationInput(pydantic.BaseModel):
+    items: typing.List[WebHookInputItem]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/web_hook_integration_input.py` & `fern_sentra-0.0.5/src/sentra/types/web_hook_output_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .web_hook_input_item import WebHookInputItem
+from .policy_severity import PolicySeverity
 
 
-class WebHookIntegrationInput(pydantic.BaseModel):
-    items: typing.List[WebHookInputItem]
+class WebHookOutputItem(pydantic.BaseModel):
+    severities: typing.Optional[typing.List[PolicySeverity]]
+    enabled: typing.Optional[bool]
+    accounts: typing.Dict[str, str]
+    webhook_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/src/sentra/types/web_hook_output_item.py` & `fern_sentra-0.0.5/src/sentra/types/data_class_config_with_user_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .policy_severity import PolicySeverity
+from .class_categories import ClassCategories
+from .class_source import ClassSource
 
 
-class WebHookOutputItem(pydantic.BaseModel):
-    severities: typing.Optional[typing.List[PolicySeverity]]
-    enabled: typing.Optional[bool]
-    accounts: typing.Dict[str, str]
-    webhook_url: str
+class DataClassConfigWithUserSchema(pydantic.BaseModel):
+    id: str
+    organization_id: int
+    name: str
+    description: typing.Optional[str] = pydantic.Field(
+        description='<span style="white-space: nowrap">`<= 1024 characters`</span>'
+    )
+    source: ClassSource
+    category: ClassCategories
+    created_by: typing.Optional[int]
+    created_at: str
+    sensitivity_weight: int
+    enabled: bool
+    experimental: bool
+    user_name: typing.Optional[str]
+    user_email: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_sentra-0.0.4/PKG-INFO` & `fern_sentra-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-sentra
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

