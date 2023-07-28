# Comparing `tmp/sfapi_client-0.0.6.tar.gz` & `tmp/sfapi_client-0.0.7.tar.gz`

## Comparing `sfapi_client-0.0.6.tar` & `sfapi_client-0.0.7.tar`

### file list

```diff
@@ -1,86 +1,85 @@
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/LEGAL
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/mkdocs.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/pytest.ini
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/requirements-dev.txt
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/.github/workflows/pytest.yml
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/examples/getting_bearer_token.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/javascript/apiselector.js
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/quickstart/index.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/scripts/run.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/paths.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/_models.py
--rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_api_async.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_client_async.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_compute.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_compute_async.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_groups.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_paths.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_paths_async.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_projects.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_projects_async.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_resources.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/tests/test_users_async.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/.gitignore
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/LICENSE
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/README.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 sfapi_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/LEGAL
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/mkdocs.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/pytest.ini
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/requirements-dev.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/.github/workflows/pytest.yml
+-rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/examples/getting_bearer_token.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/scripts/run.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    10795 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_api_async.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_client_async.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_compute.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_compute_async.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_groups.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4617 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6443 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_paths.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_paths_async.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_projects.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_resources.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/tests/test_users_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/.gitignore
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/README.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 sfapi_client-0.0.7/PKG-INFO
```

### Comparing `sfapi_client-0.0.6/LEGAL` & `sfapi_client-0.0.7/LEGAL`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/mkdocs.yml` & `sfapi_client-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.7/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/.github/workflows/pypi.yml` & `sfapi_client-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/.github/workflows/pytest.yml` & `sfapi_client-0.0.7/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/gen_examples.py` & `sfapi_client-0.0.7/docs/gen_examples.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-
 from pathlib import Path
 import os
 import json
 
-replace = Path('examples_dev') / "replacement.json"
+replace = Path("examples_dev") / "replacement.json"
 
 if replace.exists():
-    with replace.open('r'):
+    with replace.open("r"):
         replacements = json.loads(replace.read_text())
 else:
     replacements = {}
 
 # Replace personal details in notebook
-for notebook in Path('examples_dev').glob('*.ipynb'):
+for notebook in Path("examples_dev").glob("*.ipynb"):
     # Read in notebook
-    with notebook.open('r') as nb:
+    with notebook.open("r") as nb:
         full_nb = nb.read()
     # replace all key with value
     for k, v in replacements.items():
         full_nb = full_nb.replace(k, v)
 
     new_path = Path("examples") / notebook.name
     # Open to write back to notebook
-    with new_path.open('w') as nb:
+    with new_path.open("w") as nb:
         nb.write(full_nb)
 
 
 # Get our index page
-index_path = Path('docs/examples/index.md')
+index_path = Path("docs/examples/index.md")
 
 # Ensure the directory exists
 index_path.parent.mkdir(exist_ok=True)
 
 # Open it up and write heading
 with index_path.open("w") as index:
     index.write("# Examples \n\n")
 
-    for notebook in Path('examples').glob('*.ipynb'):
+    for notebook in Path("examples").glob("*.ipynb"):
         notebook_name = " ".join(notebook.stem.title().split("_"))
         index.write(f"* [{notebook_name}]({notebook.name})\n")
```

### Comparing `sfapi_client-0.0.6/docs/gen_sync.py` & `sfapi_client-0.0.7/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/index.md` & `sfapi_client-0.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.7/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/examples/getting_bearer_token.ipynb` & `sfapi_client-0.0.7/docs/examples/getting_bearer_token.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.7/docs/examples/run_job_and_check_status.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/javascript/apiselector.js` & `sfapi_client-0.0.7/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/quickstart/index.md` & `sfapi_client-0.0.7/docs/quickstart/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/SUMMARY.txt` & `sfapi_client-0.0.7/docs/reference/SUMMARY.txt`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/async/compute/index.md` & `sfapi_client-0.0.7/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/async/groups/index.md` & `sfapi_client-0.0.7/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.7/docs/reference/async/jobs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/async/paths/index.md` & `sfapi_client-0.0.7/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/docs/reference/async/projects/index.md` & `sfapi_client-0.0.7/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/scripts/run.py` & `sfapi_client-0.0.7/scripts/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -83,25 +83,56 @@
                     modified = True
 
                 if modified:
                     with path.open("w") as fp:
                         fp.write(code)
 
 
+# As the SF API doesn't list values for most of the enums, datamodel-code-generator
+# can't determine the type, so we have to patch things up, for now they are all
+# string based enums.
+def _to_str_enum(code: str) -> str:
+    pattern = re.compile(rf"(.*)\(Enum\)(.*)", re.DOTALL)
+
+    while pattern.match(code):
+        code = re.sub(pattern, rf"\1(str, Enum)\2", code)
+
+    return code
+
+
+#
+def _fix_date_import(code: str) -> str:
+    replacements = {
+        "import date": "import date as date_",
+        "date: Optional\[date\]": "date: Optional[date_]",
+    }
+
+    for target, replacement in replacements.items():
+        pattern = re.compile(rf"(.*){target}(.*)", re.DOTALL)
+        pattern.match(code)
+        code = re.sub(pattern, rf"\1{replacement}\2", code)
+
+    return code
+
+
 def _from_open_api() -> str:
     with TemporaryDirectory() as tempdir:
         output = Path(tempdir) / "model.py"
         generate(
             use_double_quotes=True,
             input_=urlparse("https://api.nersc.gov/api/v1.2/openapi.json"),
             input_file_type=InputFileType.OpenAPI,
             output=output,
+            use_subclass_enum=True,
         )
+        code = output.read_text()
+        code = _to_str_enum(code)
+        code = _fix_date_import(code)
 
-        return output.read_text()
+        return code
 
 
 def _from_json(json: Path, class_name: str) -> str:
     with TemporaryDirectory() as tempdir:
         output = Path(tempdir) / "model.py"
         generate(
             use_double_quotes=True,
@@ -109,14 +140,15 @@
             input_=json,
             input_file_type=InputFileType.Json,
             output=output,
             class_name=class_name,
             aliases={
                 "OutputItem": "JobStatus",
             },
+            use_subclass_enum=True,
         )
 
         return output.read_text()
 
 
 #
 # Generate models using datamodel-codegen using OpenAPI spec and a sample JSON job status output.
@@ -147,30 +179,30 @@
         / "sfapi_client"
         / "_models"
         / "resources.py",
         dir_okay=False,
         writable=True,
     ),
 ):
-
     import requests
     import datetime
+
     api_url = "https://api.nersc.gov/api/v1.2/status"
     response = requests.get(api_url)
     status = response.json()
     names = []
     for s in status:
-        name = s['name']
-        value = s['name']
-        name = name if name != "int" else f'_{name}'
-        name = name.replace('-', '_')
-        names.append(f"    {name} = \"{value}\"")
+        name = s["name"]
+        value = s["name"]
+        name = name if name != "int" else f"_{name}"
+        name = name.replace("-", "_")
+        names.append(f'    {name} = "{value}"')
         names.append(f"    \"\"\" {s['system_type']}: {s['full_name']}\"\"\"")
 
-    resources = '\n'.join(names)
+    resources = "\n".join(names)
     now = datetime.datetime.now()
     template = f"""# generated by resources_codegen:
 #   URL:  https://api.nersc.gov/api/v1.2/status
 #   timestamp: {now}
 
 from enum import Enum
 
@@ -200,36 +232,38 @@
             name_split = [name.capitalize() for name in name_split]
             job_model = _from_json(model, f"{''.join(name_split)}")
             fp.write(job_model)
 
 
 @cli.command(name="examples")
 def work_on_examples(
-    replace: Optional[Path] = typer.Option((Path('examples_dev') / "replacement.json"), dir_okay=False),
+    replace: Optional[Path] = typer.Option(
+        (Path("examples_dev") / "replacement.json"), dir_okay=False
+    ),
 ):
     dev_dir = Path(__file__).parent.parent / "examples_dev"
     dev_dir.mkdir(exist_ok=True)
     examples = (Path(__file__).parent.parent / "examples").glob("*.ipynb")
 
     if replace.exists():
-        with replace.open('r'):
+        with replace.open("r"):
             replacements = json.loads(replace.read_text())
     else:
         replacements = {}
 
     # Replace personal details in notebook
     for notebook in examples:
         # Read in notebook
-        with notebook.open('r') as nb:
+        with notebook.open("r") as nb:
             full_nb = nb.read()
         # replace all key with value
         for v, k in replacements.items():
             full_nb = full_nb.replace(k, v)
 
         new_path = dev_dir / notebook.name
         # Open to write back to notebook
-        with new_path.open('w') as nb:
+        with new_path.open("w") as nb:
             nb.write(full_nb)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.7/src/sfapi_client/_jobs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
 TERMINAL_STATES = [
     JobState.CANCELLED,
     JobState.COMPLETED,
     JobState.PREEMPTED,
     JobState.OUT_OF_MEMORY,
     JobState.FAILED,
     JobState.TIMEOUT,
-]
+]
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.7/src/sfapi_client/_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,17 @@
             index_of_next_type = (index_of_next_type + 1) % len(possible_job_types)
 
         self._last_job_type_fetched = job_type
 
         return job_type
 
     async def fetch_jobs(
-        self, job_type: Union[AsyncJobSacct, AsyncJobSqueue], jobids: List[Union[int, str]]
+        self,
+        job_type: Union[AsyncJobSacct, AsyncJobSqueue],
+        jobids: List[Union[int, str]],
     ) -> List[Union[AsyncJobSacct, AsyncJobSqueue]]:
         jobids = list(map(str, jobids))
         jobids_for_type = self._jobids.setdefault(job_type, set())
         jobids_for_type.update(jobids)
 
         if self._monitor_task is None:
             await self._create_task()
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,104 @@
 from __future__ import annotations
 from typing import Dict, Any, Optional, cast, List, Union
 from pathlib import Path
 import json
 
-from authlib.integrations.httpx_client.oauth2_client import AsyncOAuth2Client
+from authlib.integrations.httpx_client.oauth2_client import OAuth2Client
 from authlib.oauth2.rfc7523 import PrivateKeyJWT
 import httpx
 import tenacity
 from authlib.jose import JsonWebKey
 
-from .compute import Machine, AsyncCompute
+from .compute import Machine, Compute
 from ..exceptions import SfApiError
 from .._models import (
     JobOutput as JobStatusResponse,
     AppRoutersComputeModelsStatus as JobStatus,
     Changelog as ChangelogItem,
     Config as ConfItem,
     Outage,
     Note,
     AppRoutersStatusModelsStatus as Status,
 )
 from .._models.resources import Resource
-from .groups import AsyncGroup
-from .users import AsyncUser
+from .groups import Group, GroupMember
+from .users import User
+from .projects import Project, Role
+from .paths import RemotePath
 
 SFAPI_TOKEN_URL = "https://oidc.nersc.gov/c2id/token"
 SFAPI_BASE_URL = "https://api.nersc.gov/api/v1.2"
 MAX_RETRY = 10
 
 
-# Retry on httpx.HTTPStatusError if status code is not 401 or 403
+# Retry on httpx.HTTPStatusError recoverable status codes
 class retry_if_http_status_error(tenacity.retry_if_exception):
     def __init__(self):
         super().__init__(self._retry)
 
     def _retry(self, e: Exception):
-        dont_retry_codes = [httpx.codes.FORBIDDEN, httpx.codes.UNAUTHORIZED]
+        retry_codes = [
+            httpx.codes.TOO_MANY_REQUESTS,
+            httpx.codes.BAD_GATEWAY,
+            httpx.codes.SERVICE_UNAVAILABLE,
+            httpx.codes.GATEWAY_TIMEOUT,
+        ]
         return (
             isinstance(e, httpx.HTTPStatusError)
-            and cast(httpx.HTTPStatusError, e).response.status_code
-            not in dont_retry_codes
+            and cast(httpx.HTTPStatusError, e).response.status_code in retry_codes
         )
 
 
-class AsyncApi:
+class Api:
     """
     API information.
     """
 
-    def __init__(self, client: "AsyncClient"):
+    def __init__(self, client: "Client"):
         self._client = client
 
-    async def changelog(self) -> List[ChangelogItem]:
+    def changelog(self) -> List[ChangelogItem]:
         """
         Get the API changelog.
 
         :return: The API changelog
         :rtype: List[ChangelogItem]
         """
-        r = await self._client.get("meta/changelog")
+        r = self._client.get("meta/changelog")
 
         json_response = r.json()
 
-        return [ChangelogItem.parse_obj(i) for i in json_response]
+        return [ChangelogItem.model_validate(i) for i in json_response]
 
-    async def config(self) -> Dict[str, str]:
+    def config(self) -> Dict[str, str]:
         """
         Get the configuration information for the API.
 
         :return: The API configuration
         :rtype: Dict[str, str]
         """
-        r = await self._client.get("meta/config")
+        r = self._client.get("meta/config")
 
         json_response = r.json()
 
-        config_items = [ConfItem.parse_obj(i) for i in json_response]
+        config_items = [ConfItem.model_validate(i) for i in json_response]
 
         config = {}
         for i in config_items:
             config[i.key] = i.value
 
         return config
 
 
 StatusInfo = Union[Outage, Note, Status]
 
 
-class AsyncResources:
-    def __init__(self, client: "AsyncClient"):
+class Resources:
+    def __init__(self, client: "Client"):
         self._client = client
 
     @staticmethod
     def _resource_name(resource_name: Optional[Union[str, Machine]]):
         if resource_name is None:
             resource_name = ""
         else:
@@ -109,189 +115,191 @@
         for resource_info_list in info_list:
             for info in resource_info_list:
                 resource_info = resource_map.setdefault(info.name, [])
                 resource_info.append(info)
 
         return resource_map
 
-    async def outages(
+    def outages(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Outage]], List[Outage]]:
         """
         Get outage information for a resource.
 
         :param resource_name: The resource name
         :return: The outages
         :rtype: Union[Dict[str, List[Outage]], List[Outage]]
         """
         resource_path = self._resource_name(resource_name)
-        response = await self._client.get(f"status/outages{resource_path}")
+        response = self._client.get(f"status/outages{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            outages = [Outage.parse_obj(o) for o in json_response]
+            outages = [Outage.model_validate(o) for o in json_response]
         else:
-            outages = [[Outage.parse_obj(o) for o in r] for r in json_response]
+            outages = [[Outage.model_validate(o) for o in r] for r in json_response]
             outages = self._list_to_resource_map(outages)
 
         return outages
 
-    async def planned_outages(
+    def planned_outages(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Outage]], List[Outage]]:
         """
         Get planned outage information for a resource.
 
         :param resource_name: The resource name
         :return: The planned outages
         :rtype: Union[Dict[str, List[Outage]], List[Outage]]
         """
         resource_path = self._resource_name(resource_name)
-        response = await self._client.get(f"status/outages/planned{resource_path}")
+        response = self._client.get(f"status/outages/planned{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            outages = [Outage.parse_obj(o) for o in json_response]
+            outages = [Outage.model_validate(o) for o in json_response]
         else:
-            outages = [[Outage.parse_obj(o) for o in r] for r in json_response]
+            outages = [[Outage.model_validate(o) for o in r] for r in json_response]
             outages = self._list_to_resource_map(outages)
 
         return outages
 
-    async def notes(
+    def notes(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Note]], List[Note]]:
         """
         Get notes associated with a resource.
 
         :param resource_name: The resource name
         :return: The resource notes
         :rtype: Union[Dict[str, List[Note]], List[Note]]
         """
         resource_path = self._resource_name(resource_name)
-        response = await self._client.get(f"status/notes{resource_path}")
+        response = self._client.get(f"status/notes{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            notes = [Note.parse_obj(n) for n in json_response]
+            notes = [Note.model_validate(n) for n in json_response]
         else:
-            notes = [[Note.parse_obj(n) for n in r] for r in json_response]
+            notes = [[Note.model_validate(n) for n in r] for r in json_response]
             notes = self._list_to_resource_map(notes)
 
         return notes
 
-    async def status(
+    def status(
         self, resource_name: Optional[Union[str, Machine, Resource]] = None
     ) -> Union[Dict[str, Status], Status]:
         """
         Get the status of a resource.
 
         :param resource_name: The resource name
         :return: The resource status
         :rtype: Union[Dict[str, Status], Status]
         """
         resource_path = self._resource_name(resource_name)
 
-        response = await self._client.get(f"status{resource_path}")
+        response = self._client.get(f"status{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            status = Status.parse_obj(json_response)
+            status = Status.model_validate(json_response)
         else:
-            status = [Status.parse_obj(s) for s in json_response]
+            status = [Status.model_validate(s) for s in json_response]
             status = {s.name: s for s in status}
 
         return status
 
 
-class AsyncClient:
+class Client:
     def __init__(
         self,
         client_id: Optional[str] = None,
         secret: Optional[str] = None,
         key: Optional[Union[str, Path]] = None,
         api_base_url: Optional[str] = SFAPI_BASE_URL,
+        token_url: Optional[str] = SFAPI_TOKEN_URL,
         wait_interval: int = 10,
     ):
         """
         Create a client instance.
 
         Usage:
 
         ```python
-        >>> from sfapi_client import AsyncClient
-        >>> async with AsyncClient(client_id, client_secret) as client:
+        >>> from sfapi_client import Client
+        >>> with Client(client_id, client_secret) as client:
         >>>    # Use client
         ```
 
         :param client_id: The client ID
         :param secret: The client secret
 
         :return: The client instance
-        :rtype: AsyncClient
+        :rtype: Client
         """
         self._client_id = None
         self._secret = None
         if any(arg is None for arg in [client_id, secret]):
             self._read_client_secret_from_file(key)
         else:
             self._client_id = client_id
             self._secret = secret
         self._api_base_url = api_base_url
+        self._token_url = token_url
         self._client_user = None
         self.__oauth2_session = None
         self._api = None
         self._resources = None
         self._wait_interval = wait_interval
 
-    async def __aenter__(self):
+    def __enter__(self):
         return self
 
-    async def _oauth2_session(self):
+    def _oauth2_session(self):
         if self._client_id is None:
             raise SfApiError(f"No credentials have been provides")
 
         if self.__oauth2_session is None:
             # Create a new session if we haven't already
-            self.__oauth2_session = AsyncOAuth2Client(
+            self.__oauth2_session = OAuth2Client(
                 client_id=self._client_id,
                 client_secret=self._secret,
-                token_endpoint_auth_method=PrivateKeyJWT(SFAPI_TOKEN_URL),
+                token_endpoint_auth_method=PrivateKeyJWT(self._token_url),
                 grant_type="client_credentials",
-                token_endpoint=SFAPI_TOKEN_URL,
+                token_endpoint=self._token_url,
                 timeout=10.0,
             )
 
-            await self.__oauth2_session.fetch_token()
+            self.__oauth2_session.fetch_token()
         else:
             # We have a session
             # Make sure it's still active
-            await self.__oauth2_session.ensure_active_token(self.__oauth2_session.token)
+            self.__oauth2_session.ensure_active_token(self.__oauth2_session.token)
 
         return self.__oauth2_session
 
     @property
-    async def token(self) -> str:
+    def token(self) -> str:
         """
         Bearer token string which can be helpful for debugging through swagger UI.
         """
 
         if self._client_id is not None:
-            oauth_session = await self._oauth2_session()
+            oauth_session = self._oauth2_session()
             return oauth_session.token["access_token"]
 
-    async def close(self):
+    def close(self):
         """
         Release resources associated with the client instance.
         """
         if self.__oauth2_session is not None:
-            await self.__oauth2_session.aclose()
+            self.__oauth2_session.close()
 
-    async def __aexit__(self, type, value, traceback):
-        await self.close()
+    def __exit__(self, type, value, traceback):
+        self.close()
 
     def _read_client_secret_from_file(self, name):
         if name is not None and Path(name).exists():
             # If the user gives a full path, then use it
             key_path = Path(name)
         else:
             # If not let's search in ~/.superfacility for the name or any key
@@ -334,31 +342,31 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    async def get(self, url: str, params: Dict[str, Any] = {}) -> httpx.Response:
+    def get(self, url: str, params: Dict[str, Any] = {}) -> httpx.Response:
         if self._client_id is not None:
-            oauth_session = await self._oauth2_session()
+            oauth_session = self._oauth2_session()
 
-            r = await oauth_session.get(
+            r = oauth_session.get(
                 f"{self._api_base_url}/{url}",
                 headers={
                     "Authorization": oauth_session.token["access_token"],
                     "accept": "application/json",
                 },
                 params=params,
             )
         # Use regular client if we are hitting an endpoint that don't need
         # auth.
         else:
-            async with httpx.AsyncClient() as client:
-                r = await client.get(
+            with httpx.Client() as client:
+                r = client.get(
                     f"{self._api_base_url}/{url}",
                     headers={
                         "accept": "application/json",
                     },
                     params=params,
                 )
 
@@ -369,18 +377,18 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    async def post(self, url: str, data: Dict[str, Any]) -> httpx.Response:
-        oauth_session = await self._oauth2_session()
+    def post(self, url: str, data: Dict[str, Any]) -> httpx.Response:
+        oauth_session = self._oauth2_session()
 
-        r = await oauth_session.post(
+        r = oauth_session.post(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
             data=data,
         )
@@ -391,20 +399,20 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    async def put(
+    def put(
         self, url: str, data: Dict[str, Any] = None, files: Dict[str, Any] = None
     ) -> httpx.Response:
-        oauth_session = await self._oauth2_session()
+        oauth_session = self._oauth2_session()
 
-        r = await oauth_session.put(
+        r = oauth_session.put(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
             data=data,
             files=files,
@@ -416,83 +424,93 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    async def delete(self, url: str) -> httpx.Response:
-        oauth_session = await self._oauth2_session()
+    def delete(self, url: str) -> httpx.Response:
+        oauth_session = self._oauth2_session()
 
-        r = await oauth_session.delete(
+        r = oauth_session.delete(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
         )
         r.raise_for_status()
 
         return r
 
-    async def compute(self, machine: Union[Machine, str]) -> AsyncCompute:
+    def compute(self, machine: Union[Machine, str]) -> Compute:
         """Create a compute site to submit jobs or view jobs in the queue
 
         :param machine: Name of the compute machine to use
         :return: Compute object that can be used to start jobs,
         view the queue on the system, or list files and directories.
         """
         # Allows for creating a compute from a name string
         machine = Machine(machine)
-        response = await self.get(f"status/{machine.value}")
+        response = self.get(f"status/{machine.value}")
 
-        compute = AsyncCompute.parse_obj(response.json())
-        compute.client = self
+        values = response.json()
+        values["client"] = self
+        compute = Compute.model_validate(values)
 
         return compute
 
     # Get the user associated with the credentials
-    async def _user(self):
+    def _user(self):
         if self._client_user is None:
-            self._client_user = await self.user()
+            self._client_user = self.user()
 
         return self._client_user
 
-    async def user(self, username: Optional[str] = None) -> AsyncUser:
+    def user(self, username: Optional[str] = None) -> User:
         """
         Get a user.
 
         :param username: The username
         :return: The user
         :rtype: UserGroup
         """
-        return await AsyncUser._fetch_user(self, username)
+        return User._fetch_user(self, username)
 
-    async def group(self, name: str) -> AsyncGroup:
+    def group(self, name: str) -> Group:
         """
         Get a group.
 
         :param name: The group name
         :return: The group
-        :rtype: AsyncGroup
+        :rtype: Group
         """
-        return await AsyncGroup._fetch_group(self, name)
+        return Group._fetch_group(self, name)
 
     @property
-    def api(self) -> AsyncApi:
+    def api(self) -> Api:
         """
         API related information.
         """
         if self._api is None:
-            self._api = AsyncApi(self)
+            self._api = Api(self)
 
         return self._api
 
     @property
-    def resources(self) -> AsyncResources:
+    def resources(self) -> Resources:
         """
         Resource related information.
         """
         if self._resources is None:
-            self._resources = AsyncResources(self)
+            self._resources = Resources(self)
 
         return self._resources
+
+
+Compute.model_rebuild()
+Group.model_rebuild()
+User.model_rebuild()
+Project.model_rebuild()
+RemotePath.model_rebuild()
+Role.model_rebuild()
+GroupMember.model_rebuild()
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from typing import Dict, List, Optional, Union, Callable
 import json
 from enum import Enum
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel, PrivateAttr, ConfigDict
 from functools import wraps
 
 from ..exceptions import SfApiError
 from .._utils import _ASYNC_SLEEP
 from .jobs import AsyncJobSacct, AsyncJobSqueue, AsyncJobSqueue, JobCommand
 from .._models import (
     AppRoutersStatusModelsStatus as ComputeBase,
@@ -26,41 +26,46 @@
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self.client._client_id is None:
             raise SfApiError(
-                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client."
+            )
         elif self.status in [StatusValue.unavailable]:
             raise SfApiError(
-                f"Compute resource {self.name} is {self.status.name}, {self.notes}")
+                f"Compute resource {self.name} is {self.status.name}, {self.notes}"
+            )
         return method(self, *args, **kwargs)
+
     return wrapper
 
 
 class AsyncCompute(ComputeBase):
     client: Optional["AsyncClient"]
     _monitor: AsyncJobMonitor = PrivateAttr()
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._monitor = AsyncJobMonitor(self)
 
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"client"}
         return super().dict(*args, **kwargs)
 
     async def _wait_for_task(self, task_id) -> str:
         while True:
             r = await self.client.get(f"tasks/{task_id}")
 
             json_response = r.json()
-            task = Task.parse_obj(json_response)
+            task = Task.model_validate(json_response)
 
             if task.status.lower() in ["error", "failed"]:
                 raise SfApiError(task.result)
 
             if task.result is None:
                 await _ASYNC_SLEEP(1)
                 continue
@@ -83,25 +88,25 @@
         # If the string input looks like a script we'll set is_path to false
         elif script.startswith("#!") and "\n" in script:
             # If it starts with shebang and has multiple lines
             is_path = False
         else:
             # If we're given a path make sure it exists
             script_path = await self.ls(script)
-            if len(script_path) != 1 or not script_path[0].is_file():
-                raise SfApiError(
-                    f"Script path not present or is not a file, {script}")
+            is_file = await script_path[0].is_file()
+            if len(script_path) != 1 or not is_file:
+                raise SfApiError(f"Script path not present or is not a file, {script}")
 
         data = {"job": script, "isPath": is_path}
 
         r = await self.client.post(f"compute/jobs/{self.name}", data)
         r.raise_for_status()
 
         json_response = r.json()
-        job_response = SubmitJobResponse.parse_obj(json_response)
+        job_response = SubmitJobResponse.model_validate(json_response)
 
         if job_response.status == SubmitJobResponseStatus.ERROR:
             raise SfApiError(job_response.error)
 
         task_id = job_response.task_id
 
         # We now need waiting for the task to complete!
@@ -110,16 +115,15 @@
         if result.get("status") == "error":
             raise SfApiError(result["error"])
 
         jobid = result.get("jobid")
         if jobid is None:
             raise SfApiError(f"Unable to extract jobid if for task: {task_id}")
 
-        job = AsyncJobSqueue(jobid=jobid)
-        job.compute = self
+        job = AsyncJobSqueue(jobid=jobid, compute=self)
 
         return job
 
     @check_auth
     async def job(
         self, jobid: Union[int, str], command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["AsyncJobSacct", "AsyncJobSqueue"]:
@@ -157,21 +161,21 @@
     async def run(self, args: Union[str, AsyncRemotePath, List[str]]):
         body: RunCommandBody = {
             "executable": args if not isinstance(args, list) else " ".join(args)
         }
 
         r = await self.client.post(f"utilities/command/{self.name}", data=body)
         json_response = r.json()
-        run_response = RunCommandResponse.parse_obj(json_response)
+        run_response = RunCommandResponse.model_validate(json_response)
         if run_response.status == RunCommandResponseStatus.ERROR:
             raise SfApiError(run_response.error)
 
         task_id = run_response.task_id
         task_result = await self._wait_for_task(task_id)
-        command_result = CommandResult.parse_raw(task_result)
+        command_result = CommandResult.model_validate_json(task_result)
         if command_result.status == "error":
             raise SfApiError(command_result.error)
 
         return command_result.output
 
     async def outages(self):
         return await self.client.resources.outages(self.name)
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from typing import Optional, Union, List, Any, Callable
 from functools import wraps
-from pydantic import ValidationError, Field, BaseModel, validator
+from pydantic import ValidationError, Field, BaseModel, ConfigDict
 from .._models import BatchGroupAction as GroupAction, UserStats as GroupMemberBase
 from ..exceptions import SfApiError
 from .users import AsyncUser
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self._client_id is None:
             raise SfApiError(
-                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client."
+            )
         return method(self, *args, **kwargs)
+
     return wrapper
 
 
 class AsyncGroupMember(GroupMemberBase):
     client: Optional["AsyncClient"]
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     async def user(self) -> "AsyncUser":
         """
         Get the user associated with the membership.
         """
         return await AsyncUser._fetch_user(self.client, self.name)
 
 
 # Note: We can't use our generated model as we want user => members ( to avoid confusion with User model )
 class AsyncGroup(BaseModel):
     """
     A user group.
     """
+
     client: Optional["AsyncClient"]
     gid: Optional[int]
     name: Optional[str]
     users_: Optional[List[GroupMemberBase]] = Field(..., alias="users")
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     async def _group_action(
         self,
         users: Union[str, "AsyncUser", List[str], List["AsyncUser"]],
         action: GroupAction,
     ):
         # coerse to list
         if not isinstance(users, list):
@@ -53,15 +60,17 @@
         }
 
         r = await self.client.put(f"account/groups/{self.name}", data=params)
         json_response = r.json()
 
         # if successful will return group object
         try:
-            new_group = AsyncGroup.parse_obj(json_response)
+            new_group = AsyncGroup.model_validate(
+                dict(json_response, client=self.client)
+            )
             self._update(new_group)
         except ValidationError:
             # See if we have validation error raise it
             if "details" in json_response:
                 raise SfApiError(r.text)
             else:
                 raise RuntimeError(r.text)
@@ -83,42 +92,46 @@
         await self._group_action(users, GroupAction.batch_remove)
 
     @property
     def members(self):
         """
         The users in this group.
         """
-        members = [AsyncGroupMember.parse_obj(user_info) for user_info in self.users_]
+        members = [
+            AsyncGroupMember.model_validate(
+                dict(user_info.model_dump(), client=self.client)
+            )
+            for user_info in self.users_
+        ]
 
         def _set_client(m):
             m.client = self.client
 
             return m
 
         members = map(_set_client, members)
 
         return list(members)
 
     @staticmethod
     @check_auth
     async def _fetch_group(client: "AsyncClient", name):
         response = await client.get(f"account/groups/{name}")
-        json_response = response.json()
 
-        group = AsyncGroup.parse_obj(json_response)
-        group.client = client
+        json_response = response.json()
+        group = AsyncGroup.model_validate(dict(json_response, client=client))
 
         return group
 
     async def update(self):
         """
         Update the state of the group by fetching the state from the server.
         """
         group_state = await self._fetch_group(self.client, self.name)
         self._update(group_state)
 
     def _update(self, new_group_state: Any) -> "AsyncGroup":
-        for k in new_group_state.__fields_set__:
+        for k in new_group_state.model_fields_set:
             v = getattr(new_group_state, k)
             setattr(self, k, v)
 
         return self
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Optional, Dict, List, ClassVar
 from .._utils import _ASYNC_SLEEP
 from ..exceptions import SfApiError
 from .._models.job_status_response_sacct import OutputItem as JobSacctBase
 from .._models.job_status_response_squeue import OutputItem as JobSqueueBase
 from .._models import AppRoutersComputeModelsStatus as JobResponseStatus
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, field_validator
 
 from .._jobs import JobCommand
 from .._jobs import JobStateResponse
 from .._jobs import JobState
 from .._jobs import TERMINAL_STATES
 
 
@@ -40,15 +40,15 @@
     if partition is not None:
         kwargs = params.setdefault("kwargs", [])
         kwargs.append(f"partition={partition}")
 
     r = await compute.client.get(job_url, params)
 
     json_response = r.json()
-    job_state_response = JobStateResponse.parse_obj(json_response)
+    job_state_response = JobStateResponse.model_validate(json_response)
 
     if job_state_response == JobResponseStatus.ERROR:
         error = json_response.error
         raise SfApiError(error)
 
     return job_state_response.output
 
@@ -60,32 +60,31 @@
     user: Optional[str] = None,
     partition: Optional[str] = None,
 ):
     job_states = await _fetch_raw_state(
         compute, jobids, user, partition, job_type._command == JobCommand.sacct
     )
 
-    jobs = [job_type.parse_obj(state) for state in job_states]
-
-    for job in jobs:
-        job.compute = compute
+    jobs = [
+        job_type.model_validate(dict(state, compute=compute)) for state in job_states
+    ]
 
     return jobs
 
 
 class AsyncJob(BaseModel, ABC):
     """
     Models a job submitted to run on a compute resource.
     """
 
     compute: Optional["AsyncCompute"] = None
-    state: Optional[JobState]
-    jobid: Optional[str]
+    state: Optional[JobState] = None
+    jobid: Optional[str] = None
 
-    @validator("state", pre=True, check_fields=False)
+    @field_validator("state", mode="before", check_fields=False)
     def state_validate(cls, v):
         # sacct return a state of the form "CANCELLED by XXXX" for the
         # cancelled state, coerce into value that will match a state
         # modeled by the enum
         if v.startswith("CANCELLED by"):
             return "CANCELLED"
 
@@ -95,15 +94,15 @@
         """
         Update the state of the job by fetching the state from the compute resource.
         """
         job_state = await self._fetch_state()
         self._update(job_state)
 
     def _update(self, new_job_state: Any) -> Job:
-        for k in new_job_state.__fields_set__:
+        for k in new_job_state.model_fields_set:
             v = getattr(new_job_state, k)
             setattr(self, k, v)
 
         return self
 
     async def _wait_until(self, states: List[JobState], timeout: int = sys.maxsize):
         max_iteration = math.ceil(timeout / self.compute.client._wait_interval)
@@ -209,14 +208,15 @@
 
 
 class AsyncJobSqueue(AsyncJob, JobSqueueBase):
     """
     Models a job running on a compute resource, the information is
     fetched using `squeue`.
     """
+
     _command: ClassVar[JobCommand] = JobCommand.squeue
 
     async def _fetch_state(self):
         jobs = await self.compute._monitor.fetch_jobs(
             job_type=self.__class__, jobids=[self.jobid]
         )
         # If the job state comes back empty the job is probably no longer in
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, IO, AnyStr, Dict
+from typing import Optional, List, IO, AnyStr, Dict, Tuple
 from pathlib import PurePosixPath, Path
 from pydantic import PrivateAttr
 from io import StringIO, BytesIO
 from base64 import b64decode
 from contextlib import asynccontextmanager
 import tempfile
 
@@ -19,118 +19,121 @@
 
 
 def _is_no_such(error: SfApiError):
     return "No such file or directory" in error.message
 
 
 class AsyncRemotePath(PathBase):
+    """
+    RemotePath is used to model a remote path, it takes inspiration from
+    pathlib and shares some of its interface.
+    """
+
     compute: Optional["AsyncCompute"]
     # It would be nice to be able subclass PurePosixPath, however, this
     # require using private interfaces. So we derive by composition.
     _path: PurePosixPath = PrivateAttr()
 
     def __init__(self, path=None, **kwargs):
         super().__init__(**kwargs)
         self._path = PurePosixPath(path)
 
         if self.name is None:
             self.name = self._path.name
 
     def __truediv__(self, key):
-        remote_path = AsyncRemotePath(str(self._path / key))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        remote_path.compute = self.compute
+        remote_path = AsyncRemotePath(path=str(self._path / key), compute=self.compute)
 
         return remote_path
 
     def __rtruediv__(self, key):
-        remote_path = AsyncRemotePath(str(key / self._path))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        remote_path.compute = self.compute
+        remote_path = AsyncRemotePath(path=str(key / self._path), compute=self.compute)
 
         return remote_path
 
     def __str__(self):
         return str(self._path)
 
     @property
-    def parent(self):
+    def parent(self) -> "RemotePath":
         """
         The parent of the path.
+
+        :return: the parent
+
         """
-        parent_path = AsyncRemotePath(str(self._path.parent))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        parent_path.compute = self.compute
+        parent_path = AsyncRemotePath(path=str(self._path.parent), compute=self.compute)
 
         return parent_path
 
     @property
-    def parents(self):
+    def parents(self) -> List["RemotePath"]:
         """
         The parents of the path.
-        """
-        parents = [AsyncRemotePath(str(p)) for p in self._path.parents]
 
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        def _set_compute(p):
-            p.compute = self.compute
-            return p
-
-        parents = map(_set_compute, parents)
+        :return: the parents
+        """
+        parents = [
+            AsyncRemotePath(path=str(p), compute=self.compute)
+            for p in self._path.parents
+        ]
 
         return parents
 
     @property
-    def stem(self):
+    def stem(self) -> str:
         """
         The final path component, without its suffix.
+
+        :return: the path stem
         """
         return self._path.stem
 
     @property
-    def suffix(self):
+    def suffix(self) -> str:
         """
         The path extension.
-        """
 
+        :return: the path extension
+        """
         return self._path.suffix
 
     @property
-    def suffixes(self):
+    def suffixes(self) -> List[str]:
         """
         A list of the path extensions.
+
+        :return: the path extensions
         """
         return self._path.suffixes
 
     @property
-    def parts(self):
+    def parts(self) -> Tuple[str]:
         """
         The paths components as a tuple.
+
+        :return: the path components
         """
         return self._path.parts
 
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"compute"}
         return super().dict(*args, **kwargs)
 
-    async def is_dir(self):
+    async def is_dir(self) -> bool:
         """
         :return: Returns True if path is a directory, False otherwise.
         """
         if self.perms is None:
             await self.update()
 
         return self.perms[0] == "d"
 
-    async def is_file(self):
+    async def is_file(self) -> bool:
         """
         :return: Returns True if path is a file, False otherwise.
         """
         return not await self.is_dir()
 
     async def download(self, binary=False) -> IO[AnyStr]:
         """
@@ -143,15 +146,15 @@
         if await self.is_dir():
             raise IsADirectoryError(self._path)
 
         r = await self.compute.client.get(
             f"utilities/download/{self.compute.name}/{self._path}?binary={binary}"
         )
         json_response = r.json()
-        download_response = FileDownloadResponse.parse_obj(json_response)
+        download_response = FileDownloadResponse.model_validate(json_response)
 
         if download_response.status == FileDownloadResponseStatus.ERROR:
             raise SfApiError(download_response.error)
 
         file_data = download_response.file
         if download_response.is_binary:
             binary_file_data = b64decode(file_data)
@@ -162,25 +165,26 @@
     @staticmethod
     async def _ls(
         compute: "Compute", path, directory=False, filter_dots=True
     ) -> List["RemotePath"]:
         r = await compute.client.get(f"utilities/ls/{compute.name}/{path}")
 
         json_response = r.json()
-        directory_listing_response = DirectoryListingResponse.parse_obj(json_response)
+        directory_listing_response = DirectoryListingResponse.model_validate(
+            json_response
+        )
         if directory_listing_response.status == DirectoryListingResponseStatus.ERROR:
             raise SfApiError(directory_listing_response.error)
 
         paths = []
 
         def _to_remote_path(path, entry):
-            kwargs = entry.dict()
-            kwargs.update(path=path)
+            kwargs = entry.model_dump()
+            kwargs.update(path=path, compute=compute)
             p = AsyncRemotePath(**kwargs)
-            p.compute = compute
 
             return p
 
         # Special case for listing file
         if len(directory_listing_response.entries) == 1:
             entry = directory_listing_response.entries[0]
             # The API can add an extra /
@@ -205,14 +209,16 @@
                 paths.append(_to_remote_path(f"{path}/{entry.name}", entry))
 
         return paths
 
     async def ls(self) -> List["AsyncRemotePath"]:
         """
         List the current path
+
+        :return: the list of child paths
         """
         return await self._ls(self.compute, str(self._path))
 
     async def update(self):
         """
         Update the path in the latest information from the resource.
         """
@@ -226,15 +232,15 @@
         # case we don't want to update the name
         new_state = file_state[0]
         new_state.name = self.name
 
         self._update(new_state)
 
     def _update(self, new_file_state: "AsyncRemotePath") -> "AsyncRemotePath":
-        for k in new_file_state.__fields_set__:
+        for k in new_file_state.model_fields_set:
             v = getattr(new_file_state, k)
             setattr(self, k, v)
 
         return self
 
     async def upload(self, file: BytesIO) -> "AsyncRemotePath":
         try:
@@ -259,33 +265,31 @@
 
         url = f"utilities/upload/{self.compute.name}/{upload_path}"
         files = {"file": file}
 
         r = await self.compute.client.put(url, files=files)
 
         json_response = r.json()
-        upload_response = UploadResponse.parse_obj(json_response)
+        upload_response = UploadResponse.model_validate(json_response)
         if upload_response.status == UploadResponseStatus.ERROR:
             raise SfApiError(upload_response.error)
 
-        remote_path = AsyncRemotePath(upload_path)
-        remote_path.compute = self.compute
+        remote_path = AsyncRemotePath(path=upload_path, compute=self.compute)
 
         return remote_path
 
     @asynccontextmanager
     async def open(self, mode: str) -> IO[AnyStr]:
         """
         Open the file at this path.
 
         :param mode: The mode to open the file. Valid options are 'rwb'.
 
         raises: IsDirectoryError: If the path is not a file.
         """
-
         try:
             if await self.is_dir():
                 raise IsADirectoryError()
         except SfApiError as ex:
             # Its a valid use case to add a open a new file to an exiting directory.
             # In this case the is_dir() will raise a SfApiError with "No such file or directory"
             # So we check for that and then see if the parent directory exists, if
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/projects.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from typing import Optional
-from pydantic import ValidationError, Field
+from pydantic import ValidationError, Field, ConfigDict
 
-from .._models import (
-    ProjectStats as ProjectBase,
-    RoleStats as RoleBase
-)
+from .._models import ProjectStats as ProjectBase, RoleStats as RoleBase
 from ..exceptions import SfApiError
 
 
 class AsyncRole(RoleBase):
     client: Optional["AsyncClient"]
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
 
 class AsyncProject(ProjectBase):
     client: Optional["AsyncClient"]
     name: str = Field(alias="repo_name")
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     async def create_group(self, name: str) -> "AsyncGroup":
         """
         Create a new project.
         :param name: The project name
         """
         from .groups import AsyncGroup
 
         params = {"name": name, "repo_name": self.repo_name}
 
         r = await self.client.post("account/groups", data=params)
         json_response = r.json()
         try:
-            group = AsyncGroup.parse_obj(json_response)
+            group = AsyncGroup.model_validate(dict(json_response, client=self.client))
         except ValidationError:
             # See if we have validation error raise it
             if "details" in json_response:
                 raise SfApiError(r.text())
             else:
                 raise RuntimeError(r.text())
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/users.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,106 @@
 from typing import List, Optional, Callable
 from functools import wraps
 
+from pydantic import ConfigDict
+
 from .._models import (
     UserInfo as UserBase,
     GroupList as GroupsResponse,
 )
-from .projects import AsyncProject, AsyncRole
+from .projects import Project, Role
 from ..exceptions import SfApiError
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self._client_id is None:
             raise SfApiError(
-                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client."
+            )
         return method(self, *args, **kwargs)
+
     return wrapper
 
 
-class AsyncUser(UserBase):
-    client: Optional["AsyncClient"]
+class User(UserBase):
+    client: Optional["Client"]
+
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @staticmethod
     @check_auth
-    async def _fetch_user(client: "AsyncClient", username: Optional[str] = None):
+    def _fetch_user(client: "Client", username: Optional[str] = None):
         url = "account/"
         if username is not None:
             url = f"{url}?username={username}"
 
-        response = await client.get(url)
+        response = client.get(url)
         json_response = response.json()
 
-        user = AsyncUser.parse_obj(json_response)
-        user.client = client
+        user = User.model_validate(dict(json_response, client=client))
 
         return user
 
-    async def groups(self) -> List["AsyncGroup"]:
+    def groups(self) -> List["Group"]:
         """
         The groups that the user is a member of.
 
         :return: the groups
         """
         # Avoid circular import
-        from .groups import AsyncGroup
+        from .groups import Group
 
-        if self.name != (await self.client._user()).name:
+        if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch groups for authenticated user.")
 
-        r = await self.client.get("account/groups")
+        r = self.client.get("account/groups")
 
         json_response = r.json()
-        groups_reponse = GroupsResponse.parse_obj(json_response)
-
-        groups = [AsyncGroup.parse_obj(g) for g in groups_reponse.groups]
-
-        def _set_client(g):
-            g.client = self.client
-            return g
+        groups_reponse = GroupsResponse.model_validate(json_response)
 
-        groups = map(_set_client, groups)
+        groups = [
+            Group.model_validate(dict(g, client=self.client))
+            for g in groups_reponse.groups
+        ]
 
-        return list(groups)
+        return groups
 
-    async def projects(self) -> List[AsyncProject]:
+    def projects(self) -> List[Project]:
         """
         The projects the user is associate with.
 
         :return: the projects
         """
-        if self.name != (await self.client._user()).name:
+        if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch projects for authenticated user.")
 
-        r = await self.client.get("account/projects")
+        r = self.client.get("account/projects")
 
-        json_response = r.json()
-
-        projects = [AsyncProject.parse_obj(p) for p in json_response]
-
-        def _set_client(p):
-            p.client = self.client
-            return p
+        project_values = r.json()
 
-        projects = map(_set_client, projects)
+        projects = [
+            Project.model_validate(dict(p, client=self.client))
+            for p in project_values
+        ]
 
-        return list(projects)
+        return projects
 
-    async def roles(self) -> List[AsyncRole]:
+    def roles(self) -> List[Role]:
         """
         The roles the user is associate with.
 
         :return: the roles
         """
-        if self.name != (await self.client._user()).name:
+        if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch roles for authenticated user.")
 
-        r = await self.client.get("account/roles")
+        r = self.client.get("account/roles")
 
         json_response = r.json()
 
-        roles = [AsyncRole.parse_obj(p) for p in json_response]
-
-        def _set_client(p):
-            p.client = self.client
-            return p
-
-        roles = map(_set_client, roles)
+        roles = [
+            Role.model_validate(dict(p, client=self.client)) for p in json_response
+        ]
 
-        return list(roles)
+        return roles
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.7/src/sfapi_client/_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # generated by datamodel-codegen:
 #   filename:  https://api.nersc.gov/api/v1.2/openapi.json
-#   timestamp: 2023-02-28T14:44:12+00:00
+#   timestamp: 2023-07-05T20:00:24+00:00
 
 from __future__ import annotations
 
-from datetime import date, datetime
+from datetime import date as date_, datetime
 from enum import Enum
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
 
-class BatchGroupAction(Enum):
+class BatchGroupAction(str, Enum):
     batch_add = "batch_add"
     batch_remove = "batch_remove"
 
 
 class BodyCreateGroupAccountGroupsPost(BaseModel):
     name: str = Field(..., title="Name")
     repo_name: str = Field(..., title="Repo Name")
@@ -32,27 +32,28 @@
     infiles: str = Field(..., title="Infiles")
     username: Optional[str] = Field(None, title="Username")
 
 
 class BodySubmitJobComputeJobsMachinePost(BaseModel):
     isPath: bool = Field(..., title="Ispath")
     job: str = Field(..., title="Job")
+    args: Optional[List[str]] = Field([], title="Args")
 
 
 class BodyUpdateGroupMembershipAccountGroupsGroupPut(BaseModel):
     usernames: str = Field(..., title="Usernames")
     action: BatchGroupAction
 
 
 class BodyUploadFileUtilitiesUploadMachinePathPut(BaseModel):
     file: bytes = Field(..., title="File")
 
 
 class Changelog(BaseModel):
-    date: Optional[date] = Field(None, title="Date")
+    date: Optional[date_] = Field(None, title="Date")
     change: Optional[str] = Field(None, title="Change")
 
 
 class Config(BaseModel):
     key: str = Field(..., title="Key")
     value: Optional[str] = Field(None, title="Value")
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.7/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.7/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.7/src/sfapi_client/_models/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # generated by resources_codegen:
 #   URL:  https://api.nersc.gov/api/v1.2/status
 #   timestamp: 2023-05-11 09:04:43.496473
 
 from enum import Enum
 
+
 class Resource(str, Enum):
     perlmutter = "perlmutter"
     """ compute: Perlmutter"""
     cori = "cori"
     """ compute: Cori"""
     dna = "dna"
     """ filesystem: DNA"""
@@ -68,8 +69,9 @@
     newt = "newt"
     """ service: NEWT"""
     regent = "regent"
     """ storage: HPSS Regent (Backup)"""
     archive = "archive"
     """ storage: HPSS Archive (User)"""
 
+
 Resource.__str__ = lambda self: self.value
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.7/src/sfapi_client/_async/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,104 @@
 from __future__ import annotations
 from typing import Dict, Any, Optional, cast, List, Union
 from pathlib import Path
 import json
 
-from authlib.integrations.httpx_client.oauth2_client import OAuth2Client
+from authlib.integrations.httpx_client.oauth2_client import AsyncOAuth2Client
 from authlib.oauth2.rfc7523 import PrivateKeyJWT
 import httpx
 import tenacity
 from authlib.jose import JsonWebKey
 
-from .compute import Machine, Compute
+from .compute import Machine, AsyncCompute
 from ..exceptions import SfApiError
 from .._models import (
     JobOutput as JobStatusResponse,
     AppRoutersComputeModelsStatus as JobStatus,
     Changelog as ChangelogItem,
     Config as ConfItem,
     Outage,
     Note,
     AppRoutersStatusModelsStatus as Status,
 )
 from .._models.resources import Resource
-from .groups import Group
-from .users import User
+from .groups import AsyncGroup, AsyncGroupMember
+from .users import AsyncUser
+from .projects import AsyncProject, AsyncRole
+from .paths import AsyncRemotePath
 
 SFAPI_TOKEN_URL = "https://oidc.nersc.gov/c2id/token"
 SFAPI_BASE_URL = "https://api.nersc.gov/api/v1.2"
 MAX_RETRY = 10
 
 
-# Retry on httpx.HTTPStatusError if status code is not 401 or 403
+# Retry on httpx.HTTPStatusError recoverable status codes
 class retry_if_http_status_error(tenacity.retry_if_exception):
     def __init__(self):
         super().__init__(self._retry)
 
     def _retry(self, e: Exception):
-        dont_retry_codes = [httpx.codes.FORBIDDEN, httpx.codes.UNAUTHORIZED]
+        retry_codes = [
+            httpx.codes.TOO_MANY_REQUESTS,
+            httpx.codes.BAD_GATEWAY,
+            httpx.codes.SERVICE_UNAVAILABLE,
+            httpx.codes.GATEWAY_TIMEOUT,
+        ]
         return (
             isinstance(e, httpx.HTTPStatusError)
-            and cast(httpx.HTTPStatusError, e).response.status_code
-            not in dont_retry_codes
+            and cast(httpx.HTTPStatusError, e).response.status_code in retry_codes
         )
 
 
-class Api:
+class AsyncApi:
     """
     API information.
     """
 
-    def __init__(self, client: "Client"):
+    def __init__(self, client: "AsyncClient"):
         self._client = client
 
-    def changelog(self) -> List[ChangelogItem]:
+    async def changelog(self) -> List[ChangelogItem]:
         """
         Get the API changelog.
 
         :return: The API changelog
         :rtype: List[ChangelogItem]
         """
-        r = self._client.get("meta/changelog")
+        r = await self._client.get("meta/changelog")
 
         json_response = r.json()
 
-        return [ChangelogItem.parse_obj(i) for i in json_response]
+        return [ChangelogItem.model_validate(i) for i in json_response]
 
-    def config(self) -> Dict[str, str]:
+    async def config(self) -> Dict[str, str]:
         """
         Get the configuration information for the API.
 
         :return: The API configuration
         :rtype: Dict[str, str]
         """
-        r = self._client.get("meta/config")
+        r = await self._client.get("meta/config")
 
         json_response = r.json()
 
-        config_items = [ConfItem.parse_obj(i) for i in json_response]
+        config_items = [ConfItem.model_validate(i) for i in json_response]
 
         config = {}
         for i in config_items:
             config[i.key] = i.value
 
         return config
 
 
 StatusInfo = Union[Outage, Note, Status]
 
 
-class Resources:
-    def __init__(self, client: "Client"):
+class AsyncResources:
+    def __init__(self, client: "AsyncClient"):
         self._client = client
 
     @staticmethod
     def _resource_name(resource_name: Optional[Union[str, Machine]]):
         if resource_name is None:
             resource_name = ""
         else:
@@ -109,189 +115,191 @@
         for resource_info_list in info_list:
             for info in resource_info_list:
                 resource_info = resource_map.setdefault(info.name, [])
                 resource_info.append(info)
 
         return resource_map
 
-    def outages(
+    async def outages(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Outage]], List[Outage]]:
         """
         Get outage information for a resource.
 
         :param resource_name: The resource name
         :return: The outages
         :rtype: Union[Dict[str, List[Outage]], List[Outage]]
         """
         resource_path = self._resource_name(resource_name)
-        response = self._client.get(f"status/outages{resource_path}")
+        response = await self._client.get(f"status/outages{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            outages = [Outage.parse_obj(o) for o in json_response]
+            outages = [Outage.model_validate(o) for o in json_response]
         else:
-            outages = [[Outage.parse_obj(o) for o in r] for r in json_response]
+            outages = [[Outage.model_validate(o) for o in r] for r in json_response]
             outages = self._list_to_resource_map(outages)
 
         return outages
 
-    def planned_outages(
+    async def planned_outages(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Outage]], List[Outage]]:
         """
         Get planned outage information for a resource.
 
         :param resource_name: The resource name
         :return: The planned outages
         :rtype: Union[Dict[str, List[Outage]], List[Outage]]
         """
         resource_path = self._resource_name(resource_name)
-        response = self._client.get(f"status/outages/planned{resource_path}")
+        response = await self._client.get(f"status/outages/planned{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            outages = [Outage.parse_obj(o) for o in json_response]
+            outages = [Outage.model_validate(o) for o in json_response]
         else:
-            outages = [[Outage.parse_obj(o) for o in r] for r in json_response]
+            outages = [[Outage.model_validate(o) for o in r] for r in json_response]
             outages = self._list_to_resource_map(outages)
 
         return outages
 
-    def notes(
+    async def notes(
         self, resource_name: Optional[Union[str, Machine]] = None
     ) -> Union[Dict[str, List[Note]], List[Note]]:
         """
         Get notes associated with a resource.
 
         :param resource_name: The resource name
         :return: The resource notes
         :rtype: Union[Dict[str, List[Note]], List[Note]]
         """
         resource_path = self._resource_name(resource_name)
-        response = self._client.get(f"status/notes{resource_path}")
+        response = await self._client.get(f"status/notes{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            notes = [Note.parse_obj(n) for n in json_response]
+            notes = [Note.model_validate(n) for n in json_response]
         else:
-            notes = [[Note.parse_obj(n) for n in r] for r in json_response]
+            notes = [[Note.model_validate(n) for n in r] for r in json_response]
             notes = self._list_to_resource_map(notes)
 
         return notes
 
-    def status(
+    async def status(
         self, resource_name: Optional[Union[str, Machine, Resource]] = None
     ) -> Union[Dict[str, Status], Status]:
         """
         Get the status of a resource.
 
         :param resource_name: The resource name
         :return: The resource status
         :rtype: Union[Dict[str, Status], Status]
         """
         resource_path = self._resource_name(resource_name)
 
-        response = self._client.get(f"status{resource_path}")
+        response = await self._client.get(f"status{resource_path}")
         json_response = response.json()
 
         if resource_name:
-            status = Status.parse_obj(json_response)
+            status = Status.model_validate(json_response)
         else:
-            status = [Status.parse_obj(s) for s in json_response]
+            status = [Status.model_validate(s) for s in json_response]
             status = {s.name: s for s in status}
 
         return status
 
 
-class Client:
+class AsyncClient:
     def __init__(
         self,
         client_id: Optional[str] = None,
         secret: Optional[str] = None,
         key: Optional[Union[str, Path]] = None,
         api_base_url: Optional[str] = SFAPI_BASE_URL,
+        token_url: Optional[str] = SFAPI_TOKEN_URL,
         wait_interval: int = 10,
     ):
         """
         Create a client instance.
 
         Usage:
 
         ```python
-        >>> from sfapi_client import Client
-        >>> with Client(client_id, client_secret) as client:
+        >>> from sfapi_client import AsyncClient
+        >>> async with AsyncClient(client_id, client_secret) as client:
         >>>    # Use client
         ```
 
         :param client_id: The client ID
         :param secret: The client secret
 
         :return: The client instance
-        :rtype: Client
+        :rtype: AsyncClient
         """
         self._client_id = None
         self._secret = None
         if any(arg is None for arg in [client_id, secret]):
             self._read_client_secret_from_file(key)
         else:
             self._client_id = client_id
             self._secret = secret
         self._api_base_url = api_base_url
+        self._token_url = token_url
         self._client_user = None
         self.__oauth2_session = None
         self._api = None
         self._resources = None
         self._wait_interval = wait_interval
 
-    def __enter__(self):
+    async def __aenter__(self):
         return self
 
-    def _oauth2_session(self):
+    async def _oauth2_session(self):
         if self._client_id is None:
             raise SfApiError(f"No credentials have been provides")
 
         if self.__oauth2_session is None:
             # Create a new session if we haven't already
-            self.__oauth2_session = OAuth2Client(
+            self.__oauth2_session = AsyncOAuth2Client(
                 client_id=self._client_id,
                 client_secret=self._secret,
-                token_endpoint_auth_method=PrivateKeyJWT(SFAPI_TOKEN_URL),
+                token_endpoint_auth_method=PrivateKeyJWT(self._token_url),
                 grant_type="client_credentials",
-                token_endpoint=SFAPI_TOKEN_URL,
+                token_endpoint=self._token_url,
                 timeout=10.0,
             )
 
-            self.__oauth2_session.fetch_token()
+            await self.__oauth2_session.fetch_token()
         else:
             # We have a session
             # Make sure it's still active
-            self.__oauth2_session.ensure_active_token(self.__oauth2_session.token)
+            await self.__oauth2_session.ensure_active_token(self.__oauth2_session.token)
 
         return self.__oauth2_session
 
     @property
-    def token(self) -> str:
+    async def token(self) -> str:
         """
         Bearer token string which can be helpful for debugging through swagger UI.
         """
 
         if self._client_id is not None:
-            oauth_session = self._oauth2_session()
+            oauth_session = await self._oauth2_session()
             return oauth_session.token["access_token"]
 
-    def close(self):
+    async def close(self):
         """
         Release resources associated with the client instance.
         """
         if self.__oauth2_session is not None:
-            self.__oauth2_session.close()
+            await self.__oauth2_session.aclose()
 
-    def __exit__(self, type, value, traceback):
-        self.close()
+    async def __aexit__(self, type, value, traceback):
+        await self.close()
 
     def _read_client_secret_from_file(self, name):
         if name is not None and Path(name).exists():
             # If the user gives a full path, then use it
             key_path = Path(name)
         else:
             # If not let's search in ~/.superfacility for the name or any key
@@ -334,31 +342,31 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    def get(self, url: str, params: Dict[str, Any] = {}) -> httpx.Response:
+    async def get(self, url: str, params: Dict[str, Any] = {}) -> httpx.Response:
         if self._client_id is not None:
-            oauth_session = self._oauth2_session()
+            oauth_session = await self._oauth2_session()
 
-            r = oauth_session.get(
+            r = await oauth_session.get(
                 f"{self._api_base_url}/{url}",
                 headers={
                     "Authorization": oauth_session.token["access_token"],
                     "accept": "application/json",
                 },
                 params=params,
             )
         # Use regular client if we are hitting an endpoint that don't need
         # auth.
         else:
-            with httpx.Client() as client:
-                r = client.get(
+            async with httpx.AsyncClient() as client:
+                r = await client.get(
                     f"{self._api_base_url}/{url}",
                     headers={
                         "accept": "application/json",
                     },
                     params=params,
                 )
 
@@ -369,18 +377,18 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    def post(self, url: str, data: Dict[str, Any]) -> httpx.Response:
-        oauth_session = self._oauth2_session()
+    async def post(self, url: str, data: Dict[str, Any]) -> httpx.Response:
+        oauth_session = await self._oauth2_session()
 
-        r = oauth_session.post(
+        r = await oauth_session.post(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
             data=data,
         )
@@ -391,20 +399,20 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    def put(
+    async def put(
         self, url: str, data: Dict[str, Any] = None, files: Dict[str, Any] = None
     ) -> httpx.Response:
-        oauth_session = self._oauth2_session()
+        oauth_session = await self._oauth2_session()
 
-        r = oauth_session.put(
+        r = await oauth_session.put(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
             data=data,
             files=files,
@@ -416,83 +424,93 @@
     @tenacity.retry(
         retry=tenacity.retry_if_exception_type(httpx.TimeoutException)
         | tenacity.retry_if_exception_type(httpx.ConnectError)
         | retry_if_http_status_error(),
         wait=tenacity.wait_exponential(max=MAX_RETRY),
         stop=tenacity.stop_after_attempt(MAX_RETRY),
     )
-    def delete(self, url: str) -> httpx.Response:
-        oauth_session = self._oauth2_session()
+    async def delete(self, url: str) -> httpx.Response:
+        oauth_session = await self._oauth2_session()
 
-        r = oauth_session.delete(
+        r = await oauth_session.delete(
             f"{self._api_base_url}/{url}",
             headers={
                 "Authorization": oauth_session.token["access_token"],
                 "accept": "application/json",
             },
         )
         r.raise_for_status()
 
         return r
 
-    def compute(self, machine: Union[Machine, str]) -> Compute:
+    async def compute(self, machine: Union[Machine, str]) -> AsyncCompute:
         """Create a compute site to submit jobs or view jobs in the queue
 
         :param machine: Name of the compute machine to use
         :return: Compute object that can be used to start jobs,
         view the queue on the system, or list files and directories.
         """
         # Allows for creating a compute from a name string
         machine = Machine(machine)
-        response = self.get(f"status/{machine.value}")
+        response = await self.get(f"status/{machine.value}")
 
-        compute = Compute.parse_obj(response.json())
-        compute.client = self
+        values = response.json()
+        values["client"] = self
+        compute = AsyncCompute.model_validate(values)
 
         return compute
 
     # Get the user associated with the credentials
-    def _user(self):
+    async def _user(self):
         if self._client_user is None:
-            self._client_user = self.user()
+            self._client_user = await self.user()
 
         return self._client_user
 
-    def user(self, username: Optional[str] = None) -> User:
+    async def user(self, username: Optional[str] = None) -> AsyncUser:
         """
         Get a user.
 
         :param username: The username
         :return: The user
         :rtype: UserGroup
         """
-        return User._fetch_user(self, username)
+        return await AsyncUser._fetch_user(self, username)
 
-    def group(self, name: str) -> Group:
+    async def group(self, name: str) -> AsyncGroup:
         """
         Get a group.
 
         :param name: The group name
         :return: The group
-        :rtype: Group
+        :rtype: AsyncGroup
         """
-        return Group._fetch_group(self, name)
+        return await AsyncGroup._fetch_group(self, name)
 
     @property
-    def api(self) -> Api:
+    def api(self) -> AsyncApi:
         """
         API related information.
         """
         if self._api is None:
-            self._api = Api(self)
+            self._api = AsyncApi(self)
 
         return self._api
 
     @property
-    def resources(self) -> Resources:
+    def resources(self) -> AsyncResources:
         """
         Resource related information.
         """
         if self._resources is None:
-            self._resources = Resources(self)
+            self._resources = AsyncResources(self)
 
         return self._resources
+
+
+AsyncCompute.model_rebuild()
+AsyncGroup.model_rebuild()
+AsyncUser.model_rebuild()
+AsyncProject.model_rebuild()
+AsyncRemotePath.model_rebuild()
+AsyncRole.model_rebuild()
+AsyncGroupMember.model_rebuild()
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/compute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from typing import Dict, List, Optional, Union, Callable
 import json
 from enum import Enum
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel, PrivateAttr, ConfigDict
 from functools import wraps
 
 from ..exceptions import SfApiError
 from .._utils import _SLEEP
 from .jobs import JobSacct, JobSqueue, JobSqueue, JobCommand
 from .._models import (
     AppRoutersStatusModelsStatus as ComputeBase,
@@ -26,41 +26,46 @@
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self.client._client_id is None:
             raise SfApiError(
-                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client."
+            )
         elif self.status in [StatusValue.unavailable]:
             raise SfApiError(
-                f"Compute resource {self.name} is {self.status.name}, {self.notes}")
+                f"Compute resource {self.name} is {self.status.name}, {self.notes}"
+            )
         return method(self, *args, **kwargs)
+
     return wrapper
 
 
 class Compute(ComputeBase):
     client: Optional["Client"]
     _monitor: SyncJobMonitor = PrivateAttr()
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._monitor = SyncJobMonitor(self)
 
     def dict(self, *args, **kwargs) -> Dict:
         if "exclude" not in kwargs:
             kwargs["exclude"] = {"client"}
         return super().dict(*args, **kwargs)
 
     def _wait_for_task(self, task_id) -> str:
         while True:
             r = self.client.get(f"tasks/{task_id}")
 
             json_response = r.json()
-            task = Task.parse_obj(json_response)
+            task = Task.model_validate(json_response)
 
             if task.status.lower() in ["error", "failed"]:
                 raise SfApiError(task.result)
 
             if task.result is None:
                 _SLEEP(1)
                 continue
@@ -83,25 +88,25 @@
         # If the string input looks like a script we'll set is_path to false
         elif script.startswith("#!") and "\n" in script:
             # If it starts with shebang and has multiple lines
             is_path = False
         else:
             # If we're given a path make sure it exists
             script_path = self.ls(script)
-            if len(script_path) != 1 or not script_path[0].is_file():
-                raise SfApiError(
-                    f"Script path not present or is not a file, {script}")
+            is_file = script_path[0].is_file()
+            if len(script_path) != 1 or not is_file:
+                raise SfApiError(f"Script path not present or is not a file, {script}")
 
         data = {"job": script, "isPath": is_path}
 
         r = self.client.post(f"compute/jobs/{self.name}", data)
         r.raise_for_status()
 
         json_response = r.json()
-        job_response = SubmitJobResponse.parse_obj(json_response)
+        job_response = SubmitJobResponse.model_validate(json_response)
 
         if job_response.status == SubmitJobResponseStatus.ERROR:
             raise SfApiError(job_response.error)
 
         task_id = job_response.task_id
 
         # We now need waiting for the task to complete!
@@ -110,16 +115,15 @@
         if result.get("status") == "error":
             raise SfApiError(result["error"])
 
         jobid = result.get("jobid")
         if jobid is None:
             raise SfApiError(f"Unable to extract jobid if for task: {task_id}")
 
-        job = JobSqueue(jobid=jobid)
-        job.compute = self
+        job = JobSqueue(jobid=jobid, compute=self)
 
         return job
 
     @check_auth
     def job(
         self, jobid: Union[int, str], command: Optional[JobCommand] = JobCommand.sacct
     ) -> Union["JobSacct", "JobSqueue"]:
@@ -157,21 +161,21 @@
     def run(self, args: Union[str, RemotePath, List[str]]):
         body: RunCommandBody = {
             "executable": args if not isinstance(args, list) else " ".join(args)
         }
 
         r = self.client.post(f"utilities/command/{self.name}", data=body)
         json_response = r.json()
-        run_response = RunCommandResponse.parse_obj(json_response)
+        run_response = RunCommandResponse.model_validate(json_response)
         if run_response.status == RunCommandResponseStatus.ERROR:
             raise SfApiError(run_response.error)
 
         task_id = run_response.task_id
         task_result = self._wait_for_task(task_id)
-        command_result = CommandResult.parse_raw(task_result)
+        command_result = CommandResult.model_validate_json(task_result)
         if command_result.status == "error":
             raise SfApiError(command_result.error)
 
         return command_result.output
 
     def outages(self):
         return self.client.resources.outages(self.name)
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from typing import Optional, Union, List, Any, Callable
 from functools import wraps
-from pydantic import ValidationError, Field, BaseModel, validator
+from pydantic import ValidationError, Field, BaseModel, ConfigDict
 from .._models import BatchGroupAction as GroupAction, UserStats as GroupMemberBase
 from ..exceptions import SfApiError
 from .users import User
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self._client_id is None:
             raise SfApiError(
-                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client.")
+                f"Cannot call {self.__class__.__name__}.{method.__name__}() with an unauthenticated client."
+            )
         return method(self, *args, **kwargs)
+
     return wrapper
 
 
 class GroupMember(GroupMemberBase):
     client: Optional["Client"]
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def user(self) -> "User":
         """
         Get the user associated with the membership.
         """
         return User._fetch_user(self.client, self.name)
 
 
 # Note: We can't use our generated model as we want user => members ( to avoid confusion with User model )
 class Group(BaseModel):
     """
     A user group.
     """
+
     client: Optional["Client"]
     gid: Optional[int]
     name: Optional[str]
     users_: Optional[List[GroupMemberBase]] = Field(..., alias="users")
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def _group_action(
         self,
         users: Union[str, "User", List[str], List["User"]],
         action: GroupAction,
     ):
         # coerse to list
         if not isinstance(users, list):
@@ -53,15 +60,17 @@
         }
 
         r = self.client.put(f"account/groups/{self.name}", data=params)
         json_response = r.json()
 
         # if successful will return group object
         try:
-            new_group = Group.parse_obj(json_response)
+            new_group = Group.model_validate(
+                dict(json_response, client=self.client)
+            )
             self._update(new_group)
         except ValidationError:
             # See if we have validation error raise it
             if "details" in json_response:
                 raise SfApiError(r.text)
             else:
                 raise RuntimeError(r.text)
@@ -83,42 +92,46 @@
         self._group_action(users, GroupAction.batch_remove)
 
     @property
     def members(self):
         """
         The users in this group.
         """
-        members = [GroupMember.parse_obj(user_info) for user_info in self.users_]
+        members = [
+            GroupMember.model_validate(
+                dict(user_info.model_dump(), client=self.client)
+            )
+            for user_info in self.users_
+        ]
 
         def _set_client(m):
             m.client = self.client
 
             return m
 
         members = map(_set_client, members)
 
         return list(members)
 
     @staticmethod
     @check_auth
     def _fetch_group(client: "Client", name):
         response = client.get(f"account/groups/{name}")
-        json_response = response.json()
 
-        group = Group.parse_obj(json_response)
-        group.client = client
+        json_response = response.json()
+        group = Group.model_validate(dict(json_response, client=client))
 
         return group
 
     def update(self):
         """
         Update the state of the group by fetching the state from the server.
         """
         group_state = self._fetch_group(self.client, self.name)
         self._update(group_state)
 
     def _update(self, new_group_state: Any) -> "Group":
-        for k in new_group_state.__fields_set__:
+        for k in new_group_state.model_fields_set:
             v = getattr(new_group_state, k)
             setattr(self, k, v)
 
         return self
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Optional, Dict, List, ClassVar
 from .._utils import _SLEEP
 from ..exceptions import SfApiError
 from .._models.job_status_response_sacct import OutputItem as JobSacctBase
 from .._models.job_status_response_squeue import OutputItem as JobSqueueBase
 from .._models import AppRoutersComputeModelsStatus as JobResponseStatus
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, field_validator
 
 from .._jobs import JobCommand
 from .._jobs import JobStateResponse
 from .._jobs import JobState
 from .._jobs import TERMINAL_STATES
 
 
@@ -40,15 +40,15 @@
     if partition is not None:
         kwargs = params.setdefault("kwargs", [])
         kwargs.append(f"partition={partition}")
 
     r = compute.client.get(job_url, params)
 
     json_response = r.json()
-    job_state_response = JobStateResponse.parse_obj(json_response)
+    job_state_response = JobStateResponse.model_validate(json_response)
 
     if job_state_response == JobResponseStatus.ERROR:
         error = json_response.error
         raise SfApiError(error)
 
     return job_state_response.output
 
@@ -60,32 +60,31 @@
     user: Optional[str] = None,
     partition: Optional[str] = None,
 ):
     job_states = _fetch_raw_state(
         compute, jobids, user, partition, job_type._command == JobCommand.sacct
     )
 
-    jobs = [job_type.parse_obj(state) for state in job_states]
-
-    for job in jobs:
-        job.compute = compute
+    jobs = [
+        job_type.model_validate(dict(state, compute=compute)) for state in job_states
+    ]
 
     return jobs
 
 
 class Job(BaseModel, ABC):
     """
     Models a job submitted to run on a compute resource.
     """
 
     compute: Optional["Compute"] = None
-    state: Optional[JobState]
-    jobid: Optional[str]
+    state: Optional[JobState] = None
+    jobid: Optional[str] = None
 
-    @validator("state", pre=True, check_fields=False)
+    @field_validator("state", mode="before", check_fields=False)
     def state_validate(cls, v):
         # sacct return a state of the form "CANCELLED by XXXX" for the
         # cancelled state, coerce into value that will match a state
         # modeled by the enum
         if v.startswith("CANCELLED by"):
             return "CANCELLED"
 
@@ -95,15 +94,15 @@
         """
         Update the state of the job by fetching the state from the compute resource.
         """
         job_state = self._fetch_state()
         self._update(job_state)
 
     def _update(self, new_job_state: Any) -> Job:
-        for k in new_job_state.__fields_set__:
+        for k in new_job_state.model_fields_set:
             v = getattr(new_job_state, k)
             setattr(self, k, v)
 
         return self
 
     def _wait_until(self, states: List[JobState], timeout: int = sys.maxsize):
         max_iteration = math.ceil(timeout / self.compute.client._wait_interval)
@@ -209,14 +208,15 @@
 
 
 class JobSqueue(Job, JobSqueueBase):
     """
     Models a job running on a compute resource, the information is
     fetched using `squeue`.
     """
+
     _command: ClassVar[JobCommand] = JobCommand.squeue
 
     def _fetch_state(self):
         jobs = self.compute._monitor.fetch_jobs(
             job_type=self.__class__, jobids=[self.jobid]
         )
         # If the job state comes back empty the job is probably no longer in
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/paths.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,63 +37,49 @@
         super().__init__(**kwargs)
         self._path = PurePosixPath(path)
 
         if self.name is None:
             self.name = self._path.name
 
     def __truediv__(self, key):
-        remote_path = RemotePath(str(self._path / key))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        remote_path.compute = self.compute
+        remote_path = RemotePath(path=str(self._path / key), compute=self.compute)
 
         return remote_path
 
     def __rtruediv__(self, key):
-        remote_path = RemotePath(str(key / self._path))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        remote_path.compute = self.compute
+        remote_path = RemotePath(path=str(key / self._path), compute=self.compute)
 
         return remote_path
 
     def __str__(self):
         return str(self._path)
 
     @property
     def parent(self) -> "RemotePath":
         """
         The parent of the path.
 
         :return: the parent
 
         """
-        parent_path = RemotePath(str(self._path.parent))
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        parent_path.compute = self.compute
+        parent_path = RemotePath(path=str(self._path.parent), compute=self.compute)
 
         return parent_path
 
     @property
     def parents(self) -> List["RemotePath"]:
         """
         The parents of the path.
 
         :return: the parents
         """
-        parents = [RemotePath(str(p)) for p in self._path.parents]
-
-        # We have to set the compute field separately otherwise
-        # we run into ForwardRef issue because of circular deps
-        def _set_compute(p):
-            p.compute = self.compute
-            return p
-
-        parents = map(_set_compute, parents)
+        parents = [
+            RemotePath(path=str(p), compute=self.compute)
+            for p in self._path.parents
+        ]
 
         return parents
 
     @property
     def stem(self) -> str:
         """
         The final path component, without its suffix.
@@ -160,15 +146,15 @@
         if self.is_dir():
             raise IsADirectoryError(self._path)
 
         r = self.compute.client.get(
             f"utilities/download/{self.compute.name}/{self._path}?binary={binary}"
         )
         json_response = r.json()
-        download_response = FileDownloadResponse.parse_obj(json_response)
+        download_response = FileDownloadResponse.model_validate(json_response)
 
         if download_response.status == FileDownloadResponseStatus.ERROR:
             raise SfApiError(download_response.error)
 
         file_data = download_response.file
         if download_response.is_binary:
             binary_file_data = b64decode(file_data)
@@ -179,25 +165,26 @@
     @staticmethod
     def _ls(
         compute: "Compute", path, directory=False, filter_dots=True
     ) -> List["RemotePath"]:
         r = compute.client.get(f"utilities/ls/{compute.name}/{path}")
 
         json_response = r.json()
-        directory_listing_response = DirectoryListingResponse.parse_obj(json_response)
+        directory_listing_response = DirectoryListingResponse.model_validate(
+            json_response
+        )
         if directory_listing_response.status == DirectoryListingResponseStatus.ERROR:
             raise SfApiError(directory_listing_response.error)
 
         paths = []
 
         def _to_remote_path(path, entry):
-            kwargs = entry.dict()
-            kwargs.update(path=path)
+            kwargs = entry.model_dump()
+            kwargs.update(path=path, compute=compute)
             p = RemotePath(**kwargs)
-            p.compute = compute
 
             return p
 
         # Special case for listing file
         if len(directory_listing_response.entries) == 1:
             entry = directory_listing_response.entries[0]
             # The API can add an extra /
@@ -245,15 +232,15 @@
         # case we don't want to update the name
         new_state = file_state[0]
         new_state.name = self.name
 
         self._update(new_state)
 
     def _update(self, new_file_state: "RemotePath") -> "RemotePath":
-        for k in new_file_state.__fields_set__:
+        for k in new_file_state.model_fields_set:
             v = getattr(new_file_state, k)
             setattr(self, k, v)
 
         return self
 
     def upload(self, file: BytesIO) -> "RemotePath":
         try:
@@ -278,20 +265,19 @@
 
         url = f"utilities/upload/{self.compute.name}/{upload_path}"
         files = {"file": file}
 
         r = self.compute.client.put(url, files=files)
 
         json_response = r.json()
-        upload_response = UploadResponse.parse_obj(json_response)
+        upload_response = UploadResponse.model_validate(json_response)
         if upload_response.status == UploadResponseStatus.ERROR:
             raise SfApiError(upload_response.error)
 
-        remote_path = RemotePath(upload_path)
-        remote_path.compute = self.compute
+        remote_path = RemotePath(path=upload_path, compute=self.compute)
 
         return remote_path
 
     @contextmanager
     def open(self, mode: str) -> IO[AnyStr]:
         """
         Open the file at this path.
```

### Comparing `sfapi_client-0.0.6/src/sfapi_client/_sync/projects.py` & `sfapi_client-0.0.7/src/sfapi_client/_sync/projects.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from typing import Optional
-from pydantic import ValidationError, Field
+from pydantic import ValidationError, Field, ConfigDict
 
-from .._models import (
-    ProjectStats as ProjectBase,
-    RoleStats as RoleBase
-)
+from .._models import ProjectStats as ProjectBase, RoleStats as RoleBase
 from ..exceptions import SfApiError
 
 
 class Role(RoleBase):
     client: Optional["Client"]
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
 
 class Project(ProjectBase):
     client: Optional["Client"]
     name: str = Field(alias="repo_name")
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def create_group(self, name: str) -> "Group":
         """
         Create a new project.
         :param name: The project name
         """
         from .groups import Group
 
         params = {"name": name, "repo_name": self.repo_name}
 
         r = self.client.post("account/groups", data=params)
         json_response = r.json()
         try:
-            group = Group.parse_obj(json_response)
+            group = Group.model_validate(dict(json_response, client=self.client))
         except ValidationError:
             # See if we have validation error raise it
             if "details" in json_response:
                 raise SfApiError(r.text())
             else:
                 raise RuntimeError(r.text())
```

### Comparing `sfapi_client-0.0.6/tests/test_compute.py` & `sfapi_client-0.0.7/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/tests/test_compute_async.py` & `sfapi_client-0.0.7/tests/test_compute_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,8 @@
 
 @pytest.mark.asyncio
 async def test_planned_outages(client_id, client_secret, test_machine):
     async with AsyncClient(client_id, client_secret) as client:
         machine = await client.compute(test_machine)
         outages = await machine.planned_outages()
 
-        assert len(outages) > 0
+        assert len(outages) >= 0
```

### Comparing `sfapi_client-0.0.6/tests/test_groups.py` & `sfapi_client-0.0.7/tests/test_groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,42 @@
+import pytest
 from sfapi_client import Client
 
 
-def test_group(client_id, client_secret, test_group, dev_api_url):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+@pytest.mark.api_dev
+def test_group(
+    dev_client_id, dev_client_secret, test_group, dev_api_url, dev_token_url
+):
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         group = client.group(test_group)
         assert group is not None
         assert group.name == test_group
 
 
+@pytest.mark.api_dev
 def test_create_group(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         user = client.user(test_username)
         projects = user.projects()
 
         # Find the test project
         project = None
         for p in projects:
             if p.name == test_project:
@@ -32,23 +48,30 @@
         # Create a test group
         group = project.create_group(test_random_group)
 
         assert group is not None
         assert group.name == test_random_group
 
 
+@pytest.mark.api_dev
 def test_add_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         user = client.user(test_username)
         projects = user.projects()
 
         # Find the test project
         project = None
         for p in projects:
             if p.name == test_project:
@@ -74,23 +97,30 @@
 
         is_member = (
             len(list(filter(lambda m: m.name == test_username, group.members))) == 1
         )
         assert is_member
 
 
+@pytest.mark.api_dev
 def test_remove_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         user = client.user(test_username)
         projects = user.projects()
 
         # Find the test project
         project = None
         for p in projects:
             if p.name == test_project:
@@ -121,23 +151,30 @@
 
         # Now remove the user
         group.remove(user)
 
         assert group.members == []
 
 
+@pytest.mark.api_dev
 def test_groupmember_to_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         user = client.user(test_username)
         projects = user.projects()
 
         # Find the test project
         project = None
         for p in projects:
             if p.name == test_project:
```

### Comparing `sfapi_client-0.0.6/tests/test_groups_async.py` & `sfapi_client-0.0.7/tests/test_groups_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import pytest
 
 from sfapi_client import AsyncClient
 
 
 @pytest.mark.asyncio
-async def test_group(client_id, client_secret, test_group, dev_api_url):
+async def test_group(client_id, client_secret, test_group):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=client_id,
+        secret=client_secret,
     ) as client:
         group = await client.group(test_group)
         assert group is not None
         assert group.name == test_group
 
 
+@pytest.mark.api_dev
 @pytest.mark.asyncio
 async def test_create_group(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
     ) as client:
         user = await client.user(test_username)
         projects = await user.projects()
 
         # Find the test project
         project = None
         for p in projects:
@@ -40,25 +46,30 @@
         # Create a test group
         group = await project.create_group(test_random_group)
 
         assert group is not None
         assert group.name == test_random_group
 
 
+@pytest.mark.api_dev
 @pytest.mark.asyncio
 async def test_add_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
     ) as client:
         user = await client.user(test_username)
         projects = await user.projects()
 
         # Find the test project
         project = None
         for p in projects:
@@ -85,25 +96,30 @@
 
         is_member = (
             len(list(filter(lambda m: m.name == test_username, group.members))) == 1
         )
         assert is_member
 
 
+@pytest.mark.api_dev
 @pytest.mark.asyncio
 async def test_remove_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
     ) as client:
         user = await client.user(test_username)
         projects = await user.projects()
 
         # Find the test project
         project = None
         for p in projects:
@@ -135,25 +151,30 @@
 
         # Now remove the user
         await group.remove(user)
 
         assert group.members == []
 
 
+@pytest.mark.api_dev
 @pytest.mark.asyncio
 async def test_groupmember_to_user(
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_project,
     test_random_group,
     test_username,
     dev_api_url,
+    dev_token_url,
 ):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
     ) as client:
         user = await client.user(test_username)
         projects = await user.projects()
 
         # Find the test project
         project = None
         for p in projects:
```

### Comparing `sfapi_client-0.0.6/tests/test_jobs.py` & `sfapi_client-0.0.7/tests/test_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,48 +39,46 @@
         job = machine.submit_job(test_job_path)
 
         state = job.running()
 
         assert state == JobState.RUNNING
 
 
-def test_running_timeout(client_id, client_secret, test_job_path, test_machine):
-    with Client(client_id, client_secret, wait_interval=1) as client:
-        machine = client.compute(test_machine)
-        job = machine.submit_job(test_job_path)
-
-        with pytest.raises(TimeoutError):
-            job.running(timeout=1)
-
-
 def test_complete_timeout(client_id, client_secret, test_job_path, test_machine):
     with Client(client_id, client_secret) as client:
         machine = client.compute(test_machine)
         job = machine.submit_job(test_job_path)
 
         with pytest.raises(TimeoutError):
             job.complete(timeout=10)
 
 
+@pytest.mark.api_dev
 def test_job_monitor_check_request(
     mocker,
-    client_id,
-    client_secret,
+    dev_client_id,
+    dev_client_secret,
     test_job_path,
     test_machine,
     dev_api_url,
+    dev_token_url,
 ):
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         num_jobs = 10
         _fetch_jobs = mocker.patch("sfapi_client._monitor._fetch_jobs")
 
         machine = client.compute(test_machine)
 
         # Create some test jobs for mocking
-        test_jobs = [JobSqueue(jobid=i) for i in range(0, num_jobs)]
+        test_jobs = [JobSqueue(jobid=str(i)) for i in range(0, num_jobs)]
         for j in test_jobs:
             j.compute = machine
 
         # Patch the submit_job to return the test jobs
         submit_job = mocker.patch.object(Compute, "submit_job")
         submit_job.side_effect = test_jobs
 
@@ -121,20 +119,31 @@
         for _, kwargs in calls:
             ids.update(kwargs["jobids"])
 
         assert len(ids) == num_jobs
 
 
 # We currently run this in api-dev as its a new feature deployed there
+@pytest.mark.api_dev
 def test_job_monitor_multiple_threads(
-    client_id, client_secret, test_job_path, test_machine, dev_api_url
+    dev_client_id,
+    dev_client_secret,
+    test_job_path,
+    test_machine,
+    dev_api_url,
+    dev_token_url,
 ):
     num_jobs = 5
 
-    with Client(client_id, client_secret, api_base_url=dev_api_url) as client:
+    with Client(
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
+    ) as client:
         machine = client.compute(test_machine)
 
         jobs = []
 
         def _submit_job():
             job = machine.submit_job(test_job_path)
             jobs.append(job)
```

### Comparing `sfapi_client-0.0.6/tests/test_jobs_async.py` & `sfapi_client-0.0.7/tests/test_jobs_async.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,60 +48,52 @@
 
         state = await job.running()
 
         assert state == JobState.RUNNING
 
 
 @pytest.mark.asyncio
-async def test_running_timeout(client_id, client_secret, test_job_path, test_machine):
-    async with AsyncClient(client_id, client_secret, wait_interval=1) as client:
-        machine = await client.compute(test_machine)
-        job = await machine.submit_job(test_job_path)
-
-        with pytest.raises(TimeoutError):
-            await job.running(timeout=1)
-
-
-@pytest.mark.asyncio
 async def test_complete_timeout(client_id, client_secret, test_job_path, test_machine):
     async with AsyncClient(client_id, client_secret, wait_interval=1) as client:
         machine = await client.compute(test_machine)
         job = await machine.submit_job(test_job_path)
 
         with pytest.raises(TimeoutError):
             await job.complete(timeout=1)
 
 
 @pytest.mark.asyncio
 async def test_job_monitor_check_request(
     mocker, client_id, client_secret, test_job_path, test_machine
 ):
     async with AsyncClient(client_id, client_secret) as client:
-        _fetch_jobs_async = mocker.patch(
-            "sfapi_client._monitor._fetch_jobs_async"
-        )
+        _fetch_jobs_async = mocker.patch("sfapi_client._monitor._fetch_jobs_async")
         machine = await client.compute(test_machine)
 
         # Create some test jobs for mocking
-        test_jobs = [AsyncJobSqueue(jobid=i) for i in range(0, 10)]
-        for j in test_jobs:
-            j.compute = machine
+        test_jobs = [
+            AsyncJobSqueue(jobid=str(i), compute=machine) for i in range(0, 10)
+        ]
+        test_jobs_futures = [asyncio.Future() for _ in range(0, 10)]
+        for i in range(0, 10):
+            test_jobs_futures[i].set_result(test_jobs[i])
 
         # Patch the submit_job to return the test jobs
         submit_job = mocker.patch.object(AsyncCompute, "submit_job")
-        submit_job.side_effect = test_jobs
+        submit_job.side_effect = test_jobs_futures
 
         # Patch the return value of _fetch_jobs_async to return
         # the test jobs
         _fetch_jobs_async.return_value = test_jobs
 
         # Submit a bunch on jobs
         jobs = []
         for _ in range(0, 10):
             jobs.append(await machine.submit_job(test_job_path))
+        jobs = test_jobs
 
         # Call update on all jobs
         await asyncio.gather(*[asyncio.create_task(j.update()) for j in jobs])
 
         # We should only hit the server twice
         assert _fetch_jobs_async.await_count == 2
 
@@ -116,34 +108,36 @@
 
 
 @pytest.mark.asyncio
 async def test_job_monitor_job_types(
     mocker, client_id, client_secret, test_job_path, test_machine
 ):
     async with AsyncClient(client_id, client_secret) as client:
-        _fetch_jobs_async = mocker.patch(
-            "sfapi_client._monitor._fetch_jobs_async"
-        )
+        _fetch_jobs_async = mocker.patch("sfapi_client._monitor._fetch_jobs_async")
         machine = await client.compute(test_machine)
 
         test_job_specs = [
             (AsyncJobSqueue, 0),
             (AsyncJobSqueue, 1),
             (AsyncJobSacct, 2),
             (AsyncJobSqueue, 3),
         ]
 
         # Create some test jobs for mocking
-        test_jobs = [job_class(jobid=i) for (job_class, i) in test_job_specs]
-        for j in test_jobs:
-            j.compute = machine
+        test_jobs = [
+            job_class(jobid=str(i), compute=machine)
+            for (job_class, i) in test_job_specs
+        ]
+        test_jobs_futures = [asyncio.Future() for _ in range(len(test_job_specs))]
+        for i, f in enumerate(test_jobs_futures):
+            f.set_result(test_jobs[i])
 
-        # Patch the submit_job to return the test jobs
+        # Patch the job method to return the test jobs
         job = mocker.patch.object(AsyncCompute, "job")
-        job.side_effect = test_jobs
+        job.side_effect = test_jobs_futures
 
         # Patch the return value of _fetch_jobs_async to return
         # the test jobs
         _fetch_jobs_async.return_value = test_jobs
 
         jobs = [
             await machine.job(i, job_class._command)
@@ -166,20 +160,29 @@
         assert kwargs["job_type"] == AsyncJobSqueue
 
         _, kwargs = third_call
         assert kwargs["job_type"] == AsyncJobSacct
 
 
 # We currently run this in api-dev as its a new feature deployed there
+@pytest.mark.api_dev
 @pytest.mark.asyncio
 async def test_job_monitor_gather(
-    client_id, client_secret, test_job_path, test_machine, dev_api_url
+    dev_client_id,
+    dev_client_secret,
+    test_job_path,
+    test_machine,
+    dev_api_url,
+    dev_token_url,
 ):
     async with AsyncClient(
-        client_id, client_secret, api_base_url=dev_api_url
+        client_id=dev_client_id,
+        secret=dev_client_secret,
+        api_base_url=dev_api_url,
+        token_url=dev_token_url,
     ) as client:
         machine = await client.compute(test_machine)
 
         submit_tasks = []
         for _ in range(0, 5):
             submit_tasks.append(asyncio.create_task(machine.submit_job(test_job_path)))
```

### Comparing `sfapi_client-0.0.6/tests/test_paths.py` & `sfapi_client-0.0.7/tests/test_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import string
 
 from sfapi_client import Client
 from sfapi_client.paths import RemotePath
 
 
 def test_concat():
-    a = RemotePath("/a")
-    b = RemotePath("b")
+    a = RemotePath("/a", compute=None)
+    b = RemotePath("b", compute=None)
     c = "c"
 
     new_path = a / b
     assert isinstance(new_path, RemotePath)
     assert new_path.name == "b"
     assert new_path.group is None
     assert str(new_path) == "/a/b"
@@ -23,15 +23,15 @@
     assert isinstance(new_path, RemotePath)
     assert new_path.name == "b"
     assert new_path.group is None
     assert str(new_path) == "c/b"
 
 
 def test_parent():
-    test_path = RemotePath("/foo")
+    test_path = RemotePath("/foo", compute=None)
     assert isinstance(test_path.parent, RemotePath)
     for p in test_path.parents:
         assert isinstance(p, RemotePath)
 
 
 def test_download_text(client_id, client_secret, test_machine, test_job_path):
     with Client(client_id, client_secret) as client:
```

### Comparing `sfapi_client-0.0.6/tests/test_paths_async.py` & `sfapi_client-0.0.7/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/tests/test_projects.py` & `sfapi_client-0.0.7/tests/test_projects_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,20 @@
 import pytest
+from pathlib import Path
 
-from sfapi_client import Client
+from sfapi_client import AsyncClient
 
 
-@pytest.mark.skip(
-    reason="not sure how we can test this, there doesn't seem to be a way to remove groups?"
-)
-async def test_create_group(
-    client_id, client_secret, test_username, test_project, test_group_create
-):
-    with Client(client_id, client_secret) as client:
-        user = client.user(test_username)
-        projects = user.projects()
-
-        project = None
-        for p in projects:
-            if p.repo_name == test_project:
-                project = p
-                break
-
-        assert project
-
-        group = project.create_group(test_group_create)
-
-        assert group.name == test_create_group
-
-
-def test_projects(
-    client_id, client_secret
-):
-    with Client(client_id, client_secret) as client:
-        user = client.user()
-        projects = user.projects()
+@pytest.mark.asyncio
+async def test_projects(client_id, client_secret):
+    async with AsyncClient(client_id, client_secret) as client:
+        user = await client.user()
+        projects = await user.projects()
         assert projects
 
 
-def test_roles(
-    client_id, client_secret
-):
-    with Client(client_id, client_secret) as client:
-        user = client.user()
-        roles = user.roles()
+@pytest.mark.asyncio
+async def test_roles(client_id, client_secret):
+    async with AsyncClient(client_id, client_secret) as client:
+        user = await client.user()
+        roles = await user.roles()
         assert roles
```

### Comparing `sfapi_client-0.0.6/tests/test_resources.py` & `sfapi_client-0.0.7/tests/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     with Client() as client:
         status = client.resources.status()
 
         assert test_machine.value in status
         test_machine_status = status[test_machine.value]
         assert test_machine_status.name == test_machine
 
+
 @pytest.mark.public
 def test_resouce_status(test_resource):
     with Client() as client:
         status = client.resources.status(test_resource)
 
         assert test_resource.value in status.name
-        assert status.status in StatusValue
+        assert status.status in StatusValue
```

### Comparing `sfapi_client-0.0.6/tests/test_resources_async.py` & `sfapi_client-0.0.7/tests/test_resources_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from sfapi_client import AsyncClient, StatusValue
 
+
 @pytest.mark.public
 @pytest.mark.asyncio
 async def test_outages_by_resource(test_machine):
     async with AsyncClient() as client:
         outages = await client.resources.outages(test_machine)
 
         assert len(outages) > 0
@@ -27,14 +28,15 @@
 async def test_notes_by_resource(test_machine):
     async with AsyncClient() as client:
         notes = await client.resources.notes(test_machine)
 
         assert len(notes) > 0
         assert notes[0].name == test_machine
 
+
 @pytest.mark.public
 @pytest.mark.asyncio
 async def test_status_by_resource(test_machine):
     async with AsyncClient() as client:
         status = await client.resources.status(test_machine)
 
         assert status.name == test_machine
@@ -59,37 +61,39 @@
         outages = await client.resources.planned_outages()
 
         if test_machine.value in outages:
             test_machine_outages = outages[test_machine.value]
             assert len(test_machine_outages) > 0
             assert test_machine_outages[0].name == test_machine
 
+
 @pytest.mark.public
 @pytest.mark.asyncio
 async def test_notes(test_machine):
     async with AsyncClient() as client:
         notes = await client.resources.notes()
 
         assert test_machine.value in notes
         test_machine_notes = notes[test_machine.value]
         assert len(test_machine_notes) > 0
         assert test_machine_notes[0].name == test_machine
 
+
 @pytest.mark.public
 @pytest.mark.asyncio
 async def test_status(test_machine):
     async with AsyncClient() as client:
         status = await client.resources.status()
 
         assert test_machine.value in status
         test_machine_status = status[test_machine.value]
         assert test_machine_status.name == test_machine
 
 
 @pytest.mark.public
 @pytest.mark.asyncio
 async def test_resouce_status(test_resource):
-   async with AsyncClient() as client:
+    async with AsyncClient() as client:
         status = await client.resources.status(test_resource)
 
         assert test_resource.value in status.name
-        assert status.status in StatusValue
+        assert status.status in StatusValue
```

### Comparing `sfapi_client-0.0.6/tests/test_users.py` & `sfapi_client-0.0.7/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/tests/test_users_async.py` & `sfapi_client-0.0.7/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/LICENSE` & `sfapi_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/README.md` & `sfapi_client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.6/pyproject.toml` & `sfapi_client-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 ]
 description = "Python client for NERSC SF API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "authlib",
   "httpx",
-  "pydantic==v1.10.10",
+  "pydantic~=2.0",
+  "pydantic-settings",
   "tenacity"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sfapi_client-0.0.6/PKG-INFO` & `sfapi_client-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sfapi_client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: authlib
 Requires-Dist: httpx
-Requires-Dist: pydantic==v1.10.10
+Requires-Dist: pydantic-settings
+Requires-Dist: pydantic~=2.0
 Requires-Dist: tenacity
 Provides-Extra: docs
 Requires-Dist: mkdocs-gen-files; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-literate-nav; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs-section-index; extra == 'docs'
```

