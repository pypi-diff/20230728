# Comparing `tmp/ec2-api-9.0.0.0rc1.tar.gz` & `tmp/ec2-api-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ec2-api-9.0.0.0rc1.tar", last modified: Wed Sep 25 17:36:59 2019, max compression
+gzip compressed data, was "dist/ec2-api-9.0.1.tar", last modified: Mon Feb  1 18:32:40 2021, max compression
```

## Comparing `ec2-api-9.0.0.0rc1.tar` & `ec2-api-9.0.1.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65265 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/rally-scenarios/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       42 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/post_test_hook.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/rally-scenarios/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/extra/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3445 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3621 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_ec2_creds.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8704 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/ec2api_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13458 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_ec2_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/rally-scenarios/ec2-api-fakevirt.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/etc/ec2api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/etc/ec2api/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/etc/ec2api/README-ec2api.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/etc/ec2api/ec2api-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65265 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2_api.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3001 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/hacking.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/endpoints-creation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/metadata-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/credentials-creation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/install-sh.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1898 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/install-devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/database-creation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/install-manual.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/metadata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-ec2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-clients.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-service.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-metadata.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-common.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-database.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-s3.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/_flagmappings/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4201 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/_flagmappings/ec2api.flagmappings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/doc/source/configuration/_flagmappings/ec2api.headers
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/CONTRIBUTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11486 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/metadata/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11455 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/metadata/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/metadata/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5701 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18200 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/apirequest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74331 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30502 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/route_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3908 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9345 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24865 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7785 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/vpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5372 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/internet_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/key_pair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44615 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/customer_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8916 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21863 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/vpn_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19075 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/ec2utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17884 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/faults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20508 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6958 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/dhcp_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5923 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7281 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7486 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8618 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/vpn_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27378 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/network_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88086 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/api/cloud.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/db/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/versions/001_juno.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/migrate.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3781 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6548 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/botocoreclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26679 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    79696 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_private_key.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7631 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9828 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5760 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_apirequest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/abs.tar.gz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12986 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_integrated_scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30807 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31441 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_network_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15025 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   100441 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10271 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_internet_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10232 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/fakes_request_response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13191 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7662 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/tools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4430 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6225 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/rel.tar.gz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19411 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpn_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20627 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_db_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42764 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_s3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11227 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_ec2_validate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_customer_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39118 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpn_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_dhcp_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18157 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/matchers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_faults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17074 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56309 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_route_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15624 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_metadata_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_tools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_api_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26406 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_ec2utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9941 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4440 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_key_pair.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/s3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/s3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14197 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/s3/s3server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/s3/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15172 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/api_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/cmd/api_s3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ec2api/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/ec2api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/.zuul.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron-full/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2176 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron-full/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron-full/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-rally-fakevirt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-rally-fakevirt/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-rally-fakevirt/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57006 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/api-ref/source/supported_features.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/devstack/override-defaults
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9863 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/devstack/plugin.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12081 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/devstack/create_config
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1241 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tools/update-from-global-requirements.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/tools/db/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7031 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tools/db/schema_diff.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9057 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tools/db/ec2api-db-setup
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tools/db/import-nova-ec2-data.sql
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11899 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/tools/colorizer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59559 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31717 2019-09-25 17:36:59.000000 ec2-api-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/HACKING.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11138 2019-09-25 17:36:21.000000 ec2-api-9.0.0.0rc1/install.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.646014 ec2-api-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2021-02-01 18:31:50.000000 ec2-api-9.0.1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2021-02-01 18:31:50.000000 ec2-api-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2021-02-01 18:32:40.000000 ec2-api-9.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2021-02-01 18:31:50.000000 ec2-api-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31993 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1301 2021-02-01 18:31:50.000000 ec2-api-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-02-01 18:31:50.000000 ec2-api-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65260 2021-02-01 18:32:40.646014 ec2-api-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59559 2021-02-01 18:31:50.000000 ec2-api-9.0.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.618014 ec2-api-9.0.1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.622014 ec2-api-9.0.1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2021-02-01 18:31:50.000000 ec2-api-9.0.1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-02-01 18:31:50.000000 ec2-api-9.0.1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57006 2021-02-01 18:31:50.000000 ec2-api-9.0.1/api-ref/source/supported_features.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-02-01 18:31:50.000000 ec2-api-9.0.1/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.622014 ec2-api-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-01 18:31:50.000000 ec2-api-9.0.1/devstack/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12081 2021-02-01 18:31:50.000000 ec2-api-9.0.1/devstack/create_config
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2021-02-01 18:31:50.000000 ec2-api-9.0.1/devstack/override-defaults
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9770 2021-02-01 18:31:50.000000 ec2-api-9.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-02-01 18:31:50.000000 ec2-api-9.0.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.618014 ec2-api-9.0.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.622014 ec2-api-9.0.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3001 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.622014 ec2-api-9.0.1/doc/source/configuration/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.622014 ec2-api-9.0.1/doc/source/configuration/_flagmappings/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4201 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/_flagmappings/ec2api.flagmappings
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/_flagmappings/ec2api.headers
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/metadata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.626014 ec2-api-9.0.1/doc/source/configuration/tables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-clients.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-common.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-database.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2016 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-ec2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-metadata.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-s3.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/configuration/tables/ec2api-service.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/hacking.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.626014 ec2-api-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/credentials-creation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/database-creation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/endpoints-creation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/install-devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/install-manual.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      827 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/install-sh.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/metadata-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2021-02-01 18:31:50.000000 ec2-api-9.0.1/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.626014 ec2-api-9.0.1/ec2_api.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65260 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-02-01 18:32:40.000000 ec2-api-9.0.1/ec2_api.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.626014 ec2-api-9.0.1/ec2api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.630014 ec2-api-9.0.1/ec2api/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20508 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/apirequest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1423 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7486 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88086 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/cloud.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17919 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/customer_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6958 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/dhcp_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19075 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/ec2utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/faults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44482 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74331 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5372 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/internet_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/key_pair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27378 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/network_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30502 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/route_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24865 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5923 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8916 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3908 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7281 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9345 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7785 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/vpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21863 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/vpn_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8618 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/api/vpn_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6548 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/cmd/api_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/cmd/api_s3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3781 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/migrate.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/versions/001_juno.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15172 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11486 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/metadata/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11455 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/metadata/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/metadata/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/paths.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/s3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/s3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/s3/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14197 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/s3/s3server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5701 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.634014 ec2-api-9.0.1/ec2api/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/botocoreclient.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/ec2api/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/abs.tar.gz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13191 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79696 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10232 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/fakes_request_response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18157 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/matchers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/rel.tar.gz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30807 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_api_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5760 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_apirequest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4430 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2435 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_customer_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20627 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_db_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_dhcp_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11227 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_ec2_validate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26406 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_ec2utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_faults.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42764 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   100441 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12986 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_integrated_scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10271 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_internet_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4440 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_key_pair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15624 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_metadata_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7631 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31441 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_network_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_private_key.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56309 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_route_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_s3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26679 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6225 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15025 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9941 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_tools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9828 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17074 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_vpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39118 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_vpn_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19411 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/test_vpn_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7662 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/tests/unit/tools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18200 2021-02-01 18:31:50.000000 ec2-api-9.0.1/ec2api/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.618014 ec2-api-9.0.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/etc/ec2api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 18:31:50.000000 ec2-api-9.0.1/etc/ec2api/README-ec2api.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2021-02-01 18:31:50.000000 ec2-api-9.0.1/etc/ec2api/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2021-02-01 18:31:50.000000 ec2-api-9.0.1/etc/ec2api/ec2api-config-generator.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11049 2021-02-01 18:31:50.000000 ec2-api-9.0.1/install.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2021-02-01 18:31:50.000000 ec2-api-9.0.1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.618014 ec2-api-9.0.1/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.618014 ec2-api-9.0.1/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron-full/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron-full/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2176 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron-full/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/playbooks/legacy/ec2-api-rally-fakevirt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-rally-fakevirt/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2256 2021-02-01 18:31:50.000000 ec2-api-9.0.1/playbooks/legacy/ec2-api-rally-fakevirt/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/rally-scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1835 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/ec2-api-fakevirt.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/rally-scenarios/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/extra/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.642014 ec2-api-9.0.1/rally-scenarios/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3621 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_ec2_creds.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13458 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_ec2_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3445 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8704 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/plugins/ec2api_plugin.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       42 2021-02-01 18:31:50.000000 ec2-api-9.0.1/rally-scenarios/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2021-02-01 18:31:50.000000 ec2-api-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2021-02-01 18:32:40.646014 ec2-api-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 18:31:50.000000 ec2-api-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2021-02-01 18:31:50.000000 ec2-api-9.0.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.646014 ec2-api-9.0.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11899 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tools/colorizer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:32:40.646014 ec2-api-9.0.1/tools/db/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9057 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tools/db/ec2api-db-setup
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tools/db/import-nova-ec2-data.sql
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7031 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tools/db/schema_diff.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1241 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tools/update-from-global-requirements.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2021-02-01 18:31:50.000000 ec2-api-9.0.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ec2-api-9.0.0.0rc1/PKG-INFO` & `ec2-api-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ec2-api
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Ec2api Service
 Home-page: https://launchpad.net/ec2-api
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_images.py` & `ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_images.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_ec2_creds.py` & `ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_ec2_creds.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/rally-scenarios/plugins/ec2api_plugin.py` & `ec2-api-9.0.1/rally-scenarios/plugins/ec2api_plugin.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/rally-scenarios/plugins/context_plugin_ec2_objects.py` & `ec2-api-9.0.1/rally-scenarios/plugins/context_plugin_ec2_objects.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/rally-scenarios/ec2-api-fakevirt.yaml` & `ec2-api-9.0.1/rally-scenarios/ec2-api-fakevirt.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/etc/ec2api/api-paste.ini` & `ec2-api-9.0.1/etc/ec2api/api-paste.ini`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/setup.py` & `ec2-api-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/LICENSE` & `ec2-api-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2_api.egg-info/PKG-INFO` & `ec2-api-9.0.1/ec2_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ec2-api
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Ec2api Service
 Home-page: https://launchpad.net/ec2-api
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `ec2-api-9.0.0.0rc1/ec2_api.egg-info/SOURCES.txt` & `ec2-api-9.0.1/ec2_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/setup.cfg` & `ec2-api-9.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = ec2-api
-version = 9.0.0
 summary = OpenStack Ec2api Service
 description-file = 
 	README.rst
 license = Apache License, Version 2.0
 author = OpenStack
 author-email = openstack-discuss@lists.openstack.org
 home-page = https://launchpad.net/ec2-api
```

### Comparing `ec2-api-9.0.0.0rc1/doc/source/conf.py` & `ec2-api-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/index.rst` & `ec2-api-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/metadata-configuration.rst` & `ec2-api-9.0.1/doc/source/install/metadata-configuration.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/index.rst` & `ec2-api-9.0.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/credentials-creation.rst` & `ec2-api-9.0.1/doc/source/install/credentials-creation.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/install-sh.rst` & `ec2-api-9.0.1/doc/source/install/install-sh.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/configuration.rst` & `ec2-api-9.0.1/doc/source/install/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,13 +48,12 @@
      connection = mysql+pymysql://root:password@127.0.0.1/ec2api?charset=utf8
 
 and cache if you want to use it.
 
 .. code-block:: ini
 
      [cache]
-     backend = oslo_cache.dict
      enabled = True
 
 You can look for other configuration options in the `Configuration Reference`_
 
 .. _`Configuration Reference`: ../configuration/api.html
```

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/database-creation.rst` & `ec2-api-9.0.1/doc/source/install/database-creation.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/install-manual.rst` & `ec2-api-9.0.1/doc/source/install/install-manual.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/install/verify.rst` & `ec2-api-9.0.1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-ec2.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-ec2.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-clients.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-clients.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-service.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-service.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-metadata.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-metadata.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-common.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-common.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-database.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-database.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/tables/ec2api-s3.inc` & `ec2-api-9.0.1/doc/source/configuration/tables/ec2api-s3.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/doc/source/configuration/_flagmappings/ec2api.flagmappings` & `ec2-api-9.0.1/doc/source/configuration/_flagmappings/ec2api.flagmappings`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/CONTRIBUTING.rst` & `ec2-api-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/config.py` & `ec2-api-9.0.1/ec2api/config.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/metadata/__init__.py` & `ec2-api-9.0.1/ec2api/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/metadata/api.py` & `ec2-api-9.0.1/ec2api/metadata/api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/metadata/opts.py` & `ec2-api-9.0.1/ec2api/metadata/opts.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/paths.py` & `ec2-api-9.0.1/ec2api/paths.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/service.py` & `ec2-api-9.0.1/ec2api/service.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/version.py` & `ec2-api-9.0.1/ec2api/version.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/__init__.py` & `ec2-api-9.0.1/ec2api/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/wsgi.py` & `ec2-api-9.0.1/ec2api/wsgi.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/apirequest.py` & `ec2-api-9.0.1/ec2api/api/apirequest.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/instance.py` & `ec2-api-9.0.1/ec2api/api/instance.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/route_table.py` & `ec2-api-9.0.1/ec2api/api/route_table.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/tag.py` & `ec2-api-9.0.1/ec2api/api/tag.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/volume.py` & `ec2-api-9.0.1/ec2api/api/volume.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/security_group.py` & `ec2-api-9.0.1/ec2api/api/security_group.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/vpc.py` & `ec2-api-9.0.1/ec2api/api/vpc.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/auth.py` & `ec2-api-9.0.1/ec2api/api/auth.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/__init__.py` & `ec2-api-9.0.1/ec2api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/internet_gateway.py` & `ec2-api-9.0.1/ec2api/api/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/key_pair.py` & `ec2-api-9.0.1/ec2api/api/key_pair.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/image.py` & `ec2-api-9.0.1/ec2api/api/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,18 +898,18 @@
                 for part_name in image_parts:
                     part = _s3_download_file(s3_client, bucket_name,
                                              part_name, image_path)
                     parts.append(part)
 
                 # NOTE(vish): this may be suboptimal, should we use cat?
                 enc_filename = os.path.join(image_path, 'image.encrypted')
-                with open(enc_filename, 'w') as combined:
+                with open(enc_filename, 'wb') as combined:
                     for filename in parts:
-                        with open(filename) as part:
-                            shutil.copyfileobj(part, combined)
+                        with open(filename, "rb") as part:
+                            combined.write(part.read())
 
             except Exception:
                 LOG.exception('Failed to download %(image_location)s '
                               'to %(image_path)s', log_vars)
                 _update_image_state('failed_download')
                 return
 
@@ -931,15 +931,15 @@
                 LOG.exception('Failed to untar %(image_location)s '
                               'to %(image_path)s', log_vars)
                 _update_image_state('failed_untar')
                 return
 
             _update_image_state('uploading')
             try:
-                with open(unz_filename) as image_file:
+                with open(unz_filename, "rb") as image_file:
                     glance.images.upload(image.id, image_file)
             except Exception:
                 LOG.exception('Failed to upload %(image_location)s '
                               'to %(image_path)s', log_vars)
                 _update_image_state('failed_upload')
                 return
 
@@ -1009,35 +1009,30 @@
     return metadata, image_parts, encrypted_key, encrypted_iv
 
 
 def _s3_download_file(s3_client, bucket_name, filename, local_dir):
     s3_object = s3_client.get_object(Bucket=bucket_name, Key=filename)
     local_filename = os.path.join(local_dir, os.path.basename(filename))
     body = s3_object['Body']
-    with open(local_filename, 'w') as f:
-        if isinstance(body, six.string_types):
-            f.write(body)
-        else:
-            # TODO(andrey-mp): check big objects
-            f.write(body.read())
-        f.close()
+    with open(local_filename, 'wb') as f:
+        f.write(body.read())
     return local_filename
 
 
 def _s3_decrypt_image(context, encrypted_filename, encrypted_key,
                       encrypted_iv, decrypted_filename):
     encrypted_key = binascii.a2b_hex(encrypted_key)
     encrypted_iv = binascii.a2b_hex(encrypted_iv)
     try:
-        key = _decrypt_text(encrypted_key)
+        key = _decrypt_text(encrypted_key).decode()
     except Exception as exc:
         msg = _('Failed to decrypt private key: %s') % exc
         raise exception.EC2Exception(msg)
     try:
-        iv = _decrypt_text(encrypted_iv)
+        iv = _decrypt_text(encrypted_iv).decode()
     except Exception as exc:
         msg = _('Failed to decrypt initialization vector: %s') % exc
         raise exception.EC2Exception(msg)
 
     try:
         processutils.execute('openssl', 'enc',
                              '-d', '-aes-128-cbc',
```

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/customer_gateway.py` & `ec2-api-9.0.1/ec2api/api/customer_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/subnet.py` & `ec2-api-9.0.1/ec2api/api/subnet.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/vpn_connection.py` & `ec2-api-9.0.1/ec2api/api/vpn_connection.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/ec2utils.py` & `ec2-api-9.0.1/ec2api/api/ec2utils.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/common.py` & `ec2-api-9.0.1/ec2api/api/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,19 +371,20 @@
         if max_results and max_results > 1000:
             max_results = 1000
         formatted_items = sorted(formatted_items,
                                  key=operator.itemgetter(self.SORT_KEY))
 
         next_item = 0
         if next_token:
-            next_item = int(base64.b64decode(next_token))
+            next_item = int(base64.b64decode(next_token).decode())
         if next_item:
             formatted_items = formatted_items[next_item:]
         if max_results and max_results < len(formatted_items):
-            self.next_token = base64.b64encode(str(next_item + max_results))
+            self.next_token = base64.b64encode(
+                str(next_item + max_results).encode())
             formatted_items = formatted_items[:max_results]
 
         return formatted_items
 
     def is_selected_item(self, context, os_item_name, item):
         return (os_item_name in self.names or
                 (item and item['id'] in self.ids))
```

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/faults.py` & `ec2-api-9.0.1/ec2api/api/faults.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/address.py` & `ec2-api-9.0.1/ec2api/api/address.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/dhcp_options.py` & `ec2-api-9.0.1/ec2api/api/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/snapshot.py` & `ec2-api-9.0.1/ec2api/api/snapshot.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/validator.py` & `ec2-api-9.0.1/ec2api/api/validator.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/availability_zone.py` & `ec2-api-9.0.1/ec2api/api/availability_zone.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/vpn_gateway.py` & `ec2-api-9.0.1/ec2api/api/vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/network_interface.py` & `ec2-api-9.0.1/ec2api/api/network_interface.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/opts.py` & `ec2-api-9.0.1/ec2api/api/opts.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/api/cloud.py` & `ec2-api-9.0.1/ec2api/api/cloud.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migration.py` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/api.py` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/manage.py` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/manage.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/versions/001_juno.py` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/versions/001_juno.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/migrate_repo/migrate.cfg` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/migrate_repo/migrate.cfg`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/sqlalchemy/models.py` & `ec2-api-9.0.1/ec2api/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/__init__.py` & `ec2-api-9.0.1/ec2api/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/migration.py` & `ec2-api-9.0.1/ec2api/db/migration.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/db/api.py` & `ec2-api-9.0.1/ec2api/db/api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/clients.py` & `ec2-api-9.0.1/ec2api/clients.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/botocoreclient.py` & `ec2-api-9.0.1/ec2api/tests/botocoreclient.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_security_group.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_security_group.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/fakes.py` & `ec2-api-9.0.1/ec2api/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_private_key.pem` & `ec2-api-9.0.1/ec2api/tests/unit/test_private_key.pem`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_common.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_middleware.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_volume.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_volume.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_apirequest.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_apirequest.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_integrated_scenario.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_integrated_scenario.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_address.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_address.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_network_interface.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_subnet.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_subnet.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_instance.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_instance.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_internet_gateway.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/__init__.py` & `ec2-api-9.0.1/ec2api/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/fakes_request_response.py` & `ec2-api-9.0.1/ec2api/tests/unit/fakes_request_response.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/base.py` & `ec2-api-9.0.1/ec2api/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_clients.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/tools.py` & `ec2-api-9.0.1/ec2api/tests/unit/tools.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_availability_zone.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_snapshot.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_context.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpn_gateway.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_hacking.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_db_api.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_db_api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_image.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_s3.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_s3.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_ec2_validate.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_ec2_validate.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_metadata.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_customer_gateway.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_customer_gateway.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpn_connection.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_vpn_connection.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_dhcp_options.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_dhcp_options.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/matchers.py` & `ec2-api-9.0.1/ec2api/tests/unit/matchers.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_faults.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_faults.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_vpc.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_vpc.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_route_table.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_route_table.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_metadata_api.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_metadata_api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_tools.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_tools.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_api_init.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_api_init.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_ec2utils.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_ec2utils.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_tag.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_tag.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/tests/unit/test_key_pair.py` & `ec2-api-9.0.1/ec2api/tests/unit/test_key_pair.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/s3/__init__.py` & `ec2-api-9.0.1/ec2api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/s3/s3server.py` & `ec2-api-9.0.1/ec2api/s3/s3server.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/s3/opts.py` & `ec2-api-9.0.1/ec2api/s3/opts.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/exception.py` & `ec2-api-9.0.1/ec2api/exception.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/cmd/__init__.py` & `ec2-api-9.0.1/ec2api/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/cmd/manage.py` & `ec2-api-9.0.1/ec2api/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/cmd/api.py` & `ec2-api-9.0.1/ec2api/cmd/api.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/cmd/api_metadata.py` & `ec2-api-9.0.1/ec2api/cmd/api_metadata.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/cmd/api_s3.py` & `ec2-api-9.0.1/ec2api/cmd/api_s3.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/i18n.py` & `ec2-api-9.0.1/ec2api/i18n.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/context.py` & `ec2-api-9.0.1/ec2api/context.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/hacking/checks.py` & `ec2-api-9.0.1/ec2api/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/opts.py` & `ec2-api-9.0.1/ec2api/opts.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ec2api/utils.py` & `ec2-api-9.0.1/ec2api/utils.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/.zuul.yaml` & `ec2-api-9.0.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron-full/run.yaml` & `ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron-full/run.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-functional-neutron/run.yaml` & `ec2-api-9.0.1/playbooks/legacy/ec2-api-functional-neutron/run.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-rally-fakevirt/run.yaml` & `ec2-api-9.0.1/playbooks/legacy/ec2-api-rally-fakevirt/run.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/playbooks/legacy/ec2-api-rally-fakevirt/post.yaml` & `ec2-api-9.0.1/playbooks/legacy/ec2-api-rally-fakevirt/post.yaml`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/api-ref/source/conf.py` & `ec2-api-9.0.1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/api-ref/source/supported_features.inc` & `ec2-api-9.0.1/api-ref/source/supported_features.inc`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/devstack/plugin.sh` & `ec2-api-9.0.1/devstack/plugin.sh`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,14 @@
 
 EC2API_RABBIT_VHOST=${EC2API_RABBIT_VHOST:-''}
 
 EC2API_ADMIN_USER=${EC2API_ADMIN_USER:-ec2api}
 
 EC2API_KEYSTONE_SIGNING_DIR=${EC2API_KEYSTONE_SIGNING_DIR:-/tmp/keystone-signing-ec2api}
 
-CACHE_BACKEND="oslo_cache.dict"
-
 # Support entry points installation of console scripts
 if [[ -d $EC2API_DIR/bin ]]; then
     EC2API_BIN_DIR=$EC2API_DIR/bin
 else
     EC2API_BIN_DIR=$(get_python_exec_prefix)
 fi
 
@@ -229,15 +227,14 @@
         iniset $Q_META_CONF_FILE DEFAULT nova_metadata_port 8789
     else
         # with nova-network
         iniset $NOVA_CONF DEFAULT metadata_port 8789
         iniset $NOVA_CONF neutron service_metadata_proxy True
     fi
     iniset $EC2API_CONF_FILE cache enabled True
-    iniset $EC2API_CONF_FILE cache backend "$CACHE_BACKEND"
 
     if create_x509_server_key; then
       iniset $EC2API_CONF_FILE DEFAULT x509_root_private_key "$CA_KEY"
     fi
 }
```

### Comparing `ec2-api-9.0.0.0rc1/devstack/create_config` & `ec2-api-9.0.1/devstack/create_config`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/AUTHORS` & `ec2-api-9.0.1/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Alexandre Levine <alevine@cloudscaling.com>
 Alexandre Levine <alexandrelevine@gmail.com>
+Alfredo Moralejo <amoralej@redhat.com>
 Andreas Jaeger <aj@suse.com>
 Andrey Kurilin <akurilin@mirantis.com>
 Andrey Kurilin <andr.kurilin@gmail.com>
 Andrey Pavlov <andrey-mp@yandex.ru>
 Andrey Pavlov <andrey.mp@gmail.com>
 Anh Tran <anhtt@vn.fujitsu.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 ChangBo Guo(gcb) <eric.guo@easystack.cn>
 Corey Bryant <corey.bryant@canonical.com>
 Dirk Mueller <dirk@dmllr.de>
+Dmitry_Eremeev <Dmitry-Eremeev-progmaticlab@yandex.ru>
 Doug Hellmann <doug@doughellmann.com>
 Emilien Macchi <emilien@redhat.com>
 Feodor Tersin <ftersin@cloudscaling.com>
 Feodor Tersin <ftersin@hotmail.com>
 Flavio Percoco <flaper87@gmail.com>
 Gage Hugo <gagehugo@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
@@ -24,14 +26,15 @@
 Jeremy Stanley <fungi@yuggoth.org>
 Johannes Grassler <johannes.grassler@suse.com>
 Ken'ichi Ohmichi <ken-oomichi@wx.jp.nec.com>
 M V P Nitesh <m.nitesh@nectechnologies.in>
 Marcos Fermin Lobo <marcos.fermin.lobo@cern.ch>
 Ngo Quoc Cuong <cuongnq@vn.fujitsu.com>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
+OpenStack Release Bot <infra-root@openstack.org>
 Rafael Folco <rfolco@redhat.com>
 Ronald Bradford <ronald.bradford@gmail.com>
 Sean Dague <sean@dague.net>
 Stefan Nica <snica@suse.com>
 Stephen Finucane <stephenfin@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Tony Breeds <tony@bakeyournoodle.com>
```

### Comparing `ec2-api-9.0.0.0rc1/tox.ini` & `ec2-api-9.0.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [testenv]
 usedevelop = True
 # tox is silly... these need to be separated by a newline....
 whitelist_externals = bash
                       find
                       rm
                       env
-install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt} {opts} {packages}
+install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train} {opts} {packages}
 setenv = VIRTUAL_ENV={envdir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
 deps = -r{toxinidir}/test-requirements.txt
 commands =
   find . -type f -name "*.pyc" -delete
```

### Comparing `ec2-api-9.0.0.0rc1/test-requirements.txt` & `ec2-api-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/tools/update-from-global-requirements.sh` & `ec2-api-9.0.1/tools/update-from-global-requirements.sh`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/tools/db/schema_diff.py` & `ec2-api-9.0.1/tools/db/schema_diff.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/tools/db/ec2api-db-setup` & `ec2-api-9.0.1/tools/db/ec2api-db-setup`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/tools/db/import-nova-ec2-data.sql` & `ec2-api-9.0.1/tools/db/import-nova-ec2-data.sql`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/tools/colorizer.py` & `ec2-api-9.0.1/tools/colorizer.py`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/lower-constraints.txt` & `ec2-api-9.0.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/README.rst` & `ec2-api-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/ChangeLog` & `ec2-api-9.0.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Fix AMI image registration
+* Revert "temporary disable functional tests"
+* Fix encoding/decoding in paging of universal describer class
+* Remove version attribute from setup.cfg
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Replace git.openstack.org URLs with opendev.org URLs
 * Add Python 3 Train unit tests
 * temporary disable functional tests
 * Update api-ref location
 * tests: Avoid using mock wraps
 * OpenDev Migration Patch
```

### Comparing `ec2-api-9.0.0.0rc1/requirements.txt` & `ec2-api-9.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/HACKING.rst` & `ec2-api-9.0.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `ec2-api-9.0.0.0rc1/install.sh` & `ec2-api-9.0.1/install.sh`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 NOVA_CONF=/etc/nova/nova.conf
 CONF_FILE=$CONF_DIR/ec2api.conf
 APIPASTE_FILE=$CONF_DIR/api-paste.ini
 
 DATA_DIR=${DATA_DIR:-/var/lib/ec2api}
 AUTH_CACHE_DIR=${AUTH_CACHE_DIR:-/var/cache/ec2api}
 
-CACHE_BACKEND='oslo_cache.dict'
-
 #Check for environment
 if [[ -z "$OS_AUTH_URL" || -z "$OS_USERNAME" || -z "$OS_PASSWORD" ]]; then
     echo "Please set OS_AUTH_URL, OS_USERNAME, OS_PASSWORD"
     exit 1
 fi
 if [[ -z "$OS_TENANT_NAME" && -z "$OS_PROJECT_NAME" ]]; then
     echo "Please set OS_TENANT_NAME or OS_PROJECT_NAME"
@@ -301,15 +299,14 @@
 iniset $CONF_FILE $GROUP_AUTHTOKEN project_name $SERVICE_TENANT
 iniset $CONF_FILE $GROUP_AUTHTOKEN project_domain_name $SERVICE_DOMAIN_NAME
 iniset $CONF_FILE $GROUP_AUTHTOKEN user_domain_name $SERVICE_DOMAIN_NAME
 iniset $CONF_FILE $GROUP_AUTHTOKEN auth_type password
 
 GROUP_CACHE="cache"
 iniset $CONF_FILE $GROUP_CACHE enabled True
-iniset $CONF_FILE $GROUP_CACHE backend "$CACHE_BACKEND"
 
 if [[ -f "$NOVA_CONF" ]]; then
     # NOTE(ft): use swift instead internal s3 server if enabled
     if [[ -n $(openstack catalog show object-store 2>/dev/null) ]] &&
             [[ -n $(openstack catalog show s3 2>/dev/null) ]]; then
         s3_host="127.0.0.1"
         if ini_has_option "$NOVA_CONF" DEFAULT "s3_host"; then
```

