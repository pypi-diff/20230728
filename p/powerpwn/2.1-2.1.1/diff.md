# Comparing `tmp/powerpwn-2.1.tar.gz` & `tmp/powerpwn-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpwn-2.1.tar", last modified: Fri Jul 28 13:39:11 2023, max compression
+gzip compressed data, was "powerpwn-2.1.1.tar", last modified: Fri Jul 28 13:44:11 2023, max compression
```

## Comparing `powerpwn-2.1.tar` & `powerpwn-2.1.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:11.268410 powerpwn-2.1/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       74 2023-07-28 13:39:11.274921 powerpwn-2.1/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1590 2023-07-28 13:39:11.282516 powerpwn-2.1/setup.cfg
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-24 10:03:36.000000 powerpwn-2.1/setup.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:54.101306 powerpwn-2.1/src/
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:57.043905 powerpwn-2.1/src/powerpwn/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:59.568508 powerpwn-2.1/src/powerpwn/cli/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 06:41:41.000000 powerpwn-2.1/src/powerpwn/cli/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6917 2023-07-28 07:57:23.000000 powerpwn-2.1/src/powerpwn/cli/arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       49 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/cli/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4241 2023-07-28 07:55:29.000000 powerpwn-2.1/src/powerpwn/cli/runners.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:59.855694 powerpwn-2.1/src/powerpwn/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1399 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/enums/str_enum.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:00.484499 powerpwn-2.1/src/powerpwn/machinepwn/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/machinepwn/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:01.484744 powerpwn-2.1/src/powerpwn/machinepwn/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      231 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/enums/code_exec_type_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-28 07:20:23.000000 powerpwn-2.1/src/powerpwn/machinepwn/enums/command_to_run_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5960 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/machine_pwn.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:03.184516 powerpwn-2.1/src/powerpwn/machinepwn/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      929 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/any_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      446 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/cleanup_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      549 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/cmd_arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1601 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/cmd_results.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      448 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/code_exec_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      426 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/code_exec_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       96 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/command_args_properties_base_model.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      292 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/exflirtate_file_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      456 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/exflirtate_file_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      571 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/ransomware_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      435 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/ransomware_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      302 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/steal_cookie_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      444 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/steal_cookie_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      500 2023-07-27 09:25:53.000000 powerpwn-2.1/src/powerpwn/machinepwn/models/steal_power_automate_token_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1229 2023-07-28 07:55:33.000000 powerpwn-2.1/src/powerpwn/main.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:59.950292 powerpwn-2.1/src/powerpwn/powerdoor/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3765 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdoor/backdoor_flow.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/create_flow_model.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:00.914991 powerpwn-2.1/src/powerpwn/powerdoor/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      233 2023-07-28 07:20:23.000000 powerpwn-2.1/src/powerpwn/powerdoor/enums/action_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      126 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/enums/flow_state.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1845 2023-07-28 07:22:29.000000 powerpwn-2.1/src/powerpwn/powerdoor/flow_factory_installer.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:01.351144 powerpwn-2.1/src/powerpwn/powerdoor/samples/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/samples/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)    23081 2023-07-27 21:35:53.000000 powerpwn-2.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2579 2023-07-24 10:03:36.000000 powerpwn-2.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:59.903396 powerpwn-2.1/src/powerpwn/powerdump/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:01.301578 powerpwn-2.1/src/powerpwn/powerdump/collect/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:03.532856 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:03.928130 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3485 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:08.643771 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1577 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2507 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6158 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1767 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     7120 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4139 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5868 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3777 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3897 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3934 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4330 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1235 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:07.648215 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      132 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      280 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      211 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:08.235987 powerpwn-2.1/src/powerpwn/powerdump/collect/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      756 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/base_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      524 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/base_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      477 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1293 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/connection_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2047 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/connector_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      674 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      781 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_record_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1027 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_store_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      496 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_store_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      507 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/principal_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      370 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/models/resource_entity_base.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:09.360859 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3424 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4944 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4689 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2721 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:09.635541 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      202 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      707 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2659 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:09.914136 powerpwn-2.1/src/powerpwn/powerdump/gui/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1739 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/gui.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4377 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/prep.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:10.621883 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1367 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/base.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1150 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1728 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/connections_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      983 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/connectors_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      303 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/json_object.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1146 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/gui/templates/resources_table.html
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:39:11.215133 powerpwn-2.1/src/powerpwn/powerdump/utils/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4291 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/auth.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      376 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4593 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/json_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5133 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/model_loaders.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1107 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/path_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3124 2023-07-28 07:22:48.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/requests_wrapper.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1098 2023-07-27 11:45:05.000000 powerpwn-2.1/src/powerpwn/powerdump/utils/token_cache.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:38:54.877650 powerpwn-2.1/src/powerpwn.egg-info/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       74 2023-07-28 13:38:51.000000 powerpwn-2.1/src/powerpwn.egg-info/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5991 2023-07-28 13:38:54.000000 powerpwn-2.1/src/powerpwn.egg-info/SOURCES.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        1 2023-07-28 13:38:51.000000 powerpwn-2.1/src/powerpwn.egg-info/dependency_links.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       48 2023-07-28 13:38:51.000000 powerpwn-2.1/src/powerpwn.egg-info/entry_points.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      332 2023-07-28 13:38:51.000000 powerpwn-2.1/src/powerpwn.egg-info/requires.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        9 2023-07-28 13:38:51.000000 powerpwn-2.1/src/powerpwn.egg-info/top_level.txt
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:11.367625 powerpwn-2.1.1/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-07-28 13:44:11.367625 powerpwn-2.1.1/PKG-INFO
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1592 2023-07-28 13:44:11.367625 powerpwn-2.1.1/setup.cfg
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-24 10:03:36.000000 powerpwn-2.1.1/setup.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:03.758803 powerpwn-2.1.1/src/
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.168609 powerpwn-2.1.1/src/powerpwn/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.656009 powerpwn-2.1.1/src/powerpwn/cli/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 06:41:41.000000 powerpwn-2.1.1/src/powerpwn/cli/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6954 2023-07-28 13:42:29.000000 powerpwn-2.1.1/src/powerpwn/cli/arguments.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       49 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/cli/const.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4241 2023-07-28 07:55:29.000000 powerpwn-2.1.1/src/powerpwn/cli/runners.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.765664 powerpwn-2.1.1/src/powerpwn/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1399 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/enums/str_enum.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.875467 powerpwn-2.1.1/src/powerpwn/machinepwn/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:05.063767 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      231 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/code_exec_type_enum.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-28 07:20:23.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/enums/command_to_run_enum.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5960 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/machine_pwn.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.100522 powerpwn-2.1.1/src/powerpwn/machinepwn/models/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      929 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/any_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      446 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cleanup_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      549 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_arguments.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1601 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_results.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      448 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/code_exec_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      426 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/code_exec_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       96 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/command_args_properties_base_model.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      292 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/exflirtate_file_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      456 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/exflirtate_file_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      571 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/ransomware_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      435 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/ransomware_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      302 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_cookie_args_properties.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      444 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_cookie_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      500 2023-07-27 09:25:53.000000 powerpwn-2.1.1/src/powerpwn/machinepwn/models/steal_power_automate_token_command_args.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1229 2023-07-28 07:55:33.000000 powerpwn-2.1.1/src/powerpwn/main.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.351247 powerpwn-2.1.1/src/powerpwn/powerdoor/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3765 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/backdoor_flow.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/create_flow_model.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.537166 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      233 2023-07-28 07:20:23.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/action_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      126 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/enums/flow_state.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1845 2023-07-28 07:22:29.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/flow_factory_installer.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.731790 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)    23081 2023-07-27 21:35:53.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2579 2023-07-24 10:03:36.000000 powerpwn-2.1.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.797800 powerpwn-2.1.1/src/powerpwn/powerdump/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:06.859276 powerpwn-2.1.1/src/powerpwn/powerdump/collect/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:07.089168 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/__init__.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:07.242562 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3485 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:08.295766 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1577 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2507 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6158 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1767 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     7120 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4139 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5868 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3777 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3897 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3934 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4330 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1235 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:08.573156 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      132 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      280 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      211 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:09.416104 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      756 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      524 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_validator.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      477 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1293 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connection_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2047 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connector_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      674 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      781 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_record_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1027 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      496 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_validator.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      507 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/principal_entity.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      370 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/resource_entity_base.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:09.910849 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3424 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4944 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4689 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2721 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.061285 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      202 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      707 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2659 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.244255 powerpwn-2.1.1/src/powerpwn/powerdump/gui/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1739 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/gui.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4377 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/prep.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:10.788047 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1367 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/base.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1150 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1728 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connections_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      983 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connectors_table.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      303 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/json_object.html
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1146 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/resources_table.html
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:11.316644 powerpwn-2.1.1/src/powerpwn/powerdump/utils/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/__init__.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4291 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/auth.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      376 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/const.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4593 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/json_utils.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5133 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/model_loaders.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1107 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/path_utils.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3124 2023-07-28 07:22:48.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/requests_wrapper.py
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1098 2023-07-27 11:45:05.000000 powerpwn-2.1.1/src/powerpwn/powerdump/utils/token_cache.py
+drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 13:44:04.455745 powerpwn-2.1.1/src/powerpwn.egg-info/
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       76 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5991 2023-07-28 13:44:03.000000 powerpwn-2.1.1/src/powerpwn.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        1 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       48 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      332 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/requires.txt
+-rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        9 2023-07-28 13:44:01.000000 powerpwn-2.1.1/src/powerpwn.egg-info/top_level.txt
```

### Comparing `powerpwn-2.1/setup.cfg` & `powerpwn-2.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = powerpwn
 author = Michael Bargury
-version = 2.1
+version = 2.1.1
 
 [options]
 install_requires = 
 	pydantic[email] ==1.10.7
 	pydantic ==1.10.7
 	swagger-ui-py ==22.7.13
 	Flask ==2.2.5
```

### Comparing `powerpwn-2.1/src/powerpwn/cli/arguments.py` & `powerpwn-2.1.1/src/powerpwn/cli/arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-import argparse
-import logging
-
-from powerpwn.machinepwn.enums.code_exec_type_enum import CodeExecTypeEnum
-from powerpwn.powerdoor.enums.action_type import BackdoorActionType
-from powerpwn.powerdump.utils.const import CACHE_PATH
-
-
-def module_gui(sub_parser: argparse.ArgumentParser):
-    gui_parser = sub_parser.add_parser("gui", description="Show collected resources and data.", help="Show collected resources and data via GUI.")
-    gui_parser.add_argument("--cache-path", default=CACHE_PATH, type=str, help="Path to cached resources.")
-
-
-def module_dump(sub_parser: argparse.ArgumentParser):
-    dump_parser = sub_parser.add_parser(
-        "dump",
-        description="Recon for available data connections and dump their content",
-        help="Recon for available data connections and dump their content.",
-    )
-    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
-    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
-    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
-
-
-def module_nocodemalware(command_subparsers: argparse.ArgumentParser):
-    nocodemalware_parser = command_subparsers.add_parser(
-        "nocodemalware",
-        description="Repurpose trusted execs, service accounts and cloud services to power a malware operation",
-        help="Repurpose trusted execs, service accounts and cloud services to power a malware operation.",
-    )
-    nocodemalware_parser.add_argument(
-        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
-    )
-    nocodemalware_parser = nocodemalware_parser.add_subparsers(help="nocodemalware_subcommand", dest="nocodemalware_subcommand")
-
-    module_nocodemalware_subcommand_exec(nocodemalware_parser)
-
-
-def module_nocodemalware_subcommand_exec(command_subparsers: argparse.ArgumentParser):
-    steal_fqdn_parser = command_subparsers.add_parser("steal-cookie", description="Steal cookie of fqdn")
-    steal_fqdn_parser.add_argument("--fqdn", required=True, type=str, help="Fully qualified domain name to fetch the cookies of")
-
-    steal_power_automate_token_parser = command_subparsers.add_parser("steal-power-automate-token", description="Steal power automate token")
-
-    execute_command_parser = command_subparsers.add_parser("command-exec", description="Execute command on machine")
-    execute_command_parser.add_argument(
-        "-t", "--type", required=True, type=str, choices=[cmd_type.value for cmd_type in CodeExecTypeEnum], help="Command type"
-    )
-    execute_command_parser.add_argument("-c", "--command-to-execute", required=True, type=str, help="Command to execute")
-
-    ransomware_parser = command_subparsers.add_parser("ransomware", description="Ransomware")
-    ransomware_parser.add_argument("--crawl_depth", required=True, type=str, help="Recursively search into subdirectories this many times")
-    ransomware_parser.add_argument(
-        "-k", "--encryption-key", required=True, type=str, help="an encryption key used to encrypt each file identified (AES256)"
-    )
-    ransomware_parser.add_argument(
-        "--dirs", required=True, type=str, help="A list of directories to begin crawl from separated by a comma (e.g.'C:\\,D:\\')"
-    )
-
-    exfiltrate_file_parser = command_subparsers.add_parser("exfiltrate", description="Exfiltrate file")
-    exfiltrate_file_parser.add_argument("-f", "--file", required=True, type=str, help="Absolute path to file")
-
-    cleanup_parser = command_subparsers.add_parser("cleanup", description="Cleanup")
-
-
-def module_backdoor(command_subparsers: argparse.ArgumentParser):
-    backdoor_parser = command_subparsers.add_parser(
-        "backdoor", description="Install a backdoor on the target tenant.", help="Install a backdoor on the target tenant"
-    )
-    backdoor_parser.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id in powerplatform.")
-    backdoor_subparsers = backdoor_parser.add_subparsers(help="backdoor_subcommand", dest="backdoor_subcommand")
-
-    ## Delete Flow parser ##
-    delete_flow_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.delete_flow.value, description="Deletes flow.", help="Deletes flow using installed backdoor flow."
-    )
-    delete_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
-    delete_flow_parser.add_argument("-f", "--flow-id", type=str, help="Flow id to delete.")
-
-    ## Create Flow parser ##
-    create_flow_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.create_flow.value, description="Creates a flow.", help="Creates a flow using installed backdoor flow."
-    )
-    create_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
-    create_flow_parser.add_argument("-i", "--input", type=str, required=True, help="Path to flow details input file.")
-
-    ## Get connections parser ##
-    get_connections_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.get_connections.value, description="Get connections", help="Gets connections details in environment"
-    )
-    get_connections_parser.add_argument(
-        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
-    )
-    get_connections_parser.add_argument("-o", "--output", type=str, default="", help="Path to output file.")
-
-    ## backdoor installer parser ##
-    installer = backdoor_subparsers.add_parser(
-        BackdoorActionType.install_factory.value, description="Install flow factory", help="Installs flow factory in powerplatform"
-    )
-    installer.add_argument("-c", "--connection-id", required=True, type=str, help="The connection id of management connection")
-    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-
-
-def module_phishing(command_subparsers: argparse.ArgumentParser):
-    phishing_parser = command_subparsers.add_parser(
-        "phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app."
-    )
-
-
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-l", "--log-level", default=logging.INFO, type=lambda x: getattr(logging, x), help="Configure the logging level.")
-    command_subparsers = parser.add_subparsers(help="command", dest="command")
-
-    module_dump(command_subparsers)
-    module_gui(command_subparsers)
-    module_backdoor(command_subparsers)
-    module_nocodemalware(command_subparsers)
-    module_phishing(command_subparsers)
-
-    args = parser.parse_args()
-
-    return args
+import argparse
+import logging
+
+from powerpwn.machinepwn.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.powerdoor.enums.action_type import BackdoorActionType
+from powerpwn.powerdump.utils.const import CACHE_PATH
+
+
+def module_gui(sub_parser: argparse.ArgumentParser):
+    gui_parser = sub_parser.add_parser("gui", description="Show collected resources and data.", help="Show collected resources and data via GUI.")
+    gui_parser.add_argument("--cache-path", default=CACHE_PATH, type=str, help="Path to cached resources.")
+
+
+def module_dump(sub_parser: argparse.ArgumentParser):
+    dump_parser = sub_parser.add_parser(
+        "dump",
+        description="Recon for available data connections and dump their content",
+        help="Recon for available data connections and dump their content.",
+    )
+    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
+    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
+    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
+
+
+def module_nocodemalware(command_subparsers: argparse.ArgumentParser):
+    nocodemalware_parser = command_subparsers.add_parser(
+        "nocodemalware",
+        description="Repurpose trusted execs, service accounts and cloud services to power a malware operation",
+        help="Repurpose trusted execs, service accounts and cloud services to power a malware operation.",
+    )
+    nocodemalware_parser.add_argument(
+        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
+    )
+    nocodemalware_parser = nocodemalware_parser.add_subparsers(help="nocodemalware_subcommand", dest="nocodemalware_subcommand")
+
+    module_nocodemalware_subcommand_exec(nocodemalware_parser)
+
+
+def module_nocodemalware_subcommand_exec(command_subparsers: argparse.ArgumentParser):
+    steal_fqdn_parser = command_subparsers.add_parser("steal-cookie", description="Steal cookie of fqdn")
+    steal_fqdn_parser.add_argument("--fqdn", required=True, type=str, help="Fully qualified domain name to fetch the cookies of")
+
+    command_subparsers.add_parser("steal-power-automate-token", description="Steal power automate token")
+
+    execute_command_parser = command_subparsers.add_parser("command-exec", description="Execute command on machine")
+    execute_command_parser.add_argument(
+        "-t", "--type", required=True, type=str, choices=[cmd_type.value for cmd_type in CodeExecTypeEnum], help="Command type"
+    )
+    execute_command_parser.add_argument("-c", "--command-to-execute", required=True, type=str, help="Command to execute")
+
+    ransomware_parser = command_subparsers.add_parser("ransomware", description="Ransomware")
+    ransomware_parser.add_argument("--crawl_depth", required=True, type=str, help="Recursively search into subdirectories this many times")
+    ransomware_parser.add_argument(
+        "-k", "--encryption-key", required=True, type=str, help="an encryption key used to encrypt each file identified (AES256)"
+    )
+    ransomware_parser.add_argument(
+        "--dirs", required=True, type=str, help="A list of directories to begin crawl from separated by a comma (e.g.'C:\\,D:\\')"
+    )
+
+    exfiltrate_file_parser = command_subparsers.add_parser("exfiltrate", description="Exfiltrate file")
+    exfiltrate_file_parser.add_argument("-f", "--file", required=True, type=str, help="Absolute path to file")
+
+    command_subparsers.add_parser("cleanup", description="Cleanup")
+
+
+def module_backdoor(command_subparsers: argparse.ArgumentParser):
+    backdoor_parser = command_subparsers.add_parser(
+        "backdoor", description="Install a backdoor on the target tenant.", help="Install a backdoor on the target tenant"
+    )
+    backdoor_parser.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id in powerplatform.")
+    backdoor_subparsers = backdoor_parser.add_subparsers(help="backdoor_subcommand", dest="backdoor_subcommand")
+
+    ## Delete Flow parser ##
+    delete_flow_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.delete_flow.value, description="Deletes flow.", help="Deletes flow using installed backdoor flow."
+    )
+    delete_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
+    delete_flow_parser.add_argument("-f", "--flow-id", type=str, help="Flow id to delete.")
+
+    ## Create Flow parser ##
+    create_flow_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.create_flow.value, description="Creates a flow.", help="Creates a flow using installed backdoor flow."
+    )
+    create_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
+    create_flow_parser.add_argument("-i", "--input", type=str, required=True, help="Path to flow details input file.")
+
+    ## Get connections parser ##
+    get_connections_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.get_connections.value, description="Get connections", help="Gets connections details in environment"
+    )
+    get_connections_parser.add_argument(
+        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
+    )
+    get_connections_parser.add_argument("-o", "--output", type=str, default="", help="Path to output file.")
+
+    ## backdoor installer parser ##
+    installer = backdoor_subparsers.add_parser(
+        BackdoorActionType.install_factory.value, description="Install flow factory", help="Installs flow factory in powerplatform"
+    )
+    installer.add_argument("-c", "--connection-id", required=True, type=str, help="The connection id of management connection")
+    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+
+
+def module_phishing(command_subparsers: argparse.ArgumentParser):
+    command_subparsers.add_parser("phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app.")
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-l", "--log-level", default=logging.INFO, type=lambda x: getattr(logging, x), help="Configure the logging level.")
+    command_subparsers = parser.add_subparsers(help="command", dest="command")
+
+    module_dump(command_subparsers)
+    module_gui(command_subparsers)
+    module_backdoor(command_subparsers)
+    module_nocodemalware(command_subparsers)
+    module_phishing(command_subparsers)
+
+    args = parser.parse_args()
+
+    return args
```

### Comparing `powerpwn-2.1/src/powerpwn/cli/runners.py` & `powerpwn-2.1.1/src/powerpwn/cli/runners.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/enums/str_enum.py` & `powerpwn-2.1.1/src/powerpwn/enums/str_enum.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/machinepwn/machine_pwn.py` & `powerpwn-2.1.1/src/powerpwn/machinepwn/machine_pwn.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/machinepwn/models/any_command_args.py` & `powerpwn-2.1.1/src/powerpwn/machinepwn/models/any_command_args.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/machinepwn/models/cmd_arguments.py` & `powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_arguments.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/machinepwn/models/cmd_results.py` & `powerpwn-2.1.1/src/powerpwn/machinepwn/models/cmd_results.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/machinepwn/models/ransomware_args_properties.py` & `powerpwn-2.1.1/src/powerpwn/machinepwn/models/ransomware_args_properties.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/main.py` & `powerpwn-2.1.1/src/powerpwn/main.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdoor/backdoor_flow.py` & `powerpwn-2.1.1/src/powerpwn/powerdoor/backdoor_flow.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdoor/flow_factory_installer.py` & `powerpwn-2.1.1/src/powerpwn/powerdoor/flow_factory_installer.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json` & `powerpwn-2.1.1/src/powerpwn/powerdoor/samples/flow_factory_to_install.json`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py` & `powerpwn-2.1.1/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/data_collectors/data_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/base_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/base_validator.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/base_validator.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/connection_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connection_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/connector_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/connector_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_dump_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_record_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_record_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/models/data_store_entity.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/models/data_store_entity.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/_api.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/gui.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/gui.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/prep.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/prep.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/templates/base.html` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/canvasapps_table.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/templates/connections_table.html` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connections_table.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/templates/connectors_table.html` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/connectors_table.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/gui/templates/resources_table.html` & `powerpwn-2.1.1/src/powerpwn/powerdump/gui/templates/resources_table.html`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/auth.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/auth.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/json_utils.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/model_loaders.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/model_loaders.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/path_utils.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/requests_wrapper.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn/powerdump/utils/token_cache.py` & `powerpwn-2.1.1/src/powerpwn/powerdump/utils/token_cache.py`

 * *Files identical despite different names*

### Comparing `powerpwn-2.1/src/powerpwn.egg-info/SOURCES.txt` & `powerpwn-2.1.1/src/powerpwn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

