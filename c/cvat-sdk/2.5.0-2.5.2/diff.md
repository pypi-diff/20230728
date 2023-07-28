# Comparing `tmp/cvat_sdk-2.5.0.tar.gz` & `tmp/cvat_sdk-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.5.0.tar", last modified: Thu Jul  6 08:16:05 2023, max compression
+gzip compressed data, was "cvat_sdk-2.5.2.tar", last modified: Fri Jul 28 10:56:23 2023, max compression
```

## Comparing `cvat_sdk-2.5.0.tar` & `cvat_sdk-2.5.2.tar`

### file list

```diff
@@ -1,248 +1,265 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.667215 cvat_sdk-2.5.0/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.667215 cvat_sdk-2.5.0/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      765 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.677215 cvat_sdk-2.5.0/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16495 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/assets_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45480 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    60871 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31386 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15031 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    22684 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/guides_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30701 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    31876 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    92132 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    26738 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    34059 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24995 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    29846 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    75121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    53044 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/quality_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10671 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21215 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   131653 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    30199 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    65406 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45517 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.677215 cvat_sdk-2.5.0/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1886 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19675 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5130 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13040 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15098 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15326 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12458 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14274 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13110 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13967 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14122 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13016 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15638 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13891 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/asset_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14197 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13993 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12610 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12645 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14270 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14110 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13572 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13021 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13137 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_content.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17473 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15486 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18326 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14307 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12656 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12741 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14280 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16403 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33480 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13646 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14274 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18296 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18847 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12986 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18729 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13184 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12819 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13642 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_selection_method_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15273 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_params.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17192 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13365 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14394 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12805 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16023 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14032 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12588 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16286 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23239 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15462 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13211 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13201 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13014 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17142 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17308 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14502 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14750 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14730 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14899 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18092 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18332 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15749 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16060 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12588 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12979 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14973 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17614 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12609 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/null_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12581 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13333 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15532 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13860 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13701 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13672 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13566 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13536 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13505 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13671 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13626 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_report_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13656 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_settings_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13717 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13431 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13632 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12415 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13145 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18253 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12395 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12416 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12864 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13067 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13340 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16558 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14785 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12512 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13895 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16057 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14843 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    21878 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_quality_settings_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16207 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14830 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16214 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14960 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13267 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19348 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14942 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16022 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13745 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12974 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15891 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12349 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_create_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15289 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12849 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_target.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    22442 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_settings.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13361 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14359 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12296 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13298 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12262 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_id.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13562 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13283 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12889 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/severity_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13951 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12297 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13428 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13334 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12954 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13072 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17566 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17735 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15223 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15463 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15277 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15412 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16289 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14336 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12350 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24013 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14930 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17121 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12726 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12253 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16247 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17569 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12664 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16430 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18524 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12989 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15740 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84564 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16348 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14473 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.697215 cvat_sdk-2.5.0/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11415 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-06 08:15:36.000000 cvat_sdk-2.5.0/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)    10785 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-06 08:16:05.000000 cvat_sdk-2.5.0/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.5.0/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-07-06 08:15:35.000000 cvat_sdk-2.5.0/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.5.0/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-06 08:16:05.707215 cvat_sdk-2.5.0/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2751 2023-07-06 08:15:35.000000 cvat_sdk-2.5.0/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.402330 cvat_sdk-2.5.2/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.5.2/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-28 10:56:23.402330 cvat_sdk-2.5.2/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.5.2/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.363246 cvat_sdk-2.5.2/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.363246 cvat_sdk-2.5.2/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.363246 cvat_sdk-2.5.2/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      508 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13086 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/analytics_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16497 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/assets_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45482 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    60873 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31388 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15033 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22686 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/guides_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30703 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    31878 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    92134 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    26740 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    34061 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24997 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    29848 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    75123 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    53046 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/quality_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    10673 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21217 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   131655 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    30201 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    65408 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45634 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.363246 cvat_sdk-2.5.2/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1957 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14402 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/analytics_report.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12965 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/analytics_report_create_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13058 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/analytics_report_target_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15100 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_conflict.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15328 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_conflict_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_guide_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13112 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_guide_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13969 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14124 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id_shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13893 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/asset_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14175 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13942 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13955 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/binary_operation.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13023 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13139 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_content.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17475 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15488 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14309 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14282 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12508 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/data_frame.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16405 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33482 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12966 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/default_view_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18731 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12821 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13071 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/frame_selection_method_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15275 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13576 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call_params.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17194 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12978 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/granularity_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13367 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14396 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16025 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23241 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13203 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13016 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17144 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13540 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12981 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14975 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15176 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/metric.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14138 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/metric_granularity.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12611 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/null_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13335 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13063 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/operator_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15534 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13703 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13628 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_quality_report_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13658 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_quality_settings_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13147 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    21880 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_quality_settings_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19350 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13747 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12976 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15893 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12351 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_create_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15291 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12851 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_target.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    22444 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_settings.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13300 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12264 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_id.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13285 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12891 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/severity_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13953 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13430 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12956 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13123 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24015 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12844 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/transformation.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15184 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/transformation_binary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12666 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16432 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18526 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12991 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84700 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17411 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14269 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14651 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/core/utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/datasets/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      231 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/datasets/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11415 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/datasets/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1153 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/datasets/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5574 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/datasets/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.392330 cvat_sdk-2.5.2/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      441 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      590 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4304 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4336 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2921 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-07-28 10:55:52.000000 cvat_sdk-2.5.2/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.402330 cvat_sdk-2.5.2/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-07-28 10:56:23.000000 cvat_sdk-2.5.2/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11517 2023-07-28 10:56:23.000000 cvat_sdk-2.5.2/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-07-28 10:56:23.000000 cvat_sdk-2.5.2/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-07-28 10:56:23.000000 cvat_sdk-2.5.2/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-07-28 10:56:23.000000 cvat_sdk-2.5.2/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.5.2/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-28 10:56:23.402330 cvat_sdk-2.5.2/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-07-28 10:55:51.000000 cvat_sdk-2.5.2/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.5.2/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-07-28 10:56:23.402330 cvat_sdk-2.5.2/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-07-28 10:55:51.000000 cvat_sdk-2.5.2/setup.py
```

### Comparing `cvat_sdk-2.5.0/PKG-INFO` & `cvat_sdk-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.5.0
+Version: 2.5.2
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.5.0/README.md` & `cvat_sdk-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.5.0"
+__version__ = "2.5.2"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/assets_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/comments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/guides_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/guides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/issues_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/labels_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/quality_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/quality_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/schema_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -65,14 +65,15 @@
 
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
     Class members:
 
+    analytics_api: AnalyticsApi
     assets_api: AssetsApi
     auth_api: AuthApi
     cloudstorages_api: CloudstoragesApi
     comments_api: CommentsApi
     events_api: EventsApi
     guides_api: GuidesApi
     invitations_api: InvitationsApi
@@ -113,15 +114,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.5.0'
+        self.user_agent = 'cvat_sdk/2.5.2'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -718,14 +719,15 @@
             queries.append((auth_setting['key'], auth_setting['value']))
         else:
             raise ApiValueError(
                 'Authentication token must be in `query` or `header`'
             )
 
 
+    analytics_api: 'AnalyticsApi'
     assets_api: 'AssetsApi'
     auth_api: 'AuthApi'
     cloudstorages_api: 'CloudstoragesApi'
     comments_api: 'CommentsApi'
     events_api: 'EventsApi'
     guides_api: 'GuidesApi'
     invitations_api: 'InvitationsApi'
@@ -740,14 +742,15 @@
     schema_api: 'SchemaApi'
     server_api: 'ServerApi'
     tasks_api: 'TasksApi'
     users_api: 'UsersApi'
     webhooks_api: 'WebhooksApi'
 
     _apis: typing.Dict[str, object] = { 
+        'analytics_api': [None, 'AnalyticsApi'],
         'assets_api': [None, 'AssetsApi'],
         'auth_api': [None, 'AuthApi'],
         'cloudstorages_api': [None, 'CloudstoragesApi'],
         'comments_api': [None, 'CommentsApi'],
         'events_api': [None, 'EventsApi'],
         'guides_api': [None, 'GuidesApi'],
         'invitations_api': [None, 'InvitationsApi'],
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/apis/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from cvat_sdk.api_client.api.assets_api import AssetsApi
+#   from cvat_sdk.api_client.api.analytics_api import AnalyticsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
+from cvat_sdk.api_client.api.analytics_api import AnalyticsApi
 from cvat_sdk.api_client.api.assets_api import AssetsApi
 from cvat_sdk.api_client.api.auth_api import AuthApi
 from cvat_sdk.api_client.api.cloudstorages_api import CloudstoragesApi
 from cvat_sdk.api_client.api.comments_api import CommentsApi
 from cvat_sdk.api_client.api.events_api import EventsApi
 from cvat_sdk.api_client.api.guides_api import GuidesApi
 from cvat_sdk.api_client.api.invitations_api import InvitationsApi
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import copy
 import logging
 import multiprocessing
@@ -484,16 +484,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.6\n"\
-               "SDK Package Version: 2.5.0".\
+               "Version of the API: 2.5.2\n"\
+               "SDK Package Version: 2.5.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_conflict.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_conflict_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_conflict_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_guide_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_guide_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_guide_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_shape_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id_shape_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotation_id_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotation_id_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/asset_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/asset_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -73,14 +73,15 @@
 
     input_type: InputTypeEnum # noqa: E501
     """
     """
 
     default_value: str # noqa: E501
     """
+    [optional]
     """
 
     values: typing.List[str] # noqa: E501
     """
     [str]
     """
 
@@ -95,20 +96,20 @@
     Attributes:
       name (str):
 
       mutable (bool):
 
       input_type (InputTypeEnum):
 
-      default_value (str):
-
       values ([str]):
 
       id (int): [optional]  # noqa: E501
 
+      default_value (str): [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -158,55 +159,56 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'mutable': (bool,),  # noqa: E501
             'input_type': (InputTypeEnum,),  # noqa: E501
-            'default_value': (str,),  # noqa: E501
             'values': ([str],),  # noqa: E501
             'id': (int,),  # noqa: E501
+            'default_value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'mutable': 'mutable',  # noqa: E501
         'input_type': 'input_type',  # noqa: E501
-        'default_value': 'default_value',  # noqa: E501
         'values': 'values',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'default_value': 'default_value',  # noqa: E501
     }
 
     read_only_vars = {
         'id',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, mutable, input_type, default_value, values, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, name, mutable, input_type, values, *args, **kwargs):  # noqa: E501
         """Attribute - a model defined in OpenAPI
 
         Args:
             name (str):
             mutable (bool):
             input_type (InputTypeEnum):
-            default_value (str):
             values ([str]):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
+            default_value (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -264,15 +266,14 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.mutable = mutable
         self.input_type = input_type
-        self.default_value = default_value
         self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -286,27 +287,28 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, mutable, input_type, default_value, values, *args, **kwargs):  # noqa: E501
+    def __init__(self, name, mutable, input_type, values, *args, **kwargs):  # noqa: E501
         """Attribute - a model defined in OpenAPI
 
         Args:
             name (str):
             mutable (bool):
             input_type (InputTypeEnum):
-            default_value (str):
             values ([str]):
 
         Keyword Args:
             id (int): [optional]  # noqa: E501
 
+            default_value (str): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -362,15 +364,14 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.name = name
         self.mutable = mutable
         self.input_type = input_type
-        self.default_value = default_value
         self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,68 +39,57 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-def lazy_import():
-    from cvat_sdk.api_client.model.input_type_enum import InputTypeEnum
-    globals()['InputTypeEnum'] = InputTypeEnum
 
 
-
-class IAttributeRequest(IModelData):
+class IPlugins(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    name: str # noqa: E501
+    git_integration: bool # noqa: E501
     """
     """
 
-    mutable: bool # noqa: E501
+    analytics: bool # noqa: E501
     """
     """
 
-    input_type: InputTypeEnum # noqa: E501
+    models: bool # noqa: E501
     """
     """
 
-    default_value: str # noqa: E501
+    predict: bool # noqa: E501
     """
     """
 
-    values: typing.List[str] # noqa: E501
-    """
-    [str]
-    """
 
-
-class AttributeRequest(ModelNormal, IAttributeRequest):
+class Plugins(ModelNormal, IPlugins):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      name (str):
-
-      mutable (bool):
+      git_integration (bool):
 
-      input_type (InputTypeEnum):
+      analytics (bool):
 
-      default_value (str):
+      models (bool):
 
-      values ([str]):
+      predict (bool):
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -117,84 +106,71 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('name',): {
-            'max_length': 64,
-            'min_length': 1,
-        },
-        ('default_value',): {
-            'max_length': 128,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'mutable': (bool,),  # noqa: E501
-            'input_type': (InputTypeEnum,),  # noqa: E501
-            'default_value': (str,),  # noqa: E501
-            'values': ([str],),  # noqa: E501
+            'git_integration': (bool,),  # noqa: E501
+            'analytics': (bool,),  # noqa: E501
+            'models': (bool,),  # noqa: E501
+            'predict': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'mutable': 'mutable',  # noqa: E501
-        'input_type': 'input_type',  # noqa: E501
-        'default_value': 'default_value',  # noqa: E501
-        'values': 'values',  # noqa: E501
+        'git_integration': 'GIT_INTEGRATION',  # noqa: E501
+        'analytics': 'ANALYTICS',  # noqa: E501
+        'models': 'MODELS',  # noqa: E501
+        'predict': 'PREDICT',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, mutable, input_type, default_value, values, *args, **kwargs):  # noqa: E501
-        """AttributeRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, git_integration, analytics, models, predict, *args, **kwargs):  # noqa: E501
+        """Plugins - a model defined in OpenAPI
 
         Args:
-            name (str):
-            mutable (bool):
-            input_type (InputTypeEnum):
-            default_value (str):
-            values ([str]):
+            git_integration (bool):
+            analytics (bool):
+            models (bool):
+            predict (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -251,19 +227,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.mutable = mutable
-        self.input_type = input_type
-        self.default_value = default_value
-        self.values = values
+        self.git_integration = git_integration
+        self.analytics = analytics
+        self.models = models
+        self.predict = predict
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -276,23 +251,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, mutable, input_type, default_value, values, *args, **kwargs):  # noqa: E501
-        """AttributeRequest - a model defined in OpenAPI
+    def __init__(self, git_integration, analytics, models, predict, *args, **kwargs):  # noqa: E501
+        """Plugins - a model defined in OpenAPI
 
         Args:
-            name (str):
-            mutable (bool):
-            input_type (InputTypeEnum):
-            default_value (str):
-            values ([str]):
+            git_integration (bool):
+            analytics (bool):
+            models (bool):
+            predict (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -347,19 +321,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.mutable = mutable
-        self.input_type = input_type
-        self.default_value = default_value
-        self.values = values
+        self.git_integration = git_integration
+        self.analytics = analytics
+        self.models = models
+        self.predict = predict
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/basic_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_content.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_read_owner.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/events_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/frame_selection_method_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/frame_selection_method_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_params.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/function_call_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/function_call_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/issue_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/job_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/location_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/meta_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/null_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/null_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_annotation_conflict_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_report_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_quality_report_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_quality_settings_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_quality_settings_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_annotation_guide_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_quality_settings_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_quality_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/analytics_report_create_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,55 +41,52 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IPlugins(IModelData):
+class IAnalyticsReportCreateRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    git_integration: bool # noqa: E501
+    job_id: int # noqa: E501
     """
+    [optional]
     """
 
-    analytics: bool # noqa: E501
+    task_id: int # noqa: E501
     """
+    [optional]
     """
 
-    models: bool # noqa: E501
-    """
-    """
-
-    predict: bool # noqa: E501
+    project_id: int # noqa: E501
     """
+    [optional]
     """
 
 
-class Plugins(ModelNormal, IPlugins):
+class AnalyticsReportCreateRequest(ModelNormal, IAnalyticsReportCreateRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      git_integration (bool):
+      job_id (int): [optional]  # noqa: E501
 
-      analytics (bool):
+      task_id (int): [optional]  # noqa: E501
 
-      models (bool):
-
-      predict (bool):
+      project_id (int): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -129,50 +126,48 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'git_integration': (bool,),  # noqa: E501
-            'analytics': (bool,),  # noqa: E501
-            'models': (bool,),  # noqa: E501
-            'predict': (bool,),  # noqa: E501
+            'job_id': (int,),  # noqa: E501
+            'task_id': (int,),  # noqa: E501
+            'project_id': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'git_integration': 'GIT_INTEGRATION',  # noqa: E501
-        'analytics': 'ANALYTICS',  # noqa: E501
-        'models': 'MODELS',  # noqa: E501
-        'predict': 'PREDICT',  # noqa: E501
+        'job_id': 'job_id',  # noqa: E501
+        'task_id': 'task_id',  # noqa: E501
+        'project_id': 'project_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, git_integration, analytics, models, predict, *args, **kwargs):  # noqa: E501
-        """Plugins - a model defined in OpenAPI
-
-        Args:
-            git_integration (bool):
-            analytics (bool):
-            models (bool):
-            predict (bool):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """AnalyticsReportCreateRequest - a model defined in OpenAPI
 
         Keyword Args:
+            job_id (int): [optional]  # noqa: E501
+
+            task_id (int): [optional]  # noqa: E501
+
+            project_id (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -227,18 +222,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.git_integration = git_integration
-        self.analytics = analytics
-        self.models = models
-        self.predict = predict
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -251,24 +242,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, git_integration, analytics, models, predict, *args, **kwargs):  # noqa: E501
-        """Plugins - a model defined in OpenAPI
-
-        Args:
-            git_integration (bool):
-            analytics (bool):
-            models (bool):
-            predict (bool):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """AnalyticsReportCreateRequest - a model defined in OpenAPI
 
         Keyword Args:
+            job_id (int): [optional]  # noqa: E501
+
+            task_id (int): [optional]  # noqa: E501
+
+            project_id (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -321,18 +312,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.git_integration = git_integration
-        self.analytics = analytics
-        self.models = models
-        self.predict = predict
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_create_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_report_target.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_report_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/quality_settings.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/quality_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/role_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_id.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/severity_enum.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/severity_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/signing_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/storage_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sublabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model/webhook_write_request.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
-from copy import deepcopy
+from copy import copy, deepcopy
 import inspect
 import io
 import os
 import pprint
 import re
 import tempfile
 import uuid
@@ -1626,48 +1626,58 @@
         return input_value
     inner_required_types = child_req_types_by_current_type.get(
         type(input_value)
     )
     if inner_required_types is None:
         # for this type, there are not more inner variables left to look at
         return input_value
+
     if isinstance(input_value, list):
-        if input_value == []:
+        # avoid storing and changing the input value when the type is mutable collection
+        output_value = copy(input_value)
+
+        if output_value == []:
             # allow an empty list
-            return input_value
-        for index, inner_value in enumerate(input_value):
+            return output_value
+        for index, inner_value in enumerate(output_value):
             inner_path = list(path_to_item)
             inner_path.append(index)
-            input_value[index] = validate_and_convert_types(
+            output_value[index] = validate_and_convert_types(
                 inner_value,
                 inner_required_types,
                 inner_path,
                 spec_property_naming,
                 _check_type,
                 configuration=configuration
             )
     elif isinstance(input_value, dict):
-        if input_value == {}:
+        # avoid storing and changing the input value when the type is mutable collection
+        output_value = copy(input_value)
+
+        if output_value == {}:
             # allow an empty dict
-            return input_value
-        for inner_key, inner_val in input_value.items():
+            return output_value
+        for inner_key, inner_val in output_value.items():
             inner_path = list(path_to_item)
             inner_path.append(inner_key)
             if get_simple_class(inner_key) != str:
                 raise get_type_error(inner_key, inner_path, valid_classes,
                                      key_type=True)
-            input_value[inner_key] = validate_and_convert_types(
+            output_value[inner_key] = validate_and_convert_types(
                 inner_val,
                 inner_required_types,
                 inner_path,
                 spec_property_naming,
                 _check_type,
                 configuration=configuration
             )
-    return input_value
+    else:
+        output_value = input_value
+
+    return output_value
 
 
 def model_to_dict(model_instance, serialize=True):
     """Returns the model properties as a dict
 
     Args:
         model_instance (one of your model instances): the model instance that
@@ -1698,32 +1708,28 @@
                 try:
                     attr = model_instance.attribute_map[attr]
                     py_to_json_map.update(model_instance.attribute_map)
                     seen_json_attribute_names.add(attr)
                 except KeyError:
                     used_fallback_python_attribute_names.add(attr)
             if isinstance(value, list):
-                if not value:
-                    # empty list or None
-                    result[attr] = value
-                else:
-                    res = []
-                    for v in value:
-                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
-                            res.append(v)
-                        elif isinstance(v, ModelSimple):
-                            res.append(v.value)
-                        elif isinstance(v, dict):
-                            res.append(dict(map(
-                                extract_item,
-                                v.items()
-                            )))
-                        else:
-                            res.append(model_to_dict(v, serialize=serialize))
-                    result[attr] = res
+                res = []
+                for v in value:
+                    if isinstance(v, PRIMITIVE_TYPES) or v is None:
+                        res.append(v)
+                    elif isinstance(v, ModelSimple):
+                        res.append(v.value)
+                    elif isinstance(v, dict):
+                        res.append(dict(map(
+                            extract_item,
+                            v.items()
+                        )))
+                    else:
+                        res.append(model_to_dict(v, serialize=serialize))
+                result[attr] = res
             elif isinstance(value, dict):
                 result[attr] = dict(map(
                     extract_item,
                     value.items()
                 ))
             elif isinstance(value, ModelSimple):
                 result[attr] = value.value
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from cvat_sdk.api_client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
 from cvat_sdk.api_client.model.about import About, IAbout
+from cvat_sdk.api_client.model.analytics_report import AnalyticsReport, IAnalyticsReport
+from cvat_sdk.api_client.model.analytics_report_create_request import AnalyticsReportCreateRequest, IAnalyticsReportCreateRequest
+from cvat_sdk.api_client.model.analytics_report_target_enum import AnalyticsReportTargetEnum, IAnalyticsReportTargetEnum
 from cvat_sdk.api_client.model.annotation_conflict import AnnotationConflict, IAnnotationConflict
 from cvat_sdk.api_client.model.annotation_conflict_type_enum import AnnotationConflictTypeEnum, IAnnotationConflictTypeEnum
 from cvat_sdk.api_client.model.annotation_file_request import AnnotationFileRequest, IAnnotationFileRequest
 from cvat_sdk.api_client.model.annotation_guide_read import AnnotationGuideRead, IAnnotationGuideRead
 from cvat_sdk.api_client.model.annotation_guide_write_request import AnnotationGuideWriteRequest, IAnnotationGuideWriteRequest
 from cvat_sdk.api_client.model.annotation_id import AnnotationId, IAnnotationId
 from cvat_sdk.api_client.model.annotation_id_shape_type import AnnotationIdShapeType
@@ -34,42 +37,46 @@
 from cvat_sdk.api_client.model.attribute import Attribute, IAttribute
 from cvat_sdk.api_client.model.attribute_request import AttributeRequest, IAttributeRequest
 from cvat_sdk.api_client.model.attribute_val import AttributeVal, IAttributeVal
 from cvat_sdk.api_client.model.attribute_val_request import AttributeValRequest, IAttributeValRequest
 from cvat_sdk.api_client.model.backup_write_request import BackupWriteRequest
 from cvat_sdk.api_client.model.basic_user import BasicUser, IBasicUser
 from cvat_sdk.api_client.model.basic_user_request import BasicUserRequest, IBasicUserRequest
+from cvat_sdk.api_client.model.binary_operation import BinaryOperation, IBinaryOperation
 from cvat_sdk.api_client.model.chunk_type import ChunkType, IChunkType
 from cvat_sdk.api_client.model.client_events import ClientEvents, IClientEvents
 from cvat_sdk.api_client.model.client_events_request import ClientEventsRequest, IClientEventsRequest
 from cvat_sdk.api_client.model.cloud_storage_content import CloudStorageContent, ICloudStorageContent
 from cvat_sdk.api_client.model.cloud_storage_read import CloudStorageRead, ICloudStorageRead
 from cvat_sdk.api_client.model.cloud_storage_read_owner import CloudStorageReadOwner
 from cvat_sdk.api_client.model.cloud_storage_write_request import CloudStorageWriteRequest, ICloudStorageWriteRequest
 from cvat_sdk.api_client.model.comment_read import CommentRead, ICommentRead
 from cvat_sdk.api_client.model.comment_write_request import CommentWriteRequest, ICommentWriteRequest
 from cvat_sdk.api_client.model.comments_summary import CommentsSummary, ICommentsSummary
 from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum, ICredentialsTypeEnum
+from cvat_sdk.api_client.model.data_frame import DataFrame, IDataFrame
 from cvat_sdk.api_client.model.data_meta_read import DataMetaRead, IDataMetaRead
 from cvat_sdk.api_client.model.data_request import DataRequest, IDataRequest
 from cvat_sdk.api_client.model.dataset_file_request import DatasetFileRequest, IDatasetFileRequest
 from cvat_sdk.api_client.model.dataset_format import DatasetFormat, IDatasetFormat
 from cvat_sdk.api_client.model.dataset_formats import DatasetFormats, IDatasetFormats
 from cvat_sdk.api_client.model.dataset_write_request import DatasetWriteRequest
+from cvat_sdk.api_client.model.default_view_enum import DefaultViewEnum, IDefaultViewEnum
 from cvat_sdk.api_client.model.event import Event, IEvent
 from cvat_sdk.api_client.model.event_request import EventRequest, IEventRequest
 from cvat_sdk.api_client.model.events import Events, IEvents
 from cvat_sdk.api_client.model.events_enum import EventsEnum, IEventsEnum
 from cvat_sdk.api_client.model.file_info import FileInfo, IFileInfo
 from cvat_sdk.api_client.model.file_info_type_enum import FileInfoTypeEnum, IFileInfoTypeEnum
 from cvat_sdk.api_client.model.frame_meta import FrameMeta, IFrameMeta
 from cvat_sdk.api_client.model.frame_selection_method_enum import FrameSelectionMethodEnum, IFrameSelectionMethodEnum
 from cvat_sdk.api_client.model.function_call import FunctionCall, IFunctionCall
 from cvat_sdk.api_client.model.function_call_params import FunctionCallParams, IFunctionCallParams
 from cvat_sdk.api_client.model.function_call_request import FunctionCallRequest, IFunctionCallRequest
+from cvat_sdk.api_client.model.granularity_enum import GranularityEnum, IGranularityEnum
 from cvat_sdk.api_client.model.input_type_enum import InputTypeEnum, IInputTypeEnum
 from cvat_sdk.api_client.model.invitation_read import InvitationRead, IInvitationRead
 from cvat_sdk.api_client.model.invitation_write_request import InvitationWriteRequest, IInvitationWriteRequest
 from cvat_sdk.api_client.model.issue_read import IssueRead, IIssueRead
 from cvat_sdk.api_client.model.issue_write_request import IssueWriteRequest, IIssueWriteRequest
 from cvat_sdk.api_client.model.issues_summary import IssuesSummary, IIssuesSummary
 from cvat_sdk.api_client.model.job_annotations_update_request import JobAnnotationsUpdateRequest
@@ -90,17 +97,20 @@
 from cvat_sdk.api_client.model.labeled_track import LabeledTrack, ILabeledTrack
 from cvat_sdk.api_client.model.labeled_track_request import LabeledTrackRequest, ILabeledTrackRequest
 from cvat_sdk.api_client.model.labels_summary import LabelsSummary, ILabelsSummary
 from cvat_sdk.api_client.model.location_enum import LocationEnum, ILocationEnum
 from cvat_sdk.api_client.model.login_serializer_ex_request import LoginSerializerExRequest, ILoginSerializerExRequest
 from cvat_sdk.api_client.model.membership_read import MembershipRead, IMembershipRead
 from cvat_sdk.api_client.model.meta_user import MetaUser
+from cvat_sdk.api_client.model.metric import Metric, IMetric
+from cvat_sdk.api_client.model.metric_granularity import MetricGranularity
 from cvat_sdk.api_client.model.null_enum import NullEnum, INullEnum
 from cvat_sdk.api_client.model.online_function_call_request import OnlineFunctionCallRequest, IOnlineFunctionCallRequest
 from cvat_sdk.api_client.model.operation_status import OperationStatus, IOperationStatus
+from cvat_sdk.api_client.model.operator_enum import OperatorEnum, IOperatorEnum
 from cvat_sdk.api_client.model.organization_read import OrganizationRead, IOrganizationRead
 from cvat_sdk.api_client.model.organization_write_request import OrganizationWriteRequest, IOrganizationWriteRequest
 from cvat_sdk.api_client.model.paginated_annotation_conflict_list import PaginatedAnnotationConflictList, IPaginatedAnnotationConflictList
 from cvat_sdk.api_client.model.paginated_cloud_storage_read_list import PaginatedCloudStorageReadList, IPaginatedCloudStorageReadList
 from cvat_sdk.api_client.model.paginated_comment_read_list import PaginatedCommentReadList, IPaginatedCommentReadList
 from cvat_sdk.api_client.model.paginated_invitation_read_list import PaginatedInvitationReadList, IPaginatedInvitationReadList
 from cvat_sdk.api_client.model.paginated_issue_read_list import PaginatedIssueReadList, IPaginatedIssueReadList
@@ -175,13 +185,15 @@
 from cvat_sdk.api_client.model.task_read import TaskRead, ITaskRead
 from cvat_sdk.api_client.model.task_read_target_storage import TaskReadTargetStorage
 from cvat_sdk.api_client.model.task_write_request import TaskWriteRequest, ITaskWriteRequest
 from cvat_sdk.api_client.model.tasks_summary import TasksSummary, ITasksSummary
 from cvat_sdk.api_client.model.token import Token, IToken
 from cvat_sdk.api_client.model.tracked_shape import TrackedShape, ITrackedShape
 from cvat_sdk.api_client.model.tracked_shape_request import TrackedShapeRequest, ITrackedShapeRequest
+from cvat_sdk.api_client.model.transformation import Transformation, ITransformation
+from cvat_sdk.api_client.model.transformation_binary import TransformationBinary
 from cvat_sdk.api_client.model.user import User, IUser
 from cvat_sdk.api_client.model.webhook_content_type import WebhookContentType, IWebhookContentType
 from cvat_sdk.api_client.model.webhook_delivery_read import WebhookDeliveryRead, IWebhookDeliveryRead
 from cvat_sdk.api_client.model.webhook_read import WebhookRead, IWebhookRead
 from cvat_sdk.api_client.model.webhook_type import WebhookType, IWebhookType
 from cvat_sdk.api_client.model.webhook_write_request import WebhookWriteRequest, IWebhookWriteRequest
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.5.2/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/client.py` & `cvat_sdk-2.5.2/cvat_sdk/core/client.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/downloading.py` & `cvat_sdk-2.5.2/cvat_sdk/core/downloading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/git.py` & `cvat_sdk-2.5.2/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/helpers.py` & `cvat_sdk-2.5.2/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/progress.py` & `cvat_sdk-2.5.2/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/tasks.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.5.2/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/uploading.py` & `cvat_sdk-2.5.2/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/core/utils.py` & `cvat_sdk-2.5.2/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.5.2/cvat_sdk/datasets/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.5.0/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.5.2/cvat_sdk/pytorch/project_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 import torch.utils.data
 import torchvision.datasets
 
 import cvat_sdk.core
 import cvat_sdk.core.exceptions
 import cvat_sdk.models as models
-from cvat_sdk.pytorch.caching import UpdatePolicy, make_cache_manager
+from cvat_sdk.datasets.caching import UpdatePolicy, make_cache_manager
 from cvat_sdk.pytorch.task_dataset import TaskVisionDataset
 
 
 class ProjectVisionDataset(torchvision.datasets.VisionDataset):
     """
     Represents a project on a CVAT server as a PyTorch Dataset.
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.5.2/cvat_sdk/pytorch/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 import attrs
 import attrs.validators
 import torch
 import torch.utils.data
 from typing_extensions import TypedDict
 
-from cvat_sdk.pytorch.common import Target, UnsupportedDatasetError
+from cvat_sdk.datasets.common import UnsupportedDatasetError
+from cvat_sdk.pytorch.common import Target
 
 
 @attrs.frozen
 class ExtractSingleLabelIndex:
     """
     A target transform that takes a `Target` object and produces a single label index
     based on the tag in that object, as a 0-dimensional tensor.
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.5.2/cvat_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.5.0
+Version: 2.5.2
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.5.0/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.5.2/cvat_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ./cvat_sdk/api_client/__init__.py
 ./cvat_sdk/api_client/api_client.py
 ./cvat_sdk/api_client/configuration.py
 ./cvat_sdk/api_client/exceptions.py
 ./cvat_sdk/api_client/model_utils.py
 ./cvat_sdk/api_client/rest.py
 ./cvat_sdk/api_client/api/__init__.py
+./cvat_sdk/api_client/api/analytics_api.py
 ./cvat_sdk/api_client/api/assets_api.py
 ./cvat_sdk/api_client/api/auth_api.py
 ./cvat_sdk/api_client/api/cloudstorages_api.py
 ./cvat_sdk/api_client/api/comments_api.py
 ./cvat_sdk/api_client/api/events_api.py
 ./cvat_sdk/api_client/api/guides_api.py
 ./cvat_sdk/api_client/api/invitations_api.py
@@ -32,14 +33,17 @@
 ./cvat_sdk/api_client/api/server_api.py
 ./cvat_sdk/api_client/api/tasks_api.py
 ./cvat_sdk/api_client/api/users_api.py
 ./cvat_sdk/api_client/api/webhooks_api.py
 ./cvat_sdk/api_client/apis/__init__.py
 ./cvat_sdk/api_client/model/__init__.py
 ./cvat_sdk/api_client/model/about.py
+./cvat_sdk/api_client/model/analytics_report.py
+./cvat_sdk/api_client/model/analytics_report_create_request.py
+./cvat_sdk/api_client/model/analytics_report_target_enum.py
 ./cvat_sdk/api_client/model/annotation_conflict.py
 ./cvat_sdk/api_client/model/annotation_conflict_type_enum.py
 ./cvat_sdk/api_client/model/annotation_file_request.py
 ./cvat_sdk/api_client/model/annotation_guide_read.py
 ./cvat_sdk/api_client/model/annotation_guide_write_request.py
 ./cvat_sdk/api_client/model/annotation_id.py
 ./cvat_sdk/api_client/model/annotation_id_shape_type.py
@@ -49,42 +53,46 @@
 ./cvat_sdk/api_client/model/attribute.py
 ./cvat_sdk/api_client/model/attribute_request.py
 ./cvat_sdk/api_client/model/attribute_val.py
 ./cvat_sdk/api_client/model/attribute_val_request.py
 ./cvat_sdk/api_client/model/backup_write_request.py
 ./cvat_sdk/api_client/model/basic_user.py
 ./cvat_sdk/api_client/model/basic_user_request.py
+./cvat_sdk/api_client/model/binary_operation.py
 ./cvat_sdk/api_client/model/chunk_type.py
 ./cvat_sdk/api_client/model/client_events.py
 ./cvat_sdk/api_client/model/client_events_request.py
 ./cvat_sdk/api_client/model/cloud_storage_content.py
 ./cvat_sdk/api_client/model/cloud_storage_read.py
 ./cvat_sdk/api_client/model/cloud_storage_read_owner.py
 ./cvat_sdk/api_client/model/cloud_storage_write_request.py
 ./cvat_sdk/api_client/model/comment_read.py
 ./cvat_sdk/api_client/model/comment_write_request.py
 ./cvat_sdk/api_client/model/comments_summary.py
 ./cvat_sdk/api_client/model/credentials_type_enum.py
+./cvat_sdk/api_client/model/data_frame.py
 ./cvat_sdk/api_client/model/data_meta_read.py
 ./cvat_sdk/api_client/model/data_request.py
 ./cvat_sdk/api_client/model/dataset_file_request.py
 ./cvat_sdk/api_client/model/dataset_format.py
 ./cvat_sdk/api_client/model/dataset_formats.py
 ./cvat_sdk/api_client/model/dataset_write_request.py
+./cvat_sdk/api_client/model/default_view_enum.py
 ./cvat_sdk/api_client/model/event.py
 ./cvat_sdk/api_client/model/event_request.py
 ./cvat_sdk/api_client/model/events.py
 ./cvat_sdk/api_client/model/events_enum.py
 ./cvat_sdk/api_client/model/file_info.py
 ./cvat_sdk/api_client/model/file_info_type_enum.py
 ./cvat_sdk/api_client/model/frame_meta.py
 ./cvat_sdk/api_client/model/frame_selection_method_enum.py
 ./cvat_sdk/api_client/model/function_call.py
 ./cvat_sdk/api_client/model/function_call_params.py
 ./cvat_sdk/api_client/model/function_call_request.py
+./cvat_sdk/api_client/model/granularity_enum.py
 ./cvat_sdk/api_client/model/input_type_enum.py
 ./cvat_sdk/api_client/model/invitation_read.py
 ./cvat_sdk/api_client/model/invitation_write_request.py
 ./cvat_sdk/api_client/model/issue_read.py
 ./cvat_sdk/api_client/model/issue_write_request.py
 ./cvat_sdk/api_client/model/issues_summary.py
 ./cvat_sdk/api_client/model/job_annotations_update_request.py
@@ -105,17 +113,20 @@
 ./cvat_sdk/api_client/model/labeled_track.py
 ./cvat_sdk/api_client/model/labeled_track_request.py
 ./cvat_sdk/api_client/model/labels_summary.py
 ./cvat_sdk/api_client/model/location_enum.py
 ./cvat_sdk/api_client/model/login_serializer_ex_request.py
 ./cvat_sdk/api_client/model/membership_read.py
 ./cvat_sdk/api_client/model/meta_user.py
+./cvat_sdk/api_client/model/metric.py
+./cvat_sdk/api_client/model/metric_granularity.py
 ./cvat_sdk/api_client/model/null_enum.py
 ./cvat_sdk/api_client/model/online_function_call_request.py
 ./cvat_sdk/api_client/model/operation_status.py
+./cvat_sdk/api_client/model/operator_enum.py
 ./cvat_sdk/api_client/model/organization_read.py
 ./cvat_sdk/api_client/model/organization_write_request.py
 ./cvat_sdk/api_client/model/paginated_annotation_conflict_list.py
 ./cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
 ./cvat_sdk/api_client/model/paginated_comment_read_list.py
 ./cvat_sdk/api_client/model/paginated_invitation_read_list.py
 ./cvat_sdk/api_client/model/paginated_issue_read_list.py
@@ -190,14 +201,16 @@
 ./cvat_sdk/api_client/model/task_read.py
 ./cvat_sdk/api_client/model/task_read_target_storage.py
 ./cvat_sdk/api_client/model/task_write_request.py
 ./cvat_sdk/api_client/model/tasks_summary.py
 ./cvat_sdk/api_client/model/token.py
 ./cvat_sdk/api_client/model/tracked_shape.py
 ./cvat_sdk/api_client/model/tracked_shape_request.py
+./cvat_sdk/api_client/model/transformation.py
+./cvat_sdk/api_client/model/transformation_binary.py
 ./cvat_sdk/api_client/model/user.py
 ./cvat_sdk/api_client/model/webhook_content_type.py
 ./cvat_sdk/api_client/model/webhook_delivery_read.py
 ./cvat_sdk/api_client/model/webhook_read.py
 ./cvat_sdk/api_client/model/webhook_type.py
 ./cvat_sdk/api_client/model/webhook_write_request.py
 ./cvat_sdk/api_client/models/__init__.py
@@ -215,16 +228,19 @@
 ./cvat_sdk/core/proxies/issues.py
 ./cvat_sdk/core/proxies/jobs.py
 ./cvat_sdk/core/proxies/model_proxy.py
 ./cvat_sdk/core/proxies/organizations.py
 ./cvat_sdk/core/proxies/projects.py
 ./cvat_sdk/core/proxies/tasks.py
 ./cvat_sdk/core/proxies/users.py
+./cvat_sdk/datasets/__init__.py
+./cvat_sdk/datasets/caching.py
+./cvat_sdk/datasets/common.py
+./cvat_sdk/datasets/task_dataset.py
 ./cvat_sdk/pytorch/__init__.py
-./cvat_sdk/pytorch/caching.py
 ./cvat_sdk/pytorch/common.py
 ./cvat_sdk/pytorch/project_dataset.py
 ./cvat_sdk/pytorch/task_dataset.py
 ./cvat_sdk/pytorch/transforms.py
 cvat_sdk.egg-info/PKG-INFO
 cvat_sdk.egg-info/SOURCES.txt
 cvat_sdk.egg-info/dependency_links.txt
```

### Comparing `cvat_sdk-2.5.0/setup.py` & `cvat_sdk-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.6
+# The version of the OpenAPI document: 2.5.2
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

