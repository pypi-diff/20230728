# Comparing `tmp/cdpcli-0.9.92.tar.gz` & `tmp/cdpcli-0.9.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-0.9.92.tar", last modified: Thu Jul 13 17:29:36 2023, max compression
+gzip compressed data, was "cdpcli-0.9.93.tar", last modified: Fri Jul 28 14:53:44 2023, max compression
```

## Comparing `cdpcli-0.9.92.tar` & `cdpcli-0.9.93.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.152320 cdpcli-0.9.92/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-07-13 17:19:26.000000 cdpcli-0.9.92/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-07-13 17:19:26.000000 cdpcli-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-07-13 17:19:26.000000 cdpcli-0.9.92/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-07-13 17:29:36.152320 cdpcli-0.9.92/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-07-13 17:19:26.000000 cdpcli-0.9.92/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.152320 cdpcli-0.9.92/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-07-13 17:29:36.152320 cdpcli-0.9.92/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      222 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15591 2023-07-13 17:29:31.000000 cdpcli-0.9.92/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   144871 2023-07-13 17:29:33.000000 cdpcli-0.9.92/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   102649 2023-07-13 17:29:32.000000 cdpcli-0.9.92/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    93690 2023-07-13 17:29:32.000000 cdpcli-0.9.92/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-07-13 17:29:33.000000 cdpcli-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-07-13 17:29:32.000000 cdpcli-0.9.92/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193053 2023-07-13 17:29:31.000000 cdpcli-0.9.92/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   166105 2023-07-13 17:29:30.000000 cdpcli-0.9.92/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.136320 cdpcli-0.9.92/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   132904 2023-07-13 17:29:32.000000 cdpcli-0.9.92/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-07-13 17:29:31.000000 cdpcli-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56870 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    24469 2023-07-13 17:29:33.000000 cdpcli-0.9.92/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        6 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    43694 2023-07-13 17:29:34.000000 cdpcli-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.124320 cdpcli-0.9.92/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.140320 cdpcli-0.9.92/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.144320 cdpcli-0.9.92/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.144320 cdpcli-0.9.92/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.144320 cdpcli-0.9.92/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-07-13 17:19:26.000000 cdpcli-0.9.92/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.132320 cdpcli-0.9.92/cdpcli.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4214 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-07-13 17:29:35.000000 cdpcli-0.9.92/cdpcli.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-07-13 17:29:36.152320 cdpcli-0.9.92/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1414 2023-07-13 17:19:26.000000 cdpcli-0.9.92/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-07-13 17:19:26.000000 cdpcli-0.9.92/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.124320 cdpcli-0.9.92/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.148320 cdpcli-0.9.92/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.148320 cdpcli-0.9.92/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.148320 cdpcli-0.9.92/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.152320 cdpcli-0.9.92/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:29:36.152320 cdpcli-0.9.92/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-07-13 17:19:26.000000 cdpcli-0.9.92/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-07-13 17:19:26.000000 cdpcli-0.9.92/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-07-28 14:40:59.000000 cdpcli-0.9.93/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-07-28 14:40:59.000000 cdpcli-0.9.93/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-07-28 14:40:59.000000 cdpcli-0.9.93/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-07-28 14:53:44.038341 cdpcli-0.9.93/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-07-28 14:40:59.000000 cdpcli-0.9.93/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.042341 cdpcli-0.9.93/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-07-28 14:53:44.042341 cdpcli-0.9.93/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      222 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15591 2023-07-28 14:53:39.000000 cdpcli-0.9.93/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   144871 2023-07-28 14:53:41.000000 cdpcli-0.9.93/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   102649 2023-07-28 14:53:40.000000 cdpcli-0.9.93/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    94719 2023-07-28 14:53:41.000000 cdpcli-0.9.93/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-07-28 14:53:40.000000 cdpcli-0.9.93/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193053 2023-07-28 14:53:39.000000 cdpcli-0.9.93/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   166935 2023-07-28 14:53:38.000000 cdpcli-0.9.93/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   132904 2023-07-28 14:53:41.000000 cdpcli-0.9.93/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    19320 2023-07-28 14:53:39.000000 cdpcli-0.9.93/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    57116 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    24469 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        6 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.026341 cdpcli-0.9.93/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    43694 2023-07-28 14:53:42.000000 cdpcli-0.9.93/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.030341 cdpcli-0.9.93/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.014340 cdpcli-0.9.93/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.030341 cdpcli-0.9.93/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.030341 cdpcli-0.9.93/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.030341 cdpcli-0.9.93/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.030341 cdpcli-0.9.93/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.034341 cdpcli-0.9.93/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.034341 cdpcli-0.9.93/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.034341 cdpcli-0.9.93/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-07-28 14:40:59.000000 cdpcli-0.9.93/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.022340 cdpcli-0.9.93/cdpcli.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7819 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4214 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-07-28 14:53:43.000000 cdpcli-0.9.93/cdpcli.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-07-28 14:53:44.042341 cdpcli-0.9.93/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1414 2023-07-28 14:40:59.000000 cdpcli-0.9.93/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-07-28 14:40:59.000000 cdpcli-0.9.93/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.014340 cdpcli-0.9.93/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:53:44.038341 cdpcli-0.9.93/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-07-28 14:40:59.000000 cdpcli-0.9.93/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-07-28 14:40:59.000000 cdpcli-0.9.93/versioneer.py
```

### Comparing `cdpcli-0.9.92/LICENSE.txt` & `cdpcli-0.9.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-0.9.93/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/PKG-INFO` & `cdpcli-0.9.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli
-Version: 0.9.92
+Version: 0.9.93
 Summary: Cloudera CDP Command Line Interface
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-0.9.92/README.md` & `cdpcli-0.9.93/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/__init__.py` & `cdpcli-0.9.93/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/argparser.py` & `cdpcli-0.9.93/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/argprocess.py` & `cdpcli-0.9.93/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/arguments.py` & `cdpcli-0.9.93/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/auth.py` & `cdpcli-0.9.93/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/cdprequest.py` & `cdpcli-0.9.93/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/clicommand.py` & `cdpcli-0.9.93/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/clidriver.py` & `cdpcli-0.9.93/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/client.py` & `cdpcli-0.9.93/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/compat.py` & `cdpcli-0.9.93/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/completer.py` & `cdpcli-0.9.93/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/config.py` & `cdpcli-0.9.93/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/configloader.py` & `cdpcli-0.9.93/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/credentials.py` & `cdpcli-0.9.93/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/data/_retry.json` & `cdpcli-0.9.93/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/data/audit/audit.yaml` & `cdpcli-0.9.93/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/cli.json` & `cdpcli-0.9.93/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/data/compute/compute.yaml` & `cdpcli-0.9.93/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-0.9.93/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-0.9.92/cdpcli/data/datahub/datahub.yaml` & `cdpcli-0.9.93/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/datalake/datalake.yaml` & `cdpcli-0.9.93/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/de/de.yaml` & `cdpcli-0.9.93/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/df/df.yaml` & `cdpcli-0.9.93/cdpcli/data/df/df.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1976,14 +1976,17 @@
       configurationVersion:
         type: integer
         format: int64
         description: The version of the configuration for this deployment
       cfmNifiVersion:
         type: string
         description: The version of NiFi being used by this deployment.
+      flowMetricsScalingEnabled:
+        type: boolean
+        description: Whether or not to use Flow metrics to scale the deployment. May only be specified when autscalingEnabled is true.
   FilterOption:
     type: object
     description: A filter option
     required:
       - identifier
       - label
     properties:
@@ -2457,14 +2460,23 @@
         description: The name of the proxy that is configured for the CDP environment
       k8sServerVersion:
         type: string
         description: The kubernetes version of the cluster
       availableK8sVersionUpgrade:
         type: string
         description: The available kubernetes version that cluster can be upgraded to.
+      userDefinedRouting:
+        type: boolean
+        description: Whether User Defined Routing (UDR) mode is enabled for AKS clusters or not.
+      podCidr:
+        type: string
+        description: CIDR range from which to assign IPs to pods in the kubernetes cluster.
+      serviceCidr:
+        type: string
+        description: CIDR range from which to assign IPs to internal services in the kubernetes cluster.
   ListServicesRequest:
     type: object
     description: Request object for the ListServices method.
     properties:
       sorts:
         type: array
         items:
@@ -2601,14 +2613,23 @@
         description: Indicates whether to provision private k8s cluster.
       instanceType:
         type: string
         description: Indicates custom instance type to be used
       skipPreflightChecks:
         type: boolean
         description: Indicates whether to skip Liftie's pre-flight checks.
+      userDefinedRouting:
+        type: boolean
+        description: Indicates whether User Defined Routing (UDR) mode is enabled for AKS clusters.
+      podCidr:
+        type: string
+        description: CIDR range from which to assign IPs to pods in the kubernetes cluster.
+      serviceCidr:
+        type: string
+        description: CIDR range from which to assign IPs to internal services in the kubernetes cluster.
   EnableServiceResponse:
     type: object
     description: Response object for EnableService
     properties:
       service:
         description: The service
         $ref: '#/definitions/Service'
```

### Comparing `cdpcli-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-0.9.93/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-0.9.92/cdpcli/data/drscp/drscp.yaml` & `cdpcli-0.9.93/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-0.9.92/cdpcli/data/dw/dw.yaml` & `cdpcli-0.9.93/cdpcli/data/dw/dw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/environments/environments.yaml` & `cdpcli-0.9.93/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1749,14 +1749,15 @@
         type: string
         description: The name for the DynamoDB table backing S3Guard.
       description:
         type: string
         description: An description of the environment.
       enableTunnel:
         type: boolean
+        default: true
         description: Whether to enable SSH tunneling for the environment.
       workloadAnalytics:
         type: boolean
         description: When this is enabled, diagnostic information about job and query execution is sent to Workload Manager for Data Hub clusters created within this environment.
       reportDeploymentLogs:
         type: boolean
         description: When true, this will report additional diagnostic information back to Cloudera.
@@ -2189,14 +2190,15 @@
             type: string
             description: The range of private IPv4 addresses that resources will use under the created VNet.
       description:
         type: string
         description: An description of the environment.
       enableTunnel:
         type: boolean
+        default: true
         description: Whether to enable SSH tunneling for the environment.
       workloadAnalytics:
         type: boolean
         description: When this is enabled, diagnostic information about job and query execution is sent to Workload Manager for Data Hub clusters created within this environment.
       reportDeploymentLogs:
         type: boolean
         description: When true, this will report additional diagnostic information back to Cloudera.
@@ -2216,14 +2218,20 @@
         description: Name of the proxy config to use for the environment.
       resourceGroupName:
         type: string
         description: Name of an existing Azure resource group to be used for the environment. If it is not specified then new resource groups will be generated.
       createPrivateEndpoints:
         type: boolean
         description: When this is enabled, then Azure Postgres will be configured with Private Endpoint and a Private DNS Zone. When this is disabled, then Azure Service Endpoints will be created. The default value is disabled.
+      endpointAccessGatewayScheme:
+        type: string
+        description: The scheme for the endpoint gateway. PUBLIC creates an external endpoint that can be accessed over the Internet. Defaults to PRIVATE which restricts the traffic to be internal to the VNet.
+        enum:
+          - PUBLIC
+          - PRIVATE
       endpointAccessGatewaySubnetIds:
         type: array
         items:
           type: string
         description: The subnets to use for endpoint access gateway.
       encryptionKeyUrl:
         type: string
@@ -2271,24 +2279,31 @@
         description: GCP storage configuration for cluster and audit logs.
         $ref: '#/definitions/GcpLogStorageRequest'
       description:
         type: string
         description: A description of the environment.
       enableTunnel:
         type: boolean
+        default: true
         description: Whether to enable SSH tunneling for the environment.
       workloadAnalytics:
         type: boolean
         description: When this is enabled, diagnostic information about job and query execution is sent to Workload Manager for Data Hub clusters created within this environment.
       reportDeploymentLogs:
         type: boolean
         description: When true, this will report additional diagnostic information back to Cloudera.
       freeIpa:
         $ref: '#/definitions/GCPFreeIpaCreationRequest'
         description: The FreeIPA creation request for the environment
+      endpointAccessGatewayScheme:
+        type: string
+        description: The scheme for the endpoint gateway. PUBLIC creates an external endpoint that can be accessed over the Internet. Defaults to PRIVATE which restricts the traffic to be internal to the VPC.
+        enum:
+          - PUBLIC
+          - PRIVATE
       endpointAccessGatewaySubnetIds:
         type: array
         items:
           type: string
         description: The subnets to use for endpoint access gateway.
       tags:
         type: array
@@ -4462,14 +4477,19 @@
         description: The name or CRN of the environment.
       targetAvailabilityType:
         type: string
         enum:
           - HA
           - TWO_NODE_BASED
         description: The target FreeIPA availability type.
+      instances:
+        type: array
+        items:
+          type: string
+        description: The instance Ids to downscale.
   DownscaleFreeipaResponse:
     type: object
     description: The response object for FreeIPA downscale.
     properties:
       originalAvailabilityType:
         type: string
         enum:
```

### Comparing `cdpcli-0.9.92/cdpcli/data/iam/iam.yaml` & `cdpcli-0.9.93/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-0.9.93/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/ml/ml.yaml` & `cdpcli-0.9.93/cdpcli/data/ml/ml.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1134,14 +1134,17 @@
         $ref: '#/definitions/BackupMetadata'
       clusterID:
         type: string
         description: The Cluster ID for the workspace.
       isPrivate:
         type: boolean
         description: The value to indicate if the cluster is private or not.
+      isRestored:
+        type: boolean
+        description: The value to indicate if the workspace is restored one or not
   Workspace:
     type: object
     description: A ML workspace, which includes the cluster and storage.
     required:
       - instanceName
       - environmentName
       - instanceStatus
@@ -1266,14 +1269,17 @@
         $ref: '#/definitions/BackupMetadata'
       clusterID:
         type: string
         description: The Cluster ID for the workspace.
       isPrivate:
         type: boolean
         description: The value to indicate if the cluster is private or not.
+      isRestored:
+        type: boolean
+        description: The value to indicate if the workspace is restored one or not
   UpgradeWorkspaceRequest:
     type: object
     description: Request object for the UpgradeWorkspace method.
     properties:
       environmentName:
         type: string
         description: The environment of the workspace.
```

### Comparing `cdpcli-0.9.92/cdpcli/data/opdb/opdb.yaml` & `cdpcli-0.9.93/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-0.9.93/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-0.9.92/cdpcli/doc/docstringparser.py` & `cdpcli-0.9.93/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/doc/restdoc.py` & `cdpcli-0.9.93/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/doc/style.py` & `cdpcli-0.9.93/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/docs.py` & `cdpcli-0.9.93/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/endpoint.py` & `cdpcli-0.9.93/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/examples/configure/_description.rst` & `cdpcli-0.9.93/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/examples/configure/get/_description.rst` & `cdpcli-0.9.93/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-0.9.93/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/examples/configure/set/_description.rst` & `cdpcli-0.9.93/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-0.9.93/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/exceptions.py` & `cdpcli-0.9.93/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/__init__.py` & `cdpcli-0.9.93/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/arguments.py` & `cdpcli-0.9.93/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/cliinputjson.py` & `cdpcli-0.9.93/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/commands.py` & `cdpcli-0.9.93/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/__init__.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/classify.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/configure.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/get.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/list.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/configure/set.py` & `cdpcli-0.9.93/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/df/__init__.py` & `cdpcli-0.9.93/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/df/createdeployment.py` & `cdpcli-0.9.93/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/df/register.py` & `cdpcli-0.9.93/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-0.9.93/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/interactivelogin.py` & `cdpcli-0.9.93/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/logout.py` & `cdpcli-0.9.93/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/paginate.py` & `cdpcli-0.9.93/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/redirect.py` & `cdpcli-0.9.93/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/refdoc.py` & `cdpcli-0.9.93/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/workload.py` & `cdpcli-0.9.93/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/extensions/writer.py` & `cdpcli-0.9.93/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/formatter.py` & `cdpcli-0.9.93/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/help.py` & `cdpcli-0.9.93/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/loader.py` & `cdpcli-0.9.93/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/main.py` & `cdpcli-0.9.93/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/model.py` & `cdpcli-0.9.93/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/paginate.py` & `cdpcli-0.9.93/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/paramfile.py` & `cdpcli-0.9.93/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/paramformfactor.py` & `cdpcli-0.9.93/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/parser.py` & `cdpcli-0.9.93/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/retryhandler.py` & `cdpcli-0.9.93/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/schema.py` & `cdpcli-0.9.93/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/serialize.py` & `cdpcli-0.9.93/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/shorthand.py` & `cdpcli-0.9.93/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/signers.py` & `cdpcli-0.9.93/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/table.py` & `cdpcli-0.9.93/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/text.py` & `cdpcli-0.9.93/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/textwriter.py` & `cdpcli-0.9.93/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/thirdparty/six.py` & `cdpcli-0.9.93/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/translate.py` & `cdpcli-0.9.93/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/utils.py` & `cdpcli-0.9.93/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli/validate.py` & `cdpcli-0.9.93/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/cdpcli.egg-info/PKG-INFO` & `cdpcli-0.9.93/cdpcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli
-Version: 0.9.92
+Version: 0.9.93
 Summary: Cloudera CDP Command Line Interface
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-0.9.92/cdpcli.egg-info/SOURCES.txt` & `cdpcli-0.9.93/cdpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/setup.py` & `cdpcli-0.9.93/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/setup_common.py` & `cdpcli-0.9.93/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/__init__.py` & `cdpcli-0.9.93/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/cdp/__init__.py` & `cdpcli-0.9.93/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/__init__.py` & `cdpcli-0.9.93/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/configure/test_classify.py` & `cdpcli-0.9.93/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/configure/test_configure.py` & `cdpcli-0.9.93/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/configure/test_get.py` & `cdpcli-0.9.93/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/configure/test_list.py` & `cdpcli-0.9.93/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/configure/test_set.py` & `cdpcli-0.9.93/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-0.9.93/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-0.9.93/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-0.9.93/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_df.py` & `cdpcli-0.9.93/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-0.9.93/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-0.9.93/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_logout.py` & `cdpcli-0.9.93/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_operation_extension.py` & `cdpcli-0.9.93/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_paginate.py` & `cdpcli-0.9.93/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_redirect.py` & `cdpcli-0.9.93/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_workload.py` & `cdpcli-0.9.93/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/extensions/test_writer.py` & `cdpcli-0.9.93/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_argparser.py` & `cdpcli-0.9.93/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_argprocess.py` & `cdpcli-0.9.93/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_auth.py` & `cdpcli-0.9.93/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_cli_data.py` & `cdpcli-0.9.93/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_client.py` & `cdpcli-0.9.93/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_completer.py` & `cdpcli-0.9.93/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_credentials.py` & `cdpcli-0.9.93/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_docs.py` & `cdpcli-0.9.93/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_endpoint.py` & `cdpcli-0.9.93/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_help.py` & `cdpcli-0.9.93/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_loaders.py` & `cdpcli-0.9.93/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_model.py` & `cdpcli-0.9.93/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_paginate.py` & `cdpcli-0.9.93/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_paramfile.py` & `cdpcli-0.9.93/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_protocol.py` & `cdpcli-0.9.93/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_retryhandler.py` & `cdpcli-0.9.93/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_shorthand.py` & `cdpcli-0.9.93/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_signers.py` & `cdpcli-0.9.93/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_table_formatter.py` & `cdpcli-0.9.93/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_utils.py` & `cdpcli-0.9.93/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/tests/unit/test_validate.py` & `cdpcli-0.9.93/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-0.9.92/versioneer.py` & `cdpcli-0.9.93/versioneer.py`

 * *Files identical despite different names*

