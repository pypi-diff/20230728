# Comparing `tmp/pop-create-idem-4.3.1.tar.gz` & `tmp/pop-create-idem-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-4.3.1.tar", last modified: Fri Jul 14 11:53:04 2023, max compression
+gzip compressed data, was "pop-create-idem-4.4.0.tar", last modified: Fri Jul 28 19:02:37 2023, max compression
```

## Comparing `pop-create-idem-4.3.1.tar` & `pop-create-idem-4.4.0.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3396 2023-07-14 11:53:04.111538 pop-create-idem-4.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8621 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/sls.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/customize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/customize/contracts/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/customize/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2048 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/example.py
--rw-r--r--   0 root         (0) root         (0)     2167 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     6216 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3463 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/test.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     2209 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     4724 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5537 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)     1348 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1408 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1902 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4300 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
--rw-r--r--   0 root         (0) root         (0)     1152 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1234 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      819 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
--rw-r--r--   0 root         (0) root         (0)      456 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.099538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2805 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.107538 pop-create-idem-4.3.1/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-14 11:53:03.000000 pop-create-idem-4.3.1/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:53:04.103538 pop-create-idem-4.3.1/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3396 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8423 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-14 11:53:04.000000 pop-create-idem-4.3.1/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 11:53:04.111538 pop-create-idem-4.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3006 2023-07-14 11:52:49.000000 pop-create-idem-4.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8799 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     4041 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/sls.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/contracts/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/customize/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/example.py
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/test.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/absent/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/example/present/init.sls
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/exec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.764050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2
+-rw-r--r--   0 root         (0) root         (0)      539 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      819 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/
+-rw-r--r--   0 root         (0) root         (0)      456 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 19:02:37.760050 pop-create-idem-4.4.0/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-28 19:02:37.000000 pop-create-idem-4.4.0/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 19:02:37.768050 pop-create-idem-4.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-07-28 19:02:22.000000 pop-create-idem-4.4.0/setup.py
```

### Comparing `pop-create-idem-4.3.1/LICENSE` & `pop-create-idem-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/PKG-INFO` & `pop-create-idem-4.4.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,108 @@
-Metadata-Version: 2.1
-Name: pop-create-idem
-Version: 4.3.1
-Summary: UNKNOWN
-Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
-Author: Tyler Johnson
-Author-email: tyjohnson@vmware.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-======
-README
-======
-
-It is recommended to use a python virtualenv when creating a new Idem provider
-plugin. We'll give some instructions below, but feel free to use what
-environment tool you're comfortable with.
+===============
+pop-create-idem
+===============
 
-Create a virtual env
-++++++++++++++++++++
+Project description
++++++++++++++++++++
+
+`pop-create-idem` is an extension of `pop-create` that creates boilerplate code for new `idem-cloud` projects. `pop-create-idem` includes code that transforms a CloudSpec dictionary into idem states, tools, and exec modules. Your unique `pop_create` plugin's purpose is to convert API documentation into the CloudSpec format.
+
+**Note**: It is recommended that you use a Python virtual environment when creating a new Idem provider plugin.
+
+Create a virtual environment
+++++++++++++++++++++++++++++
 
-.. warning::
+Before you start, ensure that you installed Python 3.8 or later. If you are running 3.7 or earlier, you might need to use `python3` instead of `python` in the commands in the rest of this tutorial.
 
-   Ensure you have Python 3.8 or later available. You're good if running the
-   command `python -V` displays a version of Python 3.8 or newer. Otherwise you
-   might need to use `python3` instead of `python` in the commands in the rest
-   of this tutorial.
+To verify your Python version, run the following command:
+
+.. code-block:: bash
+
+    python -V
+
+Next, create your virtual environment:
 
 .. code-block:: bash
 
     python -m venv env
     source env/bin/activate
 
-Now you should be in your new python virtualenv.
+Now you should be in your new Python virtual environment.
+
+Update pip
+++++++++++
 
-Let's update to the latest pip inside our virtual env:
+Next, update to the latest version of `pip` inside your virtual environment:
 
 .. code-block:: bash
 
     pip install -U pip
 
 
-Install Dependencies
+Install dependencies
 ++++++++++++++++++++
 
-Now we're going to install "pop-create".
+Next, you need to install `pop-create`:
 
 .. code-block:: bash
 
     pip install pop-create
 
 
-You now have access to the `pop-create` command for creating idem plugins.
+You now have access to the `pop-create` command for creating Idem plugins.
 
+Install `pop-create-idem`
++++++++++++++++++++++++++
 
-Installation
-++++++++++++
-Install `pop-create-idem` with pip from project root:
+Install `pop-create-idem` with `pip` from the project root:
 
 .. code-block:: bash
 
     pip install -e {project_root}
 
-Install `pop-create-idem` with pip from PyPi:
+Next, install `pop-create-idem` with `pip` from PyPi:
 
 .. code-block:: bash
 
     pip install pop-create-idem
 
 
-Generating Idem Cloud Plugin
-++++++++++++++++++++++++++++
+Generate an Idem Cloud plugin
++++++++++++++++++++++++++++++
 
-To generate a new skeleton Idem cloud plugin, run:
+To generate a new skeleton Idem Cloud plugin, run the following command:
 
 .. code-block:: bash
 
     pop-create idem-cloud --directory /path/to/new/project --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-A new project will have been created with all the necessary directory structure to get started with Idem cloud plugin.
+This command creates a new project with the directory structure needed to get started with your plugin.
+
+Generate an Idem plugin with a Swagger specification
+====================================================
 
-To generate a new idem plugin project with swagger specification, run:
+To generate a new Idem plugin with a Swagger specification, run the following command:
 
 .. code-block:: bash
 
     pop-create swagger --directory /path/to/new/project --specification={swagger-spec-yaml-or-accessible-swagger-spec-json-url} --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-To generate a new Idem plugin project with openapi3 specification, run:
+Generate an Idem plugin with an OpenAPI3 specification
+======================================================
+
+To generate a new Idem plugin project with an OpenAPI3 specification, run the following command:
 
 .. code-block:: bash
 
     pop-create openapi3 --directory /path/to/new/project --specification={openapi3-spec-yaml-or-accessible-openapi3-spec-json-url} --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-A new project will have been created with all the boilerplate code needed to get started with respective provider.
-
-.. important::
-
-    Look under quickstart tutorial guide for generating and configuring Idem Cloud plugin for your provider.
 
-.. note::
+This command creates a new project with the boilerplate code needed to get started with each respective cloud provider.
 
-    There is a swagger petstore example under tutorial which walks through generated Idem plugin
-    with a sample petstore swagger.
+Next steps
+++++++++++
 
+After you generate your Idem plugin:
 
+* Try the example Swagger petstore tutorial in the `tutorial` directory, which walks you through generating an Idem plugin with a Swagger specification.
+* Configure the plugin for your provider. See the `pop-create-idem` quickstart for instructions.
```

### Comparing `pop-create-idem-4.3.1/cloudspec/__init__.py` & `pop-create-idem-4.4.0/cloudspec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,26 +212,28 @@
             cls_name="CloudSpecMember",
             fields=[("name", str), ("params", Dict[str, "CloudSpecParam"])],
         ) = None,
         param_type: str = None,
         doc: str = "",
         default: Any = None,
         snaked: str = None,
+        exclude_from_example: bool = False,
     ):
         """
         Args:
             name: Name of the parameter
             doc: Docstring for the parameter
             required: "True|False"
             target: "query|data|path|sdk-class|sdk-subclass|function-call"
             target_type: "mapping|format_str|arg|kwargs"
             param_type: A type hint for this parameter
             member: Nested member params
             default: The default value for this parameter if it is not required
             snaked: Snake case representation of the parameter name to be used, would override generated one
+            exclude_from_example: Exclude parameter from the generated example
         """
         # If the target_type is "mapping" the target is the name of a dictionary variable
         # If the target_type is "arg" or "kwargs" the target is the name of callable this param should forwarded to
         # If the target_type is "value" then it is directly dropped in and it is included in the function parameters
         if target_type not in ("mapping", "value", "arg", "kwargs"):
             raise TypeError(f"Invalid target type: {target_type}")
 
@@ -258,8 +260,9 @@
             snaked=snaked,
             param_type=param_type,
             required=required,
             default=default,
             target_type=target_type,
             member=member,
             target=target,
+            exclude_from_example=exclude_from_example,
         )
```

### Comparing `pop-create-idem-4.3.1/cloudspec/conf.py` & `pop-create-idem-4.4.0/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os.path
 import pathlib
 
 import tqdm
 
 from cloudspec import CloudSpec
 
+HEADER_TEMPLATE = "Exec module for managing {}."
+
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     exec_dir = root_directory / ctx.clean_name / "exec" / ctx.service_name
     template_dir = (
@@ -19,29 +21,37 @@
         / "templates"
         / "exec"
     )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
+        resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
+        resource_header = HEADER_TEMPLATE.format(
+            hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
+        )
 
         plugin["func_alias"] = {"list_": "list"}
         if not plugin.get("contracts"):
             # plugin["contracts"] = ["auto_state", "soft_fail"]
             # At the moment, we do not fully support auto_state
             plugin["contracts"] = ["soft_fail"]
 
         exec_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
 
         # Set up the base template
         if not plugin.functions:
-            to_write = hub.cloudspec.parse.plugin.header(plugin)
+            to_write = hub.cloudspec.parse.plugin.header(
+                plugin=plugin, resource_header=resource_header
+            )
 
         else:
-            to_write = hub.cloudspec.parse.plugin.header(plugin)
+            to_write = hub.cloudspec.parse.plugin.header(
+                plugin=plugin, resource_header=resource_header
+            )
             mod_file.write_text(to_write)
             func_data = hub.cloudspec.parse.function.parse(
                 plugin.functions, targets=("get", "list", "create", "update", "delete")
             )
 
             present_parameter = {}
             if plugin.functions.get("create"):
@@ -67,18 +77,24 @@
                             request_format = f.read().decode()
                     else:
                         request_format = cloud_spec.request_format.get(function_name)
 
                     template_str = f"{base_template}\n    {request_format}\n\n\n"
                     template = hub.tool.jinja.template(template_str)
 
-                    to_write += template.render(
-                        service_name=cloud_spec.service_name,
-                        function=dict(
-                            ref=ref,
-                            exec_ref=f"exec.{exec_ref}",
-                            **func_data[function_name]["function"],
-                        ),
-                        parameter=func_data[function_name]["parameter"],
-                        present_parameter=present_parameter,
-                    )
+                    try:
+                        to_write += template.render(
+                            service_name=cloud_spec.service_name,
+                            function=dict(
+                                ref=ref,
+                                exec_ref=f"exec.{exec_ref}",
+                                **func_data[function_name]["function"],
+                            ),
+                            parameter=func_data[function_name]["parameter"],
+                            present_parameter=present_parameter,
+                        )
+                    except Exception as err:
+                        hub.log.error(
+                            f"Failed to generate resource {resource_ref} function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                        )
+
         mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pathlib
 
 from cloudspec import CloudSpec
 
+HEADER_TEMPLATE = "Exec module for managing {}."
+
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     exec_dir = root_directory / ctx.clean_name / "exec" / ctx.service_name
     template_dir = (
@@ -18,18 +20,24 @@
         / "exec"
     )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(exec_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         cli_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
+        resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
+        resource_header = HEADER_TEMPLATE.format(
+            hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
+        )
 
         plugin["func_alias"] = {"list_": "list"}
 
-        to_write = hub.cloudspec.parse.plugin.header(plugin)
+        to_write = hub.cloudspec.parse.plugin.header(
+            plugin=plugin, resource_header=resource_header
+        )
 
         for function_name, function_data in plugin.functions.items():
             if function_name in ["present", "absent", "describe"]:
                 # If plugin comes in with all methods, let's not create for state_modules functions
                 continue
 
             request_format_template_file = f"{template_dir}/{function_name}.jinja2"
@@ -64,12 +72,12 @@
                         return_type=function_data.return_type,
                     ),
                     parameter=dict(
                         mapping=hub.cloudspec.parse.param.mappings(function_data.params)
                     ),
                 )
             except Exception as err:
-                hub.log.warning(
-                    f"Warning when generating function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                hub.log.error(
+                    f"Failed to generate resource {resource_ref} function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
                 )
 
         mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/sls.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/sls.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     for ref, plugin in cloud_spec.plugins.items():
         for function_name in ["present", "absent"]:
             func_data = plugin.functions.get(function_name)
 
             if func_data is None:
                 continue
 
-            sls_file = root_directory / "example" / function_name / f"{ref}.sls"
+            path = root_directory / "example" / function_name
+            sls_file = hub.cloudspec.parse.plugin.touch(
+                root=path, ref=ref, is_test=False, is_sls=True
+            )
             hub.tool.path.touch(sls_file)
             example_request_syntax_output = (
                 hub.cloudspec.parse.example.state_request_syntax(
                     resource_name=ref,
                     ref=hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin),
                     func_name=function_name,
                     params=func_data.params,
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pathlib
 
 from cloudspec import CloudSpec
 
+HEADER_TEMPLATE = "States module for managing {}."
+
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     states_dir = root_directory / ctx.clean_name / "states" / ctx.service_name
     template_dir = (
@@ -18,18 +20,24 @@
         / "state"
     )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(states_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         state_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
+        resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
+        resource_header = HEADER_TEMPLATE.format(
+            hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
+        )
 
         plugin["contracts"] = ["resource"]
 
-        to_write = hub.cloudspec.parse.plugin.header(plugin)
+        to_write = hub.cloudspec.parse.plugin.header(
+            plugin=plugin, resource_header=resource_header
+        )
         if not plugin.functions:
             mod_file.write_text(to_write)
             continue
         func_data = hub.cloudspec.parse.function.parse(
             plugin.functions, targets=("present", "absent", "describe")
         )
 
@@ -89,12 +97,12 @@
                             example_request_syntax=example_request_syntax,
                         ),
                         parameter=func_data[function_name]["parameter"],
                         present_parameter=present_parameter,
                         get_params=common_params,
                     )
                 except Exception as err:
-                    hub.log.warning(
-                        f"Warning when generating function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                    hub.log.error(
+                        f"Failed to generate resource {resource_ref} function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
                     )
 
                 mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import os
 import pathlib
 
 from cloudspec import CloudSpec
 from cloudspec import CloudSpecParam
 
+HEADER_TEMPLATE = "Tests for validating {}."
+
 
 def run(hub, ctx, root_directory: pathlib.Path or str):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
 
     for ref, plugin in cloud_spec.plugins.items():
+        resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
+        resource_header = HEADER_TEMPLATE.format(
+            hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
+        )
+
         plugin["imports"] = ["import pytest"]
 
         for test_type in ["exec", "states", "tool"]:
             test_dir = (
                 root_directory
                 / "tests"
                 / "integration"
@@ -49,15 +56,17 @@
             if test_type in ["states", "exec"]:
                 # Add default global parameter for tracking a resource being created inside test
                 # This helps in clean up of a created resource in test
                 plugin["file_vars"]["PARAMETER"] = {
                     "name": "idem-test-resource- + TODO: Add unique identifier generator",
                 }
 
-            to_write = hub.cloudspec.parse.plugin.header(plugin)
+            to_write = hub.cloudspec.parse.plugin.header(
+                plugin=plugin, resource_header=resource_header
+            )
 
             # Collect get_call_params beforehand from the list
             # This is helpful when a test method wants to call into GET after any operation in a test
             get_call_params = None
             test_get_func = [
                 value for key, value in plugin.functions.items() if key == "test_get"
             ]
@@ -120,11 +129,12 @@
                                 get_call_params
                             )
                             if get_call_params is not None
                             else "",
                         },
                     )
                 except Exception as err:
-                    hub.log.warning(
-                        f"Warning when generating function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
+                    hub.log.error(
+                        f"Failed to generate resource {resource_ref} function's action definitions for {function_name}: {err.__class__.__name__}: {err}"
                     )
+
             mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/create/tool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import pathlib
 
 import tqdm
 
 from cloudspec import CloudSpec
 
+HEADER_TEMPLATE = "Utility functions for {}."
+
 
 def run(hub, ctx, root_directory: pathlib.Path):
     if isinstance(root_directory, str):
         root_directory = pathlib.Path(root_directory)
     cloud_spec = CloudSpec(**ctx.cloud_spec)
     tool_dir = root_directory / ctx.clean_name / "tool" / ctx.service_name
     template_dir = (
@@ -20,20 +22,28 @@
         / "tool"
     )
 
     for ref, plugin in cloud_spec.plugins.items():
         mod_file = hub.cloudspec.parse.plugin.touch(tool_dir, ref)
         ref = hub.cloudspec.parse.plugin.ref(ctx, ref)
         module_ref = hub.cloudspec.parse.plugin.mod_ref(ctx, ref, plugin)
+        resource_ref = hub.cloudspec.parse.plugin.resource_ref(ctx, ref)
+        resource_header = HEADER_TEMPLATE.format(
+            hub.tool.format.inflect.ENGINE.plural_noun(resource_ref)
+        )
 
         # Set up the base template
         if not plugin.functions:
-            to_write = hub.cloudspec.parse.plugin.header(plugin)
+            to_write = hub.cloudspec.parse.plugin.header(
+                plugin=plugin, resource_header=resource_header
+            )
         else:
-            to_write = hub.cloudspec.parse.plugin.header(plugin)
+            to_write = hub.cloudspec.parse.plugin.header(
+                plugin=plugin, resource_header=resource_header
+            )
             for func_name, func_data in tqdm.tqdm(
                 plugin.functions.items(), desc=f"{ref} tool functions"
             ):
                 if func_name in [
                     "get",
                     "list",
                     "create",
@@ -76,12 +86,12 @@
                             ),
                         ),
                         parameter=dict(
                             mapping=hub.cloudspec.parse.param.mappings(func_data.params)
                         ),
                     )
                 except Exception as err:
-                    hub.log.warning(
-                        f"Warning when generating function's action definitions for {func_name}: {err.__class__.__name__}: {err}"
+                    hub.log.error(
+                        f"Failed to generate resource {resource_ref} function's action definitions for {func_name}: {err.__class__.__name__}: {err}"
                     )
 
         mod_file.write_text(to_write)
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/init.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/example.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
     return _display(request_syntax)
 
 
 def extract_params(hub, params: dict):
     result = {}
     for name, param in params.items():
+        if param.get("exclude_from_example"):
+            continue
+
         snaked = param.get("snaked")
         param_type = param.get("param_type")
         if param_type == "str":
             param_type = "string"
 
         if param.get("member", None):
             if param_type == "List[{}]":
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/param.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,54 +7,67 @@
     """
     Get the sphinx docs for the parameters
     """
     if not parameters:
         return ""
 
     ret = "\n    Args:\n"
-    for param in parameters.values():
-        ret += f"        {param.snaked}"
-        # Doc strings standard is lower case list[]
-        if param.param_type is None:
-            param_type = None
-        else:
-            param_type = param.param_type.replace("List[", "list[")
-        if param.member:
-            # Complex params are represented as Dict[str, Any] in the sphinx docs
-            param_type = param_type.format("Dict[str, Any]")
-
-        if param_type:
-            ret += f"({param_type}{', optional' if not param.required else ''})"
-
-        ret += f": {param.doc}"
-        if not ret.endswith("."):
-            ret += "."
-        if not param.required:
-            ret += f" Defaults to {param.default}."
 
-        ret += nested_params_docs(param, "            ")
-        ret += "\n"
+    # Add required params first
+    for name, data in parameters.items():
+        if data["required"]:
+            ret += add_param_to_sphynx_doc(data)
+
+    # Add not required params after
+    for name, data in parameters.items():
+        if not data["required"]:
+            ret += add_param_to_sphynx_doc(data)
 
     return ret.rstrip()
 
 
+def add_param_to_sphynx_doc(param: CloudSpecParam):
+    ret = f"        {param.snaked}"
+    # Doc strings standard is lower case list[]
+    if param.param_type is None:
+        param_type = None
+    else:
+        param_type = param.param_type.replace("list[", "list[")
+    if param.member:
+        # Complex params are represented as Dict[str, Any] in the sphinx docs
+        param_type = param_type.format("dict[str, Any]")
+
+    if param_type:
+        ret += f"({param_type}{', Optional' if not param.required else ''})"
+
+    ret += f": {param.doc}"
+    if not ret.endswith("."):
+        ret += "."
+    if not param.required:
+        ret += f" Defaults to {param.default}."
+
+    ret += nested_params_docs(param, "            ")
+    ret += "\n\n"
+    return ret
+
+
 def nested_params_docs(param: CloudSpecParam, offset: str):
     """
     Get the sphinx docs for the nested parameters
     """
     ret = ""
     if param.member:
         for nested_param_name, nested_param_data in param.member.params.items():
             # Doc strings standard is lower case list[]
-            param_type = nested_param_data.param_type.replace("List[", "list[")
+            param_type = nested_param_data.param_type.replace("list[", "list[")
             if nested_param_data.member:
                 # This is the next level of nested complex argument.
-                param_type = param_type.format("Dict[str, Any]")
-            ret += f"\n{offset}* "
-            ret += f"{nested_param_name} ({param_type}{', optional' if not nested_param_data.required else ''}): {nested_param_data.doc}"
+                param_type = param_type.format("dict[str, Any]")
+            ret += f"\n\n{offset}* "
+            ret += f"{nested_param_name} ({param_type}{', Optional' if not nested_param_data.required else ''}): {nested_param_data.doc}"
 
             # Recursively add doc for all nested complex arguments
             ret += nested_params_docs(nested_param_data, offset + "    ")
     return ret
 
 
 def headers(hub, parameters: CloudSpecParam) -> str:
@@ -135,16 +148,20 @@
     if param_data.member:
         # Recursively add all nested complex arguments
         ret += param_data.param_type.format(
             add_nested_param_to_header(param_data.member, offset + "    ")
         )
     else:
         ret += f"{param_data.param_type}"
+
     if param_data["required"]:
         ret += f"), "
+    elif param_data.param_type == "int" and param_data.default == 0:
+        # Since idem 23.0.3 the default values are populated automatically and value of 0 may fail.
+        ret += f", field(default=None)), "
     else:
         ret += f", field(default={param_data.default})), "
 
     return ret
 
 
 def required_call_params(hub, parameters: CloudSpecParam) -> str:
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,47 +2,59 @@
 Functions for processing plugins
 """
 import pathlib
 
 from cloudspec import CloudSpecPlugin
 
 
-def header(hub, plugin: CloudSpecPlugin) -> str:
+def header(hub, plugin: CloudSpecPlugin, resource_header: str) -> str:
     """
     Initialize the render of a plugin file and return the template
     """
     # noinspection JinjaAutoinspect
     template = hub.tool.jinja.template(hub.cloudspec.template.plugin.HEADER)
 
-    return template.render(plugin=plugin)
+    return template.render(plugin=plugin, resource_header=resource_header)
 
 
 def ref(hub, ctx, ref: str) -> str:
     split = ref.split(".")
     subs = split[:-1]
     mod = split[-1]
     return ".".join([ctx.service_name] + subs + [mod])
 
 
+def resource_ref(hub, ctx, ref: str) -> str:
+    split = ref.split(".")
+    r_ref = split[-1]
+    return r_ref
+
+
 def mod_ref(hub, ctx, ref: str, plugin: CloudSpecPlugin) -> str:
     split = ref.split(".")
     subs = split[:-1]
     mod = split[-1]
     return ".".join([ctx.service_name] + subs + [plugin.virtualname or mod])
 
 
-def touch(hub, root: pathlib.Path, ref: str, is_test: bool = False):
+def touch(
+    hub, root: pathlib.Path, ref: str, is_test: bool = False, is_sls: bool = False
+):
     """
     Create all the files underneath the new sub
     """
     split = ref.split(".")
     subs = split[:-1]
     mod = split[-1]
 
     if is_test:
         mod = f"test_{mod}"
 
     for sub in subs:
         root = root / sub
-    root = root / f"{mod}.py"
+
+    if is_sls:
+        root = root / f"{mod}.sls"
+    else:
+        root = root / f"{mod}.py"
     hub.tool.path.touch(root)
     return root
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 CREATE = """
-async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
+async def {{function.name}}(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
-
-        Resource State:
+        Using in a state:
 
         .. code-block:: sls
 
             resource_is_present:
               {{ function.ref }}.present:
                 - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
 
@@ -18,21 +15,18 @@
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 UPDATE = """
-async def {{function.name}}(hub, ctx, resource_id: str{{function.header_params}}, name: str = None, **kwargs) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
+async def {{function.name}}(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
-
-        Resource State:
+        Using in a state:
 
         .. code-block:: sls
 
             resource_is_present:
               {{ function.ref }}.present:
                 - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
 
@@ -42,20 +36,17 @@
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 
 DELETE = """
-async def {{function.name}}(hub, ctx, resource_id: str{{function.header_params}}, name: str = None) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
+async def {{function.name}}(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
-
         Resource State:
 
         .. code-block:: sls
 
             resource_is_absent:
               {{ function.ref }}.absent:
                 - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
@@ -65,22 +56,18 @@
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 GET = """
-async def {{function.name}}(hub, ctx{{function.header_params}}, name: str = None, resource_id: str = None) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
-
+async def {{function.name}}(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
-
-        Unmanaged Resource State:
+        Resource State:
 
         .. code-block:: sls
 
             unmanaged_resource:
               exec.run:
                 - path: {{ function.ref }}.{{ function.name }}
                 - kwargs:
@@ -92,20 +79,18 @@
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
     '''
 """
 
 LIST = """
 async def list_(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
-        Unmanaged Resource State:
+        Resource State:
 
         .. code-block:: sls
 
             unmanaged_resources:
               exec.run:
                 - path: {{ function.ref }}.{{ function.name }}
                 - kwargs:
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/exec.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 FUNCTION = """
-async def {{function.name}}(hub, ctx{{function.header_params}})  -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
+async def {{function.name}}(hub, ctx{{function.header_params}}) -> Dict[str, Any]:
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
     Examples:
 
         .. code-block:: bash
 
             idem exec {{ function.ref }}.{{ function.name }} {{ function.required_call_params }}
 
         .. code-block:: python
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """
 Templates for plugins
 """
 
 HEADER = '''
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-{{ plugin.doc }}
-"""
+"""{{ resource_header }} {{ plugin.doc }}"""
 
 {% if plugin.imports -%}
 {{ plugin.imports|join('\n') }}
 {%- endif %}
 
 {% if plugin.virtual_imports -%}
 try:
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-4.4.0/pop_create_idem/cloudspec/template/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 """
 Templates for state modules
 """
 
 PRESENT_FUNCTION = """
 async def {{function.name}}(
     hub,
-    ctx,
-    name: str
+    ctx
     {% if function.header_params %}
         {{function.header_params}}
     {% endif -%},
-    resource_id: str = None,
-    **kwargs
 ) -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
-    {{function.doc|replace("'" * 3, '"' * 3)}}
-    Request Syntax:
-
+    '''{{function.doc|replace("'" * 3, '"' * 3)}}
+    Example:
         .. code-block:: sls
 
-            {% if function.example_request_syntax %}
-            {{ function.example_request_syntax|indent(12) }}
-            {% else %}
-                resource_is_{{function.name}}:
-                  {{ function.ref }}.{{ function.name }}:
-                    - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
-            {% endif %}
+          {% if function.example_request_syntax %}
+          {{ function.example_request_syntax|indent(12) }}
+          {% else %}
+              resource_is_{{function.name}}:
+                {{ function.ref }}.{{ function.name }}:
+                  - {{ function.required_call_params.split(", ")|join("\n                  - ")|replace("=", ": ") }}
+          {% endif %}
     '''
 """
 
 ABSENT_FUNCTION = """
 async def {{function.name}}(
     hub,
-    ctx,
-    name: str
+    ctx
     {% if function.header_params %}
         {{function.header_params}}
     {% endif -%},
-    resource_id: str = None,
-    **kwargs
 )  -> Dict[str, Any]:
-    r'''
-    **Autogenerated function**
+    '''
     {{function.doc|replace("'" * 3, '"' * 3)}}
-    Request Syntax:
-
+    Example:
         .. code-block:: sls
 
             {% if function.example_request_syntax %}
             {{ function.example_request_syntax|indent(12) }}
             {% else %}
                 resource_is_{{function.name}}:
                   {{ function.ref }}.{{ function.name }}:
-                    - {{ function.required_call_params.split(", ")|join("\n                - ")|replace("=", ": ") }}
+                    - name: value
+                    - resource_id: value
             {% endif %}
     '''
 """
 
 DESCRIBE_FUNCTION = """
 async def {{function.name}}(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r'''
-    **Autogenerated function**
-
+    '''
     Describe the resource in a way that can be recreated/managed with the corresponding "present" function
 
     {{function.doc|replace("'" * 3, '"' * 3)}}
-    Examples:
+    Example:
 
         .. code-block:: bash
 
             $ idem describe {{ function.ref }}
     '''
 """
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/conf.py` & `pop-create-idem-4.4.0/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files 25% similar despite different names*

```diff
@@ -45,8 +45,15 @@
             )
 
         ctx.has_acct_plugin = bool(ctx.acct_plugin)
         if not ctx.has_acct_plugin:
             # Create auth plugins
             ctx.acct_plugin = ctx.service_name
 
+    # sphynx docs generation related settings
+    ctx["docs_modindex_common_prefix"] = [
+        f"{ctx['clean_name']}.states.{ctx['service_name']}",
+        f"{ctx['clean_name']}.exec.{ctx['service_name']}",
+    ]
+    ctx["docs_autogen_config"] = ["exec/", "states/"]
+
     return ctx
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/cloudspec/customize/{{cookiecutter.service_name}}.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     hub.tool.path.delete(
         root_directory / ctx.clean_name / "exec" / ctx.service_name / "sample.py"
     )
     hub.tool.path.delete(
         root_directory / ctx.clean_name / "states" / ctx.service_name / "sample.py"
     )
     hub.tool.path.delete(
+        root_directory / "docs" / "ref" / "exec" / ctx.service_name / "sample.rst"
+    )
+    hub.tool.path.delete(
+        root_directory / "docs" / "ref" / "states" / ctx.service_name / "sample.rst"
+    )
+    hub.tool.path.delete(
         root_directory
         / ctx.clean_name
         / "autogen"
         / ctx.service_name
         / "templates"
         / "sample.jinja2"
     )
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/params.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {# templates/create.jinja2 #}
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     # TODO: Change request param mapping as necessary
     resource_to_raw_input_mapping = {{ function.hardcoded.request_mappings|default("{}", true) }}
 
     payload = {}
     for key, value in desired_state.items():
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {# templates/update.jinja2 #}
     result = dict(comment=[], ret=[], result=True)
 
     desired_state = {
         k: v
         for k, v in locals().items()
-        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+        if k not in ("hub", "ctx", "result") and v is not None
     }
 
     # TODO: Change request param mapping as necessary
     resource_to_raw_input_mapping = {{ function.hardcoded.request_mappings|default("{}", true) }}
 
     payload = {}
     for key, value in desired_state.items():
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,17 @@
             comment=[], old_state={}, new_state={}, name=name, result=True, rerun_data=None
         )
 
     if not resource_id:
         resource_id = (ctx.old_state or {}).get("resource_id")
 
     if not resource_id:
-        result["comment"].append(f"'{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}' already absent")
+        result["comment"].append(f"'{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}' already absent")
         return result
 
-    # Remove resource_id from kwargs to avoid duplicate argument
     before = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.get(
         ctx,
         name=name,
         resource_id=resource_id,
     )
 
     if before["ret"]:
@@ -28,15 +27,15 @@
             resource_id=resource_id,
         )
         result["result"] = delete_ret["result"]
 
         if result["result"]:
             result["comment"].append(f"Deleted {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}")
         else:
-            # If there is any failure in create/update, it should reconcile.
+            # If there is any failure in delete, it should reconcile.
             # The type of data is less important here to use default reconciliation
             # If there are no changes for 3 runs with rerun_data, then it will come out of execution
             result["rerun_data"] = resource_id
             result["comment"].append(delete_ret["result"])
     else:
         result["comment"].append(f"{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name} already absent")
         return result
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,32 @@
         if not before["result"] or not before["ret"]:
             result["result"] = False
             result["comment"] = before["comment"]
             return result
 
         result["old_state"] = before.ret
 
-        result["comment"].append(f"'{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}:{name}' already exists")
+        result["comment"].append(f"'{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}' already exists")
 
         # If there are changes in desired state from existing state
         changes = differ.deep_diff(before.ret if before.ret else {}, desired_state)
 
         if bool(changes.get("new")):
             if ctx.test:
                 result["new_state"] = hub.tool.{{ function.hardcoded.service_name }}.test_state_utils.generate_test_state(
                     enforced_state={},
                     desired_state=desired_state
                 )
-                result["comment"] = (f"Would update {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}",)
+                result["comment"].append(f"Would update {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}")
                 return result
             else:
                 # Update the resource
                 update_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.update(
                     ctx,
-                    name=name,
-                    resource_id=resource_id,
-                    **kwargs,
-                    # TODO: Add other required parameters (including tags, if necessary): **{{ parameter.mapping.kwargs|default({}) }}
+                    **{{ parameter.mapping.kwargs|default({}) }}
                 )
                 result["result"] = update_ret["result"]
 
                 if result["result"]:
                     result["comment"].append(f"Updated '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}'")
                 else:
                     result["comment"].append(update_ret["comment"])
@@ -59,17 +56,15 @@
                 desired_state=desired_state
             )
             result["comment"] = (f"Would create {{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}",)
             return result
         else:
             create_ret = await hub.exec.{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}.create(
                 ctx,
-                name=name,
-                **kwargs
-                # TODO: Add other required parameters from: **{{ parameter.mapping.kwargs|default({})}}
+                **{{ parameter.mapping.kwargs|default({})}}
             )
             result["result"] = create_ret["result"]
 
             if result["result"]:
                 result["comment"].append(f"Created '{{ function.hardcoded.service_name }}.{{ function.hardcoded.resource_name }}: {name}'")
                 resource_id = create_ret["ret"]["resource_id"]
                 # Safeguard for any future errors so that the resource_id is saved in the ESM
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_create.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/exec/test_update.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tests/states/test_present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-4.4.0/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/tool/format/case.py` & `pop-create-idem-4.4.0/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-4.4.0/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem/tool/gradle.py` & `pop-create-idem-4.4.0/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-4.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 4.3.1
+Version: 4.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -18,102 +18,117 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-======
-README
-======
-
-It is recommended to use a python virtualenv when creating a new Idem provider
-plugin. We'll give some instructions below, but feel free to use what
-environment tool you're comfortable with.
+===============
+pop-create-idem
+===============
 
-Create a virtual env
-++++++++++++++++++++
+Project description
++++++++++++++++++++
+
+`pop-create-idem` is an extension of `pop-create` that creates boilerplate code for new `idem-cloud` projects. `pop-create-idem` includes code that transforms a CloudSpec dictionary into idem states, tools, and exec modules. Your unique `pop_create` plugin's purpose is to convert API documentation into the CloudSpec format.
 
-.. warning::
+**Note**: It is recommended that you use a Python virtual environment when creating a new Idem provider plugin.
+
+Create a virtual environment
+++++++++++++++++++++++++++++
 
-   Ensure you have Python 3.8 or later available. You're good if running the
-   command `python -V` displays a version of Python 3.8 or newer. Otherwise you
-   might need to use `python3` instead of `python` in the commands in the rest
-   of this tutorial.
+Before you start, ensure that you installed Python 3.8 or later. If you are running 3.7 or earlier, you might need to use `python3` instead of `python` in the commands in the rest of this tutorial.
+
+To verify your Python version, run the following command:
+
+.. code-block:: bash
+
+    python -V
+
+Next, create your virtual environment:
 
 .. code-block:: bash
 
     python -m venv env
     source env/bin/activate
 
-Now you should be in your new python virtualenv.
+Now you should be in your new Python virtual environment.
+
+Update pip
+++++++++++
 
-Let's update to the latest pip inside our virtual env:
+Next, update to the latest version of `pip` inside your virtual environment:
 
 .. code-block:: bash
 
     pip install -U pip
 
 
-Install Dependencies
+Install dependencies
 ++++++++++++++++++++
 
-Now we're going to install "pop-create".
+Next, you need to install `pop-create`:
 
 .. code-block:: bash
 
     pip install pop-create
 
 
-You now have access to the `pop-create` command for creating idem plugins.
+You now have access to the `pop-create` command for creating Idem plugins.
 
+Install `pop-create-idem`
++++++++++++++++++++++++++
 
-Installation
-++++++++++++
-Install `pop-create-idem` with pip from project root:
+Install `pop-create-idem` with `pip` from the project root:
 
 .. code-block:: bash
 
     pip install -e {project_root}
 
-Install `pop-create-idem` with pip from PyPi:
+Next, install `pop-create-idem` with `pip` from PyPi:
 
 .. code-block:: bash
 
     pip install pop-create-idem
 
 
-Generating Idem Cloud Plugin
-++++++++++++++++++++++++++++
+Generate an Idem Cloud plugin
++++++++++++++++++++++++++++++
 
-To generate a new skeleton Idem cloud plugin, run:
+To generate a new skeleton Idem Cloud plugin, run the following command:
 
 .. code-block:: bash
 
     pop-create idem-cloud --directory /path/to/new/project --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-A new project will have been created with all the necessary directory structure to get started with Idem cloud plugin.
+This command creates a new project with the directory structure needed to get started with your plugin.
+
+Generate an Idem plugin with a Swagger specification
+====================================================
 
-To generate a new idem plugin project with swagger specification, run:
+To generate a new Idem plugin with a Swagger specification, run the following command:
 
 .. code-block:: bash
 
     pop-create swagger --directory /path/to/new/project --specification={swagger-spec-yaml-or-accessible-swagger-spec-json-url} --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-To generate a new Idem plugin project with openapi3 specification, run:
+Generate an Idem plugin with an OpenAPI3 specification
+======================================================
+
+To generate a new Idem plugin project with an OpenAPI3 specification, run the following command:
 
 .. code-block:: bash
 
     pop-create openapi3 --directory /path/to/new/project --specification={openapi3-spec-yaml-or-accessible-openapi3-spec-json-url} --project-name=idem-{my_cloud} --simple_cloud_name={my_cloud}
 
-A new project will have been created with all the boilerplate code needed to get started with respective provider.
 
-.. important::
+This command creates a new project with the boilerplate code needed to get started with each respective cloud provider.
 
-    Look under quickstart tutorial guide for generating and configuring Idem Cloud plugin for your provider.
+Next steps
+++++++++++
 
-.. note::
+After you generate your Idem plugin:
 
-    There is a swagger petstore example under tutorial which walks through generated Idem plugin
-    with a sample petstore swagger.
+* Try the example Swagger petstore tutorial in the `tutorial` directory, which walks you through generating an Idem plugin with a Swagger specification.
+* Configure the plugin for your provider. See the `pop-create-idem` quickstart for instructions.
```

### Comparing `pop-create-idem-4.3.1/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-4.4.0/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-4.3.1/setup.py` & `pop-create-idem-4.4.0/setup.py`

 * *Files identical despite different names*

