# Comparing `tmp/tesla-ce-1.0.3.tar.gz` & `tmp/tesla-ce-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-1.0.3.tar", last modified: Mon Mar 13 12:12:05 2023, max compression
+gzip compressed data, was "tesla-ce-1.0.8.tar", last modified: Fri Jul 28 18:31:58 2023, max compression
```

## Comparing `tesla-ce-1.0.3.tar` & `tesla-ce-1.0.8.tar`

### file list

```diff
@@ -1,571 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.641456 tesla-ce-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/tep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/tip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/tep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/institution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/ui_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_report_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/institution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/send_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/send_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/ui_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/vle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/enrolment_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/provider_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/request_provider_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/assessment_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/vle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/institution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/ui_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.649456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_report_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/informed_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/informed_consent_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/institution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/send_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/send_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/ui_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/vle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/enrolment_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/provider_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/request_provider_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/vle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/celery_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    49717 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/fixtures/ui_options.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/lib/config/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/config/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22972 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/config/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/lib/data/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce/lib/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/data/messages.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.653456 tesla-ce-1.0.3/src/tesla_ce/lib/db/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/db/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/lib/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/deploy/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/deploy/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/lib/queues/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/queues/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/queues/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/lib/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/storage/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/storage/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/lib/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/vault/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/vault/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/lib/vault/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/management/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_vle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/rebuild_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/reconfigure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/register_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/register_vle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/register_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/remote_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/resend_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/resend_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/tesla_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/management/commands/unseal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.657456 tesla-ce-1.0.3/src/tesla_ce/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    37558 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0002_histograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0003_providernotification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0004_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0005_auto_20200520_2009.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0006_auto_20200520_2128.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0007_auto_20200712_1330.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0008_auto_20200721_1022.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0009_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0010_auto_20200930_1829.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0011_auto_20200930_1842.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0012_auto_20210415_1829.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0013_webhookclient_webhookmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0014_uioption.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0015_uioption_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0016_auto_20210709_1023.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0017_auto_20210715_2150.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0018_assessmentsession_auto_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0019_auto_20210907_1602.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0020_institution_allowed_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0021_alter_reportactivitysession_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0022_auto_20211124_1252.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/0023_alter_launcher_session.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.661456 tesla-ce-1.0.3/src/tesla_ce/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/assessment_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/assessment_session_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/course_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/enrolment_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/enrolment_sample_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/histogram_activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/histogram_activity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/histogram_learner_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/histogram_learner_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/informed_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/informed_consent_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/institution.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/provider_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/report_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/report_activity_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/report_activity_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/request_provider_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/request_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/send_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/send_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/ui_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/vle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/models/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.661456 tesla-ce-1.0.3/src/tesla_ce/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.665456 tesla-ce-1.0.3/src/tesla_ce/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    79874 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-114x114-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-120x120-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-144x144-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-152x152-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-180x180-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-57x57-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-60x60-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-72x72-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-76x76-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/img/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.665456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/3rdpartylicenses.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.637456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.665456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/bg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/ca.json
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/es.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/fi.json
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/keys.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/tr.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.669456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.669456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/activity.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/authorship.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/connection.png
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/connection.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/content.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/course.svg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/identity.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/informed-consent.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/integrity.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29419 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/menu_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/monitoring.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/moreinfo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.png
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/originality.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/system.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/user.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/connection.png
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/connection.svg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/dashboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.669456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.png
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.png
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.svg
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.png
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/plag.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.png
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.svg
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.png
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.669456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/error.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/error.svg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/info.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/warning.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification/warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_alert.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_error.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_error.svg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_info.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_warning.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notification_warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notifications.png
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notifications.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.669456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/admin.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/data.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/instructor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/learner.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/legal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/superadmin.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.673456 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.png
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.svg
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.png
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.png
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.svg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    73182 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)   893740 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/web-plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/tasks/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/monitor/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/tasks/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/notification/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/tasks/reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/reports/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/tasks/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/requests/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/requests/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/tasks/requests/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.641456 tesla-ce-1.0.3/src/tesla_ce/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.641456 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_frontend.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_lb_traefik.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_lti.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_moodle.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_services.yml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/vault_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/templates/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/doc/redoc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.641456 tesla-ce-1.0.3/src/tesla_ce/templates/rest_framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/templates/rest_framework/horizontal/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/rest_framework/horizontal/Jsonform_field.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tesla_ce/templates/web-plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/templates/web-plugin/connector.js
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tesla_ce/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.645456 tesla-ce-1.0.3/src/tesla_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23096 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-13 12:12:05.000000 tesla-ce-1.0.3/src/tesla_ce.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tests/api/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/test_institution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/test_ui_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/admin/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.677456 tesla-ce-1.0.3/src/tests/api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_approle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_lapi_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_launcher_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_ui_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/auth/test_userpass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/institution/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/institution/course/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/institution/course/activity/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/activity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/institution/course/activity/report/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/activity/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/test_course.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/test_instructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/course/test_learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_course_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_informed_consent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_institution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_instructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/institution/test_vle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/provider/test_api_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/api/vle/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/api/vle/test_api_vle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/auth_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23641 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/test_activity_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/test_case_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/global_admin/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/global_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/global_admin/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/inst_admin/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/inst_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/inst_admin/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/instructor/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/instructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/instructor/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/learner/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/learner/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/provider/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/vle/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/vle/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/cases/utils/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/cases/utils/worker/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/test_generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/test_reconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/test_swarm_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/test_unseal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/config/test_django_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/config/test_vault_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 12:12:05.681456 tesla-ce-1.0.3/src/tests/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/jwt/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-03-13 12:11:43.000000 tesla-ce-1.0.3/src/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.945286 tesla-ce-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.945286 tesla-ce-1.0.8/src/tesla_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/tep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/tip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/tep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/ui_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.953286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_report_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/send_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/send_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/ui_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/vle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.953286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/enrolment_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/provider_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/request_provider_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.953286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/assessment_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/vle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.953286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.957286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/ui_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.957286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_report_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/informed_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/informed_consent_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/send_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/send_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/ui_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/vle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.957286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/enrolment_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/provider_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/request_provider_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/vle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/celery_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49840 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/fixtures/ui_options.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/lib/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/config/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22972 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/config/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.961286 tesla-ce-1.0.8/src/tesla_ce/lib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce/lib/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/data/messages.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/db/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17983 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/deploy/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/deploy/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/queues/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/queues/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/storage/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/storage/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/vault/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/vault/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/vault/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/lib/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/lib/webhook/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.965286 tesla-ce-1.0.8/src/tesla_ce/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_vle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/rebuild_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/reconfigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/register_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/register_vle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/register_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/remote_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/resend_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/resend_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/tesla_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/management/commands/unseal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.969286 tesla-ce-1.0.8/src/tesla_ce/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    37558 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0002_histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0003_providernotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0004_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0005_auto_20200520_2009.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0006_auto_20200520_2128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0007_auto_20200712_1330.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0008_auto_20200721_1022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0009_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0010_auto_20200930_1829.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0011_auto_20200930_1842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0012_auto_20210415_1829.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0013_webhookclient_webhookmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0014_uioption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0015_uioption_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0016_auto_20210709_1023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0017_auto_20210715_2150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0018_assessmentsession_auto_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0019_auto_20210907_1602.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0020_institution_allowed_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0021_alter_reportactivitysession_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0022_auto_20211124_1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/0023_alter_launcher_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.973286 tesla-ce-1.0.8/src/tesla_ce/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/assessment_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/assessment_session_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/course_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/enrolment_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/enrolment_sample_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/histogram_activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/histogram_activity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/histogram_learner_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/histogram_learner_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/informed_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/informed_consent_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/provider_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/report_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/report_activity_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/report_activity_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/request_provider_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/request_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/send_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/send_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/ui_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/vle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/models/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18278 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.973286 tesla-ce-1.0.8/src/tesla_ce/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.977286 tesla-ce-1.0.8/src/tesla_ce/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79874 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-114x114-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-120x120-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-144x144-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-152x152-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-180x180-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-57x57-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-60x60-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-72x72-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-76x76-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16960 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/img/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.977286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/3rdpartylicenses.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.941286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.977286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/bg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/ca.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/fi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/tr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.981286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.985286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/activity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/authorship.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/connection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/content.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/course.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/identity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/informed-consent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/integrity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29419 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/menu_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/monitoring.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/moreinfo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/originality.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/user.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/connection.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/dashboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.985286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/plag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.985286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification/warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notification_warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notifications.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notifications.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.989286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/admin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/data.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/instructor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/learner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/legal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/superadmin.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.989286 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    73182 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)   893740 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/web-plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.993286 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.993286 tesla-ce-1.0.8/src/tesla_ce/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.993286 tesla-ce-1.0.8/src/tesla_ce/tasks/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/monitor/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.993286 tesla-ce-1.0.8/src/tesla_ce/tasks/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/notification/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.993286 tesla-ce-1.0.8/src/tesla_ce/tasks/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14558 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/reports/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tesla_ce/tasks/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/requests/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/requests/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/tasks/requests/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.945286 tesla-ce-1.0.8/src/tesla_ce/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.945286 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_core.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_frontend.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_lb_traefik.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_lti.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_moodle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_services.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/vault_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tesla_ce/templates/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/doc/redoc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.945286 tesla-ce-1.0.8/src/tesla_ce/templates/rest_framework/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tesla_ce/templates/rest_framework/horizontal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/rest_framework/horizontal/Jsonform_field.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tesla_ce/templates/web-plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/templates/web-plugin/connector.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tesla_ce/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.949286 tesla-ce-1.0.8/src/tesla_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23169 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:31:57.000000 tesla-ce-1.0.8/src/tesla_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:57.997286 tesla-ce-1.0.8/src/tests/api/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/test_institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/test_ui_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/admin/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.001286 tesla-ce-1.0.8/src/tests/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_approle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_lapi_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_launcher_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_ui_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/auth/test_userpass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.001286 tesla-ce-1.0.8/src/tests/api/institution/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.001286 tesla-ce-1.0.8/src/tests/api/institution/course/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.001286 tesla-ce-1.0.8/src/tests/api/institution/course/activity/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/activity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.001286 tesla-ce-1.0.8/src/tests/api/institution/course/activity/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/activity/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/test_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/test_instructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/course/test_learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_course_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_informed_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_institution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_instructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21465 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/institution/test_vle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/api/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/provider/test_api_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/api/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/api/vle/test_api_vle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/auth_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/test_activity_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/test_case_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/global_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/global_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/global_admin/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/inst_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/inst_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/inst_admin/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/instructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/instructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/instructor/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/learner/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/provider/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/vle/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.005287 tesla-ce-1.0.8/src/tests/cases/utils/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/cases/utils/worker/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/src/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/test_generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/test_reconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/test_swarm_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/test_unseal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/src/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/config/test_django_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/config/test_vault_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:31:58.009286 tesla-ce-1.0.8/src/tests/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/jwt/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-07-28 18:31:19.000000 tesla-ce-1.0.8/src/tests/utils.py
```

### Comparing `tesla-ce-1.0.3/LICENSE` & `tesla-ce-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/PKG-INFO` & `tesla-ce-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce
-Version: 1.0.3
+Version: 1.0.8
 Summary: TeSLA CE
 Home-page: https://github.com/tesla-ce/core
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io
 Project-URL: Source, https://github.com/tesla-ce/core
```

### Comparing `tesla-ce-1.0.3/README.md` & `tesla-ce-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/requirements.txt` & `tesla-ce-1.0.8/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,242 +4,239 @@
 #
 #    pip-compile
 #
 alabaster==0.7.13
     # via sphinx
 amqp==5.1.1
     # via kombu
-asgiref==3.6.0
+asgiref==3.7.2
     # via django
 async-timeout==4.0.2
     # via redis
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   jsonschema
-    #   pytest
+    #   referencing
 babel==2.12.1
     # via sphinx
-billiard==3.6.4.0
+billiard==4.1.0
     # via celery
-boto3==1.26.89
+boto3==1.28.14
     # via -r requirements.in
-botocore==1.29.89
+botocore==1.31.14
     # via
     #   boto3
     #   s3transfer
-celery==5.2.7
+celery==5.3.1
     # via
     #   -r requirements.in
     #   django-celery-beat
     #   django-celery-results
-certifi==2022.12.7
+certifi==2023.7.22
     # via
     #   requests
     #   sentry-sdk
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
 commonmark==0.9.1
     # via recommonmark
-coreapi==2.3.3
-    # via drf-yasg
-coreschema==0.0.4
-    # via
-    #   coreapi
-    #   drf-yasg
-coverage[toml]==7.2.1
+coverage[toml]==7.2.7
     # via pytest-cov
-django==4.1.7
+cron-descriptor==1.4.0
+    # via django-celery-beat
+django==4.2.3
     # via
     #   -r requirements.in
     #   django-celery-beat
     #   django-celery-results
     #   django-configurations
     #   django-cors-headers
     #   django-filter
     #   django-redis
     #   django-rest-auth
     #   django-sslserver
     #   django-storages
+    #   django-timezone-field
     #   djangorestframework
     #   djangorestframework-simplejwt
     #   drf-yasg
 django-cache-memoize==0.1.10
     # via -r requirements.in
-django-celery-beat==2.4.0
+django-celery-beat==2.5.0
     # via -r requirements.in
-django-celery-results==2.5.0
+django-celery-results==2.5.1
     # via -r requirements.in
-django-configurations==2.4
+django-configurations==2.4.1
     # via -r requirements.in
-django-cors-headers==3.14.0
+django-cors-headers==4.2.0
     # via -r requirements.in
-django-filter==22.1
+django-filter==23.2
     # via -r requirements.in
-django-prometheus==2.2.0
+django-prometheus==2.3.1
     # via -r requirements.in
-django-redis==5.2.0
+django-redis==5.3.0
     # via -r requirements.in
 django-rest-auth==0.9.5
     # via -r requirements.in
 django-sslserver==0.22
     # via -r requirements.in
 django-storages==1.13.2
     # via -r requirements.in
-django-timezone-field==5.0
+django-timezone-field==5.1
     # via django-celery-beat
 djangorestframework==3.14.0
     # via
     #   -r requirements.in
     #   django-rest-auth
     #   djangorestframework-datatables
     #   djangorestframework-simplejwt
     #   drf-extensions
     #   drf-yasg
 djangorestframework-datatables==0.7.0
     # via -r requirements.in
 djangorestframework-simplejwt==5.2.2
     # via -r requirements.in
-docutils==0.19
+docutils==0.20.1
     # via
     #   recommonmark
     #   sphinx
 drf-extensions==0.7.1
     # via -r requirements.in
-drf-yasg==1.21.5
+drf-yasg==1.21.7
     # via -r requirements.in
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
-gevent==22.10.2
+gevent==23.7.0
     # via -r requirements.in
 greenlet==2.0.2
     # via gevent
 html-json-forms==1.1.1
     # via -r requirements.in
-hvac==1.1.0
+hvac==1.1.1
     # via -r requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 inflection==0.5.1
     # via drf-yasg
 iniconfig==2.0.0
     # via pytest
-itypes==1.2.0
-    # via coreapi
 jinja2==3.1.2
-    # via
-    #   coreschema
-    #   sphinx
+    # via sphinx
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-jsonschema==4.17.3
+jsonschema==4.18.4
     # via -r requirements.in
-kombu==5.2.4
+jsonschema-specifications==2023.7.1
+    # via jsonschema
+kombu==5.3.1
     # via celery
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
-mysqlclient==2.1.1
+mysqlclient==2.2.0
     # via -r requirements.in
-packaging==23.0
+packaging==23.1
     # via
     #   -r requirements.in
     #   drf-yasg
     #   pytest
     #   sphinx
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-prometheus-client==0.16.0
+prometheus-client==0.17.1
     # via django-prometheus
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via click-repl
-psycopg2==2.9.5
+psycopg2==2.9.6
     # via -r requirements.in
-pygments==2.14.0
+pygments==2.15.1
     # via sphinx
 pyhcl==0.4.4
     # via hvac
-pyjwt==2.6.0
+pyjwt==2.8.0
     # via djangorestframework-simplejwt
-pyrsistent==0.19.3
-    # via jsonschema
-pytest==7.2.2
+pytest==7.4.0
     # via
     #   -r requirements.in
     #   pytest-cov
     #   pytest-dependency
     #   pytest-django
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements.in
 pytest-dependency==0.5.1
     # via -r requirements.in
 pytest-django==4.5.2
     # via -r requirements.in
-python-crontab==2.7.1
+python-crontab==3.0.0
     # via django-celery-beat
 python-dateutil==2.8.2
     # via
     #   botocore
+    #   celery
     #   python-crontab
-pytz==2022.7.1
+pytz==2023.3
     # via
-    #   celery
     #   django-timezone-field
     #   djangorestframework
     #   djangorestframework-datatables
     #   drf-yasg
-pyyaml==6.0
-    # via -r requirements.in
+pyyaml==6.0.1
+    # via
+    #   -r requirements.in
+    #   drf-yasg
 rabbitmq-admin==0.2
     # via -r requirements.in
 recommonmark==0.7.1
     # via -r requirements.in
-redis==4.5.1
+redis==4.6.0
     # via django-redis
-requests==2.28.2
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+requests==2.31.0
     # via
     #   -r requirements.in
-    #   coreapi
     #   hvac
     #   rabbitmq-admin
     #   sphinx
-ruamel-yaml==0.17.21
-    # via drf-yasg
-ruamel-yaml-clib==0.2.7
-    # via ruamel-yaml
-s3transfer==0.6.0
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
+s3transfer==0.6.1
     # via boto3
-sentry-sdk==1.16.0
+sentry-sdk==1.28.1
     # via -r requirements.in
 simplejson==3.17.4
     # via -r requirements.in
 six==1.16.0
     # via
-    #   click-repl
     #   django-rest-auth
     #   python-dateutil
     #   rabbitmq-admin
     #   sphinxcontrib-httpdomain
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==6.1.3
+sphinx==7.1.1
     # via
     #   -r requirements.in
     #   recommonmark
     #   sphinxcontrib-httpdomain
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
@@ -250,39 +247,42 @@
     # via -r requirements.in
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlparse==0.4.3
+sqlparse==0.4.4
     # via django
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-tzdata==2022.7
-    # via django-celery-beat
+typing-extensions==4.7.1
+    # via asgiref
+tzdata==2023.3
+    # via
+    #   celery
+    #   django-celery-beat
 uritemplate==4.1.1
     # via
     #   -r requirements.in
-    #   coreapi
     #   drf-yasg
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
     #   sentry-sdk
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
 wcwidth==0.2.6
     # via prompt-toolkit
-zope-event==4.6
+zope-event==5.0
     # via gevent
-zope-interface==5.5.2
+zope-interface==6.0
     # via gevent
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `tesla-ce-1.0.3/setup.py` & `tesla-ce-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/apps.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/apps.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/serializers.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/auth/views.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/auth/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,17 +350,19 @@
             :param data: Provided credentials with id and token fields
             :return: Authenticated object or None if authentication fails
         """
         with transaction.atomic():
             try:
                 launcher = models.Launcher.objects.get(id=data['id'],
                                                        token=data['token'])
+                token_pair = launcher.token_pair
+                launcher.delete()
             except models.Launcher.DoesNotExist:
                 return None
-        return launcher.token_pair
+        return token_pair
 
     def _add_token(self, auth_data):
         return decode_json(auth_data)
 
 
 class TokenRefreshView(AuthViewBase):
     """
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/permissions.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,25 @@
                 return request.user.inst_admin
             else:
                 return request.user.institutionuser.inst_admin
 
         return False
 
 
+class InstitutionAdminNotDeletePermission(InstitutionAdminPermission):
+    """
+        Only admins of the institution can access to the view
+    """
+    def has_permission(self, request, view):
+        if request.method != 'DELETE':
+            return super().has_permission(request, view)
+
+        return False
+
+
 class InstitutionAdminReadOnlyPermission(InstitutionAdminPermission):
     """
         Only admins of the institution can access to the view in read only mode
     """
     def has_permission(self, request, view):
         if request.method in permissions.SAFE_METHODS:
             return super().has_permission(request, view)
@@ -105,14 +116,21 @@
 
 class InstitutionDataAdminPermission(InstitutionMemberPermission):
     """
         Only admins of the institution can access to the view
     """
     def has_permission(self, request, view):
         if super().has_permission(request, view):
+            # todo: review if GLOBAL_ADMIN should be able to access to this view
+            '''
+                try:
+                    return request.user.institutionuser.institution
+                except User.institutionuser.RelatedObjectDoesNotExist:
+                    return None
+            '''
             if isinstance(request.user, InstitutionUser):
                 return request.user.data_admin
             else:
                 return request.user.institutionuser.data_admin
 
         return False
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/status.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/status.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/utils.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/tep.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/tep.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/serializers/tip.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/serializers/tip.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/tep.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/tep.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v1/views/tip.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v1/views/tip.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/institution.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/provider.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     credentials = serializers.SerializerMethodField(default=None, read_only=True)
 
     class Meta:
         model = Provider
         fields = ['id', 'instrument_id', 'instrument', 'name', 'queue', 'description', 'url', 'version', 'acronym',
                   'allow_validation', 'inverted_polarity', 'image', 'has_service', 'service_port', 'options_schema',
-                  'options', 'credentials', 'enabled', 'validation_active']
+                  'options', 'credentials', 'enabled', 'validation_active', 'warning_below', 'alert_below']
 
     def validate(self, attrs):
         """
             Validate the given attributes
             :param attrs: Attributes parsed from request
             :type attrs: dict
             :return: Validated attributes
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/ui_option.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/ui_option.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/admin/user.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/admin/user.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_report.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_report.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/activity_report_audit.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/activity_report_audit.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_group.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_group.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/course_learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/course_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent_document.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/informed_consent_document.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/institution.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/request.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/send_category.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/send_category.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/send_learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/send_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/ui_option.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/ui_option.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/user.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,19 +71,20 @@
         # Add predefined fields
         attrs['institution_id'] = self.context['view'].kwargs['parent_lookup_institution_id']
 
         # Check passwords
         if attrs.get('login_allowed', True):
             if 'password' in attrs and attrs.get('password') != attrs.get('password2'):
                 raise serializers.ValidationError('Passwords does not match')
-            if 'password2' in attrs:
-                del attrs['password2']
         else:
             attrs['login_allowed'] = False
 
+        if 'password2' in attrs:
+            del attrs['password2']
+
         # Apply validators
         for validator in self.get_validators():
             validator(attrs, self)
         return super().validate(attrs)
 
     def create(self, validated_data):
         new_user = super().create(validated_data)
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/institution/vle.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/institution/vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/enrolment_sample.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/enrolment_sample.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/provider_notification.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/provider_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/request_provider_result.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/request_provider_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,20 @@
         fields = ["id", "request", "learner_id", "result", "status", "error_message", "code", "audit", "audit_data"]
 
     def update(self, instance, validated_data):
         new_instance = super().update(instance, validated_data)
         new_instance.audit.save('{}__audit.json'.format(new_instance.request.data.name),
                                 ContentFile(simplejson.dumps(new_instance.audit_data).encode('utf-8')))
 
+        '''
         # If all the providers reported their results, launch summarise task
         if RequestProviderResult.objects.filter(Q(status=0) | Q(status=7),
                                                 request_id=new_instance.request_id,
                                                 provider__instrument=new_instance.provider.instrument
                                                 ).count() == 0:
             tasks.requests.verification.create_verification_summary.apply_async((
                     instance.request.id,
                     new_instance.provider.instrument_id,
             ))
+        '''
         return new_instance
+
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/validation.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/validation.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/provider/verification.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/provider/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/activity_report.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/activity_report.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/assessment_session.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/assessment_session.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/attachment.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/attachment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/course.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/course.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/instruments.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/instruments.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/launcher.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/launcher.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/request.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/serializers/vle/vle.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/serializers/vle/vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/institution.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/provider.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/ui_option.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/ui_option.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/admin/user.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/admin/user.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_report.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_report.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/activity_report_audit.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/activity_report_audit.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 from tesla_ce.apps.api.v2.serializers import InstitutionCourseSerializer
 from tesla_ce.models import Course
 from tesla_ce.models.user import is_global_admin
 from tesla_ce.models.user import get_institution_user
 
 
 # pylint: disable=too-many-ancestors
-class InstitutionCourseViewSet(NestedViewSetMixin, viewsets.ReadOnlyModelViewSet):
+class InstitutionCourseViewSet(NestedViewSetMixin, viewsets.ModelViewSet):
     """
     API endpoint that allows course in a vle to be viewed or edited.
     """
     model = Course
     serializer_class = InstitutionCourseSerializer
     filter_backends = [SearchFilter, DjangoFilterBackend, OrderingFilter]
     permission_classes = [
         permissions.InstitutionMemberReadOnlyPermission |
         permissions.GlobalAdminReadOnlyPermission |
-        permissions.InstitutionAdminPermission
+        permissions.InstitutionAdminNotDeletePermission |
+        permissions.InstitutionDataAdminPermission
     ]
     # filterset_fields = ['code', 'vle_course_id', 'description', 'vle']
     # search_fields = ['vle_course_id', 'description', 'code', 'vle']
 
     def get_queryset(self):
         # Except for global admins, and institution admins and data admins, returns only the courses where the user is
         # involved as instructor or learner
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_group.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_group.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/course_learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/course_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/informed_consent.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/informed_consent.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/informed_consent_document.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/informed_consent_document.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/institution.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/learner.py`

 * *Files 10% similar despite different names*

```diff
@@ -129,21 +129,27 @@
                 learner.save()
             else:
                 return Response('No Informed Consent to reject', status=status.HTTP_404_NOT_FOUND)
 
         serializer = self.get_serializer(learner)
         return Response(serializer.data)
 
-    @action(detail=True, methods=['GET'])
+    @action(detail=True, methods=['GET', 'DELETE'], permission_classes=[
+        permissions.InstitutionMemberReadOnlyPermission | permissions.InstitutionDataAdminPermission])
     def enrolment(self, request, *args, **kwargs):
         """
             Get learner enrolment status
         """
+        # todo: check if learner1 can not see learner2 enrolment
         learner = Learner.objects.get(
             pk=kwargs['pk'],
             institution_id=kwargs['parent_lookup_institution_id']
         )
 
-        if 'activity_id' in request.query_params:
-            return Response(learner.missing_enrolments(int(request.query_params['activity_id'])))
+        if request.method == 'GET':
+            if 'activity_id' in request.query_params:
+                return Response(learner.missing_enrolments(int(request.query_params['activity_id'])))
 
-        return Response(learner.enrolment_status)
+            return Response(learner.enrolment_status)
+        elif request.method == 'DELETE':
+            learner.delete_unused_enrolments()
+            return Response(learner.enrolment_status)
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/request.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/send_category.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/send_category.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/send_learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/send_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/ui_option.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/ui_option.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/user.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,20 +98,27 @@
     model = InstitutionUser
     serializer_class = InstitutionUserSerializer
     filter_backends = [SearchFilter, DjangoFilterBackend, OrderingFilter]
     filterset_class = InstitutionUserFilter
     search_fields = ['username', 'first_name', 'last_name', 'email', 'uid']
     permission_classes = [
         permissions.GlobalAdminReadOnlyPermission |
-        permissions.InstitutionAdminPermission |
+        permissions.InstitutionAdminNotDeletePermission |
         permissions.InstitutionLegalAdminReadOnlyPermission |
-        permissions.InstitutionDataAdminReadOnlyPermission |
+        permissions.InstitutionDataAdminPermission |
         permissions.InstitutionMemberReadOnlyPermission
     ]
 
+    def destroy(self, request, *args, **kwargs):
+        inst_user = get_institution_user(self.request.user)
+        if inst_user is not None and int(kwargs['pk']) == inst_user.id:
+            raise PermissionDenied("Cannot delete yourself")
+
+        return super().destroy(request, *args, **kwargs)
+
     def get_queryset(self):
         queryset = self.filter_queryset_by_parents_lookups(InstitutionUser.objects)
         if not is_global_admin(self.request.user):
             inst_user = get_institution_user(self.request.user)
             if not inst_user.inst_admin and not inst_user.legal_admin and not inst_user.data_admin:
                 queryset = queryset.filter(id=inst_user.id)
         return queryset.all().order_by('id')
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/institution/vle.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/institution/vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/enrolment_sample.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/enrolment_sample.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/provider.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/provider_notification.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/provider_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/request_provider_result.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/request_provider_result.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/provider/validation.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/provider/validation.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/activity_report.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/activity_report.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/course.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/course.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/learner.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/request.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/api/v2/views/vle/vle.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/api/v2/views/vle/vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/apps.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/apps.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/alert.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/alert.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/profile.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/profile.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/status.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/status.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/serializers/verification.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/serializers/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/utils.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/alert.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/alert.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/base.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/profile.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/profile.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/status.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/status.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/lapi/views/verification.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/lapi/views/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/apps.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/apps.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/base.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/client/provider.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/client/provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/exceptions.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps/webhooks/views.py` & `tesla-ce-1.0.8/src/tesla_ce/apps/webhooks/views.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/apps.py` & `tesla-ce-1.0.8/src/tesla_ce/apps.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/celery_app.py` & `tesla-ce-1.0.8/src/tesla_ce/celery_app.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/client.py` & `tesla-ce-1.0.8/src/tesla_ce/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -934,14 +934,15 @@
             'locale': locale,
             'options': options
         }
 
         # Store the session data
         session_data = models.AssessmentSessionData.objects.create(session=session)
         session_connector_data_path = os.path.join(str(learner.institution.id),
+                                                   'launchers',
                                                    str(learner.learner_id),
                                                    'sessions',
                                                    str(session.activity_id),
                                                    str(session.id), 'data.json'
                                                    )
         session_data.data.save(session_connector_data_path,
                                ContentFile(simplejson.dumps(session_connector_data).encode('utf-8')))
@@ -958,14 +959,15 @@
             'active': activity.enabled and len(instruments) > 0
         }
         session_connector = render_to_string('web-plugin/connector.js',
                                              {'session_data': simplejson.dumps(connector_data)})
 
         # Create the data path
         session_connector_path = os.path.join(str(learner.institution.id),
+                                              'launchers',
                                               str(learner.learner_id),
                                               'sessions',
                                               str(session.activity_id),
                                               str(session.id), 'connector.js'
                                     )
         # Write assessment info file
         session_data.connector.save(session_connector_path, ContentFile(session_connector.encode('utf-8')))
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/error.py` & `tesla-ce-1.0.8/src/tesla_ce/error.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/fixtures/ui_options.json` & `tesla-ce-1.0.8/src/tesla_ce/fixtures/ui_options.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/auth.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/auth.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/checks.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/checks.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/config/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/config/conf.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/config/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,14 +175,24 @@
             ('specific_ca_cert', 'Specific CA certificate', 'str', None, None, True),
         )),
         ('supervisor', 'TeSLA CE Supervisor configuration.', (
             ('secret', 'Supervisor Secret', 'str', None, None, True),
             ('admin_user', 'Administrator username', 'str', 'admin', None, True),
             ('admin_password', 'Administrator password', 'str', None, None, True),
             ('admin_email', 'Administrator email', 'str', None, None, True),
+        )),
+        ('tpt_service', 'TeSLA TPT Service configuration.', (
+            ('api_secret', 'API secret shared with TeSLA CE API', 'str', None, None, True),
+            ('db_password', 'Database password', 'str', None, None, True),
+            ('db_user', 'Database user', 'str', 'tpt_user', None, True),
+            ('db_address', 'Database address', 'str', 'localhost', None, True),
+            ('db_database', 'Database name', 'str', 'tpt_db', None, True),
+            ('db_port', 'Database port', 'int', 5432, None, True),
+            ('db_schema', 'Database schema', 'str', 'tpt_schema', None, True),
+            ('db_engine', 'Database engine', 'str', 'postgresql+psycopg2', None, True)
         ))
     )
 
     def __init__(self):
         """ Default class constructor """
 
         #: Configuration values contained in this class
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/config/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/config/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/data/messages.csv` & `tesla-ce-1.0.8/src/tesla_ce/lib/data/messages.csv`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/db/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/db/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/db/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/db/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/decorators.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/deploy/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/deploy/deployment.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/deploy/deployment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/deploy/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/deploy/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/exception.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/modules.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/modules.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/queues/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/queues/base.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/queues/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/queues/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/queues/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/storage/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/storage/bucket.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/storage/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/storage/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/vault/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/vault/manager.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/vault/manager.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/vault/policies.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/vault/policies.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/lib/vault/setup.py` & `tesla-ce-1.0.8/src/tesla_ce/lib/vault/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Vault setup module """
+import base64
 import random
 import string
 import time
+import json
+
+from django.utils import timezone
 
 import hvac
 from hvac.exceptions import InvalidPath
 from hvac.exceptions import InvalidRequest
 
 from .policies import get_policies
 from .policies import get_service_config_map
@@ -219,39 +223,71 @@
             for module in get_modules():
                 check_keys.append(MODULE_KEY_STR_TEMPLATE.format(module))
 
             result['transit']['read'] = True
             result['transit']['sign'] = True
             for check_key in check_keys:
                 # read checks
+                jwt_signing_key = None
                 try:
                     response = self._client.secrets.transit.read_key(check_key, mount_point=self._transit_mount_point)
-
+                    jwt_signing_key = response['data']
                 except hvac.exceptions.Forbidden:
                     result['transit']['read'] = False
                     result['steps'].append({"msg": "Transit read is forbidden with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
                 except hvac.exceptions.Unauthorized:
                     result['steps'].append({"msg": "Transit read is unauthorized with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
                 except hvac.exceptions.VaultError as err:
                     result['steps'].append({"msg": str(err), "status": False})
 
                 # write/sign checks
-                try:
-                    response = self._client.secrets.transit.encrypt_data(check_key, "testing")
-
-                except hvac.exceptions.Forbidden:
-                    result['transit']['sign'] = False
-                    result['steps'].append({"msg": "Transit encrypt is forbidden with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
-                except hvac.exceptions.Unauthorized:
-                    result['steps'].append({"msg": "Transit encrypt is unauthorized with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
-                except hvac.exceptions.VaultError as err:
-                    result['steps'].append({"msg": str(err), "status": False})
+                if jwt_signing_key is not None:
+                    # Sign the token
+                    try:
+                        key = check_key
+                        # Build the header
+                        header = {
+                            'alg': "RS256",
+                            'typ': "JWT",
+                            'ver': '{}:v{}'.format(key, jwt_signing_key['latest_version'])
+                        }
+
+                        # Get current time and expiration
+                        current_time = timezone.now()
+                        expiration_time = current_time + timezone.timedelta(minutes=2)
+
+                        # Build payload with basic fields
+                        vault_url = self._config.get('VAULT_URL')
+                        payload = {
+                            'iss': vault_url,
+                            'iat': int(current_time.timestamp()),
+                            'exp': int(expiration_time.timestamp()),
+                            'group': key,
+                        }
+                        b64_header = base64.urlsafe_b64encode(json.dumps(header).encode('utf8')).decode('ascii')
+                        b64_payload = base64.urlsafe_b64encode(json.dumps(payload).encode('utf8')).decode('ascii')
+                        b64_message = base64.b64encode('{}.{}'.format(b64_header, b64_payload).encode('utf8')).decode('ascii')
+
+                        sign_data_response = self._client.secrets.transit.sign_data(
+                            name=check_key,
+                            hash_input=b64_message,
+                            hash_algorithm='sha2-256',
+                            signature_algorithm='pkcs1v15',
+                            key_version=jwt_signing_key['latest_version'],
+                            mount_point=self._transit_mount_point,
+                        )
+                    except hvac.exceptions.Forbidden:
+                        result['transit']['sign'] = False
+                        result['steps'].append({"msg": "Transit encrypt is forbidden with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
+                    except hvac.exceptions.Unauthorized:
+                        result['steps'].append({"msg": "Transit encrypt is unauthorized with provided credentials. Error key {}.".format(MODULE_KEY_STR_TEMPLATE.format(module)), "status": False})
+                    except hvac.exceptions.VaultError as err:
+                        result['steps'].append({"msg": str(err), "status": False})
 
         # check policies
-        # todo: refactor
         policies = self._adapt_policies_path(get_policies())
         result['policies']['read'] = True
         for policy in policies:
             try:
                 self._client.sys.read_policy(
                     name='{}{}'.format(self._policy_prefix, policy)
                 )
@@ -481,40 +517,39 @@
 
     def check_policies(self):
         """
             Creates the policies to grant access to services
         """
         # Create generic policies
         policies = self._adapt_policies_path(get_policies())
+
         result = {
             "policies": [],
             "is_valid": True
         }
         for policy in policies:
             try:
                 vault_policy = self._client.sys.read_policy(
                     name='{}{}'.format(self._policy_prefix, policy)
                 )
+
+                vault_policy_data = json.loads(vault_policy['data']['rules'])
+
                 result['policies'].append({
                     "policy": '{}{}'.format(self._policy_prefix, policy),
-                    "expected": policy,
-                    "current": vault_policy,
-                    "exist": "True|False",
-                    "is_valid": "True|False"
+                    "expected": policies[policy],
+                    "current": vault_policy_data,
+                    "exist": True,
+                    "is_valid": (policies[policy] == vault_policy_data)
                 })
-                # todo: implement
-                # vault_policy != policy
-                # result['is_valid'] = False
 
             except hvac.exceptions.InvalidPath:
                 # policy not found
                 result['is_valid'] = False
 
-
-
         return result
 
     def setup_policies(self):
         """
             Creates the policies to grant access to services
         """
         # Create generic policies
@@ -568,15 +603,15 @@
     def setup_roles(self):
         """
             Creates the roles for the different modules that needs to authenticate with Vault
         """
         if not self._is_auth_method_enabled('{}/'.format(self._approle_mount_point)):
             config = {
                 'default_lease_ttl': self.approle_default_ttl,
-                 'max_lease_ttl': self.approle_max_ttl
+                'max_lease_ttl': self.approle_max_ttl
             }
             self._client.sys.enable_auth_method('approle', path=self._approle_mount_point, config=config,
                                                 description='TeSLA CE modules authentication')
         else:
             a = self._client.sys.read_auth_method_tuning(self._approle_mount_point)
             self._client.sys.tune_auth_method(self._approle_mount_point, default_lease_ttl=self.approle_default_ttl,
                                                max_lease_ttl=self.approle_max_ttl)
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/manage.py` & `tesla-ce-1.0.8/src/tesla_ce/manage.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/management/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/base.py` & `tesla-ce-1.0.8/src/tesla_ce/management/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_core.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_core.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_services.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_services.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/deploy_vle.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/deploy_vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/generate_config.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/rebuild_reports.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/rebuild_reports.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/reconfigure.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/reconfigure.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/register_provider.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/register_provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/register_vle.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/register_vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/register_webhook.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/register_webhook.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/remote_setup.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/remote_setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,15 +113,16 @@
             'vault_init_kv',
             'vault_init_policies',
             'vault_init_transit',
             'vault_init_roles',
             'migrate_database',
             'collect_static',
             'load_fixtures',
-            'create_superuser'
+            'create_superuser',
+            'register_tpt_webhook'
         ]
 
         status = {"status": False, "info": {}}
 
         if command not in valid_commands:
             status['info'] = "Command [{}] is not valid".format(command)
 
@@ -186,9 +187,20 @@
                                                       password=self.client.config.config.get('tesla_admin_password'),
                                                       email=self.client.config.config.get('tesla_admin_mail')
                                                       )
                 status['status'] = True
             except TeslaDatabaseException as exc:
                 status['status'] = False
                 status['info'] = str(exc)
+        elif command in ['register_tpt_webhook']:
+            try:
+                name = 'tpt'
+                client_header = 'TESLA-TPT-METHOD'
+                id_header = 'TESLA-TPT-MESSAGE-ID'
+                credentials = "{\"secret\": \""+self.client.config.config.get('tpt_service_api_secret')+"\"}"
+                provider_info = self.client.register_webhook(name, client_header, id_header, credentials)
+                status['status'] = True
+            except Exception as err:
+                status['status'] = False
+                status['info'] = str(err)
 
         self.report_remote_result(status=status)
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/resend_requests.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/resend_requests.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/resend_samples.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/resend_samples.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/tesla_version.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/tesla_version.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/management/commands/unseal.py` & `tesla-ce-1.0.8/src/tesla_ce/management/commands/unseal.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0001_initial.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0002_histograms.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0002_histograms.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0003_providernotification.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0003_providernotification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0004_launcher.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0004_launcher.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0005_auto_20200520_2009.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0005_auto_20200520_2009.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0006_auto_20200520_2128.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0006_auto_20200520_2128.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0007_auto_20200712_1330.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0007_auto_20200712_1330.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0008_auto_20200721_1022.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0008_auto_20200721_1022.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0009_monitor.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0009_monitor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0010_auto_20200930_1829.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0010_auto_20200930_1829.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0011_auto_20200930_1842.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0011_auto_20200930_1842.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0012_auto_20210415_1829.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0012_auto_20210415_1829.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0013_webhookclient_webhookmessage.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0013_webhookclient_webhookmessage.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0014_uioption.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0014_uioption.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0016_auto_20210709_1023.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0016_auto_20210709_1023.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0017_auto_20210715_2150.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0017_auto_20210715_2150.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0019_auto_20210907_1602.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0019_auto_20210907_1602.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0021_alter_reportactivitysession_session.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0021_alter_reportactivitysession_session.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0022_auto_20211124_1252.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0022_auto_20211124_1252.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/migrations/0023_alter_launcher_session.py` & `tesla-ce-1.0.8/src/tesla_ce/migrations/0023_alter_launcher_session.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/activity.py` & `tesla-ce-1.0.8/src/tesla_ce/models/activity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/models/activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/alert.py` & `tesla-ce-1.0.8/src/tesla_ce/models/alert.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Alert message model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .activity import Activity
 from .assessment_session import AssessmentSession
 from .base_model import BaseModel
 from .instrument import Instrument
 from .learner import Learner
@@ -81,7 +82,20 @@
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __repr__(self):
         return "<Alert(learner='%s', activity='%r', level='%r')>" % (
             self.learner, self.activity, self.get_level_display()
         )
+
+
+@receiver(models.signals.post_delete, sender=Alert)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.data:
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/assessment_session.py` & `tesla-ce-1.0.8/src/tesla_ce/models/assessment_session.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/assessment_session_data.py` & `tesla-ce-1.0.8/src/tesla_ce/models/assessment_session_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Assessment session data model module."""
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .assessment_session import AssessmentSession
 from .base_model import BaseModel
 
 
 class AssessmentSessionData(BaseModel):
@@ -28,10 +29,25 @@
     connector = models.FileField(help_text=_('Connector JS file for this session'))
 
     data = models.FileField(help_text=_('Data for this session'))
 
     def __repr__(self):
         return "<AssessmentSessionData(session_id='%r')>" % (self.session_id)
 
-    def delete(self, using=None, keep_parents=False):
-        # TODO: Remove data from storage
-        return super().delete(using, keep_parents)
+
+@receiver(models.signals.post_delete, sender=AssessmentSessionData)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.connector:
+        try:
+            instance.connector.delete(save=False)
+        except:
+            pass
+
+    if instance.data:
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/base_model.py` & `tesla-ce-1.0.8/src/tesla_ce/models/base_model.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/course.py` & `tesla-ce-1.0.8/src/tesla_ce/models/course.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/course_group.py` & `tesla-ce-1.0.8/src/tesla_ce/models/course_group.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/models/enrolment.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Enrolment model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .enrolment_sample import EnrolmentSample
 from .learner import Learner
 from .learner import get_learner_enrolment
 from .provider import Provider
@@ -90,7 +91,20 @@
                                                                       self.can_analyse, self.is_locked,
                                                                       self.model_total_samples)
 
     def save(self, force_insert=False, force_update=False, using=None, update_fields=None):
         super().save(force_insert, force_update, using, update_fields)
         # Invalidate cached value
         get_learner_enrolment.invalidate(self.learner_id)
+
+
+@receiver(models.signals.post_delete, sender=Enrolment)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.model:
+        try:
+            instance.model.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/enrolment_sample.py` & `tesla-ce-1.0.8/src/tesla_ce/models/enrolment_sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Enrolment sample request model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .instrument import Instrument
 from .learner import Learner
 from .message import Message
 
@@ -53,7 +54,21 @@
     data = models.FileField(max_length=250, null=False, blank=False, help_text=_("Data path on storage."))
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __repr__(self):
         return "<EnrolmentSample(learner='%s', status='%r')>" % (self.learner, self.status, )
+
+
+@receiver(models.signals.post_delete, sender=EnrolmentSample)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.data:
+        # todo: remove .valid and .error associated files
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/enrolment_sample_validation.py` & `tesla-ce-1.0.8/src/tesla_ce/models/enrolment_sample_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Enrolment sample validation model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .enrolment_sample import EnrolmentSample
 from .learner import get_learner_enrolment
 from .message import Message
 from .provider import Provider
@@ -67,7 +68,20 @@
         return "<EnrolmentSampleValidation(sample='%s', provider='%s', status='%r')>" % (
             self.sample_id, self.provider_id, self.get_status_display())
 
     def save(self, force_insert=False, force_update=False, using=None, update_fields=None):
         super().save(force_insert, force_update, using, update_fields)
         # Invalidate cached value
         get_learner_enrolment.invalidate(self.sample.learner_id)
+
+
+@receiver(models.signals.post_delete, sender=EnrolmentSampleValidation)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.info:
+        try:
+            instance.info.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/histogram_activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/models/histogram_activity_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/histogram_activity_provider.py` & `tesla-ce-1.0.8/src/tesla_ce/models/histogram_activity_provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/histogram_learner_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/models/histogram_learner_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/histogram_learner_provider.py` & `tesla-ce-1.0.8/src/tesla_ce/models/histogram_learner_provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/informed_consent.py` & `tesla-ce-1.0.8/src/tesla_ce/models/informed_consent.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/informed_consent_document.py` & `tesla-ce-1.0.8/src/tesla_ce/models/informed_consent_document.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ InformedConsentDocument model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .informed_consent import InformedConsent
 
 
 def get_upload_path(instance, filename):
@@ -55,7 +56,20 @@
 
     class Meta:
         unique_together = (('consent', 'language'),)
 
     def __repr__(self):
         return "<InformedConsentDocument(consent_id='%d', language='%s')>" % (
             self.consent.id, self.language)
+
+
+@receiver(models.signals.post_delete, sender=InformedConsentDocument)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.pdf:
+        try:
+            instance.pdf.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/institution.py` & `tesla-ce-1.0.8/src/tesla_ce/models/institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/instructor.py` & `tesla-ce-1.0.8/src/tesla_ce/models/instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/models/instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/launcher.py` & `tesla-ce-1.0.8/src/tesla_ce/models/launcher.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/learner.py` & `tesla-ce-1.0.8/src/tesla_ce/models/learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Learner model module."""
 import uuid
 
 from cache_memoize import cache_memoize
+from django.core.files.storage import default_storage
 from django.db import models
+from django.dispatch import receiver
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 from tesla_ce.apps.api.utils import decode_json
 from .informed_consent import InformedConsent
 from .user import InstitutionUser
 
@@ -249,7 +251,38 @@
     def missing_enrolments(self, activity_id):
         """
             Get the missing enrolments for a particular activity
             :param activity_id: Activity id
             :return: Aggregated values per instrument
         """
         return get_missing_enrolment(self.id, activity_id)
+
+    def delete_unused_enrolments(self):
+        """
+            Delete unused enrolments for this learner
+            :return:
+        """
+        # todo: optimize this
+        for enrolment in self.enrolment_set.all():
+            delete = True
+            for request in self.request_set.all():
+                if enrolment.provider.instrument in request.instruments.all():
+                    delete = False
+                    break
+            if delete:
+                for model_sample in enrolment.model_samples.all():
+                    model_sample.delete()
+
+                enrolment.delete()
+
+@receiver(models.signals.post_delete, sender=Learner)
+def auto_delete_folders_on_delete(sender, instance, **kwargs):
+    """
+    Deletes folders from filesystem
+    when corresponding object is deleted.
+    """
+
+    for data in ['enrolment', 'models', 'requests', 'results', 'launchers']:
+        try:
+            default_storage.delete(f'{instance.institution.id}/{data}/{instance.learner_id}')
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/message.py` & `tesla-ce-1.0.8/src/tesla_ce/models/message.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/monitor.py` & `tesla-ce-1.0.8/src/tesla_ce/models/monitor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/provider.py` & `tesla-ce-1.0.8/src/tesla_ce/models/provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/provider_notification.py` & `tesla-ce-1.0.8/src/tesla_ce/models/provider_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/report_activity.py` & `tesla-ce-1.0.8/src/tesla_ce/models/report_activity.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Report Activity model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .activity import Activity
 from .base_model import BaseModel
 from .learner import Learner
 
 REPORT_ALERT_LEVEL = (
@@ -54,7 +55,20 @@
 
     class Meta:
         unique_together = (('activity', 'learner'),)
 
     def __repr__(self):
         return "<ReportActivity(id='%r', learner_id='%r' activity_id='%r')>" % (
             self.id, self.learner_id, self.activity_id)
+
+
+@receiver(models.signals.post_delete, sender=ReportActivity)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.data:
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/report_activity_instrument.py` & `tesla-ce-1.0.8/src/tesla_ce/models/report_activity_instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """ Report Activity Instrument model module."""
 from enum import Enum
 import json
 
 from django.core.files.base import ContentFile
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .instrument import Instrument
 from .report_activity import REPORT_ALERT_LEVEL
 from .report_activity import ReportActivity
 from .request_provider_result import RequestProviderResult
@@ -335,7 +336,20 @@
                     except Exception:
                         sample_data = None
                     audit['enrolment_samples'][sample.id] = sample_data
                 audit['providers'][provider_id]['enrolment_samples'].append(sample.id)
                 audit['providers'][provider_id]['enrolment_percentage'] = enrolment.percentage
 
         return audit
+
+
+@receiver(models.signals.post_delete, sender=ReportActivityInstrument)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.audit_data:
+        try:
+            instance.audit_data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/report_activity_session.py` & `tesla-ce-1.0.8/src/tesla_ce/models/report_activity_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Report Activity model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .assessment_session import AssessmentSession
 from .base_model import BaseModel
 from .report_activity import ReportActivity
 from .report_activity import REPORT_ALERT_LEVEL
 
@@ -57,7 +58,20 @@
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __repr__(self):
         return "<ReportActivitySession(id='%r', session_id='%r', learner_id='%r' activity_id='%r')>" % (
             self.id, self.session.id, self.session.learner.learner_id, self.session.activity_id)
+
+
+@receiver(models.signals.post_delete, sender=ReportActivitySession)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.data:
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/request.py` & `tesla-ce-1.0.8/src/tesla_ce/models/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Request model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .activity import Activity
 from .assessment_session import AssessmentSession
 from .base_model import BaseModel
 from .instrument import Instrument
 from .learner import Learner
@@ -63,7 +64,21 @@
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __repr__(self):
         return "<Request(learner='%s', activity='%r', status='%r')>" % (self.learner, self.activity,
                                                                         self.status, )
+
+
+@receiver(models.signals.post_delete, sender=Request)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.data:
+        # todo: remove .valid and .error associated files
+        try:
+            instance.data.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/request_provider_result.py` & `tesla-ce-1.0.8/src/tesla_ce/models/request_provider_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Request Provider Result model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.db import transaction
+from django.db.models import Q
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .histogram_activity_instrument import HistogramActivityInstrument
 from .histogram_activity_provider import HistogramActivityProvider
 from .histogram_learner_instrument import HistogramLearnerInstrument
 from .histogram_learner_provider import HistogramLearnerProvider
@@ -115,7 +117,31 @@
                     setattr(h4, bin, getattr(h4, bin) + 1)
                     h4.save()
                 except HistogramActivityProvider.DoesNotExist:
                     h4 = HistogramActivityProvider(activity=self.request.activity,
                                                    provider=self.provider)
                     setattr(h4, bin, 1)
                     h4.save()
+
+        # If all the providers reported their results, launch summarise task
+        if RequestProviderResult.objects.filter(Q(status=0) | Q(status=7),
+                                                request_id=self.request_id,
+                                                provider__instrument=self.provider.instrument
+                                                ).count() == 0:
+            from ..tasks.requests.verification import create_verification_summary
+            create_verification_summary.apply_async((
+                self.request.id,
+                self.provider.instrument_id,
+            ))
+
+
+@receiver(models.signals.post_delete, sender=RequestProviderResult)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.audit:
+        try:
+            instance.audit.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/request_result.py` & `tesla-ce-1.0.8/src/tesla_ce/models/request_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ Request model module."""
 
 from django.db import models
+from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
 from .base_model import BaseModel
 from .instrument import Instrument
 from .message import Message
 from .request import Request
 
@@ -75,7 +76,20 @@
 
     def __repr__(self):
         return "<RequestResult(request='%s', instrument='%s', status='%r', " \
                "result='%r', code='%s')>" % (
                    self.request.id, self.instrument.acronym, self.get_status_display(),
                    self.result, self.get_code_display()
         )
+
+
+@receiver(models.signals.post_delete, sender=RequestResult)
+def auto_delete_file_on_delete(sender, instance, **kwargs):
+    """
+    Deletes file from filesystem
+    when corresponding `FieldField` object is deleted.
+    """
+    if instance.audit:
+        try:
+            instance.audit.delete(save=False)
+        except:
+            pass
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/send_category.py` & `tesla-ce-1.0.8/src/tesla_ce/models/send_category.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/send_learner.py` & `tesla-ce-1.0.8/src/tesla_ce/models/send_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/ui_option.py` & `tesla-ce-1.0.8/src/tesla_ce/models/ui_option.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/user.py` & `tesla-ce-1.0.8/src/tesla_ce/models/user.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/vle.py` & `tesla-ce-1.0.8/src/tesla_ce/models/vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/models/webhooks.py` & `tesla-ce-1.0.8/src/tesla_ce/models/webhooks.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/settings.py` & `tesla-ce-1.0.8/src/tesla_ce/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     MIDDLEWARE = [
         'django_prometheus.middleware.PrometheusBeforeMiddleware',
         'corsheaders.middleware.CorsMiddleware',
         'django.middleware.security.SecurityMiddleware',
         'django.contrib.sessions.middleware.SessionMiddleware',
         'django.middleware.common.CommonMiddleware',
         'django.middleware.csrf.CsrfViewMiddleware',
-        'corsheaders.middleware.CorsPostCsrfMiddleware',
+        #'corsheaders.middleware.CorsPostCsrfMiddleware',
         #'tesla_ce.lib.auth.tesla_token_auth_middleware',
         'django.contrib.auth.middleware.AuthenticationMiddleware',
         'django.contrib.messages.middleware.MessageMiddleware',
         'django.middleware.clickjacking.XFrameOptionsMiddleware',
         'tesla_ce.error.TeslaErrorHandlerMiddleware',
         'django_prometheus.middleware.PrometheusAfterMiddleware',
     ]
@@ -195,19 +195,37 @@
         if cls.TESLA_CONFIG.config.get('STORAGE_SSL_VERIFY') is False:
             cls.AWS_S3_VERIFY = False
 
         # Get the public bucket name
         cls.AWS_S3_STORAGE_PUBLIC_BUCKET_NAME = cls.TESLA_CONFIG.config.get('STORAGE_PUBLIC_BUCKET_NAME')
 
         if cls.AWS_ACCESS_KEY_ID is not None and cls.AWS_SECRET_ACCESS_KEY is not None:
-            cls.DEFAULT_FILE_STORAGE = 'storages.backends.s3boto3.S3Boto3Storage'
-            cls.STATICFILES_STORAGE = 'tesla_ce.lib.storage.bucket.PublicS3Boto3Storage'
+            # cls.DEFAULT_FILE_STORAGE = 'storages.backends.s3boto3.S3Boto3Storage'
+            # cls.STATICFILES_STORAGE = 'tesla_ce.lib.storage.bucket.PublicS3Boto3Storage'
             cls.STATIC_ROOT = '/'
+            cls.STORAGES = {
+                "default": {
+                    "BACKEND": 'storages.backends.s3boto3.S3Boto3Storage',
+                },
+                "staticfiles": {
+                    "BACKEND": 'tesla_ce.lib.storage.bucket.PublicS3Boto3Storage',
+                },
+            }
         else:
-            cls.DEFAULT_FILE_STORAGE = 'django.core.files.storage.FileSystemStorage'
+            #cls.DEFAULT_FILE_STORAGE = 'django.core.files.storage.FileSystemStorage'
+            cls.STORAGES = {
+                "default": {
+                    "BACKEND": 'django.core.files.storage.FileSystemStorage',
+                },
+                "staticfiles": {
+                    "BACKEND": "django.contrib.staticfiles.storage.StaticFilesStorage",
+                },
+            }
+
+
 
     @classmethod
     def pre_setup(cls):
         # Load DJango default configuration
         super().pre_setup()
 
         if len(cls.TESLA_CONFIG.modules) > 0:
@@ -411,12 +429,11 @@
                 content = response.content
                 if content is not None:
                     content = content.decode('utf8')
                 else:
                     content = ''
 
                 raise TeslaConfigException("Cannot get remote configuration. Server returns status code {}. Response content {}.".format(response.status_code, content))
-            print(os.path.dirname(output_file))
-            print(output_file)
+
             cls.TESLA_CONFIG.load_file(output_file)
         # Load Production configuration
         super().pre_setup()
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/favicon.ico` & `tesla-ce-1.0.8/src/tesla_ce/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/android-chrome-192x192.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/android-chrome-512x512.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-114x114-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-114x114-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-114x114.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-120x120-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-120x120-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-120x120.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-144x144-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-144x144-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-144x144.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-152x152-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-152x152-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-152x152.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-180x180-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-180x180-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-180x180.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-57x57-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-57x57-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-57x57.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-60x60-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-60x60-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-60x60.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-72x72-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-72x72-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-72x72.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-76x76-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-76x76-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-76x76.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon-precomposed.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/apple-touch-icon.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/favicon-16x16.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/favicon-32x32.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/favicon.ico` & `tesla-ce-1.0.8/src/tesla_ce/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/mstile-150x150.png` & `tesla-ce-1.0.8/src/tesla_ce/static/img/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/img/safari-pinned-tab.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/img/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/3rdpartylicenses.txt` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/bg.json` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/bg.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/ca.json` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/ca.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/en.json` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/en.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/es.json` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/es.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/i18n/fi.json` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/i18n/fi.json`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/activity.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/activity.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/authorship.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/authorship.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/connection.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/connection.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/content.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/content.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/course.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/course.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/dashboard.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/delete.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/delete.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/edit.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/edit.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/identity.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/identity.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/informed-consent.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/informed-consent.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/integrity.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/integrity.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/menu_logo.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/menu_logo.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/monitoring.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/monitoring.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/moreinfo.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/moreinfo.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/notifications.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/originality.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/originality.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/system.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/system.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/user.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/user.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/common/view.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/common/view.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/connection.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/connection.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/dashboard.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/dashboard.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fa.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/fr.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/ks.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/plag.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/plag.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/plagiarism.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/instrument/vr.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.png` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.png`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/menu_logo.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/notifications.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/notifications.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/admin.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/admin.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/data.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/data.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/instructor.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/instructor.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/learner.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/learner.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/legal.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/legal.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/send.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/send.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/role/superadmin.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/role/superadmin.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/assessment.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/camera.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/keyboard.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/assets/icons/sensor/microphone.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/favicon.ico` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/favicon.ico`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/styles.css` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/styles.css`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/web-plugin/web-plugin.js` & `tesla-ce-1.0.8/src/tesla_ce/static/web-plugin/web-plugin.js`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.eot` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.ttf` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.woff` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-brands-400.woff2` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.eot` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.ttf` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.woff` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-regular-400.woff2` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.eot` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.svg` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.ttf` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.woff` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/static/webfonts/fa-solid-900.woff2` & `tesla-ce-1.0.8/src/tesla_ce/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/monitor/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/monitor/celery.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/monitor/celery.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/notification/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/notification/providers.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/notification/providers.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/reports/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/reports/results.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/reports/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,20 +176,35 @@
             return
     results_qs = models.RequestResult.objects.filter(request__activity_id=activity_id,
                                                      instrument_id=instrument_id,
                                                      request__learner_id=learner_id)
 
     # Compute the final alert levels from result codes
     code_result = results_qs.filter(status=1).aggregate(Max('code'), Avg('result'))
+
+    if code_result['code__max'] is None:
+        code_result['code__max'] = 2  # Warning
+
+    if code_result['result__avg'] is None:
+        code_result['result__avg'] = 0
+
     instrument_report.result = round(code_result['result__avg'] * 100)
-    instrument_report.confidence = round(results_qs.filter(status=1).count() / results_qs.count() * 100)
+    if results_qs.count() != 0:
+        instrument_report.confidence = round(results_qs.filter(status=1).count() / results_qs.count() * 100)
+    else:
+        instrument_report.confidence = 0
+
     code = code_result['code__max']
     if code > 0:
         # Unless the code is 0 (PENDING), move to the alerts scale
         code += 1
+
+        if instrument_report.confidence < 60:
+            code = max(code, 2)  # Warning
+
     # Update levels where this instrument applies
     if instrument_report.instrument.identity:
         instrument_report.identity_level = code
     else:
         instrument_report.identity_level = 1  # No data
     if instrument_report.instrument.originality or instrument_report.instrument.authorship:
         instrument_report.content_level = code
@@ -206,14 +221,15 @@
     if instrument_report.instrument.requires_enrolment:
         instrument_report.enrolment = round(models.Enrolment.objects.filter(
             learner_id=learner_id,
             provider_id__in=results_qs.values_list(
                 'request__requestproviderresult__provider_id',
                 flat=True).distinct()
         ).aggregate(Min('percentage'))['percentage__min'] * 100)
+
     instrument_report.save()
 
     # Update the audit data
     instrument_report.update_audit()
 
     # Update the report
     update_learner_activity_report.apply_async((learner_id, activity_id,))
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/requests/__init__.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/requests/alerts.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/requests/alerts.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/tasks/requests/enrolment.py` & `tesla-ce-1.0.8/src/tesla_ce/tasks/requests/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_core.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_core.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_frontend.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_frontend.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_lb_traefik.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_lb_traefik.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_lti.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_lti.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_moodle.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_moodle.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_provider.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_provider.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/deployment/swarm/tesla_services.yml` & `tesla-ce-1.0.8/src/tesla_ce/templates/deployment/swarm/tesla_services.yml`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/doc/redoc.html` & `tesla-ce-1.0.8/src/tesla_ce/templates/doc/redoc.html`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/rest_framework/horizontal/Jsonform_field.html` & `tesla-ce-1.0.8/src/tesla_ce/templates/rest_framework/horizontal/Jsonform_field.html`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/templates/web-plugin/connector.js` & `tesla-ce-1.0.8/src/tesla_ce/templates/web-plugin/connector.js`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/urls.py` & `tesla-ce-1.0.8/src/tesla_ce/urls.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce/wsgi.py` & `tesla-ce-1.0.8/src/tesla_ce/wsgi.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tesla_ce.egg-info/PKG-INFO` & `tesla-ce-1.0.8/src/tesla_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce
-Version: 1.0.3
+Version: 1.0.8
 Summary: TeSLA CE
 Home-page: https://github.com/tesla-ce/core
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io
 Project-URL: Source, https://github.com/tesla-ce/core
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce.egg-info/SOURCES.txt` & `tesla-ce-1.0.8/src/tesla_ce.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,16 @@
 src/tesla_ce/lib/storage/__init__.py
 src/tesla_ce/lib/storage/bucket.py
 src/tesla_ce/lib/storage/manager.py
 src/tesla_ce/lib/vault/__init__.py
 src/tesla_ce/lib/vault/manager.py
 src/tesla_ce/lib/vault/policies.py
 src/tesla_ce/lib/vault/setup.py
+src/tesla_ce/lib/webhook/__init__.py
+src/tesla_ce/lib/webhook/process.py
 src/tesla_ce/management/__init__.py
 src/tesla_ce/management/base.py
 src/tesla_ce/management/commands/__init__.py
 src/tesla_ce/management/commands/deploy_core.py
 src/tesla_ce/management/commands/deploy_services.py
 src/tesla_ce/management/commands/deploy_vle.py
 src/tesla_ce/management/commands/generate_config.py
```

### Comparing `tesla-ce-1.0.3/src/tesla_ce.egg-info/requires.txt` & `tesla-ce-1.0.8/src/tesla_ce.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,105 +1,104 @@
 alabaster==0.7.13
 amqp==5.1.1
-asgiref==3.6.0
+asgiref==3.7.2
 async-timeout==4.0.2
-attrs==22.2.0
+attrs==23.1.0
 babel==2.12.1
-billiard==3.6.4.0
-boto3==1.26.89
-botocore==1.29.89
-celery==5.2.7
-certifi==2022.12.7
-charset-normalizer==3.1.0
+billiard==4.1.0
+boto3==1.28.14
+botocore==1.31.14
+celery==5.3.1
+certifi==2023.7.22
+charset-normalizer==3.2.0
 click-didyoumean==0.3.0
 click-plugins==1.1.1
-click-repl==0.2.0
-click==8.1.3
+click-repl==0.3.0
+click==8.1.6
 commonmark==0.9.1
-coreapi==2.3.3
-coreschema==0.0.4
-coverage[toml]==7.2.1
+coverage[toml]==7.2.7
+cron-descriptor==1.4.0
 django-cache-memoize==0.1.10
-django-celery-beat==2.4.0
-django-celery-results==2.5.0
-django-configurations==2.4
-django-cors-headers==3.14.0
-django-filter==22.1
-django-prometheus==2.2.0
-django-redis==5.2.0
+django-celery-beat==2.5.0
+django-celery-results==2.5.1
+django-configurations==2.4.1
+django-cors-headers==4.2.0
+django-filter==23.2
+django-prometheus==2.3.1
+django-redis==5.3.0
 django-rest-auth==0.9.5
 django-sslserver==0.22
 django-storages==1.13.2
-django-timezone-field==5.0
-django==4.1.7
+django-timezone-field==5.1
+django==4.2.3
 djangorestframework-datatables==0.7.0
 djangorestframework-simplejwt==5.2.2
 djangorestframework==3.14.0
-docutils==0.19
+docutils==0.20.1
 drf-extensions==0.7.1
-drf-yasg==1.21.5
-exceptiongroup==1.1.1
-gevent==22.10.2
+drf-yasg==1.21.7
+exceptiongroup==1.1.2
+gevent==23.7.0
 greenlet==2.0.2
 html-json-forms==1.1.1
-hvac==1.1.0
+hvac==1.1.1
 idna==3.4
 imagesize==1.4.1
 inflection==0.5.1
 iniconfig==2.0.0
-itypes==1.2.0
 jinja2==3.1.2
 jmespath==1.0.1
-jsonschema==4.17.3
-kombu==5.2.4
-markupsafe==2.1.2
-packaging==23.0
-pluggy==1.0.0
-prometheus-client==0.16.0
-prompt-toolkit==3.0.38
-pygments==2.14.0
+jsonschema-specifications==2023.7.1
+jsonschema==4.18.4
+kombu==5.3.1
+markupsafe==2.1.3
+packaging==23.1
+pluggy==1.2.0
+prometheus-client==0.17.1
+prompt-toolkit==3.0.39
+pygments==2.15.1
 pyhcl==0.4.4
-pyjwt==2.6.0
-pyrsistent==0.19.3
-pytest-cov==4.0.0
+pyjwt==2.8.0
+pytest-cov==4.1.0
 pytest-dependency==0.5.1
 pytest-django==4.5.2
-pytest==7.2.2
-python-crontab==2.7.1
+pytest==7.4.0
+python-crontab==3.0.0
 python-dateutil==2.8.2
-pytz==2022.7.1
-pyyaml==6.0
+pytz==2023.3
+pyyaml==6.0.1
 rabbitmq-admin==0.2
 recommonmark==0.7.1
-redis==4.5.1
-requests==2.28.2
-ruamel.yaml.clib==0.2.7
-ruamel.yaml==0.17.21
-s3transfer==0.6.0
-sentry-sdk==1.16.0
+redis==4.6.0
+referencing==0.30.0
+requests==2.31.0
+rpds-py==0.9.2
+s3transfer==0.6.1
+sentry-sdk==1.28.1
 simplejson==3.17.4
 six==1.16.0
 snowballstemmer==2.2.0
-sphinx==6.1.3
+sphinx==7.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-httpdomain==1.8.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.3
+sqlparse==0.4.4
 tomli==2.0.1
-tzdata==2022.7
+typing-extensions==4.7.1
+tzdata==2023.3
 uritemplate==4.1.1
-urllib3==1.26.15
+urllib3==1.26.16
 vine==5.0.0
 wcwidth==0.2.6
-zope.event==4.6
-zope.interface==5.5.2
+zope.event==5.0
+zope.interface==6.0
 
 []
 mysqlclient
 
 [all]
 mysqlclient
 psycopg2
```

### Comparing `tesla-ce-1.0.3/src/tests/__init__.py` & `tesla-ce-1.0.8/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/__init__.py` & `tesla-ce-1.0.8/src/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/__init__.py` & `tesla-ce-1.0.8/src/tests/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/test_institution.py` & `tesla-ce-1.0.8/src/tests/api/admin/test_institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/test_instrument.py` & `tesla-ce-1.0.8/src/tests/api/admin/test_instrument.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/test_provider.py` & `tesla-ce-1.0.8/src/tests/api/admin/test_provider.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/test_ui_options.py` & `tesla-ce-1.0.8/src/tests/api/admin/test_ui_options.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/admin/test_users.py` & `tesla-ce-1.0.8/src/tests/api/admin/test_users.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/__init__.py` & `tesla-ce-1.0.8/src/tests/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_approle.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_approle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_lapi_auth.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_lapi_auth.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_launcher_token.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_launcher_token.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_profile.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_profile.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_ui_options.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_ui_options.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/auth/test_userpass.py` & `tesla-ce-1.0.8/src/tests/api/auth/test_userpass.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/__init__.py` & `tesla-ce-1.0.8/src/tests/api/institution/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/__init__.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/activity/__init__.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/activity/report/__init__.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/activity/report/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/test_course.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/test_course.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/test_instructors.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/test_instructors.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/course/test_learners.py` & `tesla-ce-1.0.8/src/tests/api/institution/course/test_learners.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_course_group.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_course_group.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_informed_consent.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_informed_consent.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_institution.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_institution.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_instructor.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_instructor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_learner.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_learner.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_send.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_send.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_users.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_users.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,54 +60,92 @@
     assert profile['institution']['id'] == inst_id
     assert len(profile['roles']) == 0
     assert profile['username'] == user_name
     assert profile['email'] == email
     assert profile['first_name'] == user_name[:5]
     assert profile['last_name'] == user_name[5:]
 
-    # Grant administration privileges
+    # Grant administration privileges and data privileges (DATA privileges to remove user)
     user_mod_resp = client.patch(
         '/api/v2/institution/{}/user/{}/'.format(inst_id, user_create_resp.data['id']),
-        data={'inst_admin': True},
+        data={'inst_admin': True, 'data_admin': True},
         format='json'
     )
     assert user_mod_resp.status_code == 200
 
     # Get the user profile again
     profile = auth_utils.get_profile(user_client)
-    assert len(profile['roles']) == 1
+    assert len(profile['roles']) == 2
     assert 'ADMIN' in profile['roles']
+    assert 'DATA' in profile['roles']
 
     # Try to grant global administration privileges
     user_mod_resp2 = client.patch(
         '/api/v2/institution/{}/user/{}/'.format(inst_id, user_create_resp.data['id']),
         data={'is_staff': True},
         format='json'
     )
     assert user_mod_resp2.status_code == 200
 
     # Get the user profile again
     profile = auth_utils.get_profile(user_client)
-    assert len(profile['roles']) == 1
+    assert len(profile['roles']) == 2
     assert 'ADMIN' in profile['roles']
+    assert 'DATA' in profile['roles']
 
     # Find for this user by email
     find_user_resp = client.get('/api/v2/institution/{}/user/?email={}'.format(inst_id, email))
     assert find_user_resp.status_code == 200
     assert find_user_resp.data['count'] == 1
     assert find_user_resp.data['results'][0]['id'] == profile['id']
 
-    # Remove the user
+    # logged as user created in previous steps
+    client = auth_utils.client_with_user_credentials(user_data['email'], user_data['password'])
+    # Remove the user (it is forbidden to remove the user that is logged in)
     user_del_resp = client.delete(
         '/api/v2/institution/{}/user/{}/'.format(inst_id, user_create_resp.data['id'])
     )
+    assert user_del_resp.status_code == 403
+
+    # create other user to delete
+    # Create a new user
+    user_name2 = get_random_string(10)
+    password2 = get_random_string(10)
+    email2 = '{}@inst.tesla-ce.eu'.format(user_name2)
+    user_data2 = {
+        'username': user_name2,
+        'uid': user_name2,
+        'email': email2,
+        'first_name': user_name2[:5],
+        'last_name': user_name2[5:],
+        'login_allowed': True,
+        'is_active': True,
+        'is_staff': False,
+        'password': password2,
+        'password2': password2
+    }
+    user_create_resp2 = client.post('/api/v2/institution/{}/user/'.format(inst_id), data=user_data2, format='json')
+    assert user_create_resp2.status_code == 201
+
+    # Try to remove global administration privileges
+    user_mod_resp3 = client.patch(
+        '/api/v2/institution/{}/user/{}/'.format(inst_id, user_create_resp.data['id']),
+        data={'is_staff': False},
+        format='json'
+    )
+    assert user_mod_resp3.status_code == 200
+
+    # Remove the user
+    user_del_resp = client.delete(
+        '/api/v2/institution/{}/user/{}/'.format(inst_id, user_create_resp2.data['id'])
+    )
     assert user_del_resp.status_code == 204
 
     # Ensure that this user does not exist
-    find2_user_resp = client.get('/api/v2/institution/{}/user/?email={}'.format(inst_id, email))
+    find2_user_resp = client.get('/api/v2/institution/{}/user/?email={}'.format(inst_id, email2))
     assert find2_user_resp.status_code == 200
     assert find2_user_resp.data['count'] == 0
 
 
 @pytest.mark.django_db
 def test_api_institution_user_filters(rest_api_client, institution_course_test_case):
     """
```

### Comparing `tesla-ce-1.0.3/src/tests/api/institution/test_vle.py` & `tesla-ce-1.0.8/src/tests/api/institution/test_vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/provider/__init__.py` & `tesla-ce-1.0.8/src/tests/api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/provider/test_api_providers.py` & `tesla-ce-1.0.8/src/tests/api/provider/test_api_providers.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/test_api.py` & `tesla-ce-1.0.8/src/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/vle/__init__.py` & `tesla-ce-1.0.8/src/tests/api/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/api/vle/test_api_vle.py` & `tesla-ce-1.0.8/src/tests/api/vle/test_api_vle.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/auth_utils.py` & `tesla-ce-1.0.8/src/tests/auth_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/test_activity_case.py` & `tesla-ce-1.0.8/src/tests/cases/test_activity_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,16 +298,19 @@
     provider_verification_tasks = []
     tasks, activity_doc1 = utils.learner.lapi_learner_perform_activity(assessment_session1)
     provider_verification_tasks += tasks
     tasks, activity_doc2 = utils.learner.lapi_learner_perform_activity(assessment_session2)
     provider_verification_tasks += tasks
 
     # VLE send the activity
-    provider_verification_tasks += utils.vle.vle_send_activity(vle, assessment_session1, activity_doc1, True)
-    provider_verification_tasks += utils.vle.vle_send_activity(vle, assessment_session2, activity_doc2)
+    assessment_session3 = utils.vle.vle_create_assessment_session(vle, learners[0], activity, vle_options)
+    assessment_session4 = utils.vle.vle_create_assessment_session(vle, learners[1], activity)
+
+    provider_verification_tasks += utils.vle.vle_send_activity(vle, assessment_session3, activity_doc1, True)
+    provider_verification_tasks += utils.vle.vle_send_activity(vle, assessment_session4, activity_doc2)
 
     # The VLE creates a launcher for the learners to check the status of their requests
     launcher_stats1 = utils.vle.vle_create_launcher(vle, learners[0])
     launcher_stats2 = utils.vle.vle_create_launcher(vle, learners[1])
 
     # The learner check the status of sent requests
     utils.learner.lapi_check_requests_status(launcher_stats1, 'VALID')
```

### Comparing `tesla-ce-1.0.3/src/tests/cases/test_case_2.py` & `tesla-ce-1.0.8/src/tests/cases/test_case_2.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/global_admin/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/global_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/global_admin/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/global_admin/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/inst_admin/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/inst_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/inst_admin/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/inst_admin/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/instructor/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/instructor/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/instructor/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/learner/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/learner/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/learner/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/learner/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/provider/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/provider/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/provider/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/scenario.py` & `tesla-ce-1.0.8/src/tests/cases/utils/scenario.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/vle/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/vle/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/vle/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/worker/__init__.py` & `tesla-ce-1.0.8/src/tests/cases/utils/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/cases/utils/worker/methods.py` & `tesla-ce-1.0.8/src/tests/cases/utils/worker/methods.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/__init__.py` & `tesla-ce-1.0.8/src/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/test_generate_config.py` & `tesla-ce-1.0.8/src/tests/commands/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/test_reconfiguration.py` & `tesla-ce-1.0.8/src/tests/commands/test_reconfiguration.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/test_swarm_deployment.py` & `tesla-ce-1.0.8/src/tests/commands/test_swarm_deployment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/test_unseal.py` & `tesla-ce-1.0.8/src/tests/commands/test_unseal.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/commands/test_version.py` & `tesla-ce-1.0.8/src/tests/commands/test_version.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/config/__init__.py` & `tesla-ce-1.0.8/src/tests/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/config/test_django_config.py` & `tesla-ce-1.0.8/src/tests/config/test_django_config.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/config/test_vault_config.py` & `tesla-ce-1.0.8/src/tests/config/test_vault_config.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/conftest.py` & `tesla-ce-1.0.8/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/jwt/__init__.py` & `tesla-ce-1.0.8/src/tests/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/jwt/test_jwt.py` & `tesla-ce-1.0.8/src/tests/jwt/test_jwt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/test_client.py` & `tesla-ce-1.0.8/src/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-1.0.3/src/tests/utils.py` & `tesla-ce-1.0.8/src/tests/utils.py`

 * *Files identical despite different names*

