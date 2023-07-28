# Comparing `tmp/validio_sdk-0.6.4.tar.gz` & `tmp/validio_sdk-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.6.4.tar", max compression
+gzip compressed data, was "validio_sdk-0.6.5.tar", max compression
```

## Comparing `validio_sdk-0.6.4.tar` & `validio_sdk-0.6.5.tar`

### file list

```diff
@@ -1,229 +1,225 @@
--rw-r--r--   0        0        0    11340 2023-07-21 13:06:25.395451 validio_sdk-0.6.4/LICENSE
--rw-r--r--   0        0        0      308 2023-07-21 13:06:25.395451 validio_sdk-0.6.4/README_PUBLIC.md
--rw-r--r--   0        0        0     5010 2023-07-21 13:06:37.623433 validio_sdk-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      588 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0     7069 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/_import.py
--rw-r--r--   0        0        0      551 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4751 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5891 2023-07-21 13:06:25.401451 validio_sdk-0.6.4/validio_sdk/config.py
--rw-r--r--   0        0        0   261652 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7319 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-07-21 13:06:25.402451 validio_sdk-0.6.4/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   653049 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      506 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_athena_credential.py
--rw-r--r--   0        0        0      458 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_athena_source.py
--rw-r--r--   0        0        0      445 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-07-21 13:06:25.403451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      594 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_sasl_ssl_plain_credential.py
--rw-r--r--   0        0        0      417 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_source.py
--rw-r--r--   0        0        0      498 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_ssl_credential.py
--rw-r--r--   0        0        0      487 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_notification_rule.py
--rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-07-21 13:06:25.404451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      487 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_notification_rule.py
--rw-r--r--   0        0        0      646 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3198 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   188562 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     8055 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0     5368 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_incidents.py
--rw-r--r--   0        0        0      627 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-21 13:06:25.405451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rules.py
--rw-r--r--   0        0        0     2245 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_recommendation.py
--rw-r--r--   0        0        0      460 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    24018 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    29481 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0     1727 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_incidents.py
--rw-r--r--   0        0        0    25201 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0      551 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      286 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_athena_schema.py
--rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      269 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_kafka_schema.py
--rw-r--r--   0        0        0      290 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-07-21 13:06:25.406451 validio_sdk-0.6.4/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    39698 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0      675 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py
--rw-r--r--   0        0        0      583 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
--rw-r--r--   0        0        0     6998 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    25334 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      594 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      288 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/segments.py
--rw-r--r--   0        0        0      499 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/segments_by_resource_name.py
--rw-r--r--   0        0        0      592 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      502 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_athena_credential.py
--rw-r--r--   0        0        0      454 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_athena_source.py
--rw-r--r--   0        0        0      441 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_channel_namespace.py
--rw-r--r--   0        0        0      499 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_credential_namespace.py
--rw-r--r--   0        0        0      509 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_destination_namespace.py
--rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      560 2023-07-21 13:06:25.407451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_identity_provider_namespace.py
--rw-r--r--   0        0        0      590 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_sasl_ssl_plain_credential.py
--rw-r--r--   0        0        0      413 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_source.py
--rw-r--r--   0        0        0      494 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_ssl_credential.py
--rw-r--r--   0        0        0      534 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      483 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule.py
--rw-r--r--   0        0        0      560 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule_namespace.py
--rw-r--r--   0        0        0      540 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      519 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_segmentation_namespace.py
--rw-r--r--   0        0        0      473 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_source_namespace.py
--rw-r--r--   0        0        0      443 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0      439 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_user_namespace.py
--rw-r--r--   0        0        0      491 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_namespace.py
--rw-r--r--   0        0        0    57176 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      459 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/graphql_client/update_window_namespace.py
--rw-r--r--   0        0        0      265 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    21078 2023-07-21 13:06:25.408451 validio_sdk-0.6.4/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1505 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     4326 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4002 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    19682 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0     1355 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     6860 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    21679 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0     5273 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_update_namespace.py
--rw-r--r--   0        0        0      847 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5027 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     8164 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5601 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     6262 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4846 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/notification_rules.py
--rw-r--r--   0        0        0     2040 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    26091 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15408 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16357 2023-07-21 13:06:25.409451 validio_sdk-0.6.4/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0     5638 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    33277 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1377 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/util.py
--rw-r--r--   0        0        0     2382 2023-07-21 13:06:25.410451 validio_sdk-0.6.4/validio_sdk/validio_client.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-28 06:49:34.494246 validio_sdk-0.6.5/LICENSE
+-rw-r--r--   0        0        0      308 2023-07-28 06:49:34.494246 validio_sdk-0.6.5/README_PUBLIC.md
+-rw-r--r--   0        0        0     5010 2023-07-28 06:49:50.566210 validio_sdk-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-07-28 06:49:34.499246 validio_sdk-0.6.5/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:49:34.499246 validio_sdk-0.6.5/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0     7069 2023-07-28 06:49:34.499246 validio_sdk-0.6.5/validio_sdk/code/_import.py
+-rw-r--r--   0        0        0      551 2023-07-28 06:49:34.499246 validio_sdk-0.6.5/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4751 2023-07-28 06:49:34.499246 validio_sdk-0.6.5/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/config.py
+-rw-r--r--   0        0        0   223347 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-07-28 06:49:34.500246 validio_sdk-0.6.5/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   588785 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      506 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_athena_credential.py
+-rw-r--r--   0        0        0      458 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_athena_source.py
+-rw-r--r--   0        0        0      445 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-28 06:49:34.502246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      594 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_kafka_sasl_ssl_plain_credential.py
+-rw-r--r--   0        0        0      417 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_kafka_source.py
+-rw-r--r--   0        0        0      498 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      487 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      516 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-07-28 06:49:34.503246 validio_sdk-0.6.5/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3198 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   181669 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     8055 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     4696 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0     2245 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_recommendation.py
+-rw-r--r--   0        0        0      460 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-07-28 06:49:34.504246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    24162 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    29625 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    25201 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    37004 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    44406 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     2842 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      286 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_aws_athena_schema.py
+-rw-r--r--   0        0        0      290 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      269 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_kafka_schema.py
+-rw-r--r--   0        0        0      290 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    39475 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0      675 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py
+-rw-r--r--   0        0        0      583 2023-07-28 06:49:34.505246 validio_sdk-0.6.5/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
+-rw-r--r--   0        0        0     6998 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    25478 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    38893 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      502 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_athena_credential.py
+-rw-r--r--   0        0        0      454 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_athena_source.py
+-rw-r--r--   0        0        0      441 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_channel_namespace.py
+-rw-r--r--   0        0        0      499 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_credential_namespace.py
+-rw-r--r--   0        0        0      509 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_destination_namespace.py
+-rw-r--r--   0        0        0      464 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      560 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_identity_provider_namespace.py
+-rw-r--r--   0        0        0      590 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_kafka_sasl_ssl_plain_credential.py
+-rw-r--r--   0        0        0      413 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_kafka_source.py
+-rw-r--r--   0        0        0      494 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      534 2023-07-28 06:49:34.506246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      560 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_notification_rule_namespace.py
+-rw-r--r--   0        0        0      540 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      519 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_segmentation_namespace.py
+-rw-r--r--   0        0        0      473 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      459 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_source_namespace.py
+-rw-r--r--   0        0        0      443 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0      439 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_user_namespace.py
+-rw-r--r--   0        0        0      491 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_validator_namespace.py
+-rw-r--r--   0        0        0    52608 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    51580 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      459 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      459 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/graphql_client/update_window_namespace.py
+-rw-r--r--   0        0        0      265 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-07-28 06:49:34.507246 validio_sdk-0.6.5/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1505 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     4326 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    19682 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     6860 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21679 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0     5273 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_update_namespace.py
+-rw-r--r--   0        0        0      847 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     8164 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5601 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6262 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    26670 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:49:34.508246 validio_sdk-0.6.5/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     4459 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    33277 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-07-28 06:49:34.509246 validio_sdk-0.6.5/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.5/PKG-INFO
```

### Comparing `validio_sdk-0.6.4/LICENSE` & `validio_sdk-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/pyproject.toml` & `validio_sdk-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-sdk"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.6.4"
+version = "0.6.5"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://dev.validio.io/sdk-docs"
 packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
```

### Comparing `validio_sdk-0.6.4/validio_sdk/__init__.py` & `validio_sdk-0.6.5/validio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/code/_import.py` & `validio_sdk-0.6.5/validio_sdk/code/_import.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/code/apply.py` & `validio_sdk-0.6.5/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/code/plan.py` & `validio_sdk-0.6.5/validio_sdk/code/plan.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/code/scaffold.py` & `validio_sdk-0.6.5/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/config.py` & `validio_sdk-0.6.5/validio_sdk/config.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -122,30 +122,22 @@
     CreateNumericDistributionValidatorWithDynamicThreshold,
     CreateNumericDistributionValidatorWithDynamicThresholdNumericDistributionValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_distribution_validator_with_fixed_threshold import (
     CreateNumericDistributionValidatorWithFixedThreshold,
     CreateNumericDistributionValidatorWithFixedThresholdNumericDistributionValidatorWithFixedThresholdCreate,
 )
-from .create_numeric_distribution_validator_with_monotonic_threshold import (
-    CreateNumericDistributionValidatorWithMonotonicThreshold,
-    CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate,
-)
 from .create_numeric_validator_with_dynamic_threshold import (
     CreateNumericValidatorWithDynamicThreshold,
     CreateNumericValidatorWithDynamicThresholdNumericValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_validator_with_fixed_threshold import (
     CreateNumericValidatorWithFixedThreshold,
     CreateNumericValidatorWithFixedThresholdNumericValidatorWithFixedThresholdCreate,
 )
-from .create_numeric_validator_with_monotonic_threshold import (
-    CreateNumericValidatorWithMonotonicThreshold,
-    CreateNumericValidatorWithMonotonicThresholdNumericValidatorWithMonotonicThresholdCreate,
-)
 from .create_postgre_sql_credential import (
     CreatePostgreSqlCredential,
     CreatePostgreSqlCredentialPostgreSqlCredentialCreate,
 )
 from .create_postgre_sql_source import (
     CreatePostgreSqlSource,
     CreatePostgreSqlSourcePostgreSqlSourceCreate,
@@ -154,18 +146,14 @@
     CreateRelativeTimeValidatorWithDynamicThreshold,
     CreateRelativeTimeValidatorWithDynamicThresholdRelativeTimeValidatorWithDynamicThresholdCreate,
 )
 from .create_relative_time_validator_with_fixed_threshold import (
     CreateRelativeTimeValidatorWithFixedThreshold,
     CreateRelativeTimeValidatorWithFixedThresholdRelativeTimeValidatorWithFixedThresholdCreate,
 )
-from .create_relative_time_validator_with_monotonic_threshold import (
-    CreateRelativeTimeValidatorWithMonotonicThreshold,
-    CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate,
-)
 from .create_relative_volume_validator_with_dynamic_threshold import (
     CreateRelativeVolumeValidatorWithDynamicThreshold,
     CreateRelativeVolumeValidatorWithDynamicThresholdRelativeVolumeValidatorWithDynamicThresholdCreate,
 )
 from .create_relative_volume_validator_with_fixed_threshold import (
     CreateRelativeVolumeValidatorWithFixedThreshold,
     CreateRelativeVolumeValidatorWithFixedThresholdRelativeVolumeValidatorWithFixedThresholdCreate,
@@ -363,15 +351,14 @@
     CredentialUpdateCredentialKafkaSSLCredential,
     CredentialUpdateCredentialKafkaSSLCredentialConfig,
     CredentialUpdateCredentialPostgreSqlCredential,
     CredentialUpdateCredentialPostgreSqlCredentialConfig,
     CredentialUpdateCredentialSnowflakeCredential,
     CredentialUpdateCredentialSnowflakeCredentialConfig,
     CredentialUpdateErrors,
-    DeletedEntity,
     DestinationCreation,
     DestinationCreationDestinationAwsKinesisDestination,
     DestinationCreationDestinationAwsKinesisDestinationConfig,
     DestinationCreationDestinationAwsKinesisDestinationCredential,
     DestinationCreationDestinationDestination,
     DestinationCreationDestinationDestinationCredential,
     DestinationCreationDestinationGcpBigQueryDestination,
@@ -578,79 +565,72 @@
     UserUpdateUser,
     ValidatorCreation,
     ValidatorCreationErrors,
     ValidatorCreationValidatorCategoricalDistributionValidator,
     ValidatorCreationValidatorCategoricalDistributionValidatorConfig,
     ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfig,
     ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
     ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
     ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfig,
     ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSource,
     ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigWindow,
     ValidatorCreationValidatorFreshnessValidator,
     ValidatorCreationValidatorFreshnessValidatorConfig,
     ValidatorCreationValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorFreshnessValidatorSourceConfig,
     ValidatorCreationValidatorFreshnessValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorFreshnessValidatorSourceConfigSource,
     ValidatorCreationValidatorFreshnessValidatorSourceConfigWindow,
     ValidatorCreationValidatorNumericAnomalyValidator,
     ValidatorCreationValidatorNumericAnomalyValidatorConfig,
     ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorNumericAnomalyValidatorDestination,
     ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfig,
     ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
     ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
     ValidatorCreationValidatorNumericAnomalyValidatorSourceConfig,
     ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSource,
     ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigWindow,
     ValidatorCreationValidatorNumericDistributionValidator,
     ValidatorCreationValidatorNumericDistributionValidatorConfig,
     ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfig,
     ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigSource,
     ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
     ValidatorCreationValidatorNumericDistributionValidatorSourceConfig,
     ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSource,
     ValidatorCreationValidatorNumericDistributionValidatorSourceConfigWindow,
     ValidatorCreationValidatorNumericValidator,
     ValidatorCreationValidatorNumericValidatorConfig,
     ValidatorCreationValidatorNumericValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorNumericValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorNumericValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorNumericValidatorSourceConfig,
     ValidatorCreationValidatorNumericValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorNumericValidatorSourceConfigSource,
     ValidatorCreationValidatorNumericValidatorSourceConfigWindow,
     ValidatorCreationValidatorRelativeTimeValidator,
     ValidatorCreationValidatorRelativeTimeValidatorConfig,
     ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorRelativeTimeValidatorSourceConfig,
     ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSource,
     ValidatorCreationValidatorRelativeTimeValidatorSourceConfigWindow,
     ValidatorCreationValidatorRelativeVolumeValidator,
     ValidatorCreationValidatorRelativeVolumeValidatorConfig,
     ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfig,
     ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
     ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
     ValidatorCreationValidatorRelativeVolumeValidatorSourceConfig,
     ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSource,
     ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigWindow,
@@ -659,100 +639,91 @@
     ValidatorCreationValidatorValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorValidatorSourceConfigSource,
     ValidatorCreationValidatorValidatorSourceConfigWindow,
     ValidatorCreationValidatorVolumeValidator,
     ValidatorCreationValidatorVolumeValidatorConfig,
     ValidatorCreationValidatorVolumeValidatorConfigThresholdDynamicThreshold,
     ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorVolumeValidatorDestination,
     ValidatorCreationValidatorVolumeValidatorSourceConfig,
     ValidatorCreationValidatorVolumeValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorVolumeValidatorSourceConfigSource,
     ValidatorCreationValidatorVolumeValidatorSourceConfigWindow,
     ValidatorIncidents,
     ValidatorIncidentsMetricValidatorMetric,
     ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold,
     ValidatorIncidentsMetricValidatorMetricWithFixedThreshold,
-    ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold,
     ValidatorIncidentsSegment,
     ValidatorRecommendationApplication,
     ValidatorRecommendationDismissal,
     ValidatorRecommendationDismissalErrors,
     ValidatorUpdate,
     ValidatorUpdateErrors,
     ValidatorUpdateValidatorCategoricalDistributionValidator,
     ValidatorUpdateValidatorCategoricalDistributionValidatorConfig,
     ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig,
     ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
     ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
     ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfig,
     ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSource,
     ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow,
     ValidatorUpdateValidatorFreshnessValidator,
     ValidatorUpdateValidatorFreshnessValidatorConfig,
     ValidatorUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorFreshnessValidatorSourceConfig,
     ValidatorUpdateValidatorFreshnessValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorFreshnessValidatorSourceConfigSource,
     ValidatorUpdateValidatorFreshnessValidatorSourceConfigWindow,
     ValidatorUpdateValidatorNumericAnomalyValidator,
     ValidatorUpdateValidatorNumericAnomalyValidatorConfig,
     ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorNumericAnomalyValidatorDestination,
     ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig,
     ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
     ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
     ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfig,
     ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSource,
     ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigWindow,
     ValidatorUpdateValidatorNumericDistributionValidator,
     ValidatorUpdateValidatorNumericDistributionValidatorConfig,
     ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfig,
     ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource,
     ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
     ValidatorUpdateValidatorNumericDistributionValidatorSourceConfig,
     ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSource,
     ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigWindow,
     ValidatorUpdateValidatorNumericValidator,
     ValidatorUpdateValidatorNumericValidatorConfig,
     ValidatorUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorNumericValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorNumericValidatorSourceConfig,
     ValidatorUpdateValidatorNumericValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorNumericValidatorSourceConfigSource,
     ValidatorUpdateValidatorNumericValidatorSourceConfigWindow,
     ValidatorUpdateValidatorRelativeTimeValidator,
     ValidatorUpdateValidatorRelativeTimeValidatorConfig,
     ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorRelativeTimeValidatorSourceConfig,
     ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSource,
     ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigWindow,
     ValidatorUpdateValidatorRelativeVolumeValidator,
     ValidatorUpdateValidatorRelativeVolumeValidatorConfig,
     ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig,
     ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
     ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
     ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfig,
     ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSource,
     ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigWindow,
@@ -761,15 +732,14 @@
     ValidatorUpdateValidatorValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorValidatorSourceConfigSource,
     ValidatorUpdateValidatorValidatorSourceConfigWindow,
     ValidatorUpdateValidatorVolumeValidator,
     ValidatorUpdateValidatorVolumeValidatorConfig,
     ValidatorUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold,
     ValidatorUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    ValidatorUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     ValidatorUpdateValidatorVolumeValidatorDestination,
     ValidatorUpdateValidatorVolumeValidatorSourceConfig,
     ValidatorUpdateValidatorVolumeValidatorSourceConfigSegmentation,
     ValidatorUpdateValidatorVolumeValidatorSourceConfigSource,
     ValidatorUpdateValidatorVolumeValidatorSourceConfigWindow,
     WindowCreation,
     WindowCreationErrors,
@@ -868,15 +838,14 @@
     GetIncidentsIncidentsSchemaChangeNotification,
     GetIncidentsIncidentsSegmentLimitExceededNotification,
     GetIncidentsIncidentsSegmentLimitExceededNotificationSegmentation,
     GetIncidentsIncidentsValidatorThresholdFailureNotification,
     GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric,
     GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold,
     GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold,
-    GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold,
     GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment,
 )
 from .get_notification_rule_by_resource_name import (
     GetNotificationRuleByResourceName,
     GetNotificationRuleByResourceNameNotificationRuleByResourceName,
 )
 from .get_notification_rules import (
@@ -1099,79 +1068,72 @@
 from .get_users import GetUsers, GetUsersUsers
 from .get_validator import (
     GetValidator,
     GetValidatorValidatorCategoricalDistributionValidator,
     GetValidatorValidatorCategoricalDistributionValidatorConfig,
     GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfig,
     GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
     GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
     GetValidatorValidatorCategoricalDistributionValidatorSourceConfig,
     GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
     GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSource,
     GetValidatorValidatorCategoricalDistributionValidatorSourceConfigWindow,
     GetValidatorValidatorFreshnessValidator,
     GetValidatorValidatorFreshnessValidatorConfig,
     GetValidatorValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorFreshnessValidatorSourceConfig,
     GetValidatorValidatorFreshnessValidatorSourceConfigSegmentation,
     GetValidatorValidatorFreshnessValidatorSourceConfigSource,
     GetValidatorValidatorFreshnessValidatorSourceConfigWindow,
     GetValidatorValidatorNumericAnomalyValidator,
     GetValidatorValidatorNumericAnomalyValidatorConfig,
     GetValidatorValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorNumericAnomalyValidatorDestination,
     GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfig,
     GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
     GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
     GetValidatorValidatorNumericAnomalyValidatorSourceConfig,
     GetValidatorValidatorNumericAnomalyValidatorSourceConfigSegmentation,
     GetValidatorValidatorNumericAnomalyValidatorSourceConfigSource,
     GetValidatorValidatorNumericAnomalyValidatorSourceConfigWindow,
     GetValidatorValidatorNumericDistributionValidator,
     GetValidatorValidatorNumericDistributionValidatorConfig,
     GetValidatorValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfig,
     GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigSource,
     GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
     GetValidatorValidatorNumericDistributionValidatorSourceConfig,
     GetValidatorValidatorNumericDistributionValidatorSourceConfigSegmentation,
     GetValidatorValidatorNumericDistributionValidatorSourceConfigSource,
     GetValidatorValidatorNumericDistributionValidatorSourceConfigWindow,
     GetValidatorValidatorNumericValidator,
     GetValidatorValidatorNumericValidatorConfig,
     GetValidatorValidatorNumericValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorNumericValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorNumericValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorNumericValidatorSourceConfig,
     GetValidatorValidatorNumericValidatorSourceConfigSegmentation,
     GetValidatorValidatorNumericValidatorSourceConfigSource,
     GetValidatorValidatorNumericValidatorSourceConfigWindow,
     GetValidatorValidatorRelativeTimeValidator,
     GetValidatorValidatorRelativeTimeValidatorConfig,
     GetValidatorValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorRelativeTimeValidatorSourceConfig,
     GetValidatorValidatorRelativeTimeValidatorSourceConfigSegmentation,
     GetValidatorValidatorRelativeTimeValidatorSourceConfigSource,
     GetValidatorValidatorRelativeTimeValidatorSourceConfigWindow,
     GetValidatorValidatorRelativeVolumeValidator,
     GetValidatorValidatorRelativeVolumeValidatorConfig,
     GetValidatorValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfig,
     GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
     GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
     GetValidatorValidatorRelativeVolumeValidatorSourceConfig,
     GetValidatorValidatorRelativeVolumeValidatorSourceConfigSegmentation,
     GetValidatorValidatorRelativeVolumeValidatorSourceConfigSource,
     GetValidatorValidatorRelativeVolumeValidatorSourceConfigWindow,
@@ -1180,92 +1142,84 @@
     GetValidatorValidatorValidatorSourceConfigSegmentation,
     GetValidatorValidatorValidatorSourceConfigSource,
     GetValidatorValidatorValidatorSourceConfigWindow,
     GetValidatorValidatorVolumeValidator,
     GetValidatorValidatorVolumeValidatorConfig,
     GetValidatorValidatorVolumeValidatorConfigThresholdDynamicThreshold,
     GetValidatorValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    GetValidatorValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorValidatorVolumeValidatorDestination,
     GetValidatorValidatorVolumeValidatorSourceConfig,
     GetValidatorValidatorVolumeValidatorSourceConfigSegmentation,
     GetValidatorValidatorVolumeValidatorSourceConfigSource,
     GetValidatorValidatorVolumeValidatorSourceConfigWindow,
 )
 from .get_validator_by_resource_name import (
     GetValidatorByResourceName,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidator,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidator,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidator,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorDestination,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidator,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidator,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidator,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidator,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigWindow,
@@ -1274,15 +1228,14 @@
     GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigWindow,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidator,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfig,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdDynamicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdFixedThreshold,
-    GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdMonotonicThreshold,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorDestination,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfig,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigWindow,
 )
 from .get_validator_incidents import (
@@ -1295,16 +1248,14 @@
 )
 from .get_validator_segment_metrics import (
     GetValidatorSegmentMetrics,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistoryValues,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistoryValues,
-    GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistory,
-    GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistoryValues,
 )
 from .get_window_by_resource_name import (
     GetWindowByResourceName,
     GetWindowByResourceNameWindowByResourceNameFixedBatchWindow,
     GetWindowByResourceNameWindowByResourceNameFixedBatchWindowConfig,
     GetWindowByResourceNameWindowByResourceNameFixedBatchWindowSource,
     GetWindowByResourceNameWindowByResourceNameSessionizedWindow,
@@ -1390,15 +1341,14 @@
     KafkaSaslSSLPlainCredentialUpdateInput,
     KafkaSourceCreateInput,
     KafkaSourceUpdateInput,
     KafkaSSLCredentialCreateInput,
     KafkaSSLCredentialSecretChangedInput,
     KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
-    MonotonicThresholdCreateInput,
     NotificationRuleCreateInput,
     NotificationRuleDeleteInput,
     NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
     NumericDistributionValidatorCreateInput,
     NumericDistributionValidatorUpdateInput,
@@ -1446,15 +1396,14 @@
     ValidatorIncidentsInput,
     ValidatorRecommendationApplyInput,
     ValidatorRecommendationDismissInput,
     ValidatorSegmentIncidentsInput,
     ValidatorSegmentMetricsInput,
     ValidatorWithDynamicThresholdUpdateInput,
     ValidatorWithFixedThresholdUpdateInput,
-    ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
 from .kafka_sasl_ssl_plain_credential_secret_changed import (
     KafkaSaslSslPlainCredentialSecretChanged,
@@ -1563,79 +1512,72 @@
 )
 from .list_validators import (
     ListValidators,
     ListValidatorsValidatorsListCategoricalDistributionValidator,
     ListValidatorsValidatorsListCategoricalDistributionValidatorConfig,
     ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfig,
     ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigSource,
     ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigWindow,
     ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfig,
     ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSource,
     ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigWindow,
     ListValidatorsValidatorsListFreshnessValidator,
     ListValidatorsValidatorsListFreshnessValidatorConfig,
     ListValidatorsValidatorsListFreshnessValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListFreshnessValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListFreshnessValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListFreshnessValidatorSourceConfig,
     ListValidatorsValidatorsListFreshnessValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListFreshnessValidatorSourceConfigSource,
     ListValidatorsValidatorsListFreshnessValidatorSourceConfigWindow,
     ListValidatorsValidatorsListNumericAnomalyValidator,
     ListValidatorsValidatorsListNumericAnomalyValidatorConfig,
     ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListNumericAnomalyValidatorDestination,
     ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfig,
     ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigSource,
     ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigWindow,
     ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfig,
     ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSource,
     ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigWindow,
     ListValidatorsValidatorsListNumericDistributionValidator,
     ListValidatorsValidatorsListNumericDistributionValidatorConfig,
     ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfig,
     ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigSource,
     ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigWindow,
     ListValidatorsValidatorsListNumericDistributionValidatorSourceConfig,
     ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSource,
     ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigWindow,
     ListValidatorsValidatorsListNumericValidator,
     ListValidatorsValidatorsListNumericValidatorConfig,
     ListValidatorsValidatorsListNumericValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListNumericValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListNumericValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListNumericValidatorSourceConfig,
     ListValidatorsValidatorsListNumericValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListNumericValidatorSourceConfigSource,
     ListValidatorsValidatorsListNumericValidatorSourceConfigWindow,
     ListValidatorsValidatorsListRelativeTimeValidator,
     ListValidatorsValidatorsListRelativeTimeValidatorConfig,
     ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListRelativeTimeValidatorSourceConfig,
     ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSource,
     ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigWindow,
     ListValidatorsValidatorsListRelativeVolumeValidator,
     ListValidatorsValidatorsListRelativeVolumeValidatorConfig,
     ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfig,
     ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigSource,
     ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigWindow,
     ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfig,
     ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSource,
     ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigWindow,
@@ -1644,15 +1586,14 @@
     ListValidatorsValidatorsListValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListValidatorSourceConfigSource,
     ListValidatorsValidatorsListValidatorSourceConfigWindow,
     ListValidatorsValidatorsListVolumeValidator,
     ListValidatorsValidatorsListVolumeValidatorConfig,
     ListValidatorsValidatorsListVolumeValidatorConfigThresholdDynamicThreshold,
     ListValidatorsValidatorsListVolumeValidatorConfigThresholdFixedThreshold,
-    ListValidatorsValidatorsListVolumeValidatorConfigThresholdMonotonicThreshold,
     ListValidatorsValidatorsListVolumeValidatorDestination,
     ListValidatorsValidatorsListVolumeValidatorSourceConfig,
     ListValidatorsValidatorsListVolumeValidatorSourceConfigSegmentation,
     ListValidatorsValidatorsListVolumeValidatorSourceConfigSource,
     ListValidatorsValidatorsListVolumeValidatorSourceConfigWindow,
 )
 from .list_windows import (
@@ -1867,79 +1808,72 @@
     UpdateValidatorWithDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateErrors,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorDestination,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow,
@@ -1948,94 +1882,86 @@
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigWindow,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorDestination,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSource,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow,
 )
 from .update_validator_with_fixed_threshold import (
     UpdateValidatorWithFixedThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdate,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateErrors,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorDestination,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow,
@@ -2044,117 +1970,20 @@
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigWindow,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidator,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorDestination,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfig,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSource,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigWindow,
 )
-from .update_validator_with_monotonic_threshold import (
-    UpdateValidatorWithMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdate,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateErrors,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorDestination,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigWindow,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidator,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorDestination,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfig,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSource,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow,
-)
 from .update_volume_validator import (
     UpdateVolumeValidator,
     UpdateVolumeValidatorVolumeValidatorUpdate,
 )
 from .update_webhook_channel import (
     UpdateWebhookChannel,
     UpdateWebhookChannelWebhookChannelUpdate,
@@ -2278,32 +2107,26 @@
     "CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate",
     "CreateNumericAnomalyValidatorWithFixedThreshold",
     "CreateNumericAnomalyValidatorWithFixedThresholdNumericAnomalyValidatorWithFixedThresholdCreate",
     "CreateNumericDistributionValidatorWithDynamicThreshold",
     "CreateNumericDistributionValidatorWithDynamicThresholdNumericDistributionValidatorWithDynamicThresholdCreate",
     "CreateNumericDistributionValidatorWithFixedThreshold",
     "CreateNumericDistributionValidatorWithFixedThresholdNumericDistributionValidatorWithFixedThresholdCreate",
-    "CreateNumericDistributionValidatorWithMonotonicThreshold",
-    "CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate",
     "CreateNumericValidatorWithDynamicThreshold",
     "CreateNumericValidatorWithDynamicThresholdNumericValidatorWithDynamicThresholdCreate",
     "CreateNumericValidatorWithFixedThreshold",
     "CreateNumericValidatorWithFixedThresholdNumericValidatorWithFixedThresholdCreate",
-    "CreateNumericValidatorWithMonotonicThreshold",
-    "CreateNumericValidatorWithMonotonicThresholdNumericValidatorWithMonotonicThresholdCreate",
     "CreatePostgreSqlCredential",
     "CreatePostgreSqlCredentialPostgreSqlCredentialCreate",
     "CreatePostgreSqlSource",
     "CreatePostgreSqlSourcePostgreSqlSourceCreate",
     "CreateRelativeTimeValidatorWithDynamicThreshold",
     "CreateRelativeTimeValidatorWithDynamicThresholdRelativeTimeValidatorWithDynamicThresholdCreate",
     "CreateRelativeTimeValidatorWithFixedThreshold",
     "CreateRelativeTimeValidatorWithFixedThresholdRelativeTimeValidatorWithFixedThresholdCreate",
-    "CreateRelativeTimeValidatorWithMonotonicThreshold",
-    "CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate",
     "CreateRelativeVolumeValidatorWithDynamicThreshold",
     "CreateRelativeVolumeValidatorWithDynamicThresholdRelativeVolumeValidatorWithDynamicThresholdCreate",
     "CreateRelativeVolumeValidatorWithFixedThreshold",
     "CreateRelativeVolumeValidatorWithFixedThresholdRelativeVolumeValidatorWithFixedThresholdCreate",
     "CreateSamlIdentityProvider",
     "CreateSamlIdentityProviderSamlIdentityProviderCreate",
     "CreateSegmentation",
@@ -2402,15 +2225,14 @@
     "DeleteValidatorsValidatorsDeleteErrors",
     "DeleteWindow",
     "DeleteWindowWindowsDelete",
     "DeleteWindowWindowsDeleteErrors",
     "DeleteWindows",
     "DeleteWindowsWindowsDelete",
     "DeleteWindowsWindowsDeleteErrors",
-    "DeletedEntity",
     "DemoCredentialCreateInput",
     "DemoSourceCreateInput",
     "DestinationCreation",
     "DestinationCreationDestinationAwsKinesisDestination",
     "DestinationCreationDestinationAwsKinesisDestinationConfig",
     "DestinationCreationDestinationAwsKinesisDestinationCredential",
     "DestinationCreationDestinationDestination",
@@ -2518,15 +2340,14 @@
     "GetIncidentsIncidentsSchemaChangeNotification",
     "GetIncidentsIncidentsSegmentLimitExceededNotification",
     "GetIncidentsIncidentsSegmentLimitExceededNotificationSegmentation",
     "GetIncidentsIncidentsValidatorThresholdFailureNotification",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold",
-    "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment",
     "GetNotificationRuleByResourceName",
     "GetNotificationRuleByResourceNameNotificationRuleByResourceName",
     "GetNotificationRules",
     "GetNotificationRulesNotificationRules",
     "GetRecommendation",
     "GetRecommendationRecommendationRecommendation",
@@ -2730,79 +2551,72 @@
     "GetUsersUsers",
     "GetValidator",
     "GetValidatorByResourceName",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidator",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidator",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidator",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorDestination",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidator",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidator",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidator",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidator",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigWindow",
@@ -2811,100 +2625,90 @@
     "GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameValidatorSourceConfigWindow",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidator",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfig",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorDestination",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigWindow",
     "GetValidatorIncidents",
     "GetValidatorIncidentsValidatorIncidents",
     "GetValidatorSegmentIncidents",
     "GetValidatorSegmentIncidentsValidatorSegmentIncidents",
     "GetValidatorSegmentMetrics",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistoryValues",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistoryValues",
-    "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistory",
-    "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistoryValues",
     "GetValidatorValidatorCategoricalDistributionValidator",
     "GetValidatorValidatorCategoricalDistributionValidatorConfig",
     "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfig",
     "GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
     "GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "GetValidatorValidatorCategoricalDistributionValidatorSourceConfig",
     "GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
     "GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSource",
     "GetValidatorValidatorCategoricalDistributionValidatorSourceConfigWindow",
     "GetValidatorValidatorFreshnessValidator",
     "GetValidatorValidatorFreshnessValidatorConfig",
     "GetValidatorValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorFreshnessValidatorSourceConfig",
     "GetValidatorValidatorFreshnessValidatorSourceConfigSegmentation",
     "GetValidatorValidatorFreshnessValidatorSourceConfigSource",
     "GetValidatorValidatorFreshnessValidatorSourceConfigWindow",
     "GetValidatorValidatorNumericAnomalyValidator",
     "GetValidatorValidatorNumericAnomalyValidatorConfig",
     "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorNumericAnomalyValidatorDestination",
     "GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfig",
     "GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
     "GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
     "GetValidatorValidatorNumericAnomalyValidatorSourceConfig",
     "GetValidatorValidatorNumericAnomalyValidatorSourceConfigSegmentation",
     "GetValidatorValidatorNumericAnomalyValidatorSourceConfigSource",
     "GetValidatorValidatorNumericAnomalyValidatorSourceConfigWindow",
     "GetValidatorValidatorNumericDistributionValidator",
     "GetValidatorValidatorNumericDistributionValidatorConfig",
     "GetValidatorValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfig",
     "GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigSource",
     "GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
     "GetValidatorValidatorNumericDistributionValidatorSourceConfig",
     "GetValidatorValidatorNumericDistributionValidatorSourceConfigSegmentation",
     "GetValidatorValidatorNumericDistributionValidatorSourceConfigSource",
     "GetValidatorValidatorNumericDistributionValidatorSourceConfigWindow",
     "GetValidatorValidatorNumericValidator",
     "GetValidatorValidatorNumericValidatorConfig",
     "GetValidatorValidatorNumericValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorNumericValidatorSourceConfig",
     "GetValidatorValidatorNumericValidatorSourceConfigSegmentation",
     "GetValidatorValidatorNumericValidatorSourceConfigSource",
     "GetValidatorValidatorNumericValidatorSourceConfigWindow",
     "GetValidatorValidatorRelativeTimeValidator",
     "GetValidatorValidatorRelativeTimeValidatorConfig",
     "GetValidatorValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorRelativeTimeValidatorSourceConfig",
     "GetValidatorValidatorRelativeTimeValidatorSourceConfigSegmentation",
     "GetValidatorValidatorRelativeTimeValidatorSourceConfigSource",
     "GetValidatorValidatorRelativeTimeValidatorSourceConfigWindow",
     "GetValidatorValidatorRelativeVolumeValidator",
     "GetValidatorValidatorRelativeVolumeValidatorConfig",
     "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfig",
     "GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
     "GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
     "GetValidatorValidatorRelativeVolumeValidatorSourceConfig",
     "GetValidatorValidatorRelativeVolumeValidatorSourceConfigSegmentation",
     "GetValidatorValidatorRelativeVolumeValidatorSourceConfigSource",
     "GetValidatorValidatorRelativeVolumeValidatorSourceConfigWindow",
@@ -2913,15 +2717,14 @@
     "GetValidatorValidatorValidatorSourceConfigSegmentation",
     "GetValidatorValidatorValidatorSourceConfigSource",
     "GetValidatorValidatorValidatorSourceConfigWindow",
     "GetValidatorValidatorVolumeValidator",
     "GetValidatorValidatorVolumeValidatorConfig",
     "GetValidatorValidatorVolumeValidatorConfigThresholdDynamicThreshold",
     "GetValidatorValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "GetValidatorValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "GetValidatorValidatorVolumeValidatorDestination",
     "GetValidatorValidatorVolumeValidatorSourceConfig",
     "GetValidatorValidatorVolumeValidatorSourceConfigSegmentation",
     "GetValidatorValidatorVolumeValidatorSourceConfigSource",
     "GetValidatorValidatorVolumeValidatorSourceConfigWindow",
     "GetWindowByResourceName",
     "GetWindowByResourceNameWindowByResourceNameFixedBatchWindow",
@@ -3079,79 +2882,72 @@
     "ListSourcesSourcesListSourceSegmentations",
     "ListSourcesSourcesListSourceWindows",
     "ListValidators",
     "ListValidatorsValidatorsListCategoricalDistributionValidator",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorConfig",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfig",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigSource",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfig",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSource",
     "ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListFreshnessValidator",
     "ListValidatorsValidatorsListFreshnessValidatorConfig",
     "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListFreshnessValidatorSourceConfig",
     "ListValidatorsValidatorsListFreshnessValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListFreshnessValidatorSourceConfigSource",
     "ListValidatorsValidatorsListFreshnessValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListNumericAnomalyValidator",
     "ListValidatorsValidatorsListNumericAnomalyValidatorConfig",
     "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListNumericAnomalyValidatorDestination",
     "ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfig",
     "ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigSource",
     "ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigWindow",
     "ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfig",
     "ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSource",
     "ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListNumericDistributionValidator",
     "ListValidatorsValidatorsListNumericDistributionValidatorConfig",
     "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfig",
     "ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigSource",
     "ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigWindow",
     "ListValidatorsValidatorsListNumericDistributionValidatorSourceConfig",
     "ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSource",
     "ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListNumericValidator",
     "ListValidatorsValidatorsListNumericValidatorConfig",
     "ListValidatorsValidatorsListNumericValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListNumericValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListNumericValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListNumericValidatorSourceConfig",
     "ListValidatorsValidatorsListNumericValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListNumericValidatorSourceConfigSource",
     "ListValidatorsValidatorsListNumericValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListRelativeTimeValidator",
     "ListValidatorsValidatorsListRelativeTimeValidatorConfig",
     "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListRelativeTimeValidatorSourceConfig",
     "ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSource",
     "ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListRelativeVolumeValidator",
     "ListValidatorsValidatorsListRelativeVolumeValidatorConfig",
     "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfig",
     "ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigSource",
     "ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigWindow",
     "ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfig",
     "ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSource",
     "ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigWindow",
@@ -3160,15 +2956,14 @@
     "ListValidatorsValidatorsListValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListValidatorSourceConfigSource",
     "ListValidatorsValidatorsListValidatorSourceConfigWindow",
     "ListValidatorsValidatorsListVolumeValidator",
     "ListValidatorsValidatorsListVolumeValidatorConfig",
     "ListValidatorsValidatorsListVolumeValidatorConfigThresholdDynamicThreshold",
     "ListValidatorsValidatorsListVolumeValidatorConfigThresholdFixedThreshold",
-    "ListValidatorsValidatorsListVolumeValidatorConfigThresholdMonotonicThreshold",
     "ListValidatorsValidatorsListVolumeValidatorDestination",
     "ListValidatorsValidatorsListVolumeValidatorSourceConfig",
     "ListValidatorsValidatorsListVolumeValidatorSourceConfigSegmentation",
     "ListValidatorsValidatorsListVolumeValidatorSourceConfigSource",
     "ListValidatorsValidatorsListVolumeValidatorSourceConfigWindow",
     "ListWindows",
     "ListWindowsWindowsListFixedBatchWindow",
@@ -3179,15 +2974,14 @@
     "ListWindowsWindowsListSessionizedWindowSource",
     "ListWindowsWindowsListTumblingWindow",
     "ListWindowsWindowsListTumblingWindowConfig",
     "ListWindowsWindowsListTumblingWindowSource",
     "ListWindowsWindowsListWindow",
     "ListWindowsWindowsListWindowSource",
     "LocalIdentityProviderUpdateInput",
-    "MonotonicThresholdCreateInput",
     "NamespaceUpdate",
     "NamespaceUpdateErrors",
     "NotificationRuleCreateInput",
     "NotificationRuleCreation",
     "NotificationRuleCreationErrors",
     "NotificationRuleCreationNotificationRule",
     "NotificationRuleDeleteInput",
@@ -3501,79 +3295,72 @@
     "UpdateValidatorWithDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateErrors",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorDestination",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow",
@@ -3582,92 +3369,84 @@
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorValidatorSourceConfigWindow",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorDestination",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSource",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdate",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateErrors",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorDestination",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow",
@@ -3676,114 +3455,19 @@
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorValidatorSourceConfigWindow",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidator",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorDestination",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfig",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSource",
     "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdate",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateErrors",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorDestination",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorNumericValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorValidatorSourceConfigWindow",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidator",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorDestination",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfig",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSource",
-    "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow",
     "UpdateVolumeValidator",
     "UpdateVolumeValidatorVolumeValidatorUpdate",
     "UpdateWebhookChannel",
     "UpdateWebhookChannelWebhookChannelUpdate",
     "UpdateWindowNamespace",
     "UpdateWindowNamespaceWindowNamespaceUpdate",
     "UserCreateInput",
@@ -3807,79 +3491,72 @@
     "UserUpdateUser",
     "ValidatorCreation",
     "ValidatorCreationErrors",
     "ValidatorCreationValidatorCategoricalDistributionValidator",
     "ValidatorCreationValidatorCategoricalDistributionValidatorConfig",
     "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfig",
     "ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
     "ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfig",
     "ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSource",
     "ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigWindow",
     "ValidatorCreationValidatorFreshnessValidator",
     "ValidatorCreationValidatorFreshnessValidatorConfig",
     "ValidatorCreationValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorFreshnessValidatorSourceConfig",
     "ValidatorCreationValidatorFreshnessValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorFreshnessValidatorSourceConfigSource",
     "ValidatorCreationValidatorFreshnessValidatorSourceConfigWindow",
     "ValidatorCreationValidatorNumericAnomalyValidator",
     "ValidatorCreationValidatorNumericAnomalyValidatorConfig",
     "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorNumericAnomalyValidatorDestination",
     "ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfig",
     "ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
     "ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
     "ValidatorCreationValidatorNumericAnomalyValidatorSourceConfig",
     "ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSource",
     "ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigWindow",
     "ValidatorCreationValidatorNumericDistributionValidator",
     "ValidatorCreationValidatorNumericDistributionValidatorConfig",
     "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfig",
     "ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigSource",
     "ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
     "ValidatorCreationValidatorNumericDistributionValidatorSourceConfig",
     "ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSource",
     "ValidatorCreationValidatorNumericDistributionValidatorSourceConfigWindow",
     "ValidatorCreationValidatorNumericValidator",
     "ValidatorCreationValidatorNumericValidatorConfig",
     "ValidatorCreationValidatorNumericValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorNumericValidatorSourceConfig",
     "ValidatorCreationValidatorNumericValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorNumericValidatorSourceConfigSource",
     "ValidatorCreationValidatorNumericValidatorSourceConfigWindow",
     "ValidatorCreationValidatorRelativeTimeValidator",
     "ValidatorCreationValidatorRelativeTimeValidatorConfig",
     "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorRelativeTimeValidatorSourceConfig",
     "ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSource",
     "ValidatorCreationValidatorRelativeTimeValidatorSourceConfigWindow",
     "ValidatorCreationValidatorRelativeVolumeValidator",
     "ValidatorCreationValidatorRelativeVolumeValidatorConfig",
     "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfig",
     "ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
     "ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
     "ValidatorCreationValidatorRelativeVolumeValidatorSourceConfig",
     "ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSource",
     "ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigWindow",
@@ -3888,26 +3565,24 @@
     "ValidatorCreationValidatorValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorValidatorSourceConfigSource",
     "ValidatorCreationValidatorValidatorSourceConfigWindow",
     "ValidatorCreationValidatorVolumeValidator",
     "ValidatorCreationValidatorVolumeValidatorConfig",
     "ValidatorCreationValidatorVolumeValidatorConfigThresholdDynamicThreshold",
     "ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorVolumeValidatorDestination",
     "ValidatorCreationValidatorVolumeValidatorSourceConfig",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigSource",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigWindow",
     "ValidatorIncidents",
     "ValidatorIncidentsInput",
     "ValidatorIncidentsMetricValidatorMetric",
     "ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold",
     "ValidatorIncidentsMetricValidatorMetricWithFixedThreshold",
-    "ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold",
     "ValidatorIncidentsSegment",
     "ValidatorRecommendationApplication",
     "ValidatorRecommendationApplyInput",
     "ValidatorRecommendationDismissInput",
     "ValidatorRecommendationDismissal",
     "ValidatorRecommendationDismissalErrors",
     "ValidatorSegmentIncidentsInput",
@@ -3915,79 +3590,72 @@
     "ValidatorState",
     "ValidatorUpdate",
     "ValidatorUpdateErrors",
     "ValidatorUpdateValidatorCategoricalDistributionValidator",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorConfig",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfig",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSource",
     "ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorFreshnessValidator",
     "ValidatorUpdateValidatorFreshnessValidatorConfig",
     "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorFreshnessValidatorSourceConfig",
     "ValidatorUpdateValidatorFreshnessValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorFreshnessValidatorSourceConfigSource",
     "ValidatorUpdateValidatorFreshnessValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorNumericAnomalyValidator",
     "ValidatorUpdateValidatorNumericAnomalyValidatorConfig",
     "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorNumericAnomalyValidatorDestination",
     "ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig",
     "ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource",
     "ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow",
     "ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfig",
     "ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSource",
     "ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorNumericDistributionValidator",
     "ValidatorUpdateValidatorNumericDistributionValidatorConfig",
     "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfig",
     "ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource",
     "ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow",
     "ValidatorUpdateValidatorNumericDistributionValidatorSourceConfig",
     "ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSource",
     "ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorNumericValidator",
     "ValidatorUpdateValidatorNumericValidatorConfig",
     "ValidatorUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorNumericValidatorSourceConfig",
     "ValidatorUpdateValidatorNumericValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorNumericValidatorSourceConfigSource",
     "ValidatorUpdateValidatorNumericValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorRelativeTimeValidator",
     "ValidatorUpdateValidatorRelativeTimeValidatorConfig",
     "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorRelativeTimeValidatorSourceConfig",
     "ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSource",
     "ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorRelativeVolumeValidator",
     "ValidatorUpdateValidatorRelativeVolumeValidatorConfig",
     "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig",
     "ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource",
     "ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow",
     "ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfig",
     "ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSource",
     "ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigWindow",
@@ -3996,23 +3664,21 @@
     "ValidatorUpdateValidatorValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorValidatorSourceConfigSource",
     "ValidatorUpdateValidatorValidatorSourceConfigWindow",
     "ValidatorUpdateValidatorVolumeValidator",
     "ValidatorUpdateValidatorVolumeValidatorConfig",
     "ValidatorUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
     "ValidatorUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-    "ValidatorUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorUpdateValidatorVolumeValidatorDestination",
     "ValidatorUpdateValidatorVolumeValidatorSourceConfig",
     "ValidatorUpdateValidatorVolumeValidatorSourceConfigSegmentation",
     "ValidatorUpdateValidatorVolumeValidatorSourceConfigSource",
     "ValidatorUpdateValidatorVolumeValidatorSourceConfigWindow",
     "ValidatorWithDynamicThresholdUpdateInput",
     "ValidatorWithFixedThresholdUpdateInput",
-    "ValidatorWithMonotonicThresholdUpdateInput",
     "VolumeMetric",
     "VolumeValidatorCreateInput",
     "VolumeValidatorUpdateInput",
     "WebhookChannelCreateInput",
     "WebhookChannelUpdateInput",
     "WindowCreation",
     "WindowCreationErrors",
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/client.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,30 +129,22 @@
     CreateNumericDistributionValidatorWithDynamicThreshold,
     CreateNumericDistributionValidatorWithDynamicThresholdNumericDistributionValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_distribution_validator_with_fixed_threshold import (
     CreateNumericDistributionValidatorWithFixedThreshold,
     CreateNumericDistributionValidatorWithFixedThresholdNumericDistributionValidatorWithFixedThresholdCreate,
 )
-from .create_numeric_distribution_validator_with_monotonic_threshold import (
-    CreateNumericDistributionValidatorWithMonotonicThreshold,
-    CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate,
-)
 from .create_numeric_validator_with_dynamic_threshold import (
     CreateNumericValidatorWithDynamicThreshold,
     CreateNumericValidatorWithDynamicThresholdNumericValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_validator_with_fixed_threshold import (
     CreateNumericValidatorWithFixedThreshold,
     CreateNumericValidatorWithFixedThresholdNumericValidatorWithFixedThresholdCreate,
 )
-from .create_numeric_validator_with_monotonic_threshold import (
-    CreateNumericValidatorWithMonotonicThreshold,
-    CreateNumericValidatorWithMonotonicThresholdNumericValidatorWithMonotonicThresholdCreate,
-)
 from .create_postgre_sql_credential import (
     CreatePostgreSqlCredential,
     CreatePostgreSqlCredentialPostgreSqlCredentialCreate,
 )
 from .create_postgre_sql_source import (
     CreatePostgreSqlSource,
     CreatePostgreSqlSourcePostgreSqlSourceCreate,
@@ -161,18 +153,14 @@
     CreateRelativeTimeValidatorWithDynamicThreshold,
     CreateRelativeTimeValidatorWithDynamicThresholdRelativeTimeValidatorWithDynamicThresholdCreate,
 )
 from .create_relative_time_validator_with_fixed_threshold import (
     CreateRelativeTimeValidatorWithFixedThreshold,
     CreateRelativeTimeValidatorWithFixedThresholdRelativeTimeValidatorWithFixedThresholdCreate,
 )
-from .create_relative_time_validator_with_monotonic_threshold import (
-    CreateRelativeTimeValidatorWithMonotonicThreshold,
-    CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate,
-)
 from .create_relative_volume_validator_with_dynamic_threshold import (
     CreateRelativeVolumeValidatorWithDynamicThreshold,
     CreateRelativeVolumeValidatorWithDynamicThresholdRelativeVolumeValidatorWithDynamicThresholdCreate,
 )
 from .create_relative_volume_validator_with_fixed_threshold import (
     CreateRelativeVolumeValidatorWithFixedThreshold,
     CreateRelativeVolumeValidatorWithFixedThresholdRelativeVolumeValidatorWithFixedThresholdCreate,
@@ -404,15 +392,14 @@
     GetValidatorSegmentIncidents,
     GetValidatorSegmentIncidentsValidatorSegmentIncidents,
 )
 from .get_validator_segment_metrics import (
     GetValidatorSegmentMetrics,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory,
-    GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistory,
 )
 from .get_window_by_resource_name import (
     GetWindowByResourceName,
     GetWindowByResourceNameWindowByResourceNameFixedBatchWindow,
     GetWindowByResourceNameWindowByResourceNameSessionizedWindow,
     GetWindowByResourceNameWindowByResourceNameTumblingWindow,
     GetWindowByResourceNameWindowByResourceNameWindow,
@@ -490,15 +477,14 @@
     KafkaSaslSSLPlainCredentialUpdateInput,
     KafkaSourceCreateInput,
     KafkaSourceUpdateInput,
     KafkaSSLCredentialCreateInput,
     KafkaSSLCredentialSecretChangedInput,
     KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
-    MonotonicThresholdCreateInput,
     NotificationRuleCreateInput,
     NotificationRuleDeleteInput,
     NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
     NumericDistributionValidatorCreateInput,
     NumericDistributionValidatorUpdateInput,
@@ -541,15 +527,14 @@
     ValidatorIncidentsInput,
     ValidatorRecommendationApplyInput,
     ValidatorRecommendationDismissInput,
     ValidatorSegmentIncidentsInput,
     ValidatorSegmentMetricsInput,
     ValidatorWithDynamicThresholdUpdateInput,
     ValidatorWithFixedThresholdUpdateInput,
-    ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
 from .kafka_sasl_ssl_plain_credential_secret_changed import (
     KafkaSaslSslPlainCredentialSecretChanged,
@@ -806,18 +791,14 @@
     UpdateValidatorWithDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate,
 )
 from .update_validator_with_fixed_threshold import (
     UpdateValidatorWithFixedThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdate,
 )
-from .update_validator_with_monotonic_threshold import (
-    UpdateValidatorWithMonotonicThreshold,
-    UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdate,
-)
 from .update_volume_validator import (
     UpdateVolumeValidator,
     UpdateVolumeValidatorVolumeValidatorUpdate,
 )
 from .update_webhook_channel import (
     UpdateWebhookChannel,
     UpdateWebhookChannelWebhookChannelUpdate,
@@ -1095,14 +1076,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -1156,14 +1138,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -1421,14 +1404,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -1482,14 +1466,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -1676,14 +1661,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -1737,14 +1723,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -1840,14 +1827,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -1901,14 +1889,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -2014,17 +2003,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -2036,17 +2022,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2075,17 +2058,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2114,17 +2094,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -2141,17 +2118,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -2191,17 +2165,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -2210,17 +2181,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -2232,17 +2200,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2341,17 +2306,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -2363,17 +2325,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2402,17 +2361,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2441,17 +2397,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -2468,17 +2421,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -2518,17 +2468,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -2537,17 +2484,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -2559,17 +2503,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -2747,14 +2688,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -2808,14 +2750,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -3057,17 +3000,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -3079,17 +3019,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3118,17 +3055,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3157,17 +3091,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -3184,17 +3115,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -3234,17 +3162,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -3253,17 +3178,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -3275,17 +3197,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3379,17 +3298,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -3401,17 +3317,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3440,17 +3353,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3479,17 +3389,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -3506,17 +3413,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -3556,17 +3460,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -3575,17 +3476,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -3597,17 +3495,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -3769,14 +3664,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -3830,14 +3726,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -4022,14 +3919,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -4083,14 +3981,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -4186,14 +4085,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -4247,14 +4147,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -4350,14 +4251,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -4411,14 +4313,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -4605,14 +4508,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -4666,14 +4570,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -4934,17 +4839,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -4956,17 +4858,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -4995,17 +4894,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5034,17 +4930,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -5061,17 +4954,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -5111,17 +5001,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -5130,17 +5017,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -5152,17 +5036,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5261,17 +5142,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -5283,17 +5161,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5322,17 +5197,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5361,17 +5233,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -5388,17 +5257,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -5438,17 +5304,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -5457,17 +5320,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -5479,17 +5339,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5588,17 +5445,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -5610,17 +5464,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5649,17 +5500,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5688,17 +5536,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -5715,17 +5560,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -5765,17 +5607,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -5784,17 +5623,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -5806,17 +5642,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5915,17 +5748,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -5937,17 +5767,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -5976,17 +5803,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6015,17 +5839,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -6042,17 +5863,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -6092,17 +5910,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -6111,17 +5926,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -6133,17 +5945,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6166,341 +5975,14 @@
         variables: dict[str, object] = {"input": input, "threshold": threshold}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateNumericDistributionValidatorWithFixedThreshold.parse_obj(
             data
         ).numeric_distribution_validator_with_fixed_threshold_create
 
-    async def create_numeric_distribution_validator_with_monotonic_threshold(
-        self,
-        input: NumericDistributionValidatorCreateInput,
-        threshold: MonotonicThresholdCreateInput,
-    ) -> CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate:
-        query = gql(
-            """
-            mutation CreateNumericDistributionValidatorWithMonotonicThreshold($input: NumericDistributionValidatorCreateInput!, $threshold: MonotonicThresholdCreateInput!) {
-              numericDistributionValidatorWithMonotonicThresholdCreate(
-                input: $input
-                threshold: $threshold
-              ) {
-                ...ValidatorCreation
-              }
-            }
-
-            fragment ErrorDetails on ApiError {
-              __typename
-              code
-              message
-            }
-
-            fragment ValidatorCreation on ValidatorCreateResult {
-              errors {
-                ...ErrorDetails
-              }
-              validator {
-                ...ValidatorDetails
-              }
-            }
-
-            fragment ValidatorDetails on Validator {
-              __typename
-              id
-              name
-              hasCustomName
-              createdAt
-              updatedAt
-              sourceConfig {
-                source {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                window {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                segmentation {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                filter
-              }
-              resourceName
-              resourceNamespace
-              ... on NumericValidator {
-                config {
-                  sourceField
-                  metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on CategoricalDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  categoricalDistributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on NumericDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  distributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on VolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  sourceFields
-                  volumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on NumericAnomalyValidator {
-                config {
-                  sourceField
-                  numericAnomalyMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                  referenceSourceField
-                  sensitivity
-                  minimumReferenceDatapoints
-                  minimumAbsoluteDifference
-                  minimumRelativeDifferencePercent
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on RelativeTimeValidator {
-                config {
-                  sourceFieldMinuend
-                  sourceFieldSubtrahend
-                  relativeTimeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on FreshnessValidator {
-                config {
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on RelativeVolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  optionalReferenceSourceField: referenceSourceField
-                  relativeVolumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"input": input, "threshold": threshold}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return CreateNumericDistributionValidatorWithMonotonicThreshold.parse_obj(
-            data
-        ).numeric_distribution_validator_with_monotonic_threshold_create
-
     async def create_numeric_validator_with_dynamic_threshold(
         self, input: NumericValidatorCreateInput, threshold: DynamicThresholdCreateInput
     ) -> CreateNumericValidatorWithDynamicThresholdNumericValidatorWithDynamicThresholdCreate:
         query = gql(
             """
             mutation CreateNumericValidatorWithDynamicThreshold($input: NumericValidatorCreateInput!, $threshold: DynamicThresholdCreateInput!) {
               numericValidatorWithDynamicThresholdCreate(input: $input, threshold: $threshold) {
@@ -6564,17 +6046,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -6586,17 +6065,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6625,17 +6101,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6664,17 +6137,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -6691,17 +6161,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -6741,17 +6208,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -6760,17 +6224,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -6782,17 +6243,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6886,17 +6344,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -6908,17 +6363,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6947,17 +6399,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -6986,17 +6435,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -7013,17 +6459,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -7063,17 +6506,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -7082,17 +6522,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -7104,17 +6541,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -7137,341 +6571,14 @@
         variables: dict[str, object] = {"input": input, "threshold": threshold}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateNumericValidatorWithFixedThreshold.parse_obj(
             data
         ).numeric_validator_with_fixed_threshold_create
 
-    async def create_numeric_validator_with_monotonic_threshold(
-        self,
-        input: NumericValidatorCreateInput,
-        threshold: MonotonicThresholdCreateInput,
-    ) -> CreateNumericValidatorWithMonotonicThresholdNumericValidatorWithMonotonicThresholdCreate:
-        query = gql(
-            """
-            mutation CreateNumericValidatorWithMonotonicThreshold($input: NumericValidatorCreateInput!, $threshold: MonotonicThresholdCreateInput!) {
-              numericValidatorWithMonotonicThresholdCreate(
-                input: $input
-                threshold: $threshold
-              ) {
-                ...ValidatorCreation
-              }
-            }
-
-            fragment ErrorDetails on ApiError {
-              __typename
-              code
-              message
-            }
-
-            fragment ValidatorCreation on ValidatorCreateResult {
-              errors {
-                ...ErrorDetails
-              }
-              validator {
-                ...ValidatorDetails
-              }
-            }
-
-            fragment ValidatorDetails on Validator {
-              __typename
-              id
-              name
-              hasCustomName
-              createdAt
-              updatedAt
-              sourceConfig {
-                source {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                window {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                segmentation {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                filter
-              }
-              resourceName
-              resourceNamespace
-              ... on NumericValidator {
-                config {
-                  sourceField
-                  metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on CategoricalDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  categoricalDistributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on NumericDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  distributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on VolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  sourceFields
-                  volumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on NumericAnomalyValidator {
-                config {
-                  sourceField
-                  numericAnomalyMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                  referenceSourceField
-                  sensitivity
-                  minimumReferenceDatapoints
-                  minimumAbsoluteDifference
-                  minimumRelativeDifferencePercent
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on RelativeTimeValidator {
-                config {
-                  sourceFieldMinuend
-                  sourceFieldSubtrahend
-                  relativeTimeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on FreshnessValidator {
-                config {
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on RelativeVolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  optionalReferenceSourceField: referenceSourceField
-                  relativeVolumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"input": input, "threshold": threshold}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return CreateNumericValidatorWithMonotonicThreshold.parse_obj(
-            data
-        ).numeric_validator_with_monotonic_threshold_create
-
     async def create_postgre_sql_credential(
         self, input: PostgreSqlCredentialCreateInput
     ) -> CreatePostgreSqlCredentialPostgreSqlCredentialCreate:
         query = gql(
             """
             mutation CreatePostgreSqlCredential($input: PostgreSqlCredentialCreateInput!) {
               postgreSqlCredentialCreate(input: $input) {
@@ -7619,14 +6726,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -7680,14 +6788,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -7793,17 +6902,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -7815,17 +6921,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -7854,17 +6957,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -7893,17 +6993,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -7920,17 +7017,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -7970,17 +7064,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -7989,17 +7080,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -8011,17 +7099,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8120,17 +7205,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -8142,17 +7224,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8181,17 +7260,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8220,17 +7296,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -8247,17 +7320,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -8297,17 +7367,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -8316,17 +7383,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -8338,17 +7402,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8371,341 +7432,14 @@
         variables: dict[str, object] = {"input": input, "threshold": threshold}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateRelativeTimeValidatorWithFixedThreshold.parse_obj(
             data
         ).relative_time_validator_with_fixed_threshold_create
 
-    async def create_relative_time_validator_with_monotonic_threshold(
-        self,
-        input: RelativeTimeValidatorCreateInput,
-        threshold: MonotonicThresholdCreateInput,
-    ) -> CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate:
-        query = gql(
-            """
-            mutation CreateRelativeTimeValidatorWithMonotonicThreshold($input: RelativeTimeValidatorCreateInput!, $threshold: MonotonicThresholdCreateInput!) {
-              relativeTimeValidatorWithMonotonicThresholdCreate(
-                input: $input
-                threshold: $threshold
-              ) {
-                ...ValidatorCreation
-              }
-            }
-
-            fragment ErrorDetails on ApiError {
-              __typename
-              code
-              message
-            }
-
-            fragment ValidatorCreation on ValidatorCreateResult {
-              errors {
-                ...ErrorDetails
-              }
-              validator {
-                ...ValidatorDetails
-              }
-            }
-
-            fragment ValidatorDetails on Validator {
-              __typename
-              id
-              name
-              hasCustomName
-              createdAt
-              updatedAt
-              sourceConfig {
-                source {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                window {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                segmentation {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                filter
-              }
-              resourceName
-              resourceNamespace
-              ... on NumericValidator {
-                config {
-                  sourceField
-                  metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on CategoricalDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  categoricalDistributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on NumericDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  distributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on VolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  sourceFields
-                  volumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on NumericAnomalyValidator {
-                config {
-                  sourceField
-                  numericAnomalyMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                  referenceSourceField
-                  sensitivity
-                  minimumReferenceDatapoints
-                  minimumAbsoluteDifference
-                  minimumRelativeDifferencePercent
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on RelativeTimeValidator {
-                config {
-                  sourceFieldMinuend
-                  sourceFieldSubtrahend
-                  relativeTimeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on FreshnessValidator {
-                config {
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on RelativeVolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  optionalReferenceSourceField: referenceSourceField
-                  relativeVolumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"input": input, "threshold": threshold}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return CreateRelativeTimeValidatorWithMonotonicThreshold.parse_obj(
-            data
-        ).relative_time_validator_with_monotonic_threshold_create
-
     async def create_relative_volume_validator_with_dynamic_threshold(
         self,
         input: RelativeVolumeValidatorCreateInput,
         threshold: DynamicThresholdCreateInput,
     ) -> CreateRelativeVolumeValidatorWithDynamicThresholdRelativeVolumeValidatorWithDynamicThresholdCreate:
         query = gql(
             """
@@ -8774,17 +7508,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -8796,17 +7527,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8835,17 +7563,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -8874,17 +7599,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -8901,17 +7623,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -8951,17 +7670,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -8970,17 +7686,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -8992,17 +7705,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -9101,17 +7811,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -9123,17 +7830,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -9162,17 +7866,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -9201,17 +7902,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -9228,17 +7926,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -9278,17 +7973,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -9297,17 +7989,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -9319,17 +8008,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -9796,14 +8482,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -9857,14 +8544,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -10095,17 +8783,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -10117,17 +8802,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10156,17 +8838,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10195,17 +8874,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -10222,17 +8898,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -10272,17 +8945,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -10291,17 +8961,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -10313,17 +8980,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10417,17 +9081,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -10439,17 +9100,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10478,17 +9136,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10517,17 +9172,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -10544,17 +9196,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -10594,17 +9243,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -10613,17 +9259,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -10635,17 +9278,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -10741,22 +9381,18 @@
 
             fragment ChannelDeletion on ChannelDeleteResult {
               errors {
                 code
                 message
               }
               channel {
-                ...DeletedEntity
+                id
+                name
               }
             }
-
-            fragment DeletedEntity on DeletedEntity {
-              id
-              name
-            }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return DeleteChannel.parse_obj(data).channel_delete
 
@@ -11617,17 +10253,14 @@
               }
               ... on ValidatorMetricWithDynamicThreshold {
                 lowerBound
                 upperBound
                 decisionBoundsType
                 isBurnIn
               }
-              ... on ValidatorMetricWithMonotonicThreshold {
-                operator
-              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetIncidents.parse_obj(data).incidents
@@ -11836,17 +10469,14 @@
               }
               ... on ValidatorMetricWithDynamicThreshold {
                 lowerBound
                 upperBound
                 decisionBoundsType
                 isBurnIn
               }
-              ... on ValidatorMetricWithMonotonicThreshold {
-                operator
-              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetSegmentIncidents.parse_obj(data).segment_incidents
@@ -11989,14 +10619,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -12050,14 +10681,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -12156,14 +10788,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -12217,14 +10850,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -12572,17 +11206,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -12594,17 +11225,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -12633,17 +11261,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -12672,17 +11297,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -12699,17 +11321,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -12749,17 +11368,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -12768,17 +11384,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -12790,17 +11403,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -12892,17 +11502,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -12914,17 +11521,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -12953,17 +11557,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -12992,17 +11593,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -13019,17 +11617,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -13069,17 +11664,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -13088,17 +11680,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -13110,17 +11699,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -13193,17 +11779,14 @@
               }
               ... on ValidatorMetricWithDynamicThreshold {
                 lowerBound
                 upperBound
                 decisionBoundsType
                 isBurnIn
               }
-              ... on ValidatorMetricWithMonotonicThreshold {
-                operator
-              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetValidatorIncidents.parse_obj(data).validator_incidents
@@ -13253,31 +11836,27 @@
               }
               ... on ValidatorMetricWithDynamicThreshold {
                 lowerBound
                 upperBound
                 decisionBoundsType
                 isBurnIn
               }
-              ... on ValidatorMetricWithMonotonicThreshold {
-                operator
-              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetValidatorSegmentIncidents.parse_obj(data).validator_segment_incidents
 
     async def get_validator_segment_metrics(
         self, input: ValidatorSegmentMetricsInput
     ) -> Union[
         GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory,
         GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory,
-        GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistory,
     ]:
         query = gql(
             """
             query GetValidatorSegmentMetrics($input: ValidatorSegmentMetricsInput!) {
               validatorSegmentMetrics(input: $input) {
                 __typename
                 ... on ValidatorMetricWithFixedThresholdHistory {
@@ -13286,19 +11865,14 @@
                   }
                 }
                 ... on ValidatorMetricWithDynamicThresholdHistory {
                   values {
                     ...ValidatorMetricDetails
                   }
                 }
-                ... on ValidatorMetricWithMonotonicThresholdHistory {
-                  values {
-                    ...ValidatorMetricDetails
-                  }
-                }
               }
             }
 
             fragment ValidatorMetricDetails on ValidatorMetric {
               __typename
               startTime
               endTime
@@ -13310,17 +11884,14 @@
               }
               ... on ValidatorMetricWithDynamicThreshold {
                 lowerBound
                 upperBound
                 decisionBoundsType
                 isBurnIn
               }
-              ... on ValidatorMetricWithMonotonicThreshold {
-                operator
-              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetValidatorSegmentMetrics.parse_obj(data).validator_segment_metrics
@@ -13876,14 +12447,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -13937,14 +12509,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -14042,17 +12615,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -14064,17 +12634,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -14103,17 +12670,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -14142,17 +12706,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -14169,17 +12730,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -14219,17 +12777,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -14238,17 +12793,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -14260,17 +12812,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -14666,14 +13215,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -14727,14 +13277,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -14991,14 +13542,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -15052,14 +13604,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -15245,14 +13798,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -15306,14 +13860,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -15409,14 +13964,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -15470,14 +14026,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -15578,17 +14135,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -15600,17 +14154,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -15639,17 +14190,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -15678,17 +14226,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -15705,17 +14250,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -15755,17 +14297,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -15774,17 +14313,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -15796,17 +14332,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -16061,17 +14594,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -16083,17 +14613,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -16122,17 +14649,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -16161,17 +14685,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -16188,17 +14709,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -16238,17 +14756,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -16257,17 +14772,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -16279,17 +14791,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -16449,14 +14958,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -16510,14 +15020,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -16701,14 +15212,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -16762,14 +15274,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -16865,14 +15378,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -16926,14 +15440,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -17029,14 +15544,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -17090,14 +15606,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -17316,14 +15833,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -17377,14 +15895,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -17719,17 +16238,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -17741,17 +16257,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -17780,17 +16293,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -17819,17 +16329,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -17846,17 +16353,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -17896,17 +16400,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -17915,17 +16416,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -17937,17 +16435,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18041,17 +16536,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -18063,17 +16555,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18102,17 +16591,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18141,17 +16627,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -18168,17 +16651,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -18218,17 +16698,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -18237,17 +16714,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -18259,17 +16733,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18363,17 +16834,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -18385,17 +16853,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18424,17 +16889,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18463,17 +16925,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -18490,17 +16949,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -18540,17 +16996,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -18559,17 +17012,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -18581,17 +17031,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18766,14 +17213,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -18827,14 +17275,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -18935,17 +17384,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -18957,17 +17403,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -18996,17 +17439,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -19035,17 +17475,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -19062,17 +17499,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -19112,17 +17546,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -19131,17 +17562,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -19153,17 +17581,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -19257,17 +17682,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -19279,17 +17701,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -19318,17 +17737,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -19357,17 +17773,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -19384,17 +17797,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -19434,17 +17844,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -19453,17 +17860,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -19475,17 +17879,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -19928,14 +18329,15 @@
                   folder
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on GcpBigQuerySource {
                 config {
                   project
                   dataset
                   table
@@ -19989,14 +18391,15 @@
                   prefix
                   csv {
                     nullMarker
                     delimiter
                   }
                   schedule
                   filePattern
+                  fileFormat
                 }
               }
               ... on PostgreSqlSource {
                 config {
                   database
                   schema
                   table
@@ -20325,17 +18728,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -20347,17 +18747,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20386,17 +18783,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20425,17 +18819,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -20452,17 +18843,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -20502,17 +18890,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -20521,17 +18906,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -20543,17 +18925,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20643,17 +19022,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -20665,17 +19041,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20704,17 +19077,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20743,17 +19113,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -20770,17 +19137,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -20820,17 +19184,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -20839,17 +19200,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -20861,17 +19219,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -20894,332 +19249,14 @@
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateValidatorWithFixedThreshold.parse_obj(
             data
         ).validator_with_fixed_threshold_update
 
-    async def update_validator_with_monotonic_threshold(
-        self, input: ValidatorWithMonotonicThresholdUpdateInput
-    ) -> UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdate:
-        query = gql(
-            """
-            mutation UpdateValidatorWithMonotonicThreshold($input: ValidatorWithMonotonicThresholdUpdateInput!) {
-              validatorWithMonotonicThresholdUpdate(input: $input) {
-                errors {
-                  ...ErrorDetails
-                }
-                validator {
-                  ...ValidatorDetails
-                }
-              }
-            }
-
-            fragment ErrorDetails on ApiError {
-              __typename
-              code
-              message
-            }
-
-            fragment ValidatorDetails on Validator {
-              __typename
-              id
-              name
-              hasCustomName
-              createdAt
-              updatedAt
-              sourceConfig {
-                source {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                window {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                segmentation {
-                  id
-                  name
-                  resourceName
-                  resourceNamespace
-                }
-                filter
-              }
-              resourceName
-              resourceNamespace
-              ... on NumericValidator {
-                config {
-                  sourceField
-                  metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on CategoricalDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  categoricalDistributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on NumericDistributionValidator {
-                config {
-                  sourceField
-                  referenceSourceField
-                  distributionMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-              ... on VolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  sourceFields
-                  volumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on NumericAnomalyValidator {
-                config {
-                  sourceField
-                  numericAnomalyMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                  referenceSourceField
-                  sensitivity
-                  minimumReferenceDatapoints
-                  minimumAbsoluteDifference
-                  minimumRelativeDifferencePercent
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-                destination {
-                  name
-                  id
-                  resourceName
-                  resourceNamespace
-                }
-              }
-              ... on RelativeTimeValidator {
-                config {
-                  sourceFieldMinuend
-                  sourceFieldSubtrahend
-                  relativeTimeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on FreshnessValidator {
-                config {
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-              }
-              ... on RelativeVolumeValidator {
-                config {
-                  optionalSourceField: sourceField
-                  optionalReferenceSourceField: referenceSourceField
-                  relativeVolumeMetric: metric
-                  initializeWithBackfill
-                  threshold {
-                    __typename
-                    ... on FixedThreshold {
-                      operator
-                      value
-                    }
-                    ... on DynamicThreshold {
-                      sensitivity
-                      decisionBoundsType
-                    }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
-                  }
-                }
-                referenceSourceConfig {
-                  source {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  window {
-                    id
-                    name
-                    resourceName
-                    resourceNamespace
-                  }
-                  history
-                  offset
-                  filter
-                }
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {"input": input}
-        response = await self.execute(query=query, variables=variables)
-        data = self.get_data(response)
-        return UpdateValidatorWithMonotonicThreshold.parse_obj(
-            data
-        ).validator_with_monotonic_threshold_update
-
     async def update_volume_validator(
         self, input: VolumeValidatorUpdateInput
     ) -> UpdateVolumeValidatorVolumeValidatorUpdate:
         query = gql(
             """
             mutation UpdateVolumeValidator($input: VolumeValidatorUpdateInput!) {
               volumeValidatorUpdate(input: $input) {
@@ -21274,17 +19311,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on CategoricalDistributionValidator {
                 config {
                   sourceField
                   referenceSourceField
@@ -21296,17 +19330,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -21335,17 +19366,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
@@ -21374,17 +19402,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 destination {
                   name
                   id
                   resourceName
                   resourceNamespace
@@ -21401,17 +19426,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                   referenceSourceField
                   sensitivity
                   minimumReferenceDatapoints
                   minimumAbsoluteDifference
                   minimumRelativeDifferencePercent
                 }
@@ -21451,17 +19473,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on FreshnessValidator {
                 config {
                   initializeWithBackfill
                   threshold {
@@ -21470,17 +19489,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
               }
               ... on RelativeVolumeValidator {
                 config {
                   optionalSourceField: sourceField
                   optionalReferenceSourceField: referenceSourceField
@@ -21492,17 +19508,14 @@
                       operator
                       value
                     }
                     ... on DynamicThreshold {
                       sensitivity
                       decisionBoundsType
                     }
-                    ... on MonotonicThreshold {
-                      operator
-                    }
                   }
                 }
                 referenceSourceConfig {
                   source {
                     id
                     name
                     resourceName
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_kafka_sasl_ssl_plain_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_kafka_sasl_ssl_plain_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import ValidatorCreation
+from .fragments import ValidatorUpdate
 
 
-class CreateNumericDistributionValidatorWithMonotonicThreshold(BaseModel):
-    numeric_distribution_validator_with_monotonic_threshold_create: "CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate" = Field(
-        alias="numericDistributionValidatorWithMonotonicThresholdCreate"
+class UpdateNumericDistributionValidator(BaseModel):
+    numeric_distribution_validator_update: "UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate" = Field(
+        alias="numericDistributionValidatorUpdate"
     )
 
 
-class CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate(
-    ValidatorCreation
+class UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate(
+    ValidatorUpdate
 ):
     pass
 
 
-CreateNumericDistributionValidatorWithMonotonicThreshold.update_forward_refs()
-CreateNumericDistributionValidatorWithMonotonicThresholdNumericDistributionValidatorWithMonotonicThresholdCreate.update_forward_refs()
+UpdateNumericDistributionValidator.update_forward_refs()
+UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import ValidatorCreation
+from .fragments import ValidatorUpdate
 
 
-class CreateRelativeTimeValidatorWithMonotonicThreshold(BaseModel):
-    relative_time_validator_with_monotonic_threshold_create: "CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate" = Field(
-        alias="relativeTimeValidatorWithMonotonicThresholdCreate"
+class UpdateRelativeTimeValidator(BaseModel):
+    relative_time_validator_update: "UpdateRelativeTimeValidatorRelativeTimeValidatorUpdate" = Field(
+        alias="relativeTimeValidatorUpdate"
     )
 
 
-class CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate(
-    ValidatorCreation
-):
+class UpdateRelativeTimeValidatorRelativeTimeValidatorUpdate(ValidatorUpdate):
     pass
 
 
-CreateRelativeTimeValidatorWithMonotonicThreshold.update_forward_refs()
-CreateRelativeTimeValidatorWithMonotonicThresholdRelativeTimeValidatorWithMonotonicThresholdCreate.update_forward_refs()
+UpdateRelativeTimeValidator.update_forward_refs()
+UpdateRelativeTimeValidatorRelativeTimeValidatorUpdate.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .base_model import BaseModel
 from .enums import (
     ApiErrorCode,
     CategoricalDistributionMetric,
     ComparisonOperator,
     DecisionBoundsType,
+    FileFormat,
     IdentityDeleteErrorCode,
     IdentityProviderCreateErrorCode,
     IdentityProviderDeleteErrorCode,
     IdentityProviderUpdateErrorCode,
     NotificationSeverity,
     NotificationTypename,
     NumericAnomalyMetric,
@@ -107,31 +108,27 @@
 
 class ChannelCreationChannelWebhookChannelConfig(BaseModel):
     webhook_url: str = Field(alias="webhookUrl")
     application_link_url: str = Field(alias="applicationLinkUrl")
     auth_header: Optional[str] = Field(alias="authHeader")
 
 
-class DeletedEntity(BaseModel):
-    id: str
-    name: str
-
-
 class ChannelDeletion(BaseModel):
     errors: List["ChannelDeletionErrors"]
     channel: Optional["ChannelDeletionChannel"]
 
 
 class ChannelDeletionErrors(BaseModel):
     code: ApiErrorCode
     message: str
 
 
-class ChannelDeletionChannel(DeletedEntity):
-    pass
+class ChannelDeletionChannel(BaseModel):
+    id: Any
+    name: str
 
 
 class ChannelUpdate(BaseModel):
     errors: List["ChannelUpdateErrors"]
     channel: Optional[
         Annotated[
             Union[
@@ -1148,14 +1145,15 @@
 class SourceCreationSourceGcpStorageSourceConfig(BaseModel):
     project: str
     bucket: str
     folder: str
     csv: Optional["SourceCreationSourceGcpStorageSourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class SourceCreationSourceGcpStorageSourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -1470,14 +1468,15 @@
 
 class SourceCreationSourceAwsS3SourceConfig(BaseModel):
     bucket: str
     prefix: str
     csv: Optional["SourceCreationSourceAwsS3SourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class SourceCreationSourceAwsS3SourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -1724,14 +1723,15 @@
 class SourceUpdateSourceGcpStorageSourceConfig(BaseModel):
     project: str
     bucket: str
     folder: str
     csv: Optional["SourceUpdateSourceGcpStorageSourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class SourceUpdateSourceGcpStorageSourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -2046,14 +2046,15 @@
 
 class SourceUpdateSourceAwsS3SourceConfig(BaseModel):
     bucket: str
     prefix: str
     csv: Optional["SourceUpdateSourceAwsS3SourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class SourceUpdateSourceAwsS3SourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -2390,15 +2391,14 @@
 class ValidatorCreationValidatorNumericValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorNumericValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorNumericValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -2412,21 +2412,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorCategoricalDistributionValidator(BaseModel):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -2481,15 +2474,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -2503,21 +2495,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -2598,15 +2583,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -2620,21 +2604,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigSource"
     window: "ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -2707,15 +2684,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorVolumeValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -2727,21 +2703,14 @@
 
 class ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorVolumeValidatorDestination(BaseModel):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
@@ -2799,15 +2768,14 @@
 class ValidatorCreationValidatorNumericAnomalyValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -2830,21 +2798,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfig(BaseModel):
     source: "ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -2923,15 +2884,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -2945,21 +2905,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorFreshnessValidator(BaseModel):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -3000,15 +2953,14 @@
 
 
 class ValidatorCreationValidatorFreshnessValidatorConfig(BaseModel):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3022,21 +2974,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorRelativeVolumeValidator(BaseModel):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -3087,15 +3032,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3109,21 +3053,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfig(BaseModel):
     source: "ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -3151,15 +3088,14 @@
     id: Any
     severity: NotificationSeverity
     segment: "ValidatorIncidentsSegment"
     metric: Union[
         "ValidatorIncidentsMetricValidatorMetric",
         "ValidatorIncidentsMetricValidatorMetricWithFixedThreshold",
         "ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold",
-        "ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorIncidentsSegment(SegmentDetails):
     pass
 
 
@@ -3191,25 +3127,14 @@
     value: float
     lower_bound: float = Field(alias="lowerBound")
     upper_bound: float = Field(alias="upperBound")
     decision_bounds_type: DecisionBoundsType = Field(alias="decisionBoundsType")
     is_burn_in: bool = Field(alias="isBurnIn")
 
 
-class ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold(BaseModel):
-    typename__: Literal["ValidatorMetricWithMonotonicThreshold"] = Field(
-        alias="__typename"
-    )
-    start_time: datetime = Field(alias="startTime")
-    end_time: datetime = Field(alias="endTime")
-    is_incident: bool = Field(alias="isIncident")
-    value: float
-    operator: ComparisonOperator
-
-
 class ValidatorRecommendationApplication(BaseModel):
     typename__: str = Field(alias="__typename")
     failed_ids: List[Any] = Field(alias="failedIds")
     success_ids: List[str] = Field(alias="successIds")
 
 
 class ValidatorRecommendationDismissal(BaseModel):
@@ -3334,15 +3259,14 @@
 class ValidatorUpdateValidatorNumericValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3354,21 +3278,14 @@
 
 class ValidatorUpdateValidatorNumericValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorCategoricalDistributionValidator(BaseModel):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -3423,15 +3340,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3445,21 +3361,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -3536,15 +3445,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3558,21 +3466,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource"
     window: "ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -3645,15 +3546,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold(BaseModel):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
     sensitivity: float
     decision_bounds_type: Optional[DecisionBoundsType] = Field(
@@ -3663,21 +3563,14 @@
 
 class ValidatorUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorVolumeValidatorDestination(BaseModel):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
@@ -3733,15 +3626,14 @@
 class ValidatorUpdateValidatorNumericAnomalyValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -3764,21 +3656,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig(BaseModel):
     source: "ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -3855,15 +3740,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3877,21 +3761,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorFreshnessValidator(BaseModel):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -3932,15 +3809,14 @@
 
 
 class ValidatorUpdateValidatorFreshnessValidatorConfig(BaseModel):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -3954,21 +3830,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorRelativeVolumeValidator(BaseModel):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -4019,15 +3888,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -4041,21 +3909,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig(BaseModel):
     source: "ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -4305,15 +4166,14 @@
 ChannelCreation.update_forward_refs()
 ChannelCreationErrors.update_forward_refs()
 ChannelCreationChannelChannel.update_forward_refs()
 ChannelCreationChannelSlackChannel.update_forward_refs()
 ChannelCreationChannelSlackChannelConfig.update_forward_refs()
 ChannelCreationChannelWebhookChannel.update_forward_refs()
 ChannelCreationChannelWebhookChannelConfig.update_forward_refs()
-DeletedEntity.update_forward_refs()
 ChannelDeletion.update_forward_refs()
 ChannelDeletionErrors.update_forward_refs()
 ChannelDeletionChannel.update_forward_refs()
 ChannelUpdate.update_forward_refs()
 ChannelUpdateErrors.update_forward_refs()
 ChannelUpdateChannelChannel.update_forward_refs()
 ChannelUpdateChannelSlackChannel.update_forward_refs()
@@ -4574,98 +4434,89 @@
 ValidatorCreationValidatorNumericValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidator.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidator.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorVolumeValidator.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorVolumeValidatorDestination.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidator.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorNumericAnomalyValidatorDestination.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidator.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidator.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidator.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorSourceConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorIncidents.update_forward_refs()
 ValidatorIncidentsSegment.update_forward_refs()
 ValidatorIncidentsMetricValidatorMetric.update_forward_refs()
 ValidatorIncidentsMetricValidatorMetricWithFixedThreshold.update_forward_refs()
 ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold.update_forward_refs()
-ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold.update_forward_refs()
 ValidatorRecommendationApplication.update_forward_refs()
 ValidatorRecommendationDismissal.update_forward_refs()
 ValidatorRecommendationDismissalErrors.update_forward_refs()
 ValidatorUpdate.update_forward_refs()
 ValidatorUpdateErrors.update_forward_refs()
 ValidatorUpdateValidatorValidator.update_forward_refs()
 ValidatorUpdateValidatorValidatorSourceConfig.update_forward_refs()
@@ -4676,89 +4527,81 @@
 ValidatorUpdateValidatorNumericValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidator.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidator.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidator.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorVolumeValidatorDestination.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidator.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorNumericAnomalyValidatorDestination.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidator.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidator.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidator.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ValidatorUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
 WindowCreation.update_forward_refs()
 WindowCreationErrors.update_forward_refs()
 WindowCreationWindowWindow.update_forward_refs()
 WindowCreationWindowWindowSource.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_incidents.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_incidents.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     id: Any
     severity: NotificationSeverity
     segment: "GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment"
     metric: Union[
         "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric",
         "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold",
         "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold",
-        "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment(SegmentDetails):
     pass
 
 
@@ -105,31 +104,17 @@
     value: float
     lower_bound: float = Field(alias="lowerBound")
     upper_bound: float = Field(alias="upperBound")
     decision_bounds_type: DecisionBoundsType = Field(alias="decisionBoundsType")
     is_burn_in: bool = Field(alias="isBurnIn")
 
 
-class GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["ValidatorMetricWithMonotonicThreshold"] = Field(
-        alias="__typename"
-    )
-    start_time: datetime = Field(alias="startTime")
-    end_time: datetime = Field(alias="endTime")
-    is_incident: bool = Field(alias="isIncident")
-    value: float
-    operator: ComparisonOperator
-
-
 GetIncidents.update_forward_refs()
 GetIncidentsIncidentsNotification.update_forward_refs()
 GetIncidentsIncidentsSchemaChangeNotification.update_forward_refs()
 GetIncidentsIncidentsSegmentLimitExceededNotification.update_forward_refs()
 GetIncidentsIncidentsSegmentLimitExceededNotificationSegmentation.update_forward_refs()
 GetIncidentsIncidentsValidatorThresholdFailureNotification.update_forward_refs()
 GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment.update_forward_refs()
 GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric.update_forward_refs()
 GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold.update_forward_refs()
 GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold.update_forward_refs()
-GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_recommendation.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     JsonTypeDefinition,
     SegmentationId,
     SourceId,
     WindowId,
 )
 
 from .base_model import BaseModel
-from .enums import SourceState
+from .enums import FileFormat, SourceState
 
 
 class GetSource(BaseModel):
     source: Optional[
         Annotated[
             Union[
                 "GetSourceSourceSource",
@@ -116,14 +116,15 @@
 class GetSourceSourceGcpStorageSourceConfig(BaseModel):
     project: str
     bucket: str
     folder: str
     csv: Optional["GetSourceSourceGcpStorageSourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class GetSourceSourceGcpStorageSourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -438,14 +439,15 @@
 
 class GetSourceSourceAwsS3SourceConfig(BaseModel):
     bucket: str
     prefix: str
     csv: Optional["GetSourceSourceAwsS3SourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class GetSourceSourceAwsS3SourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     JsonTypeDefinition,
     SegmentationId,
     SourceId,
     WindowId,
 )
 
 from .base_model import BaseModel
-from .enums import SourceState
+from .enums import FileFormat, SourceState
 
 
 class GetSourceByResourceName(BaseModel):
     source_by_resource_name: Optional[
         Annotated[
             Union[
                 "GetSourceByResourceNameSourceByResourceNameSource",
@@ -124,14 +124,15 @@
     bucket: str
     folder: str
     csv: Optional[
         "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfigCsv"
     ]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -476,14 +477,15 @@
 
 class GetSourceByResourceNameSourceByResourceNameAwsS3SourceConfig(BaseModel):
     bucket: str
     prefix: str
     csv: Optional["GetSourceByResourceNameSourceByResourceNameAwsS3SourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class GetSourceByResourceNameSourceByResourceNameAwsS3SourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_incidents.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 class GetValidatorValidatorNumericValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorNumericValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorNumericValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorNumericValidatorConfigThresholdDynamicThreshold(BaseModel):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
     sensitivity: float
     decision_bounds_type: Optional[DecisionBoundsType] = Field(
@@ -152,19 +151,14 @@
 
 class GetValidatorValidatorNumericValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorNumericValidatorConfigThresholdMonotonicThreshold(BaseModel):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorCategoricalDistributionValidator(BaseModel):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -219,15 +213,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -241,21 +234,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -332,15 +318,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -354,21 +339,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfig(BaseModel):
     source: "GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigSource"
     window: "GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -439,15 +417,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorVolumeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorVolumeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorVolumeValidatorConfigThresholdDynamicThreshold(BaseModel):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
     sensitivity: float
     decision_bounds_type: Optional[DecisionBoundsType] = Field(
@@ -457,19 +434,14 @@
 
 class GetValidatorValidatorVolumeValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorVolumeValidatorConfigThresholdMonotonicThreshold(BaseModel):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorVolumeValidatorDestination(BaseModel):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
@@ -523,15 +495,14 @@
 class GetValidatorValidatorNumericAnomalyValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -554,21 +525,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfig(BaseModel):
     source: "GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -645,15 +609,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -667,21 +630,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorFreshnessValidator(BaseModel):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -722,15 +678,14 @@
 
 
 class GetValidatorValidatorFreshnessValidatorConfig(BaseModel):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorFreshnessValidatorConfigThresholdDynamicThreshold(BaseModel):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
     sensitivity: float
     decision_bounds_type: Optional[DecisionBoundsType] = Field(
@@ -740,21 +695,14 @@
 
 class GetValidatorValidatorFreshnessValidatorConfigThresholdFixedThreshold(BaseModel):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorRelativeVolumeValidator(BaseModel):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -803,15 +751,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -825,21 +772,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfig(BaseModel):
     source: "GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
     filter: Optional[JsonFilterExpression]
 
@@ -872,85 +812,77 @@
 GetValidatorValidatorNumericValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorNumericValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorNumericValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorNumericValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorNumericValidatorConfig.update_forward_refs()
 GetValidatorValidatorNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidator.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorConfig.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidator.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorConfig.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorValidatorNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorVolumeValidator.update_forward_refs()
 GetValidatorValidatorVolumeValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorVolumeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorVolumeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorVolumeValidatorConfig.update_forward_refs()
 GetValidatorValidatorVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorVolumeValidatorDestination.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidator.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorConfig.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorNumericAnomalyValidatorDestination.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidator.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorConfig.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorFreshnessValidator.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorConfig.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidator.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorSourceConfig.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -150,15 +150,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -172,21 +171,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidator(
     BaseModel
 ):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -247,15 +239,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -269,21 +260,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -370,15 +354,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -392,21 +375,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigSource"
     window: "GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -489,15 +465,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -511,21 +486,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorDestination(
     BaseModel
 ):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
@@ -595,15 +563,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -626,21 +593,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -731,15 +691,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -753,21 +712,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameFreshnessValidator(BaseModel):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -818,15 +770,14 @@
 class GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfig(
     BaseModel
 ):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -840,21 +791,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidator(
     BaseModel
 ):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -915,15 +859,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -937,21 +880,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -986,85 +922,77 @@
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorDestination.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameNumericAnomalyValidatorDestination.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidator.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 GetValidatorByResourceNameValidatorByResourceNameRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_validator_segment_incidents.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_validator_segment_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     prefix: str
 
 
 class AwsS3SourceCreateInput(BaseModel):
     bucket: str
     credential_id: CredentialId = Field(alias="credentialId")
     csv: Optional["CsvParserInput"]
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
     file_pattern: Optional[str] = Field(alias="filePattern")
     jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
     name: str
     prefix: str
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
     schedule: CronExpression
@@ -433,14 +434,15 @@
     project: str
 
 
 class GcpStorageSourceCreateInput(BaseModel):
     bucket: str
     credential_id: CredentialId = Field(alias="credentialId")
     csv: Optional["CsvParserInput"]
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
     file_pattern: Optional[str] = Field(alias="filePattern")
     folder: str
     jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
     name: str
     project: str
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
@@ -537,18 +539,14 @@
 
 class LocalIdentityProviderUpdateInput(BaseModel):
     disabled: bool
     id: str
     name: str
 
 
-class MonotonicThresholdCreateInput(BaseModel):
-    operator: ComparisonOperator
-
-
 class NotificationRuleCreateInput(BaseModel):
     channel_id: Any = Field(alias="channelId")
     name: str
     notification_typenames: List[NotificationTypename] = Field(
         alias="notificationTypenames"
     )
     resource_name: Optional[str] = Field(alias="resourceName")
@@ -989,19 +987,14 @@
 
 class ValidatorWithFixedThresholdUpdateInput(BaseModel):
     operator: ComparisonOperator
     validator_id: ValidatorId = Field(alias="validatorId")
     value: float
 
 
-class ValidatorWithMonotonicThresholdUpdateInput(BaseModel):
-    operator: ComparisonOperator
-    validator_id: ValidatorId = Field(alias="validatorId")
-
-
 class VolumeValidatorCreateInput(BaseModel):
     destination_id: Optional[DestinationId] = Field(alias="destinationId")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     metric: VolumeMetric
     name: Optional[str]
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
@@ -1093,15 +1086,14 @@
 KafkaSSLCredentialUpdateInput.update_forward_refs()
 KafkaSaslSSLPlainCredentialCreateInput.update_forward_refs()
 KafkaSaslSSLPlainCredentialSecretChangedInput.update_forward_refs()
 KafkaSaslSSLPlainCredentialUpdateInput.update_forward_refs()
 KafkaSourceCreateInput.update_forward_refs()
 KafkaSourceUpdateInput.update_forward_refs()
 LocalIdentityProviderUpdateInput.update_forward_refs()
-MonotonicThresholdCreateInput.update_forward_refs()
 NotificationRuleCreateInput.update_forward_refs()
 NotificationRuleDeleteInput.update_forward_refs()
 NotificationRuleUpdateInput.update_forward_refs()
 NumericAnomalyValidatorCreateInput.update_forward_refs()
 NumericAnomalyValidatorUpdateInput.update_forward_refs()
 NumericDistributionValidatorCreateInput.update_forward_refs()
 NumericDistributionValidatorUpdateInput.update_forward_refs()
@@ -1149,12 +1141,11 @@
 ValidatorIncidentsInput.update_forward_refs()
 ValidatorRecommendationApplyInput.update_forward_refs()
 ValidatorRecommendationDismissInput.update_forward_refs()
 ValidatorSegmentIncidentsInput.update_forward_refs()
 ValidatorSegmentMetricsInput.update_forward_refs()
 ValidatorWithDynamicThresholdUpdateInput.update_forward_refs()
 ValidatorWithFixedThresholdUpdateInput.update_forward_refs()
-ValidatorWithMonotonicThresholdUpdateInput.update_forward_refs()
 VolumeValidatorCreateInput.update_forward_refs()
 VolumeValidatorUpdateInput.update_forward_refs()
 WebhookChannelCreateInput.update_forward_refs()
 WebhookChannelUpdateInput.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/kafka_sasl_ssl_plain_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/list_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/list_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     JsonTypeDefinition,
     SegmentationId,
     SourceId,
     WindowId,
 )
 
 from .base_model import BaseModel
-from .enums import SourceState
+from .enums import FileFormat, SourceState
 
 
 class ListSources(BaseModel):
     sources_list: List[
         Annotated[
             Union[
                 "ListSourcesSourcesListSource",
@@ -116,14 +116,15 @@
 class ListSourcesSourcesListGcpStorageSourceConfig(BaseModel):
     project: str
     bucket: str
     folder: str
     csv: Optional["ListSourcesSourcesListGcpStorageSourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class ListSourcesSourcesListGcpStorageSourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
 
 
@@ -438,14 +439,15 @@
 
 class ListSourcesSourcesListAwsS3SourceConfig(BaseModel):
     bucket: str
     prefix: str
     csv: Optional["ListSourcesSourcesListAwsS3SourceConfigCsv"]
     schedule: CronExpression
     file_pattern: Optional[str] = Field(alias="filePattern")
+    file_format: Optional[FileFormat] = Field(alias="fileFormat")
 
 
 class ListSourcesSourcesListAwsS3SourceConfigCsv(BaseModel):
     null_marker: Optional[str] = Field(alias="nullMarker")
     delimiter: str
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/list_validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 class ListValidatorsValidatorsListNumericValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListNumericValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListNumericValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -156,21 +155,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListCategoricalDistributionValidator(BaseModel):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -227,15 +219,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -249,21 +240,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -344,15 +328,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -366,21 +349,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigSource"
     window: "ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -453,15 +429,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListVolumeValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListVolumeValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -475,21 +450,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListVolumeValidatorDestination(BaseModel):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
@@ -547,15 +515,14 @@
 class ListValidatorsValidatorsListNumericAnomalyValidatorConfig(BaseModel):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -578,21 +545,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -673,15 +633,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -695,21 +654,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListFreshnessValidator(BaseModel):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -750,15 +702,14 @@
 
 
 class ListValidatorsValidatorsListFreshnessValidatorConfig(BaseModel):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -772,21 +723,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListRelativeVolumeValidator(BaseModel):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
@@ -837,15 +781,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -859,21 +802,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -908,85 +844,77 @@
 ListValidatorsValidatorsListNumericValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidator.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidator.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidator.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListVolumeValidatorDestination.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidator.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListNumericAnomalyValidatorDestination.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidator.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidator.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidator.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorConfig.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-ListValidatorsValidatorsListRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 ListValidatorsValidatorsListRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_identity_provider_namespace.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_identity_provider_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_kafka_sasl_ssl_plain_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_kafka_sasl_ssl_plain_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_notification_rule_namespace.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_notification_rule_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_segmentation_namespace.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_segmentation_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,15 +172,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -194,21 +193,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator(
     BaseModel
 ):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -269,15 +261,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -291,21 +282,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -392,15 +376,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -414,21 +397,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -515,15 +491,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -537,21 +512,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorDestination(
     BaseModel
 ):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
@@ -621,15 +589,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -652,21 +619,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -759,15 +719,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -781,21 +740,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidator(
     BaseModel
 ):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -848,15 +800,14 @@
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfig(
     BaseModel
 ):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -870,21 +821,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidator(
     BaseModel
 ):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -945,15 +889,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -967,21 +910,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -1018,85 +954,77 @@
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorVolumeValidatorDestination.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorNumericAnomalyValidatorDestination.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidator.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.6.5/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     metric: NumericMetric
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -194,21 +193,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidator(
     BaseModel
 ):
     typename__: Literal["CategoricalDistributionValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -269,15 +261,14 @@
     categorical_distribution_metric: CategoricalDistributionMetric = Field(
         alias="categoricalDistributionMetric"
     )
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -291,21 +282,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -392,15 +376,14 @@
     source_field: JsonPointer = Field(alias="sourceField")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     distribution_metric: NumericDistributionMetric = Field(alias="distributionMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -414,21 +397,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -515,15 +491,14 @@
     optional_source_field: Optional[JsonPointer] = Field(alias="optionalSourceField")
     source_fields: List[JsonPointer] = Field(alias="sourceFields")
     volume_metric: VolumeMetric = Field(alias="volumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -537,21 +512,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorDestination(
     BaseModel
 ):
     name: str
     id: DestinationId
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
@@ -621,15 +589,14 @@
 ):
     source_field: JsonPointer = Field(alias="sourceField")
     numeric_anomaly_metric: NumericAnomalyMetric = Field(alias="numericAnomalyMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
     reference_source_field: JsonPointer = Field(alias="referenceSourceField")
     sensitivity: float
     minimum_reference_datapoints: Optional[float] = Field(
         alias="minimumReferenceDatapoints"
     )
     minimum_absolute_difference: float = Field(alias="minimumAbsoluteDifference")
@@ -652,21 +619,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -759,15 +719,14 @@
     source_field_minuend: JsonPointer = Field(alias="sourceFieldMinuend")
     source_field_subtrahend: JsonPointer = Field(alias="sourceFieldSubtrahend")
     relative_time_metric: RelativeTimeMetric = Field(alias="relativeTimeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -781,21 +740,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidator(
     BaseModel
 ):
     typename__: Literal["FreshnessValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -848,15 +800,14 @@
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfig(
     BaseModel
 ):
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -870,21 +821,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidator(
     BaseModel
 ):
     typename__: Literal["RelativeVolumeValidator"] = Field(alias="__typename")
     id: ValidatorId
     name: str
     has_custom_name: bool = Field(alias="hasCustomName")
@@ -945,15 +889,14 @@
         alias="optionalReferenceSourceField"
     )
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
     initialize_with_backfill: bool = Field(alias="initializeWithBackfill")
     threshold: Union[
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold",
         "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold",
-        "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold",
     ] = Field(discriminator="typename__")
 
 
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold(
     BaseModel
 ):
     typename__: Literal["DynamicThreshold"] = Field(alias="__typename")
@@ -967,21 +910,14 @@
     BaseModel
 ):
     typename__: Literal["FixedThreshold"] = Field(alias="__typename")
     operator: ComparisonOperator
     value: float
 
 
-class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold(
-    BaseModel
-):
-    typename__: Literal["MonotonicThreshold"] = Field(alias="__typename")
-    operator: ComparisonOperator
-
-
 class UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig(
     BaseModel
 ):
     source: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource"
     window: "UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow"
     history: int
     offset: int
@@ -1018,85 +954,77 @@
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorCategoricalDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericDistributionValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorVolumeValidatorDestination.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorReferenceSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorNumericAnomalyValidatorDestination.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeTimeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorFreshnessValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidator.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigWindow.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
-UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdateValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
```

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_diff.py` & `validio_sdk-0.6.5/validio_sdk/resource/_diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_diff_util.py` & `validio_sdk-0.6.5/validio_sdk/resource/_diff_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_diffable.py` & `validio_sdk-0.6.5/validio_sdk/resource/_diffable.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_errors.py` & `validio_sdk-0.6.5/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.6.5/validio_sdk/resource/_field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_resource.py` & `validio_sdk-0.6.5/validio_sdk/resource/_resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.6.5/validio_sdk/resource/_resource_graph.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_serde.py` & `validio_sdk-0.6.5/validio_sdk/resource/_serde.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.6.5/validio_sdk/resource/_server_resources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_update_namespace.py` & `validio_sdk-0.6.5/validio_sdk/resource/_update_namespace.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/_util.py` & `validio_sdk-0.6.5/validio_sdk/resource/_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/channels.py` & `validio_sdk-0.6.5/validio_sdk/resource/channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/credentials.py` & `validio_sdk-0.6.5/validio_sdk/resource/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/destinations.py` & `validio_sdk-0.6.5/validio_sdk/resource/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/filters.py` & `validio_sdk-0.6.5/validio_sdk/resource/filters.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/notification_rules.py` & `validio_sdk-0.6.5/validio_sdk/resource/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/segmentations.py` & `validio_sdk-0.6.5/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/sources.py` & `validio_sdk-0.6.5/validio_sdk/resource/sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any, cast
 
 from camel_converter import to_snake
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
-from validio_sdk.graphql_client import CsvParserInput
+from validio_sdk.graphql_client import CsvParserInput, FileFormat
 from validio_sdk.resource._diffable import Diffable
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     NODE_TYPE_FIELD_NAME,
     ImportValue,
     _api_create_input_params,
@@ -701,16 +701,17 @@
 
     def __init__(
         self,
         name: str,
         credential: Credential,
         bucket: str,
         file_pattern: str | None,
-        csv: CsvParserConfig | None,
         schedule: str,
+        csv: CsvParserConfig | None = None,
+        file_format: FileFormat | None = None,
         jtd_schema: JsonTypeDefinition | None = None,
     ):
         """
         Constructor.
 
         :param bucket: Name of the bucket to ingest files from.
         :param file_pattern: Glob pattern against file names, used to filter in
@@ -724,19 +725,29 @@
         self.file_pattern = file_pattern
         self.schedule = schedule
         self.csv = (
             CsvParserConfig(null_marker=None, delimiter=",")
             if csv is None
             else CsvParserConfig._from_any(csv)
         )
+        self.file_format = (
+            None
+            if file_format is None
+            else (
+                # When we decode, enums are passed in a strings
+                file_format
+                if isinstance(file_format, FileFormat)
+                else FileFormat(file_format)
+            )
+        )
 
     def _immutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
-            *{"bucket"},
+            *{"bucket", "file_format"},
         }
 
     def _mutable_fields(self) -> set[str]:
         return {
             *super()._mutable_fields(),
             *{
                 "schedule",
@@ -772,30 +783,32 @@
     def __init__(
         self,
         name: str,
         credential: AwsCredential,
         bucket: str,
         prefix: str,
         file_pattern: str | None,
-        csv: CsvParserConfig | None,
         schedule: str,
+        csv: CsvParserConfig | None = None,
+        file_format: FileFormat | None = None,
         jtd_schema: JsonTypeDefinition | None = None,
     ):
         """
         Constructor.
 
         :param bucket: Name of the bucket to read files from.
         :param prefix: Folder prefix. e.g. if '/a/b' is specified as a prefix,
             then only files located in the '/a/b' folder will be ingested
         """
         super().__init__(
             name=name,
             credential=credential,
             bucket=bucket,
             csv=csv,
+            file_format=file_format,
             file_pattern=file_pattern,
             schedule=schedule,
             jtd_schema=jtd_schema,
         )
 
         self.prefix = prefix
 
@@ -827,30 +840,32 @@
         self,
         name: str,
         credential: GcpCredential,
         project: str,
         bucket: str,
         folder: str,
         file_pattern: str | None,
-        csv: CsvParserConfig | None,
         schedule: str,
+        csv: CsvParserConfig | None = None,
+        file_format: FileFormat | None = None,
         jtd_schema: JsonTypeDefinition | None = None,
     ):
         """
         Constructor.
 
         :param project: Name of GCP project where the bucket resides.
         :param bucket: Name of the bucket to ingest files from.
         :param folder: Name of a folder within the bucket, to ingest files from.
         """
         super().__init__(
             name=name,
             credential=credential,
             bucket=bucket,
             csv=csv,
+            file_format=file_format,
             file_pattern=file_pattern,
             schedule=schedule,
             jtd_schema=jtd_schema,
         )
 
         self.project = project
         self.folder = folder
```

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.6.5/validio_sdk/resource/tests/test__diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.6.5/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.6.5/validio_sdk/resource/tests/test__resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/thresholds.py` & `validio_sdk-0.6.5/validio_sdk/resource/thresholds.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 
 from validio_sdk.graphql_client import (
     BaseModel,
     ComparisonOperator,
     DecisionBoundsType,
     DynamicThresholdCreateInput,
     FixedThresholdCreateInput,
-    MonotonicThresholdCreateInput,
     ValidatorWithDynamicThresholdUpdateInput,
     ValidatorWithFixedThresholdUpdateInput,
-    ValidatorWithMonotonicThresholdUpdateInput,
 )
 from validio_sdk.resource._diffable import Diffable
 from validio_sdk.resource._serde import NODE_TYPE_FIELD_NAME
 
 
 class Threshold(Diffable):
     """
@@ -152,55 +150,11 @@
             # type: ignore[call-arg]
             validator_id=validator_id,
             value=self.value,
             operator=self.operator,
         )
 
 
-class MonotonicThreshold(Threshold):
-    """
-    A monotonic threshold configuration.
-
-    https://docs.validio.io/docs/thresholds#monotonic-threshold
-    """
-
-    def __init__(
-        self,
-        operator: ComparisonOperator,
-    ):
-        """
-        Constructor.
-
-        :param operator: Operator to compare against the previous value.
-        """
-        super().__init__()
-
-        self.operator = (
-            operator
-            if isinstance(operator, ComparisonOperator)
-            else ComparisonOperator(operator)
-        )
-
-    def _immutable_fields(self) -> set[str]:
-        return set({})
-
-    def _mutable_fields(self) -> set[str]:
-        return {"operator"}
-
-    def _api_create_input(self) -> BaseModel:
-        return MonotonicThresholdCreateInput(
-            operator=self.operator,
-        )
-
-    def _api_update_input(self, validator_id: str) -> BaseModel:
-        return ValidatorWithMonotonicThresholdUpdateInput(
-            # type: ignore[call-arg]
-            validator_id=validator_id,
-            operator=self.operator,
-        )
-
-
 THRESHOLD_CLASSES: set[type] = {
     DynamicThreshold,
     FixedThreshold,
-    MonotonicThreshold,
 }
```

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/validators.py` & `validio_sdk-0.6.5/validio_sdk/resource/validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/resource/windows.py` & `validio_sdk-0.6.5/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/scalars.py` & `validio_sdk-0.6.5/validio_sdk/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/util.py` & `validio_sdk-0.6.5/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/validio_sdk/validio_client.py` & `validio_sdk-0.6.5/validio_sdk/validio_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.6.4/PKG-INFO` & `validio_sdk-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-sdk
-Version: 0.6.4
+Version: 0.6.5
 Summary: SDK to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

