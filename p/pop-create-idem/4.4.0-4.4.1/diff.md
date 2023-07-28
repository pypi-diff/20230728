# Comparing `tmp/pop-create-idem-4.4.0.tar.gz` & `tmp/pop-create-idem-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-4.4.0.tar", last modified: Fri Jul 28 19:02:37 2023, max compression
+gzip compressed data, was "pop-create-idem-4.4.1.tar", last modified: Fri Jul 28 19:15:10 2023, max compression
```

## Comparing `pop-create-idem-4.4.0.tar` & `pop-create-idem-4.4.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8799 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     4041 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     1123 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/sls.py
--rw-r--r--   0 root         (0) root         (0)     4488 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)     5908 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/contracts/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2116 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/example.py
--rw-r--r--   0 root         (0) root         (0)     3756 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     6705 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3114 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/test.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2209 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     4216 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     5663 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     7937 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     4724 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5537 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)     1338 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1398 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1831 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4032 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
--rw-r--r--   0 root         (0) root         (0)     1152 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      819 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2805 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8423 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8799 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/sls.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/customize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/customize/contracts/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/customize/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     3132 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/example.py
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/test.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6503 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.312396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      819 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 19:15:09.000000 pop-create-idem-4.4.1/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:15:10.308396 pop-create-idem-4.4.1/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-28 19:15:10.000000 pop-create-idem-4.4.1/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 19:15:10.316396 pop-create-idem-4.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-28 19:14:56.000000 pop-create-idem-4.4.1/setup.py
```

### Comparing `pop-create-idem-4.4.0/LICENSE` & `pop-create-idem-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/PKG-INFO` & `pop-create-idem-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.4.0
+Version: 4.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-4.4.0/README.rst` & `pop-create-idem-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/cloudspec/__init__.py` & `pop-create-idem-4.4.1/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/cloudspec/conf.py` & `pop-create-idem-4.4.1/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import copy
 import os.path
 import pathlib
 
 import tqdm
 
-from cloudspec import CloudSpec
 
 HEADER_TEMPLATE = "Exec module for managing {}."
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
-    cloud_spec = CloudSpec(**ctx.cloud_spec)
+    cloud_spec = copy.deepcopy(ctx.cloud_spec)
     exec_dir = root_directory / ctx.clean_name / "exec" / ctx.service_name
     template_dir = (
         root_directory
         / ctx.clean_name
         / "autogen"
         / ctx.service_name
         / "templates"
         / "exec"
     )
 
-    for ref, plugin in cloud_spec.plugins.items():
+    for ref, plugin in tqdm.tqdm(
+        cloud_spec.plugins.items(), desc=f"Generating exec functions"
+    ):
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
         resource_header = HEADER_TEMPLATE.format(
             hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
         )
 
@@ -56,18 +58,15 @@
             present_parameter = {}
             if plugin.functions.get("create"):
                 present_parameter = hub.cloudspec.parse.param.simple_map(
                     plugin.functions["create"].params
                 )
 
             # Make the get, list, create, delete, and update functions; these are required for every auto_state exec module
-            for function_name in tqdm.tqdm(
-                ["get", "list", "create", "update", "delete"],
-                desc=f"{ref} auto_state functions",
-            ):
+            for function_name in ["get", "list", "create", "update", "delete"]:
                 if func_data.get(function_name):
                     base_template = hub.cloudspec.template.auto_state[
                         function_name.upper()
                     ]
 
                     request_format_template_file = (
                         f"{template_dir}/{function_name}.jinja2"
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         / ctx.clean_name
         / "autogen"
         / ctx.service_name
         / "templates"
         / "exec"
     )
 
-    for ref, plugin in cloud_spec.plugins.items():
+    for ref, plugin in tqdm.tqdm(
+        cloud_spec.plugins.items(), desc=f"Generating exec functions"
+    ):
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         cli_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
         resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
         resource_header = HEADER_TEMPLATE.format(
             hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
         )
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/sls.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/sls.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+import copy
 import os
 import pathlib
 
-from cloudspec import CloudSpec
+import tqdm
 
 HEADER_TEMPLATE = "States module for managing {}."
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
-    cloud_spec = CloudSpec(**ctx.cloud_spec)
+    cloud_spec = copy.deepcopy(ctx.cloud_spec)
     states_dir = root_directory / ctx.clean_name / "states" / ctx.service_name
     template_dir = (
         root_directory
         / ctx.clean_name
         / "autogen"
         / ctx.service_name
         / "templates"
         / "state"
     )
 
-    for ref, plugin in cloud_spec.plugins.items():
+    for ref, plugin in tqdm.tqdm(
+        cloud_spec.plugins.items(), desc=f"Generating state modules functions"
+    ):
         mod_file = hub.cloudspec.parse.plugin.touch(states_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         state_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
         resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
         resource_header = HEADER_TEMPLATE.format(
             hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
         )
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,76 @@
+import copy
 import os
 import pathlib
 
-from cloudspec import CloudSpec
+import tqdm
+from dict_tools.data import NamespaceDict
+
 from cloudspec import CloudSpecParam
 
 HEADER_TEMPLATE = "Tests for validating {}."
 
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
-    cloud_spec = CloudSpec(**ctx.cloud_spec)
+    cloud_spec = copy.deepcopy(ctx.cloud_spec)
 
-    for ref, plugin in cloud_spec.plugins.items():
+    exec_tests_order = [
+        "test_create",
+        "test_get",
+        "test_list",
+        "test_update",
+        "test_delete",
+    ]
+
+    for ref, plugin in tqdm.tqdm(
+        cloud_spec.plugins.items(), desc=f"Generating test functions"
+    ):
         resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
         resource_header = HEADER_TEMPLATE.format(
             hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
         )
 
         plugin["imports"] = ["import pytest"]
 
-        for test_type in ["exec", "states", "tool"]:
+        for test_module_type in ["exec", "states", "tool"]:
             test_dir = (
                 root_directory
                 / "tests"
                 / "integration"
                 # test_module_type = exec, states, tool
-                / test_type
+                / test_module_type
             )
 
             template_dir = (
                 root_directory
                 / ctx.clean_name
                 / "autogen"
                 / ctx.service_name
                 / "templates"
                 / "tests"
                 # test_module_type = exec, states, tool
-                / test_type
+                / test_module_type
             )
 
             mod_file = hub.cloudspec.parse.plugin.touch(
                 root=test_dir, ref=ref, is_test=True
             )
 
             plugin["file_vars"] = {}
-            if test_type == "states":
+            if test_module_type == "states":
                 # The states test should be run with --test and actual run mode
                 plugin["file_vars"]["PARAMETRIZE"] = {
                     "argnames": "__test",
                     "argvalues": [True, False],
                     "ids": ["--test", "run"],
                 }
 
-            if test_type in ["states", "exec"]:
+            if test_module_type in ["states", "exec"]:
                 # Add default global parameter for tracking a resource being created inside test
                 # This helps in clean up of a created resource in test
                 plugin["file_vars"]["PARAMETER"] = {
                     "name": "idem-test-resource- + TODO: Add unique identifier generator",
                 }
 
             to_write = hub.cloudspec.parse.plugin.header(
@@ -75,23 +88,33 @@
                     name: CloudSpecParam(name=name, **param_spec)
                     for name, param_spec in test_get_func[0]
                     .get("hardcoded", {})
                     .get("method_call_params", {})
                     .items()
                 }
 
-            for function_name, function_data in plugin.functions.items():
-                if not function_name.startswith("test_"):
-                    # Only process test functions
-                    continue
-
-                if test_type != function_data.hardcoded.test_module_type:
-                    # Let's not add to the file if it doesn't belong to the module
-                    continue
+            test_functions = NamespaceDict(
+                filter(
+                    # It is an integration test, and it is matching the current test type being generated.
+                    lambda item: "test_module_type" in item[1].hardcoded
+                    and test_module_type == item[1].hardcoded.test_module_type,
+                    plugin.functions.items(),
+                )
+            )
+
+            if test_module_type == "exec":
+                # This makes sure create is executed first
+                test_functions = NamespaceDict(
+                    [
+                        (exec_test_func_name, test_functions[exec_test_func_name])
+                        for exec_test_func_name in exec_tests_order
+                    ]
+                )
 
+            for function_name, function_data in test_functions.items():
                 request_format_template_file = f"{template_dir}/{function_name}.jinja2"
                 default_request_format_template_file = f"{template_dir}/default.jinja2"
                 if os.path.isfile(request_format_template_file):
                     with open(f"{template_dir}/{function_name}.jinja2", "rb+") as f:
                         request_format = f.read().decode()
                 elif os.path.isfile(default_request_format_template_file):
                     with open(default_request_format_template_file, "rb+") as f:
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/create/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import copy
 import os
 import pathlib
 
 import tqdm
-
-from cloudspec import CloudSpec
+from dict_tools.data import NamespaceDict
 
 HEADER_TEMPLATE = "Utility functions for {}."
 
 
 def run(hub, ctx, root_directory: pathlib.Path):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
-    cloud_spec = CloudSpec(**ctx.cloud_spec)
+    cloud_spec = copy.deepcopy(ctx.cloud_spec)
     tool_dir = root_directory / ctx.clean_name / "tool" / ctx.service_name
     template_dir = (
         root_directory
         / ctx.clean_name
         / "autogen"
         / ctx.service_name
         / "templates"
         / "tool"
     )
 
-    for ref, plugin in cloud_spec.plugins.items():
+    for ref, plugin in tqdm.tqdm(
+        cloud_spec.plugins.items(), desc=f"Generating tool functions"
+    ):
         mod_file = hub.cloudspec.parse.plugin.touch(tool_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         module_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
         resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
         resource_header = HEADER_TEMPLATE.format(
             hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
         )
@@ -36,30 +38,34 @@
             to_write = hub.cloudspec.parse.plugin.header(
                 plugin=plugin, resource_header=resource_header
             )
         else:
             to_write = hub.cloudspec.parse.plugin.header(
                 plugin=plugin, resource_header=resource_header
             )
-            for func_name, func_data in tqdm.tqdm(
-                plugin.functions.items(), desc=f"{ref} tool functions"
-            ):
-                if func_name in [
-                    "get",
-                    "list",
-                    "create",
-                    "update",
-                    "delete",
-                    "present",
-                    "absent",
-                    "describe",
-                ] or func_name.startswith("test_"):
-                    # These functions are not for tool module
-                    continue
 
+            tool_functions = NamespaceDict(
+                filter(
+                    # It is not a known function for Idem, and it is not a test function.
+                    lambda item: item[0]
+                    not in [
+                        "get",
+                        "list",
+                        "create",
+                        "update",
+                        "delete",
+                        "present",
+                        "absent",
+                        "describe",
+                    ]
+                    and "test_module_type" not in item[1].hardcoded,
+                    plugin.functions.items(),
+                )
+            )
+            for func_name, func_data in tool_functions.items():
                 function_request_format_template_file = (
                     f"{template_dir}/{func_name}.jinja2"
                 )
                 default_request_format_template_file = f"{template_dir}/default.jinja2"
                 if os.path.isfile(function_request_format_template_file):
                     with open(function_request_format_template_file, "rb+") as f:
                         request_format = f.read().decode()
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/init.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,26 @@
             hub.cloudspec.init.run_customize_cloud_spec(ctx, customize_plugin)
     else:
         # Run through all loaded customization. This can support multiple abstracted customization plugins (e.g.
         # state, exec, test etc.) in a generated idem plugin
         for customize_plugin in hub.cloudspec.customize._loaded:
             hub.cloudspec.init.run_customize_cloud_spec(ctx, customize_plugin)
 
+    ctx.cloud_spec = CloudSpec(**ctx.cloud_spec)
+
     for create_plugin in create_plugins:
         try:
             hub.log.info(f"Running create plugin: {create_plugin}")
             hub.cloudspec.create[create_plugin].run(ctx, root_directory)
         except Exception as e:
             hub.log.error(f"Failed to run create plugin: {create_plugin}")
             hub.log.error(e)
-            raise
-    print(f"Total Duration: {timeit.default_timer() - start_time} seconds")
+    print(
+        f"Total time in creating plugins: {timeit.default_timer() - start_time} seconds"
+    )
 
 
 def run_customize_cloud_spec(hub, ctx, cloud_spec_customize_plugin):
     try:
         hub.log.debug(
             f"Running customization with plugin: {cloud_spec_customize_plugin}"
         )
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/example.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/example.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-4.4.1/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/conf.py` & `pop-create-idem-4.4.1/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,29 +121,29 @@
                         "method": "TODO",
                         "path": "TODO",
                         "service_name": ctx.service_name,
                         "resource_name": ref,
                     },
                 }
 
-    if ctx.create_plugin in ["state_modules", "sls"]:
-        for ref in list(plugins):
-            for func_name in list(plugins.get(ref).get("functions", {})):
-                if func_name == "create":
-                    plugins[ref]["functions"]["present"] = (
-                        plugins.get(ref).get("functions", {}).get(func_name)
-                    )
-                elif func_name == "delete":
-                    plugins[ref]["functions"]["absent"] = (
-                        plugins.get(ref).get("functions", {}).get(func_name)
-                    )
-                elif func_name == "list":
-                    plugins[ref]["functions"]["describe"] = (
-                        plugins.get(ref).get("functions", {}).get(func_name)
-                    )
+    # Just add these state modules functions by default
+    for ref in list(plugins):
+        for func_name in list(plugins.get(ref).get("functions", {})):
+            if func_name == "create":
+                plugins[ref]["functions"]["present"] = (
+                    plugins.get(ref).get("functions", {}).get(func_name)
+                )
+            elif func_name == "delete":
+                plugins[ref]["functions"]["absent"] = (
+                    plugins.get(ref).get("functions", {}).get(func_name)
+                )
+            elif func_name == "list":
+                plugins[ref]["functions"]["describe"] = (
+                    plugins.get(ref).get("functions", {}).get(func_name)
+                )
 
     return plugins
 
 
 def add_tests_functions(hub, ctx, plugins):
     for ref in list(plugins):
         functions = plugins[ref].get("functions", {}).copy()
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/params.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 refs = subs + [plugin]
             elif func.get_path():
                 # e.g. "/pets", /pets/{id} -> "pets" become plugin
                 # func.get_path() could look like this "paths./pets/{id}.get
                 # second element is always the actual path itself
                 func_path = func.get_path().split(".")[1]
                 plugin = func_path.lstrip("/").split("/")[0]
-                refs = [plugin]
+                refs = [hub.tool.format.case.snake(plugin)]
 
             if not plugin:
                 raise AttributeError(
                     f"Not sure how to find plugin for {name}. Try using 'tags'"
                 )
 
             # service name is already added in pop-create
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-4.4.1/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/tool/format/case.py` & `pop-create-idem-4.4.1/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-4.4.1/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem/tool/gradle.py` & `pop-create-idem-4.4.1/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-4.4.1/pop_create_idem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.4.0
+Version: 4.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-4.4.0/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-4.4.1/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.4.0/setup.py` & `pop-create-idem-4.4.1/setup.py`

 * *Files identical despite different names*

