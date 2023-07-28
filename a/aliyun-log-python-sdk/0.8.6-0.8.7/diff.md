# Comparing `tmp/aliyun-log-python-sdk-0.8.6.tar.gz` & `tmp/aliyun-log-python-sdk-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliyun-log-python-sdk-0.8.6.tar", last modified: Mon Apr 10 03:27:02 2023, max compression
+gzip compressed data, was "dist/aliyun-log-python-sdk-0.8.7.tar", last modified: Fri Jul 28 08:58:17 2023, max compression
```

## Comparing `aliyun-log-python-sdk-0.8.6.tar` & `aliyun-log-python-sdk-0.8.7.tar`

### file list

```diff
@@ -1,128 +1,127 @@
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.925645 aliyun-log-python-sdk-0.8.6/
--rw-r--r--   0 zhhfan     (502) staff       (20)     1070 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/LICENSE
--rw-r--r--   0 zhhfan     (502) staff       (20)      863 2023-04-10 03:27:02.925244 aliyun-log-python-sdk-0.8.6/PKG-INFO
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     2677 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/README.md
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.641391 aliyun-log-python-sdk-0.8.6/aliyun/
--rwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/__init__.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.799490 aliyun-log-python-sdk-0.8.6/aliyun/log/
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1648 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/__init__.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      879 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/acl_config.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1629 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/acl_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     6712 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/auth.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2784 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/common_response.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.809408 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      152 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/__init__.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     2319 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/checkpoint_tracker.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4379 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/config.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4577 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/consumer_client.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      531 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/exceptions.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      590 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/fetched_log_group.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4159 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/heart_beat.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)    11472 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/shard_worker.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     7454 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/tasks.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     8589 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/worker.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     3285 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer_group_request.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     5252 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/consumer_group_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      813 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/cursor_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      808 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/cursor_time_response.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.816082 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/
--rw-r--r--   0 zhhfan     (502) staff       (20)      171 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/__init__.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     1690 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/doc_logitem_converter.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2583 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/index_logstore_mappings.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    11037 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/mapping_index_converter.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2347 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_log.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    16932 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_manager.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      281 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     8326 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_task.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      194 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/util.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     4373 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_config_response.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.821073 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/
--rw-r--r--   0 zhhfan     (502) staff       (20)      128 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/__init__.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2301 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/config_parser.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     5370 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/etl_util.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      450 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/exceptions.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2723 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/restrict_config_parser.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     1245 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/runner.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     1422 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/settings.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.916154 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/
--rw-r--r--   0 zhhfan     (502) staff       (20)      500 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/__init__.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2523 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_base.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2031 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_csv.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    14656 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_json.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     3649 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_kv.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     9141 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_lookup.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     4051 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_mv.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     5215 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_regex.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     3704 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_set_field.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.920954 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/
--rw-r--r--   0 zhhfan     (502) staff       (20)      156 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/__init__.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     4419 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_list.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     1923 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_transform.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      903 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_util.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      145 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/transform_base.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2126 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/transform_list.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     3680 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/transform_meta.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2764 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/export_response.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.922480 aliyun-log-python-sdk-0.8.6/aliyun/log/ext/
--rwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/ext/__init__.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    13130 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/ext/jupyter_magic.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     7247 2023-03-29 01:29:33.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/ext/syslogclient.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     8125 2023-04-10 03:24:29.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/external_store_config.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     4315 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/external_store_config_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2931 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/getcontextlogsresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     3400 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/gethistogramsrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1922 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/gethistogramsresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     6186 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/getlogsrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4460 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/getlogsresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1733 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/histogram.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)    10335 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/index_config.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     2220 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/index_config_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     5180 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/ingestion_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     6360 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/job.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      407 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/listlogstoresrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1902 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/listlogstoresresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1897 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/listtopicsrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1570 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/listtopicsresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     8952 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/log_logs_pb2.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     9641 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/log_logs_raw_pb2.py
--rw-r--r--   0 zhhfan     (502) staff       (20)   203428 2023-04-10 03:24:22.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logclient.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)    12625 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logclient_core.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    39275 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logclient_operator.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1998 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logexception.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    23176 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logger_hanlder.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1922 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logitem.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      700 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1375 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     5722 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logstore_config_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)    41883 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logtail_config_detail.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4086 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/logtail_config_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     2826 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/machine_group_detail.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     9341 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/machinegroup_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2438 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/odps_sink.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2517 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/oss_sink.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     2293 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/pluralize.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     3795 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/project_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     6141 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/pulllog_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     3388 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/putlogsrequest.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)      545 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/putlogsresponse.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1247 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/queriedlog.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     9831 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/resource_params.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     7925 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/resource_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     1358 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/shard_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     4652 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/shipper_config.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     7532 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/shipper_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      358 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/sink.py
--rw-r--r--   0 zhhfan     (502) staff       (20)     1775 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/sql_instance_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     5833 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/substore_config_response.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    13437 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/topostore_params.py
--rw-r--r--   0 zhhfan     (502) staff       (20)    13619 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/topostore_response.py
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     9206 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/util.py
--rw-r--r--   0 zhhfan     (502) staff       (20)      341 2023-04-10 03:26:25.000000 aliyun-log-python-sdk-0.8.6/aliyun/log/version.py
-drwxr-xr-x   0 zhhfan     (502) staff       (20)        0 2023-04-10 03:27:02.924719 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/
--rw-r--r--   0 zhhfan     (502) staff       (20)      863 2023-04-10 03:27:02.000000 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zhhfan     (502) staff       (20)     3957 2023-04-10 03:27:02.000000 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)        1 2023-04-10 03:27:02.000000 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)       86 2023-04-10 03:27:02.000000 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/requires.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)        7 2023-04-10 03:27:02.000000 aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 zhhfan     (502) staff       (20)       38 2023-04-10 03:27:02.925789 aliyun-log-python-sdk-0.8.6/setup.cfg
--rwxr-xr-x   0 zhhfan     (502) staff       (20)     2847 2023-03-29 01:29:34.000000 aliyun-log-python-sdk-0.8.6/setup.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/
+-rw-r--r--   0 haha       (502) staff       (20)      935 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/PKG-INFO
+-rwxr-xr-x   0 haha       (502) staff       (20)     2677 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/README.md
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/
+-rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/__init__.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/
+-rwxr-xr-x   0 haha       (502) staff       (20)     1648 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/__init__.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      879 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/acl_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1629 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/acl_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     6712 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/auth.py
+-rw-r--r--   0 haha       (502) staff       (20)     2784 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/common_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/
+-rwxr-xr-x   0 haha       (502) staff       (20)      152 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/__init__.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2319 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/checkpoint_tracker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4379 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4577 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/consumer_client.py
+-rw-r--r--   0 haha       (502) staff       (20)      531 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/exceptions.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      590 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/fetched_log_group.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4159 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/heart_beat.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    11472 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/shard_worker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7454 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/tasks.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     8589 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/worker.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3285 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_request.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5252 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      813 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      808 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_time_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/
+-rw-r--r--   0 haha       (502) staff       (20)      171 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     1690 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/doc_logitem_converter.py
+-rw-r--r--   0 haha       (502) staff       (20)     2583 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/index_logstore_mappings.py
+-rw-r--r--   0 haha       (502) staff       (20)    11037 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/mapping_index_converter.py
+-rw-r--r--   0 haha       (502) staff       (20)     2347 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_log.py
+-rw-r--r--   0 haha       (502) staff       (20)    16932 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_manager.py
+-rw-r--r--   0 haha       (502) staff       (20)      281 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     8326 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_task.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      194 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/util.py
+-rw-r--r--   0 haha       (502) staff       (20)     4373 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_config_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/
+-rw-r--r--   0 haha       (502) staff       (20)      128 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     2301 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/config_parser.py
+-rw-r--r--   0 haha       (502) staff       (20)     5370 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/etl_util.py
+-rw-r--r--   0 haha       (502) staff       (20)      450 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/exceptions.py
+-rw-r--r--   0 haha       (502) staff       (20)     2723 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/restrict_config_parser.py
+-rw-r--r--   0 haha       (502) staff       (20)     1245 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/runner.py
+-rw-r--r--   0 haha       (502) staff       (20)     1422 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/settings.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/
+-rw-r--r--   0 haha       (502) staff       (20)      500 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     2523 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_base.py
+-rw-r--r--   0 haha       (502) staff       (20)     2031 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_csv.py
+-rw-r--r--   0 haha       (502) staff       (20)    14656 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_json.py
+-rw-r--r--   0 haha       (502) staff       (20)     3649 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_kv.py
+-rw-r--r--   0 haha       (502) staff       (20)     9141 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_lookup.py
+-rw-r--r--   0 haha       (502) staff       (20)     4051 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_mv.py
+-rw-r--r--   0 haha       (502) staff       (20)     5215 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_regex.py
+-rw-r--r--   0 haha       (502) staff       (20)     3704 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_set_field.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/
+-rw-r--r--   0 haha       (502) staff       (20)      156 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)     4419 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_list.py
+-rw-r--r--   0 haha       (502) staff       (20)     1923 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_transform.py
+-rw-r--r--   0 haha       (502) staff       (20)      903 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_util.py
+-rw-r--r--   0 haha       (502) staff       (20)      145 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_base.py
+-rw-r--r--   0 haha       (502) staff       (20)     2126 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_list.py
+-rw-r--r--   0 haha       (502) staff       (20)     3680 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_meta.py
+-rw-r--r--   0 haha       (502) staff       (20)     2764 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/export_response.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/
+-rwxr-xr-x   0 haha       (502) staff       (20)        0 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/__init__.py
+-rw-r--r--   0 haha       (502) staff       (20)    13130 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/jupyter_magic.py
+-rw-r--r--   0 haha       (502) staff       (20)     7247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ext/syslogclient.py
+-rw-r--r--   0 haha       (502) staff       (20)     8125 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config.py
+-rw-r--r--   0 haha       (502) staff       (20)     4315 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     2931 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getcontextlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3400 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7154 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     6297 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1733 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/histogram.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    10335 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/index_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2220 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/index_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     5180 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/ingestion_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     6360 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/job.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      407 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1902 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1897 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1570 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     8952 2023-07-28 08:41:13.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_pb2.py
+-rw-r--r--   0 haha       (502) staff       (20)     9641 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_raw_pb2.py
+-rw-r--r--   0 haha       (502) staff       (20)   207442 2023-07-28 08:41:25.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    12625 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_core.py
+-rw-r--r--   0 haha       (502) staff       (20)    39270 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_operator.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1998 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logexception.py
+-rw-r--r--   0 haha       (502) staff       (20)    23176 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logger_hanlder.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1922 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logitem.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      700 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1375 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5722 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logstore_config_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)    41883 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_detail.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4086 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     2826 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/machine_group_detail.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     9341 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/machinegroup_response.py
+-rw-r--r--   0 haha       (502) staff       (20)     2438 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/odps_sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     2517 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/oss_sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     2293 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/pluralize.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3795 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/project_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     6141 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/pulllog_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     3388 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsrequest.py
+-rwxr-xr-x   0 haha       (502) staff       (20)      545 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsresponse.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1247 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/queriedlog.py
+-rw-r--r--   0 haha       (502) staff       (20)     9831 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/resource_params.py
+-rw-r--r--   0 haha       (502) staff       (20)     7925 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/resource_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     1358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shard_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     4652 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_config.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     7532 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_response.py
+-rw-r--r--   0 haha       (502) staff       (20)      358 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/sink.py
+-rw-r--r--   0 haha       (502) staff       (20)     1775 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/sql_instance_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     5833 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/substore_config_response.py
+-rw-r--r--   0 haha       (502) staff       (20)    13437 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_params.py
+-rw-r--r--   0 haha       (502) staff       (20)    13619 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_response.py
+-rwxr-xr-x   0 haha       (502) staff       (20)     9206 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/util.py
+-rw-r--r--   0 haha       (502) staff       (20)      341 2023-07-28 08:58:04.000000 aliyun-log-python-sdk-0.8.7/aliyun/log/version.py
+drwxr-xr-x   0 haha       (502) staff       (20)        0 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/
+-rw-r--r--   0 haha       (502) staff       (20)      935 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haha       (502) staff       (20)     3949 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haha       (502) staff       (20)        1 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haha       (502) staff       (20)       86 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 haha       (502) staff       (20)        7 2023-07-28 08:58:16.000000 aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haha       (502) staff       (20)       38 2023-07-28 08:58:17.000000 aliyun-log-python-sdk-0.8.7/setup.cfg
+-rwxr-xr-x   0 haha       (502) staff       (20)     2847 2023-06-07 06:09:47.000000 aliyun-log-python-sdk-0.8.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aliyun-log-python-sdk-0.8.6/PKG-INFO` & `aliyun-log-python-sdk-0.8.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: aliyun-log-python-sdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Aliyun log service Python client SDK
 Home-page: https://github.com/aliyun/aliyun-log-python-sdk
 Author: Aliyun
+Author-email: UNKNOWN
+License: UNKNOWN
+Description: 
+        Python SDK for Alicloud Log Service 
+        http://aliyun-log-python-sdk.readthedocs.io
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-License-File: LICENSE
-
-
-Python SDK for Alicloud Log Service 
-http://aliyun-log-python-sdk.readthedocs.io
```

### Comparing `aliyun-log-python-sdk-0.8.6/README.md` & `aliyun-log-python-sdk-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/__init__.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/__init__.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/acl_config.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/acl_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/acl_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/acl_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/auth.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/auth.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/common_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/common_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/checkpoint_tracker.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/checkpoint_tracker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/config.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/consumer_client.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/consumer_client.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/exceptions.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/exceptions.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/fetched_log_group.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/fetched_log_group.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/heart_beat.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/heart_beat.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/shard_worker.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/shard_worker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/tasks.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer/worker.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer/worker.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer_group_request.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_request.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/consumer_group_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/consumer_group_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/cursor_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/cursor_time_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/cursor_time_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/doc_logitem_converter.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/doc_logitem_converter.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/index_logstore_mappings.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/index_logstore_mappings.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/mapping_index_converter.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/mapping_index_converter.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_log.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_log.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_manager.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_manager.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/es_migration/migration_task.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/es_migration/migration_task.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/config_parser.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/config_parser.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/etl_util.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/etl_util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/restrict_config_parser.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/restrict_config_parser.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/runner.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/runner.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/settings.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/settings.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_base.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_base.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_csv.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_csv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_json.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_json.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_kv.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_kv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_lookup.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_lookup.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_mv.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_mv.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_regex.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_regex.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/trans_comp/trans_set_field.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/trans_comp/trans_set_field.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_list.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_list.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_transform.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_transform.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/condition_util.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/condition_util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/transform_list.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_list.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/etl_core/transform/transform_meta.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/etl_core/transform/transform_meta.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/export_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/export_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/ext/jupyter_magic.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/ext/jupyter_magic.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/ext/syslogclient.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/ext/syslogclient.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/external_store_config.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/external_store_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/external_store_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/getcontextlogsresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/getcontextlogsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/gethistogramsrequest.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/gethistogramsresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/gethistogramsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/getlogsrequest.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,28 +35,36 @@
     :param offset: line offset of return logs
     
     :type reverse: bool
     :param reverse: if reverse is set to true, the query will return the latest logs first
 
     :type power_sql: bool
     :param power_sql: if power_sql is set to true, the query will run on enhanced sql mode
+
+    :type scan: bool
+    :param scan: if scan is set to true, the query will use scan mode
+
+    :type forward: bool
+    :param forward: only for scan query, if forward is set to true, the query will get next page, otherwise previous page
     """
 
     def __init__(self, project=None, logstore=None, fromTime=None, toTime=None, topic=None,
-                 query=None, line=100, offset=0, reverse=False, power_sql=False):
+                 query=None, line=100, offset=0, reverse=False, power_sql=False, scan=False, forward=True):
         LogRequest.__init__(self, project)
         self.logstore = logstore
         self.fromTime = fromTime
         self.toTime = toTime
         self.topic = topic
         self.query = query
         self.line = line
         self.offset = offset
         self.reverse = reverse
         self.power_sql = power_sql
+        self.scan = scan
+        self.forward = forward
 
     def get_logstore(self):
         """ Get logstore name
         
         :return: string, logstore name
         """
         return self.logstore if self.logstore else ''
@@ -185,14 +193,43 @@
         """ Set request power_sql flag
 
         :type power_sql: bool
         :param power_sql: power_sql flag
         """
         self.power_sql = power_sql
 
+    def get_scan(self):
+        """ Get request scan flag
+
+        :return: bool, scan flag
+        """
+        return self.scan
+
+    def set_scan(self, scan):
+        """ Set request scan flag
+
+        :type scan: bool
+        :param scan: scan flag
+        """
+        self.scan = scan
+
+    def get_forward(self):
+        """ Get request forward flag
+
+        :return: bool, forward flag
+        """
+        return self.forward
+
+    def set_forward(self, forward):
+        """ Set request forward flag
+
+        :type forward: bool
+        :param forward: scan flag
+        """
+        self.forward = forward
 
 class GetProjectLogsRequest(LogRequest):
     """ The request used to get logs by a query from log cross multiple logstores.
 
     :type project: string
     :param project: project name
```

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/getlogsresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/getlogsresponse.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,37 +5,56 @@
 # All rights reserved.
 
 from .logresponse import LogResponse
 from .queriedlog import QueriedLog
 from .logexception import LogException
 import six
 from .util import Util
+from enum import Enum
+import json
 
 
 class GetLogsResponse(LogResponse):
     """ The response of the GetLog API from log.
     
     :type resp: dict
     :param resp: GetLogsResponse HTTP response body
     
     :type header: dict
     :param header: GetLogsResponse HTTP response header
     """
 
+    class QueryMode(Enum):
+        """ The enum of query type"""
+        NORMAL = 0
+        PHRASE = 1
+        SCAN = 2
+        SCAN_SQL = 3
+
     def __init__(self, resp, header):
         LogResponse.__init__(self, header, resp)
         try:
             self.progress = Util.h_v_t(header, 'x-log-progress')
             self.processed_rows = Util.h_v_td(header, 'x-log-processed-rows', '0')
             self.elapsed_mills = Util.h_v_td(header, 'x-log-elapsed-millisecond', '0')
             self.has_sql = Util.h_v_td(header, 'x-log-has-sql', 'False')
             self.where_query = Util.h_v_td(header, 'x-log-where-query', '')
             self.agg_query = Util.h_v_td(header, 'x-log-agg-query', '')
             self.cpu_sec = Util.h_v_td(header, 'x-log-cpu-sec', '0')
             self.cpu_cores = Util.h_v_td(header, 'x-log-cpu-cores', '0')
+            query_info_str = Util.h_v_td(header, 'x-log-query-info', '')
+            query_info = json.loads(query_info_str)
+            self.query_mode = GetLogsResponse.QueryMode(Util.h_v_td(query_info, 'mode', 0))
+            if self.query_mode is GetLogsResponse.QueryMode.SCAN or self.query_mode is GetLogsResponse.QueryMode.SCAN_SQL:
+                self.scan_bytes = Util.h_v_td(query_info, 'scanBytes', 0)
+            if self.query_mode is GetLogsResponse.QueryMode.PHRASE or self.query_mode is GetLogsResponse.QueryMode.SCAN:
+                scan_query_info = Util.h_v_td(query_info, 'phraseQueryInfo', dict())
+                self.scan_all = Util.h_v_td(scan_query_info, 'scanAll', 'false')
+                self.begin_offset = Util.h_v_td(scan_query_info, 'beginOffset', '0')
+                self.end_offset = Util.h_v_td(scan_query_info, 'endOffset', '0')
             self.logs = []
             for data in resp:
                 contents = {}
                 source = ""
                 if "__source__" in data:
                     source = data['__source__']
 
@@ -117,14 +136,49 @@
     def get_cpu_cores(self):
         """ Get cpu cores used from the response
 
         :return: cpu_cores
         """
         return self.cpu_cores
 
+    def get_query_mode(self):
+        """ Get query_mode from the response
+
+        :return: query_mode
+        """
+        return self.query_mode
+
+    def get_scan_bytes(self):
+        """ Get scan_bytes from the response
+
+        :return: scan_bytes
+        """
+        return self.scan_bytes
+
+    def get_begin_offset(self):
+        """ Get begin_offset from the response
+
+        :return: begin_offset
+        """
+        return self.begin_offset
+
+    def get_end_offset(self):
+        """ Get end_offset from the response
+
+        :return: end_offset
+        """
+        return self.end_offset
+
+    def get_scan_all(self):
+        """ Get scan_all from the response
+
+        :return: scan_all
+        """
+        return self.scan_all
+
     def log_print(self):
         print('GetLogsResponse:')
         print('headers:', self.get_all_headers())
         print('count:', self.get_count())
         print('progress:', self.progress)
         print('\nQueriedLog class:\n')
         for log in self.logs:
```

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/histogram.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/histogram.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/index_config.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/index_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/index_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/index_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/ingestion_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/ingestion_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/job.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/job.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/listlogstoresresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/listlogstoresresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/listtopicsrequest.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/listtopicsresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/listtopicsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/log_logs_pb2.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_pb2.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/log_logs_raw_pb2.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/log_logs_raw_pb2.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logclient.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 import json
 import requests
 import six
 import time
 import zlib
 from datetime import datetime
 import logging
-import locale
 from itertools import cycle
-from .acl_response import *
 from .consumer_group_request import *
 from .consumer_group_response import *
 from .getlogsrequest import *
 from .cursor_response import GetCursorResponse
 from .cursor_time_response import GetCursorTimeResponse
 from .gethistogramsresponse import GetHistogramsResponse
 from .getlogsresponse import GetLogsResponse
 from .getcontextlogsresponse import GetContextLogsResponse
 from .index_config_response import *
 from .ingestion_response import *
 from .sql_instance_response import *
 from .listlogstoresresponse import ListLogstoresResponse
 from .listtopicsresponse import ListTopicsResponse
-from .logclient_core import make_lcrud_methods
 from .logclient_operator import copy_project, list_more, query_more, pull_log_dump, copy_logstore, copy_data, \
     get_resource_usage, arrange_shard, transform_data
 from .logexception import LogException
 from .logstore_config_response import *
 from .substore_config_response import *
 from .logtail_config_response import *
 from .machinegroup_response import *
@@ -41,20 +38,19 @@
 from .putlogsresponse import PutLogsResponse
 from .shard_response import *
 from .shipper_response import *
 from .resource_response import *
 from .resource_params import *
 from .topostore_response import *
 from .topostore_params import *
-from .util import Util, parse_timestamp, base64_encodestring as b64e, is_stats_query
-from .util import base64_encodestring as e64, base64_decodestring as d64, oss_sink_deserialize, maxcompute_sink_deserialize, export_deserialize
+from .util import base64_encodestring as b64e
+from .util import base64_encodestring as e64, base64_decodestring as d64
 from .version import API_VERSION, USER_AGENT
 
 from .log_logs_raw_pb2 import LogGroupRaw as LogGroup
-from .external_store_config import ExternalStoreConfig
 from .external_store_config_response import *
 import struct
 from .logresponse import LogResponse
 from copy import copy
 from .pluralize import pluralize
 from .etl_config_response import *
 from .export_response import *
@@ -544,15 +540,15 @@
         logstore = request.get_logstore()
         project = request.get_project()
         resource = "/logstores/" + logstore
         (resp, header) = self._send("GET", project, None, resource, params, headers)
         return GetHistogramsResponse(resp, header)
 
     def get_log(self, project, logstore, from_time, to_time, topic=None,
-                query=None, reverse=False, offset=0, size=100, power_sql=False):
+                query=None, reverse=False, offset=0, size=100, power_sql=False, scan=False, forward=True):
         """ Get logs from log service.
         will retry DEFAULT_QUERY_RETRY_COUNT when incomplete.
         Unsuccessful operation will cause an LogException.
         Note: for larger volume of data (e.g. > 1 million logs), use get_log_all
 
         :type project: string
         :param project: project name
@@ -580,24 +576,42 @@
 
         :type size: int
         :param size: max line number of return logs, -1 means get all
 
         :type power_sql: bool
         :param power_sql: if power_sql is set to true, the query will run on enhanced sql mode
 
+        :type scan: bool
+        :param scan: if scan is set to true, the query will use scan mode
+
+        :type forward: bool
+        :param forward: only for scan query, if forward is set to true, the query will get next page, otherwise previous page
+
         :return: GetLogsResponse
 
         :raise: LogException
         """
 
-        # need to use extended method to get more when: it's not select query, and size > default page size
-        if not is_stats_query(query) and (int(size) == -1 or int(size) > MAX_GET_LOG_PAGING_SIZE):
-            return query_more(self.get_log, int(offset), int(size), MAX_GET_LOG_PAGING_SIZE,
-                              project, logstore, from_time, to_time, topic,
-                              query, reverse)
+        # need to use extended method to get more when:
+        # it's not select query, and size > default page size
+        size, offset = int(size), int(offset)
+        if not is_stats_query(query) and (size == -1 or size > MAX_GET_LOG_PAGING_SIZE):
+            return query_more(
+                self.get_log,
+                offset=offset,
+                size=size,
+                batch_size=MAX_GET_LOG_PAGING_SIZE,
+                project=project,
+                logstore=logstore,
+                from_time=from_time,
+                to_time=to_time,
+                topic=topic,
+                query=query,
+                reverse=reverse,
+            )
 
         ret = None
         for _c in xrange(DEFAULT_QUERY_RETRY_COUNT):
             headers = {}
             params = {'from': parse_timestamp(from_time),
                       'to': parse_timestamp(to_time),
                       'type': 'log',
@@ -606,14 +620,17 @@
                       'reverse': 'true' if reverse else 'false',
                       'powerSql': power_sql}
 
             if topic:
                 params['topic'] = topic
             if query:
                 params['query'] = query
+            if scan:
+                params['session'] = 'mode=scan'
+                params['forward'] = 'true' if forward else 'false'
 
             resource = "/logstores/" + logstore
             (resp, header) = self._send("GET", project, None, resource, params, headers)
             ret = GetLogsResponse(resp, header)
             if ret.is_completed():
                 break
 
@@ -640,17 +657,19 @@
         to_time = request.get_to()
         topic = request.get_topic()
         query = request.get_query()
         reverse = request.get_reverse()
         offset = request.get_offset()
         size = request.get_line()
         power_sql = request.get_power_sql()
+        scan = request.get_scan()
+        forward = request.get_forward()
 
         return self.get_log(project, logstore, from_time, to_time, topic,
-                            query, reverse, offset, size, power_sql)
+                            query, reverse, offset, size, power_sql, scan, forward)
 
     def get_log_all(self, project, logstore, from_time, to_time, topic=None,
                     query=None, reverse=False, offset=0, power_sql=False):
         """ Get logs from log service. will retry when incomplete.
         Unsuccessful operation will cause an LogException. different with `get_log` with size=-1,
         It will try to iteratively fetch all data every 100 items and yield them, in CLI, it could apply jmes filter to
         each batch and make it possible to fetch larger volume of data.
@@ -694,14 +713,81 @@
 
             count = response.get_count()
             offset += count
 
             if count == 0 or is_stats_query(query):
                 break
 
+    def get_log_all_v2(self, project, logstore, from_time, to_time, topic=None,
+                    query=None, reverse=False, offset=0, power_sql=False, scan=False, forward=True):
+        """ FOR PHRASE AND SCAN WHERE.
+                Get logs from log service. will retry when incomplete.
+                Unsuccessful operation will cause an LogException. different with `get_log` with size=-1,
+                It will try to iteratively fetch all data every 100 items and yield them, in CLI, it could apply jmes filter to
+                each batch and make it possible to fetch larger volume of data.
+
+                :type project: string
+                :param project: project name
+
+                :type logstore: string
+                :param logstore: logstore name
+
+                :type from_time: int/string
+                :param from_time: the begin timestamp or format of time in readable time like "%Y-%m-%d %H:%M:%S<time_zone>" e.g. "2018-01-02 12:12:10+8:00", also support human readable string, e.g. "1 hour ago", "now", "yesterday 0:0:0", refer to https://aliyun-log-cli.readthedocs.io/en/latest/tutorials/tutorial_human_readable_datetime.html
+
+                :type to_time: int/string
+                :param to_time: the end timestamp or format of time in readable time like "%Y-%m-%d %H:%M:%S<time_zone>" e.g. "2018-01-02 12:12:10+8:00", also support human readable string, e.g. "1 hour ago", "now", "yesterday 0:0:0", refer to https://aliyun-log-cli.readthedocs.io/en/latest/tutorials/tutorial_human_readable_datetime.html
+
+                :type topic: string
+                :param topic: topic name of logs, could be None
+
+                :type query: string
+                :param query: user defined query, could be None
+
+                :type reverse: bool
+                :param reverse: if reverse is set to true, the query will return the latest logs first, default is false
+
+                :type offset: int
+                :param offset: offset to start, by default is 0
+
+                :type power_sql: bool
+                :param power_sql: if power_sql is set to true, the query will run on enhanced sql mode
+
+                :type scan: bool
+                :param scan: if scan is set to true, the query will use scan mode
+
+                :type forward: bool
+                :param forward: only for scan query, if forward is set to true, the query will get next page, otherwise previous page
+
+                :return: GetLogsResponse iterator
+
+                :raise: LogException
+                """
+        while True:
+            response = self.get_log(project, logstore, from_time, to_time, topic=topic,
+                                    query=query, reverse=reverse, offset=offset, size=100, power_sql=power_sql,
+                                    scan=scan, forward=forward)
+
+            yield response
+
+            count = response.get_count()
+            query_mode = response.get_query_mode()
+            scan_all = False
+            if query_mode is GetLogsResponse.QueryMode.NORMAL or query_mode is GetLogsResponse.QueryMode.SCAN_SQL:
+                offset += count
+            else:
+                scan_all = (response.get_scan_all() == 'true')
+                if forward:
+                    offset = response.get_end_offset()
+                else:
+                    offset = response.get_begin_offset()
+
+            if count == 0 or is_stats_query(query) or scan_all:
+                break
+
     def execute_logstore_sql(self, project, logstore, from_time, to_time, sql, power_sql):
         """ Execute SQL from log service.
         will retry DEFAULT_QUERY_RETRY_COUNT when incomplete.
         Unsuccessful operation will cause an LogException.
 
         :type project: string
         :param project: project name
@@ -4304,15 +4390,15 @@
             raise TypeError("node_id type must be str, got %s" % type(node_id))
         headers = {}
         params = {}
         resource = "/topostores/" + topostore_name + "/nodes/" + node_id
         (resp, header) = self._send("GET", None, None, resource, params, headers)
         return GetTopostoreNodeResponse(header, resp)
 
-    def list_topostore_node(self, topostore_name, node_ids=None, node_types=None, property_key=None, 
+    def list_topostore_node(self, topostore_name, node_ids=None, node_types=None, property_key=None,
                 property_value=None, offset=0, size=100):
         """list Topostore nodes
         Unsuccessful operation will cause an LogException.
 
         :type topostore_name: string
         :param topostore_name: topostore name
 
@@ -4344,15 +4430,15 @@
         if node_types and not isinstance(node_types, list):
             raise TypeError("node_types must be list of string")
 
         if node_types and isinstance(node_types, list):
             for node_type in node_types:
                 if not isinstance(node_type, str):
                     raise TypeError("node_types must be list of string")
-            
+
         if property_key and not isinstance(property_key, str):
             raise TypeError("property_key must be str")
 
         if property_value and not isinstance(property_value, str):
             raise TypeError("property_value must be str")
 
         if not (isinstance(size, int) and isinstance(offset, int)):
@@ -4492,15 +4578,15 @@
             raise TypeError("relation_id type must be str")
         headers = {}
         params = {}
         resource = "/topostores/" + topostore_name + "/relations/" + relation_id
         (resp, header) = self._send("GET", None, None, resource, params, headers)
         return GetTopostoreRelationResponse(header, resp)
 
-    def list_topostore_relation(self, topostore_name, relation_ids=None, relation_types=None, 
+    def list_topostore_relation(self, topostore_name, relation_ids=None, relation_types=None,
             src_node_ids=None, dst_node_ids=None,
             property_key=None, property_value=None, offset=0, size=100):
         """list Topostore relationss
         Unsuccessful operation will cause an LogException.
 
         :type topostore_name: string
         :param topostore_name: topostore name
@@ -4534,15 +4620,15 @@
             raise TypeError("resource_name type must be str")
 
         if relation_ids and not isinstance(relation_ids, list):
             raise TypeError("relation_ids type must be list,element is relation id which type is str")
 
         if relation_types and not isinstance(relation_types, list):
             raise TypeError("relation_types must be list of string")
-        
+
         if relation_types and isinstance(relation_types, list):
             for relation_type in relation_types:
                 if not isinstance(relation_type, str):
                     raise TypeError("relation_types must be list of string")
 
         if src_node_ids and not isinstance(src_node_ids, list):
             raise TypeError("src_node_ids must be list of string")
@@ -4570,15 +4656,15 @@
         headers = {}
         params = {"offset": offset, "size": size}
         if relation_ids is not None:
             params["relationIds"] = ','.join(relation_ids)
 
         if relation_types is not None:
             params["relationTypes"] = ",".join(relation_types)
-    
+
         if src_node_ids is not None:
             params["srcNodeIds"] = ",".join(src_node_ids)
 
         if dst_node_ids is not None:
             params["dstNodeIds"] = ",".join(dst_node_ids)
 
         if property_key is not None:
```

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logclient_core.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_core.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logclient_operator.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logclient_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,28 +335,27 @@
 
         if count == 0 or offset >= total or total_count_got >= expected_total_size:
             break
 
     return response
 
 
-def query_more(fn, offset, size, batch_size, *args):
+def query_more(fn, offset=0, size=100, batch_size=100, **kwargs):
     """list all data using the fn
     """
     if size < 0:
         expected_total_size = six.MAXSIZE
     else:
         expected_total_size = size
         batch_size = min(size, batch_size)
 
     response = None
     total_count_got = 0
-    complete = False
     while True:
-        ret = fn(*args, offset=offset, size=batch_size)
+        ret = fn(offset=offset, size=batch_size, **kwargs)
 
         if response is None:
             response = ret
         else:
             response.merge(ret)
 
         # if incompete, exit
```

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logexception.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logexception.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logger_hanlder.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logger_hanlder.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logitem.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logitem.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logrequest.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logstore_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logstore_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logtail_config_detail.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_detail.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/logtail_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/logtail_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/machine_group_detail.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/machine_group_detail.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/machinegroup_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/machinegroup_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/odps_sink.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/odps_sink.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/oss_sink.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/oss_sink.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/pluralize.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/pluralize.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/project_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/project_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/pulllog_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/pulllog_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/putlogsrequest.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsrequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/putlogsresponse.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/putlogsresponse.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/queriedlog.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/queriedlog.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/resource_params.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/resource_params.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/resource_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/resource_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/shard_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/shard_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/shipper_config.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_config.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/shipper_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/shipper_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/sql_instance_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/sql_instance_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/substore_config_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/substore_config_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/topostore_params.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_params.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/topostore_response.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/topostore_response.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun/log/util.py` & `aliyun-log-python-sdk-0.8.7/aliyun/log/util.py`

 * *Files identical despite different names*

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/PKG-INFO` & `aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: aliyun-log-python-sdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Aliyun log service Python client SDK
 Home-page: https://github.com/aliyun/aliyun-log-python-sdk
 Author: Aliyun
+Author-email: UNKNOWN
+License: UNKNOWN
+Description: 
+        Python SDK for Alicloud Log Service 
+        http://aliyun-log-python-sdk.readthedocs.io
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-License-File: LICENSE
-
-
-Python SDK for Alicloud Log Service 
-http://aliyun-log-python-sdk.readthedocs.io
```

### Comparing `aliyun-log-python-sdk-0.8.6/aliyun_log_python_sdk.egg-info/SOURCES.txt` & `aliyun-log-python-sdk-0.8.7/aliyun_log_python_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 aliyun/__init__.py
 aliyun/log/__init__.py
 aliyun/log/acl_config.py
 aliyun/log/acl_response.py
 aliyun/log/auth.py
```

### Comparing `aliyun-log-python-sdk-0.8.6/setup.py` & `aliyun-log-python-sdk-0.8.7/setup.py`

 * *Files identical despite different names*

