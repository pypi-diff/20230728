# Comparing `tmp/cdpcli-beta-0.9.92.tar.gz` & `tmp/cdpcli-beta-0.9.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.92.tar", last modified: Thu Jul 13 16:50:38 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.93.tar", last modified: Fri Jul 28 14:52:42 2023, max compression
```

## Comparing `cdpcli-beta-0.9.92.tar` & `cdpcli-beta-0.9.93.tar`

### file list

```diff
@@ -1,185 +1,187 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.601861 cdpcli-beta-0.9.92/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   150925 2023-07-13 16:50:36.000000 cdpcli-beta-0.9.92/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   105668 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    93690 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193989 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   181639 2023-07-13 16:50:33.000000 cdpcli-beta-0.9.92/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56972 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    73060 2023-07-13 16:50:36.000000 cdpcli-beta-0.9.92/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    54815 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.597861 cdpcli-beta-0.9.92/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.597861 cdpcli-beta-0.9.92/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      264 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-07-28 14:52:38.000000 cdpcli-beta-0.9.93/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    96796 2023-07-28 14:52:38.000000 cdpcli-beta-0.9.93/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/consumption/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5016 2023-07-28 14:52:39.000000 cdpcli-beta-0.9.93/cdpcli/data/consumption/consumption.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   150925 2023-07-28 14:52:40.000000 cdpcli-beta-0.9.93/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   107524 2023-07-28 14:52:39.000000 cdpcli-beta-0.9.93/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    94719 2023-07-28 14:52:39.000000 cdpcli-beta-0.9.93/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-07-28 14:52:39.000000 cdpcli-beta-0.9.93/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193989 2023-07-28 14:52:38.000000 cdpcli-beta-0.9.93/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   181832 2023-07-28 14:52:37.000000 cdpcli-beta-0.9.93/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-07-28 14:52:40.000000 cdpcli-beta-0.9.93/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-07-28 14:52:38.000000 cdpcli-beta-0.9.93/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    65173 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.731238 cdpcli-beta-0.9.93/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    73060 2023-07-28 14:52:40.000000 cdpcli-beta-0.9.93/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    54815 2023-07-28 14:52:41.000000 cdpcli-beta-0.9.93/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.723238 cdpcli-beta-0.9.93/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.735238 cdpcli-beta-0.9.93/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.739238 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4338 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-07-28 14:52:42.000000 cdpcli-beta-0.9.93/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.723238 cdpcli-beta-0.9.93/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.739238 cdpcli-beta-0.9.93/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.739238 cdpcli-beta-0.9.93/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:52:42.743239 cdpcli-beta-0.9.93/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-07-28 14:40:00.000000 cdpcli-beta-0.9.93/versioneer.py
```

### Comparing `cdpcli-beta-0.9.92/LICENSE.txt` & `cdpcli-beta-0.9.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.93/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/PKG-INFO` & `cdpcli-beta-0.9.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.92
+Version: 0.9.93
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.92/README.md` & `cdpcli-beta-0.9.93/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/__init__.py` & `cdpcli-beta-0.9.93/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/argparser.py` & `cdpcli-beta-0.9.93/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/argprocess.py` & `cdpcli-beta-0.9.93/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/arguments.py` & `cdpcli-beta-0.9.93/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/auth.py` & `cdpcli-beta-0.9.93/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.93/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/clicommand.py` & `cdpcli-beta-0.9.93/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/clidriver.py` & `cdpcli-beta-0.9.93/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/client.py` & `cdpcli-beta-0.9.93/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/compat.py` & `cdpcli-beta-0.9.93/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/completer.py` & `cdpcli-beta-0.9.93/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/config.py` & `cdpcli-beta-0.9.93/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/configloader.py` & `cdpcli-beta-0.9.93/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/credentials.py` & `cdpcli-beta-0.9.93/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.93/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/audit/audit.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/cli.json` & `cdpcli-beta-0.9.93/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.92
+  version: 0.9.93
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/compute/compute.yaml`

 * *Files 1% similar despite different names*

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
@@ -734,53 +734,24 @@
   CommonLoggingResp:
     type: object
     description: Logging response structure.
     properties:
       enabled:
         type: boolean
         description: True to enable logging installation (default false).
-  CommonAcmCertificateResp:
-    type: object
-    description: ACM certificate response structure.
-    properties:
-      arn:
-        type: string
-        description: The ARN of the ACM certificate.
-  CommonIstioIngressResp:
-    type: object
-    description: Istio ingress response structure.
-    properties:
-      acmCertificates:
-        type: array
-        items:
-          $ref: '#/definitions/CommonAcmCertificateResp'
-        description: Array of ACM certificates.
-  CommonIstioGatewaysResp:
-    type: object
-    description: Istio gateways response structure.
-    properties:
-      ingress:
-        description: Configuration options for istio ingress.
-        $ref: '#/definitions/CommonIstioIngressResp'
   CommonIstioResp:
     type: object
     description: Istio response structure.
     properties:
       enabled:
         type: boolean
         description: True to enable istio installation (default false).
-      sidecarCpu:
+      deploymentProfile:
         type: string
-        description: CPU request for istio sidecar container (default 50m).
-      sidecarMemory:
-        type: string
-        description: Memory request for istio sidecar container (default 128Mi).
-      gateways:
-        description: Configuration options for Istio gateways (ingress and egress).
-        $ref: '#/definitions/CommonIstioGatewaysResp'
+        description: Deployment profile to use. Currently supported are cml and cde.
   CommonHorizontalPodAutoScalerResp:
     type: object
     description: Horizontal pod autoscaler response structure.
     properties:
       enabled:
         type: boolean
         description: Enable flag.
@@ -1412,14 +1383,30 @@
     type: object
     description: Storage spec response structure.
     properties:
       csiEnabled:
         type: boolean
         description: Flag to enable CSI (Container Storage Interface). It further sets specific inline cloud formation policies required for CSI.
     x-form-factors: public
+  CommonNodeImageAvailableUpgrade:
+    type: object
+    description: Structure to list the currently used images and the new upgrades available.
+    properties:
+      instanceGroup:
+        type: string
+        description: Instance group name.
+      current:
+        type: string
+        description: Currently used node image version.
+      upgrades:
+        type: array
+        items:
+          type: string
+        description: Available node image upgrade versions.
+    x-form-factors: public
   DescribeClusterResponse:
     type: object
     description: Describe cluster response.
     properties:
       envName:
         type: string
         description: CDP environment name.
@@ -1542,14 +1529,20 @@
         description: EKS state.
         $ref: '#/definitions/EksState'
         x-form-factors: public
       nodeImageUpgradeAvailable:
         type: boolean
         description: Is a node image upgrade available.
         x-form-factors: public
+      nodeImageUpgrades:
+        type: array
+        items:
+          $ref: '#/definitions/CommonNodeImageAvailableUpgrade'
+        description: Lists the currently used images and the new upgrades available.
+        x-form-factors: public
   ListClustersRequest:
     type: object
     description: Request object to list clusters.
     properties:
       envNameOrCrn:
         type: string
         description: Environment name or crn.
@@ -2075,53 +2068,24 @@
   CommonLogging:
     type: object
     description: Logging request structure.
     properties:
       enabled:
         type: boolean
         description: True to enable logging installation (default false).
-  CommonAcmCertificate:
-    type: object
-    description: ACM certificate request structure.
-    properties:
-      arn:
-        type: string
-        description: The ARN of the ACM certificate.
-  CommonIstioIngress:
-    type: object
-    description: Istio ingress request structure.
-    properties:
-      acmCertificates:
-        type: array
-        items:
-          $ref: '#/definitions/CommonAcmCertificate'
-        description: An array of ACM certificates.
-  CommonIstioGateway:
-    type: object
-    description: Istio gateways request structure.
-    properties:
-      ingress:
-        description: Configuration options for istio ingress.
-        $ref: '#/definitions/CommonIstioIngress'
   CommonIstio:
     type: object
     description: Istio request structure.
     properties:
       enabled:
         type: boolean
         description: True to enable istio installation (default false).
-      sidecarCpu:
-        type: string
-        description: CPU request for istio sidecar container (default 50m).
-      sidecarMemory:
+      deploymentProfile:
         type: string
-        description: Memory request for istio sidecar container (default 128Mi).
-      gateway:
-        description: Configuration options for Istio gateways (ingress and egress).
-        $ref: '#/definitions/CommonIstioGateway'
+        description: Deployment profile to use. Currently supported are cml and cde.
   CommonHorizontalPodAutoScaler:
     type: object
     description: Horizontal pod autoscaler request structure.
     properties:
       enabled:
         type: boolean
         description: Enable flag.
@@ -2502,14 +2466,18 @@
         description: The name of the chart to install.
       chartVersion:
         type: string
         description: The version of the chart to install. Defaults to latest version.
       overrides:
         type: string
         description: Escaped JSON overrides for the deployment's properties.
+      deploymentProfile:
+        type: string
+        description: Deployment profile to use. Currently supported are cml and cde.
+        x-form-factors: public
   InstallDeploymentResponse:
     type: object
     description: Response structure for installing a deployment.
     properties:
       name:
         type: string
         description: The name of the deployment.
```

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/datacatalog/datacatalog.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/datahub/datahub.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/datalake/datalake.yaml`

 * *Files 1% similar despite different names*

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
@@ -754,14 +754,35 @@
           description: Expected response to a valid resize datalake request.
           schema:
             $ref: '#/definitions/ResizeDatalakeResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/datalake/startDatalakeHorizontalScaling:
+    post:
+      summary: Horizontally scale the Data Lake nodes, to add additional compute nodes to the cluster.
+      description: Horizontally scale the target host group in the Data Lake cluster. The possible option for the instance group are raz_scale_out, hms_scale_out, kafka_scale_out, solr_scale_out, storage_scale_out
+      operationId: startDatalakeHorizontalScaling
+      x-mutating: true
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/StartDatalakeHorizontalScalingRequest'
+      responses:
+        200:
+          description: Successful response to a valid Data Lake horizontal scaling request.
+          schema:
+            $ref: '#/definitions/StartDatalakeHorizontalScalingResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
   /api/v1/datalake/recoverDatalake:
     post:
       summary: Recover data lake to the original version after a failed upgrade.
       description: Recover data lake to the original version after a failed upgrade.
       operationId: recoverDatalake
       x-mutating: true
       parameters:
@@ -2763,14 +2784,39 @@
         description: The current status of the datalake.
       statusReason:
         type: string
         description: The reason for the current status of the datalake.
       cloudbreakVersion:
         type: string
         description: The Cloudbreak version used to create the data lake.
+  StartDatalakeHorizontalScalingRequest:
+    type: object
+    description: Data lake horizontal scaling request.
+    required:
+      - datalakeName
+      - instanceGroupName
+      - instanceGroupDesiredCount
+    properties:
+      datalakeName:
+        type: string
+        description: the name of the Data Lake
+      instanceGroupName:
+        type: string
+        description: The target host group name to be scaled.
+      instanceGroupDesiredCount:
+        type: integer
+        format: int32
+        description: The target number of the scaling operation. If the desired count is less than the actual node count the scaling action will be a downscale operation.
+  StartDatalakeHorizontalScalingResponse:
+    type: object
+    description: Data Lake horizontal scaling response
+    properties:
+      datalakeName:
+        type: string
+        description: The name of the datalake.
   ReplaceRecipesRequest:
     type: object
     description: The request for replacing recipes.
     required:
       - datalake
       - instanceGroupRecipes
     properties:
```

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/de/de.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/df/df.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/dfworkload/dfworkload.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/drscp/drscp.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/dw/dw.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/environments/environments.yaml`

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
@@ -1954,14 +1954,15 @@
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
@@ -2394,14 +2395,15 @@
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
@@ -2482,14 +2484,15 @@
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
@@ -4846,14 +4849,19 @@
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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/iam/iam.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/imagecatalog/imagecatalog.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/ml/ml.yaml`

 * *Files 8% similar despite different names*

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
@@ -35,14 +35,35 @@
           schema:
             $ref: '#/definitions/BackupWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/ml/createModelRegistry:
+    post:
+      summary: Creates a new model registry.
+      description: Create a new model registry by creating a new workspace and install model registry on it.
+      operationId: createModelRegistry
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/CreateModelRegistryRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/CreateModelRegistryResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+      x-mutating: true
   /api/v1/ml/createWorkspace:
     post:
       summary: Create a Cloudera Machine Learning workspace.
       description: Provision a Kubernetes cluster and install the Cloudera Machine Learning application in it.
       operationId: createWorkspace
       parameters:
         - name: input
@@ -98,14 +119,35 @@
           schema:
             $ref: '#/definitions/DeleteInstanceGroupResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/ml/deleteModelRegistry:
+    post:
+      summary: Deletes a model registry.
+      description: Delete a model registry.
+      operationId: deleteModelRegistry
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/DeleteModelRegistryRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/DeleteModelRegistryResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+      x-mutating: true
   /api/v1/ml/deleteWorkspace:
     post:
       summary: Delete Cloudera Machine Learning Workspace.
       description: Deletes a Cloudera Machine Learning workspace.
       operationId: deleteWorkspace
       parameters:
         - name: input
@@ -245,14 +287,35 @@
           schema:
             $ref: '#/definitions/GrantWorkspaceAccessResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/ml/listModelRegistries:
+    post:
+      summary: Lists all model registries.
+      description: List all model registries.
+      operationId: listModelRegistries
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/ListModelRegistriesRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/ListModelRegistriesResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+      x-mutating: false
   /api/v1/ml/listWorkspaceAccess:
     post:
       summary: ListWorkspaceAccess Cloudera Machine Learning Workspace.
       description: Lists users that can perform Kubernetes operations on a Cloudera Machine Learning workspace via EKS.
       operationId: listWorkspaceAccess
       parameters:
         - name: input
@@ -371,14 +434,35 @@
           schema:
             $ref: '#/definitions/ModifyWorkspaceLoadBalancerResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/ml/refreshModelRegistryConfigmap:
+    post:
+      summary: Refreshes the model registry configmap of the workspace.
+      description: Refreshes the model registry configmap of the workspace from the control plane.
+      operationId: refreshModelRegistryConfigmap
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/RefreshModelRegistryConfigmapRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/RefreshModelRegistryConfigmapResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+      x-mutating: true
   /api/v1/ml/requestWorkflowCancellation:
     post:
       summary: Request a workflow cancellation.
       description: Request a long running workflow cancellation by resource ID and workflow type.
       operationId: requestWorkflowCancellation
       parameters:
         - name: input
@@ -476,14 +560,35 @@
           schema:
             $ref: '#/definitions/SuspendWorkspaceResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
       x-mutating: true
+  /api/v1/ml/updateModelRegistry:
+    post:
+      summary: Updates a model registry.
+      description: Update a model registry.
+      operationId: updateModelRegistry
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/UpdateModelRegistryRequest'
+      responses:
+        200:
+          description: Expected response to a valid request.
+          schema:
+            $ref: '#/definitions/UpdateModelRegistryResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
+      x-mutating: true
   /api/v1/ml/upgradeWorkspace:
     post:
       summary: Upgrade Cloudera Machine Learning workspace.
       description: Upgrades a Cloudera Machine Learning workspace to the latest available version.
       operationId: upgradeWorkspace
       parameters:
         - name: input
@@ -1137,14 +1242,17 @@
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
@@ -1269,14 +1377,17 @@
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
@@ -1674,8 +1785,144 @@
     description: Response object for RequestWorkflowCancellation.
     properties:
       workflowMetadata:
         type: array
         items:
           $ref: '#/definitions/WorkflowMetadata'
         description: The list of workflow metedata for cancelled workflows.
+  CreateModelRegistryRequest:
+    type: object
+    description: Request object for creating model registry.
+    properties:
+      namespace:
+        type: string
+        description: The namespace of the model registry.
+      s3AccessKey:
+        type: string
+        description: The S3 access key of Ozone.
+        x-sensitive: true
+      s3SecretKey:
+        type: string
+        description: The S3 secret key of Ozone.
+        x-sensitive: true
+      s3Bucket:
+        type: string
+        description: The s3Bucket of Ozone.
+      s3Endpoint:
+        type: string
+        description: The endpoint of Ozone.
+        x-no-paramfile: true
+      creatorCrn:
+        type: string
+        description: The creator of model registry.
+      environmentCrn:
+        type: string
+        description: The environment CRN of model registry.
+      environmentName:
+        type: string
+        description: The environment name.
+      createWorkspacePayload:
+        description: The create workspace request on which model registry helm chart is deployed.
+        $ref: '#/definitions/CreateWorkspaceRequest'
+      modelRegistryVersion:
+        type: string
+        description: The version of model registry app to install.
+  CreateModelRegistryResponse:
+    type: object
+    description: Response for creating model registry request.
+  ListModelRegistriesRequest:
+    type: object
+    description: Request object for deleting model registry.
+  ListModelRegistriesResponse:
+    type: object
+    description: List of all available model registries.
+    properties:
+      modelRegistries:
+        type: array
+        items:
+          $ref: '#/definitions/ModelRegistry'
+        description: The list of model registry.
+  ModelRegistry:
+    type: object
+    description: Model registry object
+    properties:
+      id:
+        type: integer
+        format: int64
+        description: The id of model registry.
+      namespace:
+        type: string
+        description: The namespace of model registry.
+      s3Bucket:
+        type: string
+        description: The s3 bucket of model registry.
+      s3Endpoint:
+        type: string
+        description: The Ozone endpoint of model registry.
+      creator:
+        type: string
+        description: The creator of model registry.
+      status:
+        type: string
+        description: The status of model registry.
+      environmentCrn:
+        type: string
+        description: The environment CRN of model registry.
+      createdAt:
+        type: string
+        format: date-time
+        description: The creation time of model registry.
+      crn:
+        type: string
+        description: ModelRegistry CRN.
+      workspaceCrn:
+        type: string
+        description: WorkSpace CRN.
+      environmentName:
+        type: string
+        description: Environment name.
+      workspaceName:
+        type: string
+        description: Workspace name.
+      machineUserCrn:
+        type: string
+        description: The machine user CRN of the model registry.
+  DeleteModelRegistryRequest:
+    type: object
+    description: Request for deleting model registry.
+    properties:
+      id:
+        type: string
+        description: The environment CRN of the model registry.
+      workspaceCrn:
+        type: string
+        description: The workspace CRN of the model registry (Public cloud only).
+      force:
+        type: boolean
+        description: Force delete a model registry workspace even if errors occur during deletion. Force delete removes the guarantee that resources in your cloud account will be cleaned up. By default, force is set to false.
+  DeleteModelRegistryResponse:
+    type: object
+    description: Delete model registry response.
+  UpdateModelRegistryRequest:
+    type: object
+    description: Request for updating model registry.
+    properties:
+      id:
+        type: string
+        description: The id of model registry.
+      modelRegistryVersion:
+        type: string
+        description: The namespace of model registry.
+  UpdateModelRegistryResponse:
+    type: object
+    description: Response for updating model registry request.
+  RefreshModelRegistryConfigmapRequest:
+    type: object
+    description: Request for refreshing workspace's model registry configmap.
+    properties:
+      workspaceCrn:
+        type: string
+        description: Workspace CRN.
+  RefreshModelRegistryConfigmapResponse:
+    type: object
+    description: Response for refreshing workspace's model registry configmap.
 x-audit: true
```

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/opdb/opdb.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.93/cdpcli/data/replicationmanager/replicationmanager.yaml`

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

### Comparing `cdpcli-beta-0.9.92/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.93/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.93/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/doc/style.py` & `cdpcli-beta-0.9.93/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/docs.py` & `cdpcli-beta-0.9.93/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/endpoint.py` & `cdpcli-beta-0.9.93/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.93/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.93/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.93/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.93/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.93/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/exceptions.py` & `cdpcli-beta-0.9.93/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.93/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/formatter.py` & `cdpcli-beta-0.9.93/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/help.py` & `cdpcli-beta-0.9.93/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/loader.py` & `cdpcli-beta-0.9.93/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/main.py` & `cdpcli-beta-0.9.93/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/model.py` & `cdpcli-beta-0.9.93/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/paginate.py` & `cdpcli-beta-0.9.93/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/paramfile.py` & `cdpcli-beta-0.9.93/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.93/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/parser.py` & `cdpcli-beta-0.9.93/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.93/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/schema.py` & `cdpcli-beta-0.9.93/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/serialize.py` & `cdpcli-beta-0.9.93/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/shorthand.py` & `cdpcli-beta-0.9.93/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/signers.py` & `cdpcli-beta-0.9.93/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/table.py` & `cdpcli-beta-0.9.93/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/text.py` & `cdpcli-beta-0.9.93/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/textwriter.py` & `cdpcli-beta-0.9.93/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.93/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/translate.py` & `cdpcli-beta-0.9.93/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/utils.py` & `cdpcli-beta-0.9.93/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli/validate.py` & `cdpcli-beta-0.9.93/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.93/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.92
+Version: 0.9.93
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.92/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.93/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 cdpcli/data/_retry.json
 cdpcli/data/aliases.yaml
 cdpcli/data/cli.json
 cdpcli/data/release.txt
 cdpcli/data/audit/audit.yaml
 cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
 cdpcli/data/compute/compute.yaml
+cdpcli/data/consumption/consumption.yaml
 cdpcli/data/datacatalog/datacatalog.yaml
 cdpcli/data/datahub/datahub.yaml
 cdpcli/data/datalake/datalake.yaml
 cdpcli/data/de/de.yaml
 cdpcli/data/df/df.yaml
 cdpcli/data/dfworkload/dfworkload.yaml
 cdpcli/data/drscp/drscp.yaml
```

### Comparing `cdpcli-beta-0.9.92/setup.py` & `cdpcli-beta-0.9.93/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/setup_common.py` & `cdpcli-beta-0.9.93/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/__init__.py` & `cdpcli-beta-0.9.93/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.93/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.93/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.93/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.93/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_auth.py` & `cdpcli-beta-0.9.93/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.93/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_client.py` & `cdpcli-beta-0.9.93/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_completer.py` & `cdpcli-beta-0.9.93/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.93/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_docs.py` & `cdpcli-beta-0.9.93/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.93/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_help.py` & `cdpcli-beta-0.9.93/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.93/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_model.py` & `cdpcli-beta-0.9.93/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.93/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.93/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.93/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.93/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.93/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_signers.py` & `cdpcli-beta-0.9.93/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.93/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_utils.py` & `cdpcli-beta-0.9.93/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/tests/unit/test_validate.py` & `cdpcli-beta-0.9.93/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.92/versioneer.py` & `cdpcli-beta-0.9.93/versioneer.py`

 * *Files identical despite different names*

