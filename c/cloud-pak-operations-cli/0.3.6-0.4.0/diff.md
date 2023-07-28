# Comparing `tmp/cloud-pak-operations-cli-0.3.6.tar.gz` & `tmp/cloud-pak-operations-cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-pak-operations-cli-0.3.6.tar", last modified: Thu Jun 15 14:41:24 2023, max compression
+gzip compressed data, was "cloud-pak-operations-cli-0.4.0.tar", last modified: Fri Jul 28 06:51:23 2023, max compression
```

## Comparing `cloud-pak-operations-cli-0.3.6.tar` & `cloud-pak-operations-cli-0.4.0.tar`

### file list

```diff
@@ -1,319 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 14:41:24.000000 cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.805862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/download_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/get-shell-completion-script-location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/store_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/adm/update_dev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/get_cluster_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_odf_storage_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/use.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.809862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/accept_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add_worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/copy_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/create_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/disable_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_inf_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/edit_worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/enable_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/init_node_for_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/reboot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/redeploy_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/shutdown_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/transfer_ownership.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/check_cluster_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_default_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_max_hours.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quick_burn_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/wait_for_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/regenerate_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.813862 cloud-pak-operations-cli-0.3.6/cpo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/binaries_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/cluster_credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/config/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/cpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.801862 cloud-pak-operations-cli-0.3.6/cpo/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/deploy_odf_playbook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/abstract_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/openshift_playbook_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/click/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/cpd_service_spec_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/lazy_loading_multi_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/terraform_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.817862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.821862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.821862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/check_hostname_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocp_available_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/ocpplus_cluster_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/openshift_version_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/product_group_quota_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_max_hours_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/quick_burn_size_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/request_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/data/status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31273 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/ocp_plus_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/check_hostname_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/json_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_accept_transfer_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_add_additional_nodes_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_available_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_cluster_action_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_default_post_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disable_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_disk_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_enable_delete_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_get_manager_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_node_action_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_post_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_max_hours_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_quick_burn_sizes_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_resource_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_status_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/ocp_transfer_put_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/request_managers/quota_request_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/check_hostname_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/default_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/json_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_available_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_get_response_manager_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_post_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_max_hours_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_quick_burn_sizes_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_request_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/ocp_status_get_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/response_managers/quota_get_response_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.825862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/check_hostname_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_add_additional_nodes_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_available_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_disk_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_max_hours_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_quick_burn_sizes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_request_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_resource_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_status_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_transfer_put_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/quota_get_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/node_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/openshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/request_status_progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/ingress_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/jmespath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/token_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/user_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/global_pull_secret_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.829862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/oc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45780 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/openshift_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/auths_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/catalog_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/get_pod_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/kind_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/object_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/operator_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/utils/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/distribution_entry_point_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/package_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.833862 cloud-pak-operations-cli-0.3.6/cpo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/scripts/get_current_cluster_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/cpo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/importlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/cpo/utils/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-15 14:41:16.000000 cloud-pak-operations-cli-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 14:41:24.837862 cloud-pak-operations-cli-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-28 06:51:23.000000 cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/config/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/download_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/get-shell-completion-script-location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/store_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/adm/update_dev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.120691 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/get_cluster_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/install_nfs_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/install_odf_storage_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/use.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/regenerate_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/config/binaries_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/config/cluster_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/config/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/cpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.116691 cloud-pak-operations-cli-0.4.0/cpo/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/deps/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/deps/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/deps/playbooks/deploy_odf_playbook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.124691 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/abstract_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/openshift_playbook_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/click/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/click/cpd_service_spec_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/click/lazy_loading_multi_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/dependency_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/terraform_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/ingress_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.128692 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/jmespath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/generic_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/generic_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/user_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/data/global_pull_secret_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.132692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/nfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/nfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/openshift_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/auths_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/catalog_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/get_pod_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/kind_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/object_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/operator_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/utils/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/distribution_entry_point_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/cpo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/scripts/get_current_cluster_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/cpo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/cpo/utils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 06:51:13.000000 cloud-pak-operations-cli-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 06:51:23.136692 cloud-pak-operations-cli-0.4.0/setup.cfg
```

### Comparing `cloud-pak-operations-cli-0.3.6/LICENSE` & `cloud-pak-operations-cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/PKG-INFO` & `cloud-pak-operations-cli-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.3.6
+Version: 0.4.0
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IBM Cloud Pak Operations CLI
 
 <div align="center">
     <p>
@@ -23,21 +23,19 @@
         <a href="https://github.com/IBM/cloud-pak-operations-cli/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/IBM/cloud-pak-operations-cli?style=for-the-badge"></a>
         <a href="https://github.com/IBM/cloud-pak-operations-cli/actions?query=workflow%3A%22Python+Testing%22+branch%3Amaster"><img alt="GitHub Workflow Status (branch)" src="https://img.shields.io/github/actions/workflow/status/IBM/cloud-pak-operations-cli/python-package.yml?branch=master&style=for-the-badge"></a>
     </p>
 </div>
 
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://github.com/IBM/cpd-cli) (cpd-cli).
 
-For IBM-internal users, the IBM Cloud Pak Operations CLI additionally supports managing OpenShift clusters on Fyre.
-
 ## Installation & Configuration
 
 ### Installation
 
-#### Python installation (3.8 or higher)
+#### Python installation (3.10 or higher)
 
 - macOS (requires [Homebrew](https://brew.sh)):
 
   ```shell
   brew install python
   ```
 
@@ -221,22 +219,14 @@
 
   ```shell
   cpo cluster install-odf-storage-classes
   ```
 
   Note: Currently, opinionated configuration values are used for deploying the `StorageCluster` custom resource (see [Ansible playbook](cpo/deps/playbooks/deploy_odf_playbook.yaml)).
 
-### IBM-internal
-
-- Enable Fyre-specific commands:
-
-  ```shell
-  cpo adm config set --key fyre_commands --value true
-  ```
-
 ## Development
 
 - [Development Guide](docs/development_guide.md)
 
 ## Known issues
 
 ### OpenShift CLI (macOS)
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.6 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.4.0 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
-System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # IBM Cloud Pak Operations CLI
    [GitHub_license] [GitHub_issues] [GitHub_stars] [GitHub_Workflow_Status_
                                    (branch)]
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat
 OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top
 of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://
-github.com/IBM/cpd-cli) (cpd-cli). For IBM-internal users, the IBM Cloud Pak
-Operations CLI additionally supports managing OpenShift clusters on Fyre. ##
-Installation & Configuration ### Installation #### Python installation (3.8 or
-higher) - macOS (requires [Homebrew](https://brew.sh)): ```shell brew install
-python ``` - Windows: - [Winget](https://github.com/microsoft/winget-cli):
-```shell winget install --exact --id=Python.Python.3.11 ``` - [Chocolatey]
-(https://chocolatey.org) ```shell choco install python ``` #### IBM Cloud Pak
-Operations CLI installation and update (latest release build)
+github.com/IBM/cpd-cli) (cpd-cli). ## Installation & Configuration ###
+Installation #### Python installation (3.10 or higher) - macOS (requires
+[Homebrew](https://brew.sh)): ```shell brew install python ``` - Windows: -
+[Winget](https://github.com/microsoft/winget-cli): ```shell winget install --
+exact --id=Python.Python.3.11 ``` - [Chocolatey](https://chocolatey.org)
+```shell choco install python ``` #### IBM Cloud Pak Operations CLI
+installation and update (latest release build)
 Action                              Command
 Installation (provides cpo command) ```shell pip3 install cloud-pak-operations-
                                     cli ```
 Update                              ```shell pip3 install --upgrade cloud-pak-
                                     operations-cli ```
 #### IBM Cloud Pak Operations CLI installation and update (latest development
 code)
@@ -52,14 +51,13 @@
 cluster: ```shell cpo cluster get-cluster-access-token ``` - Manage the global
 pull secret: ```shell cpo cluster pull-secret ``` ### Storage management -
 Deploy Kubernetes NFS Subdir External Provisioner: ```shell cpo cluster
 install-nfs-storage-class ``` - Deploy OpenShift Data Foundation (Linux and
 macOS): ```shell cpo cluster install-odf-storage-classes ``` Note: Currently,
 opinionated configuration values are used for deploying the `StorageCluster`
 custom resource (see [Ansible playbook](cpo/deps/playbooks/
-deploy_odf_playbook.yaml)). ### IBM-internal - Enable Fyre-specific commands:
-```shell cpo adm config set --key fyre_commands --value true ``` ## Development
-- [Development Guide](docs/development_guide.md) ## Known issues ### OpenShift
-CLI (macOS) ```shell Unable to connect to the server: dial tcp: lookup â¦ on
-â¦:53: no such host ``` - [GitHub issue](https://github.com/openshift/oc/
-issues/315) - Workaround: Edit `/etc/hosts` and add IP address of OpenShift
-cluster - Example: ``` 9.AA.BBB.CC your.cluster.domain.com ```
+deploy_odf_playbook.yaml)). ## Development - [Development Guide](docs/
+development_guide.md) ## Known issues ### OpenShift CLI (macOS) ```shell Unable
+to connect to the server: dial tcp: lookup â¦ on â¦:53: no such host ``` -
+[GitHub issue](https://github.com/openshift/oc/issues/315) - Workaround: Edit
+`/etc/hosts` and add IP address of OpenShift cluster - Example: ``` 9.AA.BBB.CC
+your.cluster.domain.com ```
```

### Comparing `cloud-pak-operations-cli-0.3.6/README.md` & `cloud-pak-operations-cli-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,19 @@
         <a href="https://github.com/IBM/cloud-pak-operations-cli/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/IBM/cloud-pak-operations-cli?style=for-the-badge"></a>
         <a href="https://github.com/IBM/cloud-pak-operations-cli/actions?query=workflow%3A%22Python+Testing%22+branch%3Amaster"><img alt="GitHub Workflow Status (branch)" src="https://img.shields.io/github/actions/workflow/status/IBM/cloud-pak-operations-cli/python-package.yml?branch=master&style=for-the-badge"></a>
     </p>
 </div>
 
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://github.com/IBM/cpd-cli) (cpd-cli).
 
-For IBM-internal users, the IBM Cloud Pak Operations CLI additionally supports managing OpenShift clusters on Fyre.
-
 ## Installation & Configuration
 
 ### Installation
 
-#### Python installation (3.8 or higher)
+#### Python installation (3.10 or higher)
 
 - macOS (requires [Homebrew](https://brew.sh)):
 
   ```shell
   brew install python
   ```
 
@@ -205,22 +203,14 @@
 
   ```shell
   cpo cluster install-odf-storage-classes
   ```
 
   Note: Currently, opinionated configuration values are used for deploying the `StorageCluster` custom resource (see [Ansible playbook](cpo/deps/playbooks/deploy_odf_playbook.yaml)).
 
-### IBM-internal
-
-- Enable Fyre-specific commands:
-
-  ```shell
-  cpo adm config set --key fyre_commands --value true
-  ```
-
 ## Development
 
 - [Development Guide](docs/development_guide.md)
 
 ## Known issues
 
 ### OpenShift CLI (macOS)
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
 # IBM Cloud Pak Operations CLI
    [GitHub_license] [GitHub_issues] [GitHub_stars] [GitHub_Workflow_Status_
                                    (branch)]
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat
 OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top
 of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://
-github.com/IBM/cpd-cli) (cpd-cli). For IBM-internal users, the IBM Cloud Pak
-Operations CLI additionally supports managing OpenShift clusters on Fyre. ##
-Installation & Configuration ### Installation #### Python installation (3.8 or
-higher) - macOS (requires [Homebrew](https://brew.sh)): ```shell brew install
-python ``` - Windows: - [Winget](https://github.com/microsoft/winget-cli):
-```shell winget install --exact --id=Python.Python.3.11 ``` - [Chocolatey]
-(https://chocolatey.org) ```shell choco install python ``` #### IBM Cloud Pak
-Operations CLI installation and update (latest release build)
+github.com/IBM/cpd-cli) (cpd-cli). ## Installation & Configuration ###
+Installation #### Python installation (3.10 or higher) - macOS (requires
+[Homebrew](https://brew.sh)): ```shell brew install python ``` - Windows: -
+[Winget](https://github.com/microsoft/winget-cli): ```shell winget install --
+exact --id=Python.Python.3.11 ``` - [Chocolatey](https://chocolatey.org)
+```shell choco install python ``` #### IBM Cloud Pak Operations CLI
+installation and update (latest release build)
 Action                              Command
 Installation (provides cpo command) ```shell pip3 install cloud-pak-operations-
                                     cli ```
 Update                              ```shell pip3 install --upgrade cloud-pak-
                                     operations-cli ```
 #### IBM Cloud Pak Operations CLI installation and update (latest development
 code)
@@ -44,14 +43,13 @@
 cluster: ```shell cpo cluster get-cluster-access-token ``` - Manage the global
 pull secret: ```shell cpo cluster pull-secret ``` ### Storage management -
 Deploy Kubernetes NFS Subdir External Provisioner: ```shell cpo cluster
 install-nfs-storage-class ``` - Deploy OpenShift Data Foundation (Linux and
 macOS): ```shell cpo cluster install-odf-storage-classes ``` Note: Currently,
 opinionated configuration values are used for deploying the `StorageCluster`
 custom resource (see [Ansible playbook](cpo/deps/playbooks/
-deploy_odf_playbook.yaml)). ### IBM-internal - Enable Fyre-specific commands:
-```shell cpo adm config set --key fyre_commands --value true ``` ## Development
-- [Development Guide](docs/development_guide.md) ## Known issues ### OpenShift
-CLI (macOS) ```shell Unable to connect to the server: dial tcp: lookup â¦ on
-â¦:53: no such host ``` - [GitHub issue](https://github.com/openshift/oc/
-issues/315) - Workaround: Edit `/etc/hosts` and add IP address of OpenShift
-cluster - Example: ``` 9.AA.BBB.CC your.cluster.domain.com ```
+deploy_odf_playbook.yaml)). ## Development - [Development Guide](docs/
+development_guide.md) ## Known issues ### OpenShift CLI (macOS) ```shell Unable
+to connect to the server: dial tcp: lookup â¦ on â¦:53: no such host ``` -
+[GitHub issue](https://github.com/openshift/oc/issues/315) - Workaround: Edit
+`/etc/hosts` and add IP address of OpenShift cluster - Example: ``` 9.AA.BBB.CC
+your.cluster.domain.com ```
```

### Comparing `cloud-pak-operations-cli-0.3.6/cloud_pak_operations_cli.egg-info/PKG-INFO` & `cloud-pak-operations-cli-0.4.0/cloud_pak_operations_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.3.6
+Version: 0.4.0
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IBM Cloud Pak Operations CLI
 
 <div align="center">
     <p>
@@ -23,21 +23,19 @@
         <a href="https://github.com/IBM/cloud-pak-operations-cli/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/IBM/cloud-pak-operations-cli?style=for-the-badge"></a>
         <a href="https://github.com/IBM/cloud-pak-operations-cli/actions?query=workflow%3A%22Python+Testing%22+branch%3Amaster"><img alt="GitHub Workflow Status (branch)" src="https://img.shields.io/github/actions/workflow/status/IBM/cloud-pak-operations-cli/python-package.yml?branch=master&style=for-the-badge"></a>
     </p>
 </div>
 
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://github.com/IBM/cpd-cli) (cpd-cli).
 
-For IBM-internal users, the IBM Cloud Pak Operations CLI additionally supports managing OpenShift clusters on Fyre.
-
 ## Installation & Configuration
 
 ### Installation
 
-#### Python installation (3.8 or higher)
+#### Python installation (3.10 or higher)
 
 - macOS (requires [Homebrew](https://brew.sh)):
 
   ```shell
   brew install python
   ```
 
@@ -221,22 +219,14 @@
 
   ```shell
   cpo cluster install-odf-storage-classes
   ```
 
   Note: Currently, opinionated configuration values are used for deploying the `StorageCluster` custom resource (see [Ansible playbook](cpo/deps/playbooks/deploy_odf_playbook.yaml)).
 
-### IBM-internal
-
-- Enable Fyre-specific commands:
-
-  ```shell
-  cpo adm config set --key fyre_commands --value true
-  ```
-
 ## Development
 
 - [Development Guide](docs/development_guide.md)
 
 ## Known issues
 
 ### OpenShift CLI (macOS)
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.3.6 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.4.0 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
-System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # IBM Cloud Pak Operations CLI
    [GitHub_license] [GitHub_issues] [GitHub_stars] [GitHub_Workflow_Status_
                                    (branch)]
 The IBM Cloud Pak Operations CLI provides basic functionality to manage Red Hat
 OpenShift clusters and IBM Cloud Pak for Data on various cloud platforms on top
 of the OpenShift CLI (oc) and the [IBM Cloud Pak for Data CLI](https://
-github.com/IBM/cpd-cli) (cpd-cli). For IBM-internal users, the IBM Cloud Pak
-Operations CLI additionally supports managing OpenShift clusters on Fyre. ##
-Installation & Configuration ### Installation #### Python installation (3.8 or
-higher) - macOS (requires [Homebrew](https://brew.sh)): ```shell brew install
-python ``` - Windows: - [Winget](https://github.com/microsoft/winget-cli):
-```shell winget install --exact --id=Python.Python.3.11 ``` - [Chocolatey]
-(https://chocolatey.org) ```shell choco install python ``` #### IBM Cloud Pak
-Operations CLI installation and update (latest release build)
+github.com/IBM/cpd-cli) (cpd-cli). ## Installation & Configuration ###
+Installation #### Python installation (3.10 or higher) - macOS (requires
+[Homebrew](https://brew.sh)): ```shell brew install python ``` - Windows: -
+[Winget](https://github.com/microsoft/winget-cli): ```shell winget install --
+exact --id=Python.Python.3.11 ``` - [Chocolatey](https://chocolatey.org)
+```shell choco install python ``` #### IBM Cloud Pak Operations CLI
+installation and update (latest release build)
 Action                              Command
 Installation (provides cpo command) ```shell pip3 install cloud-pak-operations-
                                     cli ```
 Update                              ```shell pip3 install --upgrade cloud-pak-
                                     operations-cli ```
 #### IBM Cloud Pak Operations CLI installation and update (latest development
 code)
@@ -52,14 +51,13 @@
 cluster: ```shell cpo cluster get-cluster-access-token ``` - Manage the global
 pull secret: ```shell cpo cluster pull-secret ``` ### Storage management -
 Deploy Kubernetes NFS Subdir External Provisioner: ```shell cpo cluster
 install-nfs-storage-class ``` - Deploy OpenShift Data Foundation (Linux and
 macOS): ```shell cpo cluster install-odf-storage-classes ``` Note: Currently,
 opinionated configuration values are used for deploying the `StorageCluster`
 custom resource (see [Ansible playbook](cpo/deps/playbooks/
-deploy_odf_playbook.yaml)). ### IBM-internal - Enable Fyre-specific commands:
-```shell cpo adm config set --key fyre_commands --value true ``` ## Development
-- [Development Guide](docs/development_guide.md) ## Known issues ### OpenShift
-CLI (macOS) ```shell Unable to connect to the server: dial tcp: lookup â¦ on
-â¦:53: no such host ``` - [GitHub issue](https://github.com/openshift/oc/
-issues/315) - Workaround: Edit `/etc/hosts` and add IP address of OpenShift
-cluster - Example: ``` 9.AA.BBB.CC your.cluster.domain.com ```
+deploy_odf_playbook.yaml)). ## Development - [Development Guide](docs/
+development_guide.md) ## Known issues ### OpenShift CLI (macOS) ```shell Unable
+to connect to the server: dial tcp: lookup â¦ on â¦:53: no such host ``` -
+[GitHub issue](https://github.com/openshift/oc/issues/315) - Workaround: Edit
+`/etc/hosts` and add IP address of OpenShift cluster - Example: ``` 9.AA.BBB.CC
+your.cluster.domain.com ```
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/config/set.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/config/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/download_dependencies.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/download_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/get-shell-completion-script-location.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/get-shell-completion-script-location.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/install.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/ls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,34 +10,44 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import click
 
+from tabulate import tabulate
+
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
-import cpo.lib.ibm_internal_plugin.install
 
+from cpo.lib.ibm_internal_plugin.ibm_internal_plugin_manager import IBMInternalPluginInstaller
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command(
     context_settings=cpo.lib.click.utils.create_default_map_from_dict(
         cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_credentials()
     )
 )
-@click.argument("distribution-package-name")
 @click.option(
     "--artifactory-username",
-    help="Artifactory username. The username is usually the IBM e-mail address.",
+    help="Artifactory username (IBM e-mail address)",
     required=True,
 )
 @click.option(
     "--artifactory-password",
-    help="Artifactory password. The password is usually the API key located in the 'Edit Profile' page in Artifactory.",
+    help="Artifactory identity token (Artifactory website → 'Edit Profile' → 'Identity Tokens')",
     required=True,
 )
-def install(distribution_package_name: str, artifactory_username: str, artifactory_password: str):
-    """Install an IBM-internal CLI plug-in"""
+@click.option(
+    "--repository-url",
+    default="https://na.artifactory.swg-devops.com/artifactory/api/pypi/hyc-ibm-sap-cp4d-team-pypi-local/simple",
+)
+def ls(artifactory_username: str, artifactory_password: str, repository_url: str):
+    """List available IBM-internal CLI plug-ins"""
 
-    cpo.lib.ibm_internal_plugin.install.install(distribution_package_name, artifactory_username, artifactory_password)
+    click.echo(
+        tabulate(
+            IBMInternalPluginInstaller(artifactory_username, artifactory_password, repository_url).get_packages(),
+            headers=["name", "version"],
+        )
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/ibm_internal_plugin/ls.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/ibm_internal_plugin/install.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,31 +12,46 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
-import cpo.lib.ibm_internal_plugin.list
 
+from cpo.lib.ibm_internal_plugin.ibm_internal_plugin_manager import IBMInternalPluginInstaller
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command(
     context_settings=cpo.lib.click.utils.create_default_map_from_dict(
         cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_credentials()
     )
 )
 @click.option(
     "--artifactory-username",
-    help="Artifactory username. The username is usually the IBM e-mail address.",
+    help="Artifactory username (IBM e-mail address)",
     required=True,
 )
 @click.option(
     "--artifactory-password",
-    help="Artifactory password. The password is usually the API key located in the 'Edit Profile' page in Artifactory.",
+    help="Artifactory identity token (Artifactory website → 'Edit Profile' → 'Identity Tokens')",
     required=True,
 )
-def ls(artifactory_username, artifactory_password):
-    """List available IBM-internal CLI plug-ins"""
-
-    cpo.lib.ibm_internal_plugin.list.list(artifactory_username, artifactory_password)
+@click.option(
+    "--repository-url",
+    default="https://na.artifactory.swg-devops.com/artifactory/api/pypi/hyc-ibm-sap-cp4d-team-pypi-local/simple",
+)
+@click.option("--user", help="Install to user site-packages directory", is_flag=True)
+@click.argument("distribution-package-names", nargs=-1)
+def install(
+    artifactory_username: str,
+    artifactory_password: str,
+    distribution_package_names: list[str],
+    repository_url: str,
+    user: bool,
+):
+    """Install IBM-internal CLI plug-ins"""
+
+    for distribution_package_name in distribution_package_names:
+        IBMInternalPluginInstaller(artifactory_username, artifactory_password, repository_url).install(
+            distribution_package_name, user
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/store_credentials.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/store_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/adm/update_dev.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/adm/update_dev.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/add.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/add.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.openshift.cluster
 
 from cpo.utils.logging import loglevel_command
@@ -32,15 +32,15 @@
     default=None,
     help="Skips checking the server's certificate for validity",
     is_flag=True,
 )
 def add(server: str, alias: Optional[str], username: str, password: str, insecure_skip_tls_verify: Optional[bool]):
     """Register an existing Red Hat OpenShift cluster"""
 
-    data: Dict[str, Any] = {
+    data: dict[str, Any] = {
         "username": username,
         "password": password,
     }
 
     if insecure_skip_tls_verify is not None:
         data["insecure_skip_tls_verify"] = insecure_skip_tls_verify
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/current.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/current.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/edit.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/edit.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/get_cluster_access_token.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/get_cluster_access_token.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_nfs_storage_class.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/install_nfs_storage_class.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/install_odf_storage_classes.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/install_odf_storage_classes.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/login.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/ls.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/ls.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/rm.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/pull_secret/set.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/pull_secret/set.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/rm.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/cluster/use.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/cluster/use.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Fyre/OCP+-specific commands"
+__doc__ = "IBM Cloud-specific commands"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,8 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Manage a Fyre/OCP+ cluster"
+from typing import Final
+
+EXTERNAL_IBM_CLOUD_API_KEY_NAME: Final[str] = "cloud-pak-operations-cli"
+INTERNAL_KEY_NAME_FOR_IBM_CLOUD_API_KEY: Final[str] = "ibm_cloud_api_key"
+INTERNAL_KEY_NAME_FOR_IBM_CLOUD_API_KEY_ID: Final[str] = "ibm_cloud_api_key_id"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/add.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/login.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
-from cpo.lib.fyre.ocp_plus_api_manager import OCPPlusAPIManager
+from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
+from cpo.lib.ibmcloud.oc.cluster.roks_cluster_factory import roks_cluster_factory
+from cpo.utils.error import CloudPakOperationsCLIException
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
-@click.option("--alias", help="Alias used to reference a cluster instead of its server URL")
-@click.option("--cluster-name", help="Name of the OCP+ cluster to be registered", required=True)
-@click.option("--password", help="kubeadmin password", required=True)
-@click.option("--site", help="OCP+ site", type=click.Choice(["rtp", "svl"]))
-def add(alias: Optional[str], cluster_name: str, password: str, site: Optional[str]):
-    """Register an existing OCP+ cluster"""
-
-    OCPPlusAPIManager.add_cluster(alias, cluster_name, password, site)
+@click.option("--cluster-name", help="cluster name", required=True)
+def login(cluster_name: str):
+    """Log in to a Red Hat OpenShift on IBM Cloud cluster"""
+
+    cluster_status = IBMCloudAPIManager().get_cluster_status(cluster_name)
+
+    if cluster_status.is_ready():
+        cluster = roks_cluster_factory.create_cluster(cluster_status.get_server_url(), {})
+        cluster.login()
+    else:
+        raise CloudPakOperationsCLIException(f"Cluster {cluster_name} is not yet ready")
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/cluster/boot_node.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/add.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,47 +12,32 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Optional
 
 import click
 
-import cpo.config
 import cpo.config.cluster_credentials_manager
-import cpo.lib.click.utils
-import cpo.lib.fyre.cluster
-import cpo.utils.network
-
-from cpo.lib.fyre.ocp_plus_api_manager import OCPPlusAPIManager
-from cpo.lib.fyre.utils.click import fyre_command_options
-from cpo.lib.fyre.utils.node_name import validate_node_name
+import cpo.lib.ibmcloud.oc.cluster
+
+from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
 
-@loglevel_command(
-    context_settings=cpo.lib.click.utils.create_default_map_from_dict(
-        cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_credentials()
-    )
+@loglevel_command()
+@click.option("--alias", help="Alias used to reference a cluster instead of its server URL")
+@click.option(
+    "--cluster-name", help="Name of the Red Hat OpenShift on IBM Cloud cluster to be registered", required=True
 )
-@fyre_command_options
-@click.option("--cluster-name", help="Name of the OCP+ cluster", required=True)
-@click.option("--force", "-f", help="Skip confirmation", is_flag=True)
-@click.option("--node-name", callback=validate_node_name, help="Name of the node to be booted", required=True)
-@click.option("--site", help="OCP+ site", type=click.Choice(["rtp", "svl"]))
-def boot_node(
-    fyre_api_user_name: str,
-    fyre_api_key: str,
-    disable_strict_response_schema_check: bool,
-    cluster_name: str,
-    force: bool,
-    node_name: str,
-    site: Optional[str],
-):
-    """Boot a node of an OCP+ cluster"""
-
-    if not force:
-        click.confirm(f"Do you really want to boot node '{node_name}' of cluster '{cluster_name}'?", abort=True)
-
-    cpo.utils.network.disable_insecure_request_warning()
-    OCPPlusAPIManager(fyre_api_user_name, fyre_api_key, disable_strict_response_schema_check).boot_node(
-        cluster_name, node_name, site
+def add(alias: Optional[str], cluster_name: str):
+    """Register an existing Red Hat OpenShift on IBM Cloud cluster"""
+
+    server = IBMCloudAPIManager().get_cluster_status(cluster_name).get_server_url()
+
+    cpo.config.cluster_credentials_manager.cluster_credentials_manager.add_cluster(
+        alias if (alias is not None) else "",
+        server,
+        cpo.lib.ibmcloud.oc.cluster.CLUSTER_TYPE_ID,
+        {
+            "cluster_name": cluster_name,
+        },
     )
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Get OCP+ information"
+__doc__ = "Manage Red Hat OpenShift on IBM Cloud"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_openshift_versions_all_platforms.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/logout.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,37 +8,32 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
+import logging
 
 import click
 
-import cpo.config
-import cpo.lib.click.utils
-import cpo.utils.network
-
-from cpo.lib.fyre.ocp_plus_api_manager import OCPPlusAPIManager
-from cpo.lib.fyre.utils.click import fyre_command_options
+from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
+logger = logging.getLogger(__name__)
+
 
-@loglevel_command(
-    context_settings=cpo.lib.click.utils.create_default_map_from_json_file(
-        cpo.config.configuration_manager.get_credentials_file_path()
-    )
+@loglevel_command()
+@click.option(
+    "--delete-api-key",
+    help="Delete the API key created for the IBM Cloud Pak Operations CLI (in IBM Cloud and on disk)",
+    is_flag=True,
 )
-@fyre_command_options
-@click.option("--site", help="OCP+ site", type=click.Choice(["rtp", "svl"]))
-def get_openshift_versions_all_platforms(
-    fyre_api_user_name: str, fyre_api_key: str, disable_strict_response_schema_check: bool, site: Optional[str]
-):
-    """Get available OpenShift Container Platform versions for all
-    platforms"""
-
-    cpo.utils.network.disable_insecure_request_warning()
-    OCPPlusAPIManager(
-        fyre_api_user_name, fyre_api_key, disable_strict_response_schema_check
-    ).get_openshift_versions_all_platforms(site).format()
+def logout(delete_api_key: bool):
+    """Log out from IBM Cloud"""
+
+    ibm_cloud_api_manager = IBMCloudAPIManager()
+
+    if delete_api_key:
+        ibm_cloud_api_manager.delete_api_key_in_ibm_cloud_and_on_disk()
+
+    ibm_cloud_api_manager.log_out()
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/info/get_quota.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/status.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,41 +8,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
-import cpo.config
-import cpo.lib.click.utils
-import cpo.utils.network
-
-from cpo.lib.fyre.ocp_plus_api_manager import OCPPlusAPIManager
-from cpo.lib.fyre.utils.click import fyre_command_options
+from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
 
-@loglevel_command(
-    context_settings=cpo.lib.click.utils.create_default_map_from_json_file(
-        cpo.config.configuration_manager.get_credentials_file_path()
-    )
-)
-@fyre_command_options
+@loglevel_command()
+@click.option("--cluster-name", help="cluster name", required=True)
 @click.option("--json", help="Prints the command output in JSON format", is_flag=True)
-@click.option("--site", help="OCP+ site", type=click.Choice(["rtp", "svl"]))
-def get_quota(
-    fyre_api_user_name: str,
-    fyre_api_key: str,
-    disable_strict_response_schema_check: bool,
-    json: bool,
-    site: Optional[str],
-):
-    """Get quotas for product groups the given Fyre user is part of"""
-
-    cpo.utils.network.disable_insecure_request_warning()
-    OCPPlusAPIManager(fyre_api_user_name, fyre_api_key, disable_strict_response_schema_check).get_quota(site).format(
-        json
-    )
+def status(cluster_name: str, json: bool):
+    """Display the status of a Red Hat OpenShift on IBM Cloud cluster"""
+
+    cluster_status = IBMCloudAPIManager().get_cluster_status(cluster_name)
+    status_output = cluster_status.get_json() if json else str(cluster_status)
+
+    click.echo(status_output)
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/fyre/logout.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/auths_dict.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import cpo.config
-import cpo.lib.click
+from typing import TypedDict
 
-from cpo.utils.logging import loglevel_command
 
+class AuthDict(TypedDict):
+    auth: str
 
-@loglevel_command()
-def logout():
-    """Log out from Fyre"""
 
-    credentials_to_be_stored = {"fyre_api_key": "", "fyre_api_user_name": ""}
-
-    cpo.config.configuration_manager.store_credentials(credentials_to_be_stored)
+class AuthsDict(TypedDict):
+    auths: dict[str, AuthDict]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/credentials.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "IBM Cloud-specific commands"
+from dataclasses import dataclass
+
+
+@dataclass
+class Credentials:
+    password: str
+    username: str
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/login.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/logout.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/rm.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,32 +8,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import logging
-
 import click
 
 from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
-logger = logging.getLogger(__name__)
-
 
 @loglevel_command()
-@click.option(
-    "--delete-api-key",
-    help="Delete the API key created for the IBM Cloud Pak Operations CLI (in IBM Cloud and on disk)",
-    is_flag=True,
-)
-def logout(delete_api_key: bool):
-    """Log out from IBM Cloud"""
-
-    ibm_cloud_api_manager = IBMCloudAPIManager()
+@click.option("--cluster-name", help="Name of the Red Hat OpenShift on IBM Cloud cluster to be deleted", required=True)
+@click.option("--force", help="Skip confirmation", is_flag=True)
+def rm(cluster_name: str, force: bool):
+    """Delete a Red Hat OpenShift on IBM Cloud cluster"""
 
-    if delete_api_key:
-        ibm_cloud_api_manager.delete_api_key_in_ibm_cloud_and_on_disk()
+    if not force:
+        click.confirm(f"Do you really want to delete cluster '{cluster_name}'?", abort=True)
 
-    ibm_cloud_api_manager.log_out()
+    IBMCloudAPIManager().delete_cluster(cluster_name)
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Manage Red Hat OpenShift on IBM Cloud"
+__doc__ = "Manage a Red Hat OpenShift on IBM Cloud cluster"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/http_method.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,21 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Manage a Red Hat OpenShift on IBM Cloud cluster"
+from enum import Enum, auto
+
+
+class HTTPMethod(Enum):
+    DELETE = auto()
+    GET = auto()
+    HEAD = auto()
+    OPTIONS = auto()
+    PATCH = auto()
+    POST = auto()
+    PUT = auto()
+
+    def __str__(self):
+        return self.name
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/login.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/oc/cluster/ls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,25 +10,17 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import click
 
-from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
-from cpo.lib.ibmcloud.oc.cluster.roks_cluster_factory import roks_cluster_factory
-from cpo.utils.error import CloudPakOperationsCLIException
+from cpo.lib.ibmcloud.oc.cluster.ls import list_existing_clusters
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
-@click.option("--cluster-name", help="cluster name", required=True)
-def login(cluster_name: str):
-    """Log in to a Red Hat OpenShift on IBM Cloud cluster"""
+@click.option("--json", help="Prints the command output in JSON format", is_flag=True)
+def ls(json: bool):
+    """List Red Hat OpenShift on IBM Cloud clusters"""
 
-    cluster_status = IBMCloudAPIManager().get_cluster_status(cluster_name)
-
-    if cluster_status.is_ready():
-        cluster = roks_cluster_factory.create_cluster(cluster_status.get_server_url(), {})
-        cluster.login()
-    else:
-        raise CloudPakOperationsCLIException(f"Cluster {cluster_name} is not yet ready")
+    click.echo(list_existing_clusters(json))
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/ls.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/ls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import click
+from typing import Any
 
-from cpo.lib.ibmcloud.oc.cluster.ls import list_existing_clusters
-from cpo.utils.logging import loglevel_command
+from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 
 
-@loglevel_command()
-@click.option("--json", help="Prints the command output in JSON format", is_flag=True)
-def ls(json: bool):
-    """List Red Hat OpenShift on IBM Cloud clusters"""
+def list_existing_clusters(json: bool) -> str | Any:
+    """List all available clusters"""
 
-    click.echo(list_existing_clusters(json))
+    args = ["oc", "cluster", "ls"]
+
+    if json:
+        args.append("--json")
+
+    result = IBMCloudAPIManager().execute_ibmcloud_command(args, capture_output=True)
+
+    return result.stdout
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/oc/cluster/rm.py` & `cloud-pak-operations-cli-0.4.0/cpo/commands/ibmcloud/regenerate_api_key.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import click
-
 from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
-@click.option("--cluster-name", help="Name of the Red Hat OpenShift on IBM Cloud cluster to be deleted", required=True)
-@click.option("--force", help="Skip confirmation", is_flag=True)
-def rm(cluster_name: str, force: bool):
-    """Delete a Red Hat OpenShift on IBM Cloud cluster"""
-
-    if not force:
-        click.confirm(f"Do you really want to delete cluster '{cluster_name}'?", abort=True)
+def regenerate_api_key():
+    """Deletes the current IBM Cloud API key and generates a new one"""
 
-    IBMCloudAPIManager().delete_cluster(cluster_name)
+    ibm_cloud_api_manager = IBMCloudAPIManager()
+    ibm_cloud_api_manager.regenerate_api_key()
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/commands/ibmcloud/regenerate_api_key.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/custom_resource_event_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
-from cpo.utils.logging import loglevel_command
+from dataclasses import dataclass
+from typing import Optional
 
 
-@loglevel_command()
-def regenerate_api_key():
-    """Deletes the current IBM Cloud API key and generates a new one"""
-
-    ibm_cloud_api_manager = IBMCloudAPIManager()
-    ibm_cloud_api_manager.regenerate_api_key()
+@dataclass
+class CustomResourceEventResult:
+    succeeded: bool
+    message: Optional[str] = None
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/config/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/config/binaries_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/config/binaries_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,26 +11,26 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Dict, Optional
+from typing import Optional
 
 from cpo.config import configuration_manager
 
-BinariesFileContents = Dict[str, str]
+BinariesFileContents = dict[str, str]
 
 
 class BinariesManager:
     """Manages downloaded binaries"""
 
     def __init__(self):
-        self._binaries_file_contents: Optional[Dict[str, str]] = None
+        self._binaries_file_contents: Optional[dict[str, str]] = None
 
     def get_binaries_file_contents(self) -> Optional[BinariesFileContents]:
         """Returns the contents of the binaries file
 
         Returns
         -------
         Optional[BinariesFileContents]
@@ -80,15 +80,15 @@
 
     def set_binary_version(self, binary_alias: str, version: str):
         binary_versions = self._get_binary_versions()
 
         binary_versions[binary_alias] = version
         self._save_binaries_file()
 
-    def _get_binary_versions(self) -> Dict[str, str]:
+    def _get_binary_versions(self) -> dict[str, str]:
         """Returns versions of downloaded binaries
 
         Returns
         -------
         dict[str, str]
             versions of downloaded binaries
         """
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/config/cluster_credentials_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/config/cluster_credentials_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,37 +11,38 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Dict, List, Optional, TypedDict
+from typing import Any, Optional, TypedDict
 
 from tabulate import tabulate
 
 import cpo.lib.cluster
 
 from cpo.config import configuration_manager
 from cpo.lib.cluster.cluster import AbstractCluster, ClusterData
 from cpo.utils.error import CloudPakOperationsCLIException
 
-ContextData = Dict[str, Any]
+ContextData = dict[str, Any]
 
 
 class ClustersFileContents(TypedDict):
-    clusters: Dict[str, ClusterData]
+    clusters: dict[str, ClusterData]
     current_cluster: str
 
 
 class ClusterCredentialsManager:
     """Manages registered OpenShift clusters"""
 
     def __init__(self):
         self._clusters_file_contents = self.get_clusters_file_contents_with_default()
+        self._current_credentials: Optional[ContextData] = None
 
     def add_cluster(self, alias: str, server: str, type: str, cluster_data: ClusterData):
         """Registers an existing OpenShift cluster
 
         Parameters
         ----------
         alias
@@ -155,22 +156,22 @@
 
         Returns
         -------
         str
             metadata of registered OpenShift clusters as a pretty-printed string
         """
 
-        cluster_list: List[List[str]] = []
+        cluster_list: list[list[str]] = []
         server_of_current_cluster = self._get_server_of_current_cluster()
 
         for server, cluster_data in self._get_clusters().items():
             alias = cluster_data["alias"] if "alias" in cluster_data else ""
             cluster_factory = cpo.lib.cluster.cluster_factories[cluster_data["type"]]
 
-            cluster_list_element: List[str] = [
+            cluster_list_element: list[str] = [
                 "*" if (server == server_of_current_cluster) else "",
                 server,
                 alias,
                 cluster_factory.get_cluster_type_name(),
             ]
 
             cluster_list.append(cluster_list_element)
@@ -253,30 +254,30 @@
 
         Returns
         -------
         ContextData
             user and current cluster credentials
         """
 
-        credentials_file_path = configuration_manager.get_credentials_file_path()
-        result: ContextData
+        if self._current_credentials is None:
+            credentials_file_path = configuration_manager.get_credentials_file_path()
 
-        if credentials_file_path.exists() and (credentials_file_path.stat().st_size != 0):
-            with open(credentials_file_path) as json_file:
-                result = json.load(json_file)
-        else:
-            result = {}
-
-        current_cluster = self.get_current_cluster()
-
-        if current_cluster is not None:
-            result.update(current_cluster.get_cluster_data())
-            result["server"] = current_cluster.get_server()
+            if credentials_file_path.exists() and (credentials_file_path.stat().st_size != 0):
+                with open(credentials_file_path) as json_file:
+                    self._current_credentials = json.load(json_file)
+            else:
+                self._current_credentials = {}
+
+            current_cluster = self.get_current_cluster()
+
+            if current_cluster is not None:
+                self._current_credentials.update(current_cluster.get_cluster_data())
+                self._current_credentials["server"] = current_cluster.get_server()
 
-        return result
+        return self._current_credentials
 
     def raise_if_alias_exists(self, alias_to_be_searched: str):
         """Raises an exception if the given alias is already associated with a
         registered OpenShift cluster
 
         Parameters
         ----------
@@ -340,15 +341,15 @@
             raise CloudPakOperationsCLIException(f"Cluster not found ({alias_or_server})")
 
         self._clusters_file_contents["current_cluster"] = cluster.get_server()
         self._save_clusters_file()
 
         return cluster
 
-    def _get_clusters(self) -> Dict[str, ClusterData]:
+    def _get_clusters(self) -> dict[str, ClusterData]:
         """Returns registered OpenShift clusters
 
         Returns
         -------
         dict[str, ClusterData]
             registered OpenShift clusters
         """
@@ -365,14 +366,19 @@
         -------
         str
             server URL of the current registered OpenShift cluster
         """
 
         return self._clusters_file_contents["current_cluster"]
 
+    def _invalidate_current_credentials(self):
+        """Invalidates current credentials"""
+
+        self._current_credentials = None
+
     def _raise_if_alias_exists(self, alias_to_be_searched: str):
         """Raises an exception if the given alias is already associated with a
         registered OpenShift cluster
 
         Parameters
         ----------
         alias_to_be_searched
@@ -414,9 +420,11 @@
             json.dump(
                 self._clusters_file_contents,
                 clusters_file,
                 indent="\t",
                 sort_keys=True,
             )
 
+        self._invalidate_current_credentials()
+
 
 cluster_credentials_manager = ClusterCredentialsManager()
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/config/configuration_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/config/configuration_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,48 +11,24 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import cpo
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 class ConfigurationManager:
     """Manages the CLI configuration"""
 
-    def are_fyre_commands_hidden(self) -> bool:
-        """Returns whether Fyre options shall be displayed in help texts. The
-        functionality is always usable.
-
-        Returns
-        -------
-        bool
-            true, if Fyre options shall be hidden in help texts
-        """
-
-        return not self.get_bool_config_value("fyre_commands", False)
-
-    def are_nuclear_commands_hidden(self) -> bool:
-        """Returns whether nuclear options shall be displayed in help texts. The
-        functionality is always usable.
-
-        Returns
-        -------
-        bool
-            true, if nuclear options shall be hidden in help texts
-        """
-
-        return not self.get_bool_config_value("nuclear_commands", False)
-
     def get_bool_config_value(self, key: str, default_value: bool) -> bool:
         """Gets the value for a given key from the settings file
 
         Parameters
         ----------
         key
             name of the key of the value to get
@@ -235,29 +211,29 @@
             settings = {key: value}
 
         with open(self.get_settings_file_path(), "w+") as f:
             f.write(json.dumps(settings, indent="\t", sort_keys=True))
 
     def store_credentials(
         self,
-        credentials_to_be_stored: Dict[str, Any],
+        credentials_to_be_stored: dict[str, Any],
     ):
         """Stores credentials in a configuration file
 
         Parameters
         ----------
         credentials_to_be_stored
             dictionary containing key-value pairs to be stored (key-value pairs
             whose value is None are ignored)
         """
 
         if all(value is None for value in credentials_to_be_stored.values()):
             return
 
-        credentials: Optional[Dict[Any, Any]] = None
+        credentials: Optional[dict[Any, Any]] = None
         credentials_file_path = self.get_credentials_file_path()
 
         if credentials_file_path.exists():
             with open(credentials_file_path) as credentials_file:
                 credentials = json.load(credentials_file)
 
                 if credentials is None:
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/cpo.py` & `cloud-pak-operations-cli-0.4.0/cpo/cpo.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-bash.sh` & `cloud-pak-operations-cli-0.4.0/cpo/deps/autocomplete/cpo-autocomplete-bash.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh` & `cloud-pak-operations-cli-0.4.0/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/deps/playbooks/deploy_odf_playbook.yaml` & `cloud-pak-operations-cli-0.4.0/cpo/deps/playbooks/deploy_odf_playbook.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+#  Copyright 2022, 2023 IBM Corporation
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#  http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
 ---
 - connection: local
   hosts: localhost
   gather_facts: false
   tasks:
     - name: "Create Namespace resource (name: openshift-local-storage)"
       kubernetes.core.k8s:
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/abstract_module.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/abstract_module.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/custom_resource_event_result.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,28 +11,28 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Optional
 
 from ansible.module_utils.basic import AnsibleModule
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.modules.abstract_module import AbstractModule
 from cpo.lib.openshift.types.kind_metadata import KindMetadata
 
 
 @dataclass
 class CustomResourceDefinitionsEventData:
-    expected_crd_kinds: Set[str]
-    encountered_crd_kinds: Set[str] = field(default_factory=set)
+    expected_crd_kinds: set[str]
+    encountered_crd_kinds: set[str] = field(default_factory=set)
 
 
 class WaitForCustomResourceDefinitionsModule(AbstractModule):
     def __init__(self):
         argument_spec = {
             "custom_resource_definitions": {
                 "type": "list",
@@ -44,25 +44,25 @@
             },
         }
 
         self._module = AnsibleModule(argument_spec=argument_spec, supports_check_mode=True)
 
         super().__init__(self._module.params["kubeconfig"])  # type: ignore
 
-        self._custom_resource_definitions: List[str] = self._module.params[
+        self._custom_resource_definitions: list[str] = self._module.params[
             "custom_resource_definitions"
         ]  # type: ignore
 
     # override
     def get_module(self) -> AnsibleModule:
         return self._module
 
     # override
     def run(self):
-        result: Optional[Dict]
+        result: Optional[dict]
 
         try:
             self._wait_for_custom_resource(
                 KindMetadata(
                     "apiextensions.k8s.io",
                     "CustomResourceDefinition",
                     "customresourcedefinitions",
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-
 from dataclasses import dataclass
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from ansible.module_utils.basic import AnsibleModule
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.modules.abstract_module import AbstractModule
 from cpo.lib.ansible.modules.custom_resource_event_result import CustomResourceEventResult
@@ -84,15 +83,15 @@
 
     # override
     def get_module(self) -> AnsibleModule:
         return self._module
 
     # override
     def run(self):
-        result: Optional[Dict]
+        result: Optional[dict]
 
         try:
             self._wait_for_namespaced_custom_resource(
                 self._project,
                 self._kind_metadata,
                 self._log,
                 self._success_callback,
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/openshift_playbook_runner.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/openshift_playbook_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.playbook_runner import PlaybookRunner
 from cpo.lib.openshift.credentials.credentials import AbstractCredentials
 from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.utils.error import CloudPakOperationsCLIException
@@ -30,15 +30,15 @@
     """Base class to be inherited by all OpenShift-based playbook runners"""
 
     def __init__(self, playbook_name: str, credentials: AbstractCredentials):
         super().__init__(playbook_name)
 
         self._openshift_api_manager = OpenShiftAPIManager(credentials)
         self._token_expired = False
-        self.kube_config: Optional[Dict[str, Any]] = None
+        self.kube_config: Optional[dict[str, Any]] = None
 
     # override
     def run_playbook(self):
         """Runs a playbook
 
         If the OpenShift-based playbook fails due to an expired OAuth access
         token, it is refreshed an the playbook is rerun.
@@ -62,16 +62,24 @@
                 raise CloudPakOperationsCLIException("Ansible playbook failed")
 
     # override
     def _event_handler(self, event_data: Any):
         try:
             event = cpo.lib.jmespath.get_jmespath_string("event", event_data)
 
-            if event == "runner_on_failed":
-                msg = cpo.lib.jmespath.get_jmespath_string("event_data.res.msg", event_data)
-
-                if msg.startswith("Failed to get client due to 401"):
-                    self._token_expired = True
+            if (event == "runner_on_failed") and self._check_if_unauthorized(event_data):
+                self._token_expired = True
         except cpo.lib.jmespath.JmespathPathExpressionNotFoundException:
             pass
 
         super()._event_handler(event_data)
+
+    def _check_if_unauthorized(self, event_data: Any) -> bool:
+        msg = cpo.lib.jmespath.get_jmespath_string("event_data.res.msg", event_data)
+
+        return msg.startswith("Failed to get client due to 401") or (
+            (msg == "MODULE FAILURE\nSee stdout/stderr for the exact error")
+            and (
+                "kubernetes.dynamic.exceptions.UnauthorizedError: 401\nReason: Unauthorized"
+                in cpo.lib.jmespath.get_jmespath_string("event_data.res.module_stderr", event_data)
+            )
+        )
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runner.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,25 +12,24 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import pathlib
 import re as regex
 
-from typing import Any, Union
+from abc import ABC, abstractmethod
+from typing import Any
 
 import ansible_runner
 
 from ansible_runner.runner import Runner
 from ansible_runner.streaming import Processor, Transmitter, Worker
 
 from cpo.config import configuration_manager
 from cpo.utils.error import CloudPakOperationsCLIException
-from cpo.utils.string import removeprefix, removesuffix
-from abc import ABC, abstractmethod
 
 logger = logging.getLogger(__name__)
 
 
 class PlaybookRunner(ABC):
     """Base class to be inherited by all playbook runners"""
 
@@ -65,17 +64,17 @@
         ----------
         event_data
             Ansible Runner event data
         """
 
         if ("stdout" in event_data) and (event_data["stdout"] != ""):
             if ("event" in event_data) and (event_data["event"] == "runner_on_failed"):
-                logger.log(logging.ERROR, removeprefix(event_data["stdout"], "\r\n"))
+                logger.log(logging.ERROR, event_data["stdout"].removeprefix("\r\n"))
             else:
-                logger.log(logging.DEBUG, removeprefix(event_data["stdout"], "\r\n"))
+                logger.log(logging.DEBUG, event_data["stdout"].removeprefix("\r\n"))
 
     def _get_extra_vars(self) -> dict:
         """Returns extra vars/additional variables
 
         Returns
         -------
         dict
@@ -93,30 +92,30 @@
 
         Returns
         -------
         str
             playbook name
         """
 
-        class_name_without_runner_suffix = removesuffix(self.__class__.__name__, "Runner")
+        class_name_without_runner_suffix = self.__class__.__name__.removesuffix("Runner")
         # AAABbbbCccc → AAA_BbbbCccc
         class_name_using_snake_case = regex.sub("([0-9A-Z])([A-Z][a-z]+)", r"\1_\2", class_name_without_runner_suffix)
         # AAA_BbbbCccc → AAA_Bbbb_Cccc
         class_name_using_snake_case = regex.sub("([0-9a-z])([A-Z])", r"\1_\2", class_name_using_snake_case)
         # AAA_Bbbb_Cccc → aaa_bbbb_cccc.yml
         playbook_name = f"{class_name_using_snake_case}.yaml".lower()
 
         return playbook_name
 
-    def _run_playbook(self) -> Union[Processor, Runner, Transmitter, Worker]:
+    def _run_playbook(self) -> Processor | Runner | Transmitter | Worker:
         """Runs the playbook with the name passed in the constructor
 
         Returns
         -------
-        Union[Processor, Runner, Transmitter, Worker]
+        Processor | Runner | Transmitter | Worker
             object returned by Ansible Runner for post-processing purposes"""
 
         runner = ansible_runner.run(
             artifact_dir=configuration_manager.get_cli_data_directory_path() / "artifacts",
             envvars={
                 "ANSIBLE_JINJA2_NATIVE": True,
                 "ANSIBLE_LIBRARY": configuration_manager.get_root_package_path() / "lib" / "ansible" / "modules",
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ansible/playbook_runners/deploy_odf_playbook_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/click/cpd_service_spec_param_type.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/click/cpd_service_spec_param_type.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/click/lazy_loading_multi_command.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/click/lazy_loading_multi_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 import importlib.metadata
 import importlib.util
 import logging
 import pathlib
 
 from dataclasses import dataclass, field
 from types import ModuleType
-from typing import Dict, List, Optional
+from typing import Optional
 
 import click
 
 import cpo
 import cpo.utils.debugger
 
 from cpo import commands_package_path
@@ -40,16 +40,16 @@
 class CommandDetails:
     command: click.Command
     distribution_package_name: str
 
 
 @dataclass
 class CommandData:
-    command_names: List[str] = field(default_factory=list)
-    commands: Dict[str, CommandDetails] = field(default_factory=dict)
+    command_names: list[str] = field(default_factory=list)
+    commands: dict[str, CommandDetails] = field(default_factory=dict)
 
 
 class LazyLoadingMultiCommand(click.MultiCommand):
     """Provides Click commands found within modules of the package passed to
     the constructor
 
     For each found subpackage of the package passed to the constructor, a
@@ -90,15 +90,15 @@
 
         if self._command_data is not None:
             command = self._command_data.commands[cmd_name].command if cmd_name in self._command_data.commands else None
 
         return command
 
     # override
-    def list_commands(self, ctx: click.Context) -> List[str]:
+    def list_commands(self, ctx: click.Context) -> list[str]:
         self._initialize_command_data_if_required()
 
         return self._command_data.command_names if self._command_data is not None else []
 
     def _append_distribution_package_name_to_help_text(
         self, help_text: Optional[str], distribution_package_name: str
     ) -> Optional[str]:
@@ -128,15 +128,15 @@
 
         module = importlib.util.module_from_spec(spec)
 
         spec.loader.exec_module(module)
 
         return module
 
-    def _import_modules(self, command_data: CommandData, modules: List[PackageElementDescriptor]):
+    def _import_modules(self, command_data: CommandData, modules: list[PackageElementDescriptor]):
         """Imports the given modules and updates the given command data object
 
         Parameters
         ----------
         command_data
             object storing Click command names and Click commands
         modules
@@ -156,15 +156,15 @@
                 if command_name in command_data.command_names:
                     self._raise_registration_error(command_name, command_data, package_element_descriptor)
 
                 command_data.command_names.append(command_name)
 
             command_data.commands.update(command_dict)
 
-    def _import_subpackages(self, command_data: CommandData, subpackages: List[PackageElementDescriptor]):
+    def _import_subpackages(self, command_data: CommandData, subpackages: list[PackageElementDescriptor]):
         """Imports the given subpackages and updates the given command data
         object
 
         Parameters
         ----------
         command_data
             object storing Click command names and Click commands
@@ -272,15 +272,15 @@
             f"{package_element_descriptor.distribution_package_name}'{command_hierarchy_path}) cannot be registered as "
             f"a {command_type_2} with the same name was already provided by distribution package '"
             f"{command_data.commands[command_name].distribution_package_name}'"
         )
 
     def _search_for_commands(
         self, package_element_descriptor: PackageElementDescriptor, module: ModuleType
-    ) -> Dict[str, CommandDetails]:
+    ) -> dict[str, CommandDetails]:
         """Searches the given module for Click commands
 
         Parameters
         ----------
         package_element_descriptor
             object describing a module or a subpackage within a package
         module
@@ -288,15 +288,15 @@
 
         Returns
         -------
         dict[str, click.Command]
             dictionary associating Click command names with Click commands
         """
 
-        commands: Dict[str, CommandDetails] = {}
+        commands: dict[str, CommandDetails] = {}
 
         for attribute_name in dir(module):
             attribute = getattr(module, attribute_name)
 
             if isinstance(attribute, click.Command):
                 if package_element_descriptor.distribution_package_name != cpo.distribution_package_name:
                     attribute.help = self._append_distribution_package_name_to_help_text(
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/click/utils.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/click/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,28 +11,28 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.openshift.oc
 
 from cpo.lib.openshift.credentials.cluster_based_user_credentials import ClusterBasedUserCredentials
 from cpo.lib.openshift.credentials.credentials import AbstractCredentials
 from cpo.lib.openshift.credentials.token_credentials import TokenCredentials
 from cpo.lib.openshift.credentials.user_credentials import UserCredentials
 
 
-def create_default_map_from_dict(dict: Dict[str, Any]):
+def create_default_map_from_dict(dict: dict[str, Any]):
     default_map_dict = {}
     default_map_dict["default_map"] = dict
 
     return default_map_dict
 
 
 def create_default_map_from_json_file(path: pathlib.Path):
@@ -43,15 +43,15 @@
             credentials_file_contents = json.load(json_file)
 
             default_map_dict["default_map"] = credentials_file_contents
 
     return default_map_dict
 
 
-def get_cluster_credentials(ctx: click.Context, options: Dict[str, Any]) -> AbstractCredentials:
+def get_cluster_credentials(ctx: click.Context, options: dict[str, Any]) -> AbstractCredentials:
     """Returns cluster credentials based on the options passed to a Click
     command or the current cluster
 
     Parameters
     ----------
     ctx
         Click context
@@ -107,15 +107,15 @@
             "You must either set options --server/--username/--password, --server/--token, or set a current cluster.",
             ctx,
         )
 
     return result
 
 
-def get_oc_login_command_for_remote_host(ctx: click.Context, options: Dict[str, Any]) -> str:
+def get_oc_login_command_for_remote_host(ctx: click.Context, options: dict[str, Any]) -> str:
     result: Optional[str] = None
 
     if (
         ("server" in options)
         and (options["server"] is not None)
         and ("username" in options)
         and (options["username"] is not None)
@@ -148,15 +148,15 @@
             "You must either set options --server/--username/--password, --server/--token, or set a current cluster.",
             ctx,
         )
 
     return result
 
 
-def log_in_to_openshift_cluster(ctx: click.Context, options: Dict[str, Any]):
+def log_in_to_openshift_cluster(ctx: click.Context, options: dict[str, Any]):
     if (
         ("server" in options)
         and (options["server"] is not None)
         and ("username" in options)
         and (options["username"] is not None)
         and ("password" in options)
         and (options["password"] is not None)
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Dict
-
 import cpo.lib.cluster.cluster_factory
-import cpo.lib.fyre.cluster
-import cpo.lib.fyre.cluster.ocpplus_cluster_factory
 import cpo.lib.ibmcloud.oc.cluster
 import cpo.lib.ibmcloud.oc.cluster.roks_cluster_factory
 import cpo.lib.openshift.cluster
 import cpo.lib.openshift.cluster.generic_cluster_factory
 
 from cpo.lib.cluster.cluster_factory import AbstractClusterFactory
 
-cluster_factories: Dict[str, AbstractClusterFactory] = {}
+cluster_factories: dict[str, AbstractClusterFactory] = {}
 cluster_factories[
     cpo.lib.ibmcloud.oc.cluster.CLUSTER_TYPE_ID
 ] = cpo.lib.ibmcloud.oc.cluster.roks_cluster_factory.roks_cluster_factory
 
 cluster_factories[
-    cpo.lib.fyre.cluster.CLUSTER_TYPE_ID
-] = cpo.lib.fyre.cluster.ocpplus_cluster_factory.ocpplus_cluster_factory
-
-cluster_factories[
     cpo.lib.openshift.cluster.CLUSTER_TYPE_ID
 ] = cpo.lib.openshift.cluster.generic_cluster_factory.generic_cluster_factory
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/cluster.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC, abstractmethod
-from typing import Any, Dict
+from typing import Any
 
-ClusterData = Dict[str, Any]
+ClusterData = dict[str, Any]
 
 
 class AbstractCluster(ABC):
     def __init__(self, server: str, cluster_data: ClusterData):
         self.cluster_data = cluster_data
         self.server = server
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/cluster/cluster_factory.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/cluster/cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/dependency_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,35 +11,35 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
 import pathlib
 
-from typing import Dict, List, Optional, Type
+from typing import Optional
 
 import cpo.utils.process
 
 from cpo.config.binaries_manager import binaries_manager
 from cpo.lib.dependency_manager.dependency_manager_plugin import AbstractDependencyManagerPlugIn
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 class DependencyManager:
     """Responsible for managing dependencies"""
 
     def __init__(self):
-        self._download_manager_dict: Dict[Type[AbstractDependencyManagerPlugIn], AbstractDependencyManagerPlugIn] = {}
-        self._download_manager_plugins: List[AbstractDependencyManagerPlugIn] = []
+        self._download_manager_dict: dict[type[AbstractDependencyManagerPlugIn], AbstractDependencyManagerPlugIn] = {}
+        self._download_manager_plugins: list[AbstractDependencyManagerPlugIn] = []
 
     def execute_binary(
         self,
-        cls: Type[AbstractDependencyManagerPlugIn],
-        args: List[str],
-        env: Dict[str, str] = os.environ.copy(),
+        cls: type[AbstractDependencyManagerPlugIn],
+        args: list[str],
+        env: dict[str, str] = os.environ.copy(),
         capture_output=False,
         check=True,
         print_captured_output=False,
     ) -> cpo.utils.process.ProcessResult:
         """Executes the binary provided by the dependency corresponding to the
         dependency manager plug-in of the given type
 
@@ -88,15 +88,15 @@
             plugin.download_dependency_version(latest_dependency_version)
             binaries_manager.set_binary_version(plugin.get_dependency_alias(), str(latest_dependency_version))
 
         return plugin.execute_binary(
             args, env, capture_output=capture_output, check=check, print_captured_output=print_captured_output
         )
 
-    def get_binary_path(self, cls: Type[AbstractDependencyManagerPlugIn]) -> Optional[pathlib.Path]:
+    def get_binary_path(self, cls: type[AbstractDependencyManagerPlugIn]) -> Optional[pathlib.Path]:
         """Returns the path of the binary provided by the dependency
         corresponding to the dependency manager plug-in of the given type
 
         Returns
         -------
         cls
             dependency manager plug-in type
@@ -109,15 +109,15 @@
         plugin = self._download_manager_dict.get(cls)
 
         if plugin is None:
             raise CloudPakOperationsCLIException(f"Plug-in with class name '{cls.__name__} was not registered")
 
         return plugin.get_binary_path()
 
-    def register_plugin(self, cls: Type[AbstractDependencyManagerPlugIn]):
+    def register_plugin(self, cls: type[AbstractDependencyManagerPlugIn]):
         """Registers a dependency manager plug-in of the given type
 
         Parameters
         ----------
         cls
             dependency manager plug-in type
         """
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/dependency_manager_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/dependency_manager_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 
 import json
 import os
 import pathlib
 import re as regex
 
 from abc import ABC, abstractmethod
-from typing import Dict, List, Optional
+from typing import Optional
 
 import requests
 import semver
 
 import cpo.utils.process
 
 from cpo.config import configuration_manager
@@ -42,16 +42,16 @@
             version of the dependency to be downloaded
         """
 
         pass
 
     def execute_binary(
         self,
-        args: List[str],
-        env: Dict[str, str] = os.environ.copy(),
+        args: list[str],
+        env: dict[str, str] = os.environ.copy(),
         capture_output=False,
         check=True,
         print_captured_output=False,
     ) -> cpo.utils.process.ProcessResult:
         """Executes the binary associated with the dependency
 
         If the dependency does not provide a binary, an exception is raised.
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
 import pathlib
 import urllib.parse
 
-from typing import Dict, List, Optional
+from typing import Optional
 
 import semver
 
 import cpo.config
 import cpo.utils.compression
 import cpo.utils.download
 import cpo.utils.file
@@ -47,16 +47,16 @@
         archive_path = cpo.utils.download.download_file(urllib.parse.urlsplit(url))
 
         self._extract_archive(archive_path)
 
     # override
     def execute_binary(
         self,
-        args: List[str],
-        env: Dict[str, str] = os.environ.copy(),
+        args: list[str],
+        env: dict[str, str] = os.environ.copy(),
         capture_output=False,
         check=True,
         print_captured_output=False,
     ) -> cpo.utils.process.ProcessResult:
         try:
             return super().execute_binary(
                 args, env, capture_output=capture_output, check=check, print_captured_output=print_captured_output
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/openshift_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/dependency_manager/plugins/terraform_plugin.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/dependency_manager/plugins/terraform_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/__init__.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,8 +11,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Final
 
 # randomly generated universally unique identifier (generated by https://www.uuidgenerator.net/)
-CLUSTER_TYPE_ID: Final[str] = "dcd2a055-652b-448f-8e39-4edb3e8695de"
+CLUSTER_TYPE_ID: Final[str] = "6446c4cb-7e82-4f68-88bb-458bd5a0bcc4"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/generic_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 import cpo.lib.openshift.oc
 
 from cpo.lib.cluster.cluster import AbstractCluster, ClusterData
 
 
-class OCPPlusCluster(AbstractCluster):
+class GenericCluster(AbstractCluster):
     def __init__(self, server: str, cluster_data: ClusterData):
         super().__init__(server, cluster_data)
 
     def get_password(self) -> str:
         return self.cluster_data["password"]
 
     def get_username(self) -> str:
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/cluster/ocpplus_cluster_factory.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,22 +10,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from cpo.lib.cluster.cluster import AbstractCluster
 from cpo.lib.cluster.cluster_factory import AbstractClusterFactory, ClusterData
-from cpo.lib.fyre.cluster.ocpplus_cluster import OCPPlusCluster
+from cpo.lib.ibmcloud.oc.cluster.roks_cluster import ROKSCluster
 
 
-class OCPPlusClusterFactory(AbstractClusterFactory):
+class ROKSClusterFactory(AbstractClusterFactory):
     def create_cluster(self, server: str, cluster_data: ClusterData) -> AbstractCluster:
-        return OCPPlusCluster(server, cluster_data)
-
-    def create_cluster_using_cluster_name(self, cluster_name: str, cluster_data: ClusterData) -> AbstractCluster:
-        return OCPPlusCluster(f"https://api.{cluster_name}.cp.fyre.ibm.com:6443", cluster_data)
+        return ROKSCluster(server, cluster_data)
 
     def get_cluster_type_name(self) -> str:
-        return "Fyre (OCP+)"
+        return "IBM Cloud (Red Hat OpenShift on IBM Cloud)"
 
 
-ocpplus_cluster_factory = OCPPlusClusterFactory()
+roks_cluster_factory = ROKSClusterFactory()
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/check_hostname_get_response.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/debugger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,34 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import TypedDict
+import inspect
 
 
-class CheckHostnameGetResponse(TypedDict):
-    details: str
-    name_id: str
-    owning_user: str
-    status: str
+def is_debugpy_running() -> bool:
+    """Returns whether debugpy is running
+
+    Visual Studio Code uses debugpy (https://github.com/microsoft/debugpy)
+    as the default Python debugger.
+
+    Returns
+    -------
+    bool
+        True, if debugpy is running
+    """
+
+    for frame in inspect.stack():
+        if frame.filename.endswith("debugpy/__main__.py"):
+            return True
+
+    return False
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_error_response.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, TypedDict, Union
+from typing import TypedDict
 
 
-class Error(TypedDict):
-    errors: List[str]
-
-
-class DefaulErrorResponse(TypedDict):
-    details: Union[Error, str]
-    status: str
+class RoleRule(TypedDict, total=False):
+    apiGroups: list[str]
+    resourceNames: list[str]
+    resources: list[str]
+    verbs: list[str]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/default_success_response.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/kind_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import TypedDict
+from dataclasses import dataclass
 
 
-class DefaultSuccessResponse(TypedDict):
-    details: str
-    request_id: str
-    status: str
+@dataclass
+class KindMetadata:
+    group: str
+    kind: str
+    plural: str
+    version: str
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_available_get_response.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/custom_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, TypedDict
+from dataclasses import dataclass
+from typing import Any, TypedDict
 
+from cpo.lib.openshift.types.object_meta import ObjectMeta
 
-class NodeSize(TypedDict):
-    additional_disk_size: str
-    additional_disk: str
-    base_disk_size: str
-    count: str
-    cpu: str
-    max_cpu: str
-    max_disk_size: str
-    max_disk: str
-    max_memory: str
-    memory: str
-
-
-class DefaultClusterSizeData(TypedDict):
-    inf: NodeSize
-    master: NodeSize
-    worker: NodeSize
-
-
-class OCPAvailableGetResponse(TypedDict):
-    default_size: DefaultClusterSizeData
-    ocp_versions: List[str]
+
+class CustomResourceDict(TypedDict):
+    apiVersion: str
+    kind: str
+    metadata: ObjectMeta
+    spec: dict[str, Any]
+
+
+@dataclass
+class CustomResource:
+    group: str
+    kind: str
+    metadata: ObjectMeta
+    spec: dict[str, Any]
+    version: str
+
+    def create_custom_resource_dict(self) -> CustomResourceDict:
+        return {
+            "apiVersion": f"{self.group}/{self.version}",
+            "kind": self.kind,
+            "metadata": self.metadata,
+            "spec": self.spec,
+        }
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_disk_put_request.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, TypedDict
+from typing import Final
 
-OCPDiskPutRequest = TypedDict("OCPDiskPutRequest", {"additional_disk": List[str]})
+# randomly generated universally unique identifier (generated by https://www.uuidgenerator.net/)
+CLUSTER_TYPE_ID: Final[str] = "d3ca538f-c5cf-474a-a17c-afec42f7bf9f"
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_get_response_for_single_cluster.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/catalog_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,50 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, Optional, TypedDict
+from typing import TypedDict
 
-from cpo.lib.fyre.types.shared import IP
+from cpo.lib.openshift.types.object_meta import ObjectMeta
 
 
-class VM(TypedDict):
-    additional_disk: List[str]
-    cpu: str
-    hostname: str
-    in_progress: str
-    ip_address: str
-    ip_type: str
-    ips: List[IP]
-    memory: str
-    os_disk: str
-    os_state: str
-    pingable_last_checked: Optional[str]
-    pingable: str
-    vm_id: str
-
-
-class Cluster(TypedDict):
-    access_url: str
-    auto_patch: str
-    cluster_count: str
-    cluster_id: str
-    cluster_name: str
-    cluster_type: str
-    compliance: str
-    created: str
-    deployment_status: str
-    description: str
-    expiration: str
-    fips_enabled: str
-    kubeadmin_password: Optional[str]
-    locked_for_delete: str
-    ocp_username: str
-    ocp_version: str
-    product_group_id: str
-    vm_count: int
-    vms: List[VM]
-
-
-class OCPGetResponseForSingleCluster(TypedDict):
-    cluster_count: int
-    clusters: List[Cluster]
-    location_name: str
+class CatalogSourceSpecUpdateStrategyRegistryPoll(TypedDict):
+    interval: str
+
+
+class CatalogSourceSpecUpdateStrategy(TypedDict):
+    registryPoll: CatalogSourceSpecUpdateStrategyRegistryPoll
+
+
+class CatalogSourceSpec(TypedDict, total=False):
+    displayName: str
+    image: str
+    imagePullPolicy: str
+    publisher: str
+    sourceType: str
+    updateStrategy: CatalogSourceSpecUpdateStrategy
+
+
+class CatalogSource(TypedDict):
+    """
+    Notes
+    -----
+    https://docs.openshift.com/container-platform/latest/rest_api/operatorhub_apis/catalogsource-operators-coreos-com-v1alpha1.html#catalogsource-operators-coreos-com-v1alpha1
+    """
+
+    apiVersion: str
+    kind: str
+    metadata: ObjectMeta
+    spec: CatalogSourceSpec
+
+
+CatalogSourceList = list[CatalogSource]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_post_response.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/service_account.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,32 +8,22 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, TypedDict, Union
+from typing import TypedDict
 
-from cpo.lib.fyre.types.default_success_response import DefaultSuccessResponse
+from cpo.lib.openshift.types.object_meta import ObjectMeta
 
 
-class Error(TypedDict):
-    error: str
-    issued: str
+class ServiceAccount(TypedDict):
+    """
+    Notes
+    -----
+    https://docs.openshift.com/container-platform/latest/rest_api/security_apis/serviceaccount-core-v1.html#serviceaccount-core-v1
+    """
 
-
-class Details(TypedDict):
-    errors: List[Union[Error, str]]
-
-
-class OCPPostErrorResponseOptional(TypedDict, total=False):
-    build_errors: List[str]
-
-
-class OCPPostErrorResponse(OCPPostErrorResponseOptional):
-    details: Union[Details, str]
-    status: str
-
-
-class OCPPostResponse(DefaultSuccessResponse):
-    cluster_name: str
+    apiVersion: str
+    kind: str
+    metadata: ObjectMeta
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/ocp_resource_put_request.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/operator_group.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,11 +10,25 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import TypedDict
 
+from cpo.lib.openshift.types.object_meta import ObjectMeta
 
-class OCPResourcePutRequest(TypedDict, total=False):
-    cpu: str
-    memory: str
+
+class OperatorGroupSpec(TypedDict):
+    targetNamespaces: list[str]
+
+
+class OperatorGroup(TypedDict):
+    """
+    Notes
+    -----
+    https://docs.openshift.com/container-platform/latest/rest_api/operatorhub_apis/operatorgroup-operators-coreos-com-v1.html#operatorgroup-operators-coreos-com-v1
+    """
+
+    apiVersion: str
+    kind: str
+    metadata: ObjectMeta
+    spec: OperatorGroupSpec
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/types/shared.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/ingress_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import TypedDict
+from typing import Any
 
 
-class IP(TypedDict):
-    address: str
-    ip_scope: str
-    type: str
+class IngressStatus:
+    def __init__(self, status_output: Any):
+        self._status_output = status_output
+
+    def is_ready(self) -> bool:
+        result = False
+
+        if ("status" in self._status_output) and (self._status_output["status"] == "healthy"):
+            result = True
+
+        return result
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/fyre/utils/click.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/utils/click.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,33 +17,36 @@
 from typing import Any, Callable
 
 import click
 
 from click_option_group import optgroup
 
 
-def fyre_command_optgroup_options(f: Callable[..., Any]) -> Callable[..., Any]:
+def openshift_server_command_optgroup_options(f: Callable[..., Any]) -> Callable[..., Any]:
     options = [
-        optgroup.option("--fyre-api-key", help="Fyre API key (see https://fyre.svl.ibm.com/account)", required=True),
-        optgroup.option("--fyre-api-user-name", help="Fyre API user name", required=True),
         optgroup.option(
-            "--disable-strict-response-schema-check",
-            help="Disable strict schema check for OCP+ API response",
-            is_flag=True,
+            "--insecure-skip-tls-verify", help="Skips checking the server's certificate for validity", is_flag=True
         ),
+        optgroup.option("--token", help="OpenShift OAuth access token"),
+        optgroup.option("--password", help="OpenShift password"),
+        optgroup.option("--username", help="OpenShift username"),
+        optgroup.option("--server", help="OpenShift server URL"),
     ]
 
     return functools.reduce(lambda result, option: option(result), options, f)
 
 
-def fyre_command_options(f: Callable[..., Any]) -> Callable[..., Any]:
+def openshift_server_options(f: Callable[..., Any]) -> Callable[..., Any]:
     options = [
-        click.option("--fyre-api-key", help="Fyre API key (see https://fyre.svl.ibm.com/account)", required=True),
-        click.option("--fyre-api-user-name", help="Fyre API user name", required=True),
         click.option(
-            "--disable-strict-response-schema-check",
-            help="Disable strict schema check for OCP+ API response",
+            "--insecure-skip-tls-verify",
+            default=None,
+            help="Skips checking the server's certificate for validity",
             is_flag=True,
         ),
+        click.option("--token", help="OpenShift OAuth access token"),
+        click.option("--password", help="OpenShift password"),
+        click.option("--username", help="OpenShift username"),
+        click.option("--server", help="OpenShift server URL"),
     ]
 
     return functools.reduce(lambda result, option: option(result), options, f)
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ibm_internal_plugin/install.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/object_meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import cpo.utils.process
+from typing import Optional, TypedDict
 
 
-def install(distribution_package_name: str, artifactory_username: str, artifactory_password: str):
-    """Installs the distribution package with the given name"""
+class ObjectMetaOptional(TypedDict, total=False):
+    creationTimestamp: Optional[str]
+    labels: dict[str, str]
+    namespace: str
 
-    cpo.utils.process.execute_command(
-        "pip3",  # type: ignore
-        [
-            "install",
-            distribution_package_name,
-            "--index-url",
-            (
-                f"https://{artifactory_username}:{artifactory_password}@"
-                "na.artifactory.swg-devops.com/artifactory/api/pypi/idaa-data-gate-cli-pypi-local/simple"
-            ),
-            "--user",
-        ],
-    )
+
+class ObjectMetaRequired(TypedDict):
+    name: str
+
+
+class ObjectMeta(ObjectMetaOptional, ObjectMetaRequired, total=False):
+    """
+    Notes
+    -----
+    https://docs.openshift.com/container-platform/latest/rest_api/objects/index.html#objectmeta_v2-meta-v1"""
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/cluster_status.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/data/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/data/ingress_status.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/wait.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,44 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2021, 2022 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any
+import logging
 
+from time import sleep
 
-class IngressStatus:
-    def __init__(self, status_output: Any):
-        self._status_output = status_output
+import click
 
-    def is_ready(self) -> bool:
-        result = False
+from cpo.utils.error import CloudPakOperationsCLIException
 
-        if ("status" in self._status_output) and (self._status_output["status"] == "healthy"):
-            result = True
+logger = logging.getLogger(__name__)
 
-        return result
+
+def wait_for(timeout, interval, action_name, predicate, *args, **kwargs):
+    time_passed = 0
+
+    while time_passed < timeout:
+        time_passed_output = f"Time spent / timeout ({str(time_passed).rjust(4, ' ')}s / {str(timeout).rjust(4, ' ')}s)"
+
+        if predicate(*args, **kwargs):
+            if time_passed != 0:
+                click.echo(time_passed_output)
+
+            logger.info(f"{action_name} finished successfully.")
+
+            break
+
+        click.echo(f"{time_passed_output}\r", nl=False)
+        sleep(interval)
+        time_passed += interval
+    else:
+        raise CloudPakOperationsCLIException(f"{action_name} timed out.")
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/ibm_cloud_api_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/ibm_cloud_api_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,15 +15,15 @@
 import json
 import logging
 import os
 import re as regex
 import subprocess
 
 from dataclasses import dataclass
-from typing import Any, Final, List, Optional
+from typing import Any, Final, Optional
 
 import cpo.utils.process
 
 from cpo.config import configuration_manager
 from cpo.config.cluster_credentials_manager import cluster_credentials_manager
 from cpo.lib.dependency_manager import dependency_manager
 from cpo.lib.dependency_manager.plugins.ibm_cloud_cli_plugin import IBMCloudCLIPlugIn
@@ -144,15 +144,15 @@
 
         ibmcloud config --check-version=false disables this behavior
         """
 
         self._execute_ibmcloud_command(["config", "--check-version=false"], capture_output=True)
 
     def execute_ibmcloud_command(
-        self, args: List[str], capture_output=False, check=True, print_captured_output=False, skip_login=False
+        self, args: list[str], capture_output=False, check=True, print_captured_output=False, skip_login=False
     ) -> cpo.utils.process.ProcessResult:
         """Executes the IBM Cloud CLI
 
         Parameters
         ----------
         args
             arguments to be passed to the IBM Cloud CLI
@@ -199,15 +199,15 @@
                 )
             else:
                 result.raise_for_status()
 
         return result
 
     def execute_ibmcloud_command_without_check(
-        self, args: List[str], capture_output=False, print_captured_output=False
+        self, args: list[str], capture_output=False, print_captured_output=False
     ) -> cpo.utils.process.ProcessResult:
         """Executes the IBM Cloud CLI without checking its return code
 
         Parameters
         ----------
         args
             arguments to be passed to the IBM Cloud CLI
@@ -424,15 +424,15 @@
             {
                 INTERNAL_KEY_NAME_FOR_IBM_CLOUD_API_KEY: api_key.api_key,
                 INTERNAL_KEY_NAME_FOR_IBM_CLOUD_API_KEY_ID: api_key.api_key_id,
             }
         )
 
     def _execute_ibmcloud_command(
-        self, args: List[str], capture_output=False, check=True, print_captured_output=False
+        self, args: list[str], capture_output=False, check=True, print_captured_output=False
     ) -> cpo.utils.process.ProcessResult:
         """Executes the IBM Cloud CLI
 
         Parameters
         ----------
         args
             arguments to be passed to the IBM Cloud CLI
@@ -460,29 +460,29 @@
             args,
             env,
             capture_output=capture_output,
             check=check,
             print_captured_output=print_captured_output,
         )
 
-    def _execute_ibmcloud_command_interactively(self, args: List[str]) -> int:
+    def _execute_ibmcloud_command_interactively(self, args: list[str]) -> int:
         command = [str(dependency_manager.get_binary_path(IBMCloudCLIPlugIn))] + args
 
         logging.debug(f"Executing command: {' '.join(command)}")
 
         env = os.environ.copy()
         env["IBMCLOUD_HOME"] = str(configuration_manager.get_cli_data_directory_path())
 
         proc = subprocess.Popen(command, env=env)
         proc.communicate()
 
         return proc.returncode
 
     def _execute_ibmcloud_command_without_check(
-        self, args: List[str], capture_output=False, print_captured_output=False
+        self, args: list[str], capture_output=False, print_captured_output=False
     ) -> cpo.utils.process.ProcessResult:
         """Executes the IBM Cloud CLI without checking its return code
 
         Parameters
         ----------
         args
             arguments to be passed to the IBM Cloud CLI
@@ -540,22 +540,22 @@
     def install_required_plug_ins(self):
         self._install_plugin("catalogs-management")
         self._install_plugin("container-service")
 
     def refresh(self):
         self._plug_ins = self._get_plug_ins()
 
-    def _get_plug_ins(self) -> List[str]:
+    def _get_plug_ins(self) -> list[str]:
         ibmcloud_plugin_list_command_args = ["plugin", "list", "--output", "json"]
         ibmcloud_plugin_list_command_result = self._ibm_cloud_api_manager.execute_ibmcloud_command(
             ibmcloud_plugin_list_command_args, capture_output=True
         )
 
         ibmcloud_plugin_list_command_result_json = json.loads(ibmcloud_plugin_list_command_result.stdout)
-        plug_ins: List[str] = []
+        plug_ins: list[str] = []
 
         for plugin in ibmcloud_plugin_list_command_result_json:
             if "Name" in plugin:
                 plug_ins.append(plugin["Name"])
 
         return plug_ins
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/jmespath.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/jmespath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, List
+from typing import Any
 
 import jmespath
 
 from cpo.utils.error import JmespathPathExpressionNotFoundException, UnexpectedTypeException
 
 
 def get_jmespath_bool(expression: str, data: Any) -> bool:
@@ -44,38 +44,38 @@
 
     if not isinstance(search_result, bool):
         raise UnexpectedTypeException(search_result)
 
     return search_result
 
 
-def get_jmespath_list_of_strings(expression: str, data: Any) -> List[str]:
+def get_jmespath_list_of_strings(expression: str, data: Any) -> list[str]:
     """Returns a list of strings extracted from the given object based on
     the given JMESPath expression
 
     Parameters
     ----------
     expression
         JMESPath expression
     data
         object to be searched
 
     Returns
     -------
-    List[str]
+    list[str]
         list of strings extracted from the given object based on the given
         JMESPath expression
     """
 
     search_result: Any = jmespath.search(expression, data)
 
     if search_result is None:
         raise JmespathPathExpressionNotFoundException(expression)
 
-    if not isinstance(search_result, List) or not all(isinstance(element, str) for element in search_result):
+    if not isinstance(search_result, list) or not all(isinstance(element, str) for element in search_result):
         raise UnexpectedTypeException(search_result)
 
     return search_result
 
 
 def get_jmespath_string(expression: str, data: Any) -> str:
     """Returns a string extracted from the given object based on the given
@@ -86,15 +86,15 @@
     expression
         JMESPath expression
     data
         object to be searched
 
     Returns
     -------
-    List[str]
+    list[str]
         string extracted from the given object based on the given JMESPath
         expression
     """
 
     search_result = jmespath.search(expression, data)
 
     if search_result is None:
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/cluster/generic_cluster_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import cpo.lib.openshift.oc
+from cpo.lib.cluster.cluster import AbstractCluster
+from cpo.lib.cluster.cluster_factory import AbstractClusterFactory, ClusterData
+from cpo.lib.openshift.cluster.generic_cluster import GenericCluster
 
-from cpo.lib.cluster.cluster import AbstractCluster, ClusterData
 
+class GenericClusterFactory(AbstractClusterFactory):
+    def create_cluster(self, server: str, cluster_data: ClusterData) -> AbstractCluster:
+        return GenericCluster(server, cluster_data)
 
-class GenericCluster(AbstractCluster):
-    def __init__(self, server: str, cluster_data: ClusterData):
-        super().__init__(server, cluster_data)
+    def get_cluster_type_name(self) -> str:
+        return "Generic"
 
-    def get_password(self) -> str:
-        return self.cluster_data["password"]
 
-    def get_username(self) -> str:
-        return self.cluster_data["username"]
-
-    # override
-    def login(self):
-        cpo.lib.openshift.oc.log_in_to_openshift_cluster_with_password(
-            self.server, self.cluster_data["username"], self.cluster_data["password"]
-        )
+generic_cluster_factory = GenericClusterFactory()
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/cluster/generic_cluster_factory.py` & `cloud-pak-operations-cli-0.4.0/cpo/scripts/get_current_cluster_alias.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from cpo.lib.cluster.cluster import AbstractCluster
-from cpo.lib.cluster.cluster_factory import AbstractClusterFactory, ClusterData
-from cpo.lib.openshift.cluster.generic_cluster import GenericCluster
+from cpo.config.cluster_credentials_manager import cluster_credentials_manager
 
 
-class GenericClusterFactory(AbstractClusterFactory):
-    def create_cluster(self, server: str, cluster_data: ClusterData) -> AbstractCluster:
-        return GenericCluster(server, cluster_data)
+def get_current_cluster_alias():
+    current_cluster = cluster_credentials_manager.get_current_cluster()
 
-    def get_cluster_type_name(self) -> str:
-        return "Generic"
+    if current_cluster is not None:
+        cluster_data = current_cluster.get_cluster_data()
 
-
-generic_cluster_factory = GenericClusterFactory()
+        if "alias" in cluster_data:
+            print(cluster_data["alias"])
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/cluster_based_user_credentials.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/cluster_based_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/credentials.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/token_credentials.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/token_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/credentials/user_credentials.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/credentials/user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/data/global_pull_secret_data.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/data/global_pull_secret_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
 import json
 import re as regex
 
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 import click
 import jmespath
 
 from tabulate import tabulate
 
 from cpo.lib.openshift.types.auths_dict import AuthDict, AuthsDict
@@ -93,29 +93,29 @@
             flag indicating whether the JSON response of the OpenShift server shall
             be printed
         """
 
         if use_json:
             click.echo(json.dumps(self._secret_get_response, indent="\t", sort_keys=True))
         else:
-            auth_list: List[List[str]] = []
+            auth_list: list[list[str]] = []
             auths = self._secret_get_response["auths"]
 
             for image_registry, auth in auths.items():
                 search_result = regex.match("(.*)\\:(.*)", base64.standard_b64decode(auth["auth"]).decode("utf-8"))
 
                 if search_result is None:
                     raise CloudPakOperationsCLIException("…")
 
                 image_registry_password = search_result.group(2)
 
                 if len(image_registry_password) > 5:
                     image_registry_password = image_registry_password[0:5] + "…"
 
-                auth_list_element: List[str] = [image_registry, search_result.group(1), image_registry_password]
+                auth_list_element: list[str] = [image_registry, search_result.group(1), image_registry_password]
 
                 auth_list.append(auth_list_element)
 
             auth_list.sort(key=lambda auth_list_element: auth_list_element[0])
             click.echo(tabulate(auth_list, headers=["registry location", "username", "password"]))
 
     def get_credentials(self, registry_location: str) -> Optional[Credentials]:
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,16 +10,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
-from typing import List
-
 from cpo.lib.openshift.credentials.credentials import AbstractCredentials
 from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.lib.openshift.types.object_meta import ObjectMeta
 from cpo.lib.openshift.types.role_rule import RoleRule
 
 logger = logging.getLogger(__name__)
 
@@ -62,15 +60,15 @@
 
         cluster_role_name = "system:openshift:scc:hostmount-anyuid"
         cluster_role_binding_name = "system:openshift:scc:hostmount-anyuid"
 
         if not self._openshift_api_manager.cluster_role_exists(cluster_role_name):
             logger.info(f"Creating cluster role '{cluster_role_name}'")
 
-            rules: List[RoleRule] = [
+            rules: list[RoleRule] = [
                 {
                     "apiGroups": [
                         "security.openshift.io",
                     ],
                     "resourceNames": [
                         "hostmount-anyuid",
                     ],
@@ -86,15 +84,15 @@
             self._openshift_api_manager.create_system_cluster_role(cluster_role_name, rules)
         else:
             logger.info(f"Skipping creation of cluster role '{cluster_role_name}'")
 
         if not self._openshift_api_manager.cluster_role_binding_exists(cluster_role_binding_name):
             logger.info(f"Creating cluster role binding '{cluster_role_binding_name}'")
 
-            subjects: List[ObjectMeta] = [
+            subjects: list[ObjectMeta] = [
                 {
                     "name": "nfs-client-provisioner",
                     "namespace": self._project,
                 }
             ]
 
             self._openshift_api_manager.create_system_cluster_role_binding(
@@ -107,15 +105,15 @@
         """Creates the 'nfs-client-provisioner-runner' cluster role"""
 
         cluster_role_name = "nfs-client-provisioner-runner"
 
         if not self._openshift_api_manager.cluster_role_exists(cluster_role_name):
             logger.info(f"Creating cluster role '{cluster_role_name}'")
 
-            rules: List[RoleRule] = [
+            rules: list[RoleRule] = [
                 {
                     "apiGroups": [""],
                     "resources": ["events"],
                     "verbs": [
                         "create",
                         "patch",
                         "update",
@@ -175,15 +173,15 @@
         """
 
         cluster_role_binding_name = "run-nfs-client-provisioner"
 
         if not self._openshift_api_manager.cluster_role_binding_exists(cluster_role_binding_name):
             logger.info(f"Creating cluster role binding '{cluster_role_binding_name}'")
 
-            subjects: List[ObjectMeta] = [
+            subjects: list[ObjectMeta] = [
                 {
                     "name": "nfs-client-provisioner",
                     "namespace": self._project,
                 }
             ]
 
             self._openshift_api_manager.create_cluster_role_binding(
@@ -279,15 +277,15 @@
         project specified in the constructor"""
 
         role_name = "leader-locking-nfs-client-provisioner"
 
         if not self._openshift_api_manager.role_exists(self._project, role_name):
             logger.info(f"Creating role '{role_name}'")
 
-            rules: List[RoleRule] = [
+            rules: list[RoleRule] = [
                 {
                     "apiGroups": [""],
                     "resources": ["endpoints"],
                     "verbs": [
                         "create",
                         "get",
                         "list",
@@ -312,15 +310,15 @@
         """
 
         role_binding_name = "leader-locking-nfs-client-provisioner"
 
         if not self._openshift_api_manager.role_binding_exists(self._project, role_binding_name):
             logger.info(f"Creating role binding '{role_binding_name}'")
 
-            subjects: List[ObjectMeta] = [
+            subjects: list[ObjectMeta] = [
                 {
                     "name": "nfs-client-provisioner",
                     "namespace": self._project,
                 }
             ]
 
             self._openshift_api_manager.create_role_binding(
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/oc.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/oc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,27 +11,26 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import tempfile
 
-from typing import Final, List
+from typing import Final
 
 import semver
 
 import cpo.config
 import cpo.utils.network
 import cpo.utils.process
 
 from cpo.lib.dependency_manager import dependency_manager
 from cpo.lib.dependency_manager.plugins.openshift_cli_plugin import OpenShiftCLIPlugIn
 from cpo.lib.openshift.types.get_pod_entry import GetPodEntry
 from cpo.utils.error import CloudPakOperationsCLIException
-from cpo.utils.string import removeprefix, removesuffix
 
 OPENSHIFT_REST_API_VERSION: Final[str] = "v1"
 
 
 def enable_image_registry_default_route():
     """Enables the Image Registry default route with the Custom Resource
     Definition
@@ -48,15 +47,15 @@
         "merge",
     ]
 
     execute_oc_command(oc_patch_args)
 
 
 def execute_oc_command(
-    args: List[str],
+    args: list[str],
     capture_output=False,
     check=True,
     print_captured_output=False,
 ) -> cpo.utils.process.ProcessResult:
     """Executes the OpenShift Container Platform CLI
 
     Parameters
@@ -105,28 +104,28 @@
     ]
 
     oc_whoami_command_result = execute_oc_command(oc_whoami_args, capture_output=True)
 
     return oc_whoami_command_result.stdout.rstrip()
 
 
-def get_oc_login_args_with_password(server: str, username: str, password: str) -> List[str]:
+def get_oc_login_args_with_password(server: str, username: str, password: str) -> list[str]:
     return [
         "login",
         "--insecure-skip-tls-verify",
         "--password",
         password,
         "--server",
         server,
         "--username",
         username,
     ]
 
 
-def get_oc_login_args_with_token(server: str, token: str) -> List[str]:
+def get_oc_login_args_with_token(server: str, token: str) -> list[str]:
     return [
         "login",
         "--insecure-skip-tls-verify",
         "--server",
         server,
         "--token",
         token,
@@ -160,16 +159,16 @@
         "route",
         "--namespace",
         "openshift-image-registry",
         "--output",
         "jsonpath='{.items[?(@.metadata.name==\"" + route_name + "\")].spec.host}'",
     ]
 
-    oc_get_route_command_result = removesuffix(
-        removeprefix(execute_oc_command(oc_get_route_args, capture_output=True).stdout, "'"), "'"
+    oc_get_route_command_result = (
+        execute_oc_command(oc_get_route_args, capture_output=True).stdout.removeprefix("'").removesuffix("'")
     )
 
     return oc_get_route_command_result
 
 
 def get_openshift_version() -> semver.VersionInfo:
     oc_version_args = ["version", "--output", "json"]
@@ -205,16 +204,16 @@
     oc_get_pv_args = [
         "get",
         "pv",
         "--output",
         f"jsonpath='{{.items[?(@.metadata.name==\"{persistent_volume_name}\")].metadata.labels.volumeId}}'",
     ]
 
-    oc_get_pv_command_result = removesuffix(
-        removeprefix(execute_oc_command(oc_get_pv_args, capture_output=True).stdout, "'"), "'"
+    oc_get_pv_command_result = (
+        execute_oc_command(oc_get_pv_args, capture_output=True).stdout.removeprefix("'").removesuffix("'")
     )
 
     if oc_get_pv_command_result == "":
         raise CloudPakOperationsCLIException(
             f"Persistent volume with name '{persistent_volume_name}' could not be found"
         )
 
@@ -234,15 +233,15 @@
     token"""
 
     oc_login_args = get_oc_login_args_with_token(server, token)
 
     execute_oc_command(oc_login_args)
 
 
-def get_deployment_name(search_string: str) -> List[str]:
+def get_deployment_name(search_string: str) -> list[str]:
     """Returns the available OpenShift deployment(s) for a given search string"""
 
     oc_get_deployments_args = ["get", "deployments"]
 
     oc_get_deployments_result = execute_oc_command(oc_get_deployments_args, capture_output=True).stdout
 
     result = []
@@ -254,15 +253,15 @@
         raise CloudPakOperationsCLIException(
             f"Deployment(s) containing the string '{search_string}' could not be found"
         )
 
     return result
 
 
-def get_pod_name(search_string: str) -> List[str]:
+def get_pod_name(search_string: str) -> list[str]:
     """Returns the available OpenShift pod(s) for a given search string"""
 
     oc_get_pods_args = ["get", "pods"]
 
     oc_get_pods_result = execute_oc_command(oc_get_pods_args, capture_output=True).stdout
 
     result = []
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/openshift_api_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/openshift_api_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Optional
 
 import semver
 import urllib3.exceptions
 
 from kubernetes import client, config, watch
 
 import cpo.lib.jmespath
@@ -50,15 +50,15 @@
     client (https://github.com/openshift/openshift-restclient-python) was
     deliberately not used as its performance suffers from the amount of REST
     API calls during endpoint discovery.
     """
 
     def __init__(self, credentials: AbstractCredentials):
         self._credentials = credentials
-        self._kube_config_dict: Dict[str, Any] = {}
+        self._kube_config_dict: dict[str, Any] = {}
         self._kube_config_initialized = False
 
     def cluster_role_exists(self, name: str) -> bool:
         """Returns whether the cluster role with the given name exists
 
         Parameters
         ----------
@@ -106,15 +106,15 @@
             project in which the catalog source shall be created
         catalog_source
             catalog source specification
         """
 
         self.execute_kubernetes_client(self._create_catalog_source, catalog_source=catalog_source, project=project)
 
-    def create_cluster_role(self, name: str, rules: List[RoleRule]):
+    def create_cluster_role(self, name: str, rules: list[RoleRule]):
         """Creates a cluster role
 
         Parameters
         ----------
         name
             cluster role name
         rules
@@ -125,15 +125,15 @@
             self._create_cluster_role,
             metadata={
                 "name": name,
             },
             rules=rules,
         )
 
-    def create_cluster_role_binding(self, name: str, subjects: List[ObjectMeta], role_ref_name: str):
+    def create_cluster_role_binding(self, name: str, subjects: list[ObjectMeta], role_ref_name: str):
         """Creates a cluster role binding
 
         Parameters
         ----------
         name
             cluster role binding name
         subjects
@@ -200,30 +200,30 @@
         ----------
         name
             name of the project to be created
         """
 
         self.execute_kubernetes_client(self._create_project, name=name)
 
-    def create_role(self, project: str, name: str, rules: List[RoleRule]):
+    def create_role(self, project: str, name: str, rules: list[RoleRule]):
         """Creates a role
 
         Parameters
         ----------
         project
             project in which the role shall be created
         name
             role name
         rules
             rule specifications
         """
 
         self.execute_kubernetes_client(self._create_role, name=name, project=project, rules=rules)
 
-    def create_role_binding(self, project: str, name: str, subjects: List[ObjectMeta], role_ref_name: str):
+    def create_role_binding(self, project: str, name: str, subjects: list[ObjectMeta], role_ref_name: str):
         """Creates a role binding
 
         Parameters
         ----------
         project
             project in which the role binding shall be created
         name
@@ -235,15 +235,15 @@
             role defining permissions granted to the given subjects
         """
 
         self.execute_kubernetes_client(
             self._create_role_binding, name=name, project=project, role_ref_name=role_ref_name, subjects=subjects
         )
 
-    def create_storage_class(self, name: str, provisioner: str, parameters: Dict[str, str]):
+    def create_storage_class(self, name: str, provisioner: str, parameters: dict[str, str]):
         """Creates a storage class
 
         Parameters
         ----------
         name
             storage class name
         provisioner
@@ -268,15 +268,15 @@
             project in which the subscription shall be created
         name
             subscription specification
         """
 
         self.execute_kubernetes_client(self._create_subscription, project=project, subscription=subscription)
 
-    def create_system_cluster_role(self, name: str, rules: List[RoleRule]):
+    def create_system_cluster_role(self, name: str, rules: list[RoleRule]):
         """Creates a system cluster role
 
         Parameters
         ----------
         name
             cluster role name
         rules
@@ -288,15 +288,15 @@
             metadata={
                 "creationTimestamp": None,
                 "name": name,
             },
             rules=rules,
         )
 
-    def create_system_cluster_role_binding(self, name: str, subjects: List[ObjectMeta], role_ref_name: str):
+    def create_system_cluster_role_binding(self, name: str, subjects: list[ObjectMeta], role_ref_name: str):
         """Creates a system cluster role binding
 
         Parameters
         ----------
         name
             cluster role binding name
         subjects
@@ -471,15 +471,15 @@
         return self.execute_kubernetes_client(
             self._namespaced_custom_object_exists,
             kind_metadata=KindMetadata("apps", "Deployment", "deployments", "v1"),
             name=name,
             project=project,
         )
 
-    def get_kube_config(self) -> Dict[str, Any]:
+    def get_kube_config(self) -> dict[str, Any]:
         if not self._kube_config_initialized:
             self._set_kube_config()
 
         return self._kube_config_dict
 
     def namespaced_custom_resource_exists(self, project: str, name: str, kind_metadata: KindMetadata) -> bool:
         """Returns whether the custom resource with the given name in the given
@@ -591,25 +591,25 @@
         -------
         Any
             custom resource definitions
         """
 
         return self.execute_kubernetes_client(self._get_custom_resource_definitions)
 
-    def get_custom_resources(self, kind_metadata: KindMetadata) -> List[Any]:
+    def get_custom_resources(self, kind_metadata: KindMetadata) -> list[Any]:
         """Returns custom resources of the given kind
 
         Parameters
         ----------
         kind_metadata
             kind metadata of custom resources to return
 
         Returns
         -------
-        List[Any]
+        list[Any]
             custom resources of the given kind
         """
 
         return self.execute_kubernetes_client(self._get_custom_resources, kind_metadata=kind_metadata)
 
     def get_global_pull_secret_data(self) -> GlobalPullSecretData:
         """Returns the global pull secret as a data object
@@ -704,14 +704,15 @@
         return self.execute_kubernetes_client(self._project_exists, name=name)
 
     def refresh_access_token(self):
         if not self._credentials.is_refreshable():
             raise CloudPakOperationsCLIException("OAuth access token expired and cannot be refreshed")
 
         self._credentials.refresh_access_token()
+        self._kube_config_initialized = False
 
     def role_binding_exists(self, project: str, name: str) -> bool:
         """Returns whether the role binding with the given name exists in the
         given project
 
         Parameters
         ----------
@@ -841,15 +842,15 @@
         )
 
     def wait_for_custom_resource(
         self,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
         success_callback: Callable[..., bool],
-        **kwargs
+        **kwargs,
     ):
         """Waits for a specific custom resource of the given kind to be created
 
         The passed callback is used for checking wheter a created custom resource
         of the given kind is the sought-after custom resource.
 
         Parameters
@@ -865,24 +866,24 @@
         """
 
         self.execute_kubernetes_client(
             self._wait_for_custom_resource,
             kind_metadata=kind_metadata,
             log_callback=log_callback,
             success_callback=success_callback,
-            **kwargs
+            **kwargs,
         )
 
     def wait_for_namespaced_custom_resource(
         self,
         project: str,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
         success_callback: Callable[..., Optional[CustomResourceEventResult]],
-        **kwargs
+        **kwargs,
     ) -> CustomResourceEventResult:
         """Waits for a specific custom resource of the given kind to be created in
         the given project
 
         The passed callback is used for checking wheter a created custom resource
         of the given kind is the sought-after custom resource.
 
@@ -902,35 +903,35 @@
 
         return self.execute_kubernetes_client(
             self._wait_for_namespaced_custom_resource,
             kind_metadata=kind_metadata,
             log_callback=log_callback,
             project=project,
             success_callback=success_callback,
-            **kwargs
+            **kwargs,
         )
 
     def _create_catalog_source(self, project: str, catalog_source: CatalogSource):
         custom_objects_api = client.CustomObjectsApi()
         custom_objects_api.create_namespaced_custom_object(
             "operators.coreos.com", "v1alpha1", project, "catalogsources", catalog_source
         )
 
-    def _create_cluster_role(self, metadata: ObjectMeta, rules: List[RoleRule]):
+    def _create_cluster_role(self, metadata: ObjectMeta, rules: list[RoleRule]):
         cluster_role: Role = {
             "kind": "ClusterRole",
             "apiVersion": "rbac.authorization.k8s.io/v1",
             "metadata": metadata,
             "rules": rules,
         }
 
         custom_objects_api = client.CustomObjectsApi()
         custom_objects_api.create_cluster_custom_object("rbac.authorization.k8s.io", "v1", "clusterroles", cluster_role)
 
-    def _create_cluster_role_binding(self, metadata: ObjectMeta, subjects: List[ObjectMeta], role_ref_name: str):
+    def _create_cluster_role_binding(self, metadata: ObjectMeta, subjects: list[ObjectMeta], role_ref_name: str):
         cluster_role_binding: RoleBinding = {
             "apiVersion": "rbac.authorization.k8s.io/v1",
             "kind": "ClusterRoleBinding",
             "metadata": metadata,
             "roleRef": {
                 "apiGroup": "rbac.authorization.k8s.io",
                 "kind": "ClusterRole",
@@ -1011,29 +1012,29 @@
                 "kind": "Namespace",
                 "metadata": {
                     "name": name,
                 },
             }
         )
 
-    def _create_role(self, project: str, name: str, rules: List[RoleRule]):
+    def _create_role(self, project: str, name: str, rules: list[RoleRule]):
         role: Role = {
             "apiVersion": "rbac.authorization.k8s.io/v1",
             "kind": "Role",
             "metadata": {
                 "name": name,
                 "namespace": project,
             },
             "rules": rules,
         }
 
         custom_objects_api = client.CustomObjectsApi()
         custom_objects_api.create_namespaced_custom_object("rbac.authorization.k8s.io", "v1", project, "roles", role)
 
-    def _create_role_binding(self, project: str, name: str, subjects: List[ObjectMeta], role_ref_name: str):
+    def _create_role_binding(self, project: str, name: str, subjects: list[ObjectMeta], role_ref_name: str):
         role_binding: RoleBinding = {
             "apiVersion": "rbac.authorization.k8s.io/v1",
             "kind": "RoleBinding",
             "metadata": {
                 "name": name,
                 "namespace": project,
             },
@@ -1068,15 +1069,15 @@
                 "namespace": project,
             },
         }
 
         core_v1_api = client.CoreV1Api()
         core_v1_api.create_namespaced_service_account(project, service_account)
 
-    def _create_storage_class(self, name: str, provisioner: str, parameters: Dict[str, str]):
+    def _create_storage_class(self, name: str, provisioner: str, parameters: dict[str, str]):
         storage_class = {
             "apiVersion": "storage.k8s.io/v1",
             "kind": "StorageClass",
             "metadata": {
                 "name": name,
             },
             "provisioner": provisioner,
@@ -1154,22 +1155,22 @@
 
     def _get_credentials(self) -> GlobalPullSecretData:
         core_v1_api = client.CoreV1Api()
         core_v1_api_result: Any = core_v1_api.read_namespaced_secret("pull-secret", "openshift-config")
 
         return GlobalPullSecretData(core_v1_api_result.data)
 
-    def _get_custom_resources(self, kind_metadata: KindMetadata) -> List[Any]:
+    def _get_custom_resources(self, kind_metadata: KindMetadata) -> list[Any]:
         custom_objects_api = client.CustomObjectsApi()
         custom_objects_api_result: Any = custom_objects_api.list_cluster_custom_object(
             kind_metadata.group, kind_metadata.version, kind_metadata.plural
         )
 
         assert "items" in custom_objects_api_result
-        assert isinstance(custom_objects_api_result["items"], List)
+        assert isinstance(custom_objects_api_result["items"], list)
 
         return custom_objects_api_result["items"]
 
     def _get_namespaced_custom_resource_if_exists(self, project: str, name: str, kind_metadata: KindMetadata) -> Any:
         custom_objects_api = client.CustomObjectsApi()
         custom_resource: Optional[Any] = None
 
@@ -1327,15 +1328,15 @@
         self._kube_config_initialized = True
 
     def _wait_for_custom_resource(
         self,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
         success_callback: Callable[..., bool],
-        **kwargs
+        **kwargs,
     ):
         custom_objects_api = client.CustomObjectsApi()
         succeeded = False
 
         while not succeeded:
             try:
                 resource_version: Optional[str] = None
@@ -1361,15 +1362,15 @@
 
     def _wait_for_namespaced_custom_resource(
         self,
         project: str,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
         success_callback: Callable[..., Optional[CustomResourceEventResult]],
-        **kwargs
+        **kwargs,
     ) -> CustomResourceEventResult:
         custom_objects_api = client.CustomObjectsApi()
         custom_resource_event_result: Optional[CustomResourceEventResult] = None
 
         while custom_resource_event_result is None:
             try:
                 resource_version: Optional[str] = None
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/get_pod_entry.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/get_pod_entry.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/object_meta.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Dict, Optional, TypedDict
+from typing import TypedDict
 
+from cpo.lib.openshift.types.object_meta import ObjectMeta
+from cpo.lib.openshift.types.role_rule import RoleRule
 
-class ObjectMetaOptional(TypedDict, total=False):
-    creationTimestamp: Optional[str]
-    labels: Dict[str, str]
-    namespace: str
 
-
-class ObjectMetaRequired(TypedDict):
-    name: str
-
-
-class ObjectMeta(ObjectMetaOptional, ObjectMetaRequired, total=False):
+class Role(TypedDict):
     """
     Notes
     -----
-    https://docs.openshift.com/container-platform/latest/rest_api/objects/index.html#objectmeta_v2-meta-v1"""
+    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/clusterrole-rbac-authorization-k8s-io-v1.html#clusterrole-rbac-authorization-k8s-io-v1
+    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/role-rbac-authorization-k8s-io-v1.html#role-rbac-authorization-k8s-io-v1
+    """
+
+    apiVersion: str
+    kind: str
+    metadata: ObjectMeta
+    rules: list[RoleRule]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/role.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/role_binding.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import List, TypedDict
+from typing import TypedDict
 
 from cpo.lib.openshift.types.object_meta import ObjectMeta
-from cpo.lib.openshift.types.role_rule import RoleRule
 
 
-class Role(TypedDict):
+class RoleBindingRoleRef(TypedDict):
+    apiGroup: str
+    kind: str
+    name: str
+
+
+class RoleBindingSubject(TypedDict):
+    kind: str
+    name: str
+    namespace: str
+
+
+class RoleBinding(TypedDict):
     """
     Notes
     -----
-    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/clusterrole-rbac-authorization-k8s-io-v1.html#clusterrole-rbac-authorization-k8s-io-v1
-    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/role-rbac-authorization-k8s-io-v1.html#role-rbac-authorization-k8s-io-v1
+    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/clusterrolebinding-rbac-authorization-k8s-io-v1.html#clusterrolebinding-rbac-authorization-k8s-io-v1
+    https://docs.openshift.com/container-platform/latest/rest_api/rbac_apis/rolebinding-rbac-authorization-k8s-io-v1.html#rolebinding-rbac-authorization-k8s-io-v1
     """
 
     apiVersion: str
     kind: str
     metadata: ObjectMeta
-    rules: List[RoleRule]
+    roleRef: RoleBindingRoleRef
+    subjects: list[RoleBindingSubject]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/openshift/types/subscription.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/openshift/types/subscription.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/distribution_entry_point_loader.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/distribution_entry_point_loader.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/package_data.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/package_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import pathlib
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import Optional
 
 
 @dataclass
 class PackageElementDescriptor:
     command_hierarchy_path: Optional[str]
     distribution_package_name: str
     name: str
@@ -70,17 +70,17 @@
                         command_hierarchy_path, distribution_package_name, file_path.name[:-3], file_path
                     )
                 )
 
         return package_data
 
     def __init__(self):
-        self._modules: List[PackageElementDescriptor] = []
-        self._subpackages: List[PackageElementDescriptor] = []
+        self._modules: list[PackageElementDescriptor] = []
+        self._subpackages: list[PackageElementDescriptor] = []
 
     @property
-    def modules(self) -> List[PackageElementDescriptor]:
+    def modules(self) -> list[PackageElementDescriptor]:
         return self._modules
 
     @property
-    def subpackages(self) -> List[PackageElementDescriptor]:
+    def subpackages(self) -> list[PackageElementDescriptor]:
         return self._subpackages
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/lib/plugin_manager/plugin_manager.py` & `cloud-pak-operations-cli-0.4.0/cpo/lib/plugin_manager/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 import logging
 import pathlib
 
 from importlib.metadata import entry_points
 from types import ModuleType
-from typing import Dict, Optional
+from typing import Optional
 
 from cpo.lib.plugin_manager.distribution_entry_point_loader import DistributionEntryPointLoader
 from cpo.lib.plugin_manager.package_data import PackageData
 from cpo.utils.error import CloudPakOperationsCLIException
 
 logger = logging.getLogger(__name__)
 
@@ -63,25 +63,25 @@
 
     Notes
     -----
     https://packaging.python.org/guides/creating-and-discovering-plugins/#using-package-metadata
     """
 
     def __init__(self):
-        self._package_data_dict: Optional[Dict[str, PackageData]] = None
+        self._package_data_dict: Optional[dict[str, PackageData]] = None
 
     def reload(self):
         """Reloads CLI plug-ins"""
 
         self._package_data_dict = None
 
         self._load_plugins_if_required()
 
     @property
-    def package_data_dict(self) -> Dict[str, PackageData]:
+    def package_data_dict(self) -> dict[str, PackageData]:
         self._load_plugins_if_required()
 
         assert self._package_data_dict is not None
 
         return self._package_data_dict
 
     def _load_plugins_if_required(self):
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/compression.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/compression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,16 +18,14 @@
 import tarfile
 import zipfile
 
 from typing import Any, Callable
 
 import cpo.utils.file
 
-from cpo.utils.string import removeprefix
-
 MemberIdentificationFunc = Callable[[str, cpo.utils.file.FileType], bool]
 PostExtractionFunc = Callable[[pathlib.Path], None]
 
 
 def execute_post_extraction_func_if_exists(extracted_file_path: pathlib.Path, **kwargs: Any):
     """Calls an optional function to perform post-extraction actions
 
@@ -107,15 +105,15 @@
                 if "directoryPathToStartExtraction" in kwargs:
                     directory_path_to_start_extraction = kwargs["directoryPathToStartExtraction"]
                     search_result = regex.search(f"({directory_path_to_start_extraction}/).*", member.name)
 
                     if search_result is None:
                         continue
 
-                    member.name = removeprefix(member.name, search_result.group(1))
+                    member.name = member.name.removeprefix(search_result.group(1))
 
                 if is_directory_structure_to_be_ignored(**kwargs):
                     member.name = os.path.basename(member.name)
 
                 tar_file.extract(member, target_directory_path)
                 execute_post_extraction_func_if_exists(target_directory_path / member.name, **kwargs)
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/download.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 import logging
 import os
 import pathlib
 import re as regex
 import tempfile
 import urllib.parse
 
-from typing import Any, Dict
+from typing import Any
 
 import requests
 
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
@@ -49,15 +49,15 @@
 
     Returns
     -------
     pathlib.Path
         Path of the downloaded file
     """
 
-    args: Dict[str, Any] = {}
+    args: dict[str, Any] = {}
 
     if "auth" in kwargs:
         args["auth"] = kwargs["auth"]
 
     if "headers" in kwargs:
         args["headers"] = kwargs["headers"]
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/error.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/error.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/file.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/file.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/importlib.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/importlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,31 +11,29 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import collections
 import importlib.metadata
 
-from typing import List
-
 import cpo
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 def get_distribution_package_name() -> str:
     """Returns the name of the distribution package providing the "cpo" top-level package
 
     Returns
     -------
     str
         name of the distribution package providing the "cpo" top-level package
     """
 
-    packages_to_distribution_packages_dict: collections.defaultdict[str, List[str]] = collections.defaultdict(list)
+    packages_to_distribution_packages_dict: collections.defaultdict[str, list[str]] = collections.defaultdict(list)
 
     for distribution in importlib.metadata.distributions():
         file_contents = distribution.read_text("top_level.txt")
 
         if file_contents is None:
             continue
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/logging.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import time
 
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable, Optional
 
 import click
 
 from halo import Halo
 
 
 class ClickLoggingFormatter(logging.Formatter):
@@ -59,15 +59,15 @@
             "CRITICAL": dict(fg="magenta"),
             "DEBUG": dict(fg="blue"),
             "ERROR": dict(fg="red"),
             "WARNING": dict(fg="yellow"),
         }
 
         return (
-            click.style(logging.Formatter.format(self, record), **colors[record.levelname])
+            click.style(logging.Formatter.format(self, record), **colors[record.levelname])  # type: ignore
             if record.levelname in colors
             else logging.Formatter.format(self, record)
         )
 
 
 class ClickLoggingHandler(logging.Handler):
     """Click-based log handler"""
@@ -183,15 +183,15 @@
         expose_value=False,
         help="Log level",
         is_eager=True,
         type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False),
     )
 
 
-def _get_click_command_with_log_level_option(default_log_level: str) -> Type[click.Command]:
+def _get_click_command_with_log_level_option(default_log_level: str) -> type[click.Command]:
     """Creates a definition of a subclass of click.Command
 
     This method creates a definition of a subclass of click.Command. Click
     commands based on this subclass have a --loglevel option.
 
     Parameters
     ----------
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/network.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,16 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import ipaddress
 import socket
 import warnings
 
-from typing import List
-
 import netifaces
 import urllib3
 import urllib3.exceptions
 
 
 class ScopedInsecureRequestWarningDisabler:
     """Temporarily disables warnings of type InsecureRequestWarning"""
@@ -56,24 +54,24 @@
     # disable warning:
     # InsecureRequestWarning: Unverified HTTPS request is being made to host
     # '…'. Adding certificate verification is strongly advised. See:
     # https://urllib3.readthedocs.io/en/latest/advanced-usage.html#ssl-warnings
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
-def get_local_ipv4_addresses() -> List[ipaddress.IPv4Address]:
+def get_local_ipv4_addresses() -> list[ipaddress.IPv4Address]:
     """Returns all IPv4 addresses bound to local network interfaces
 
     Returns
     -------
     list[ipaddress.IPv4Address]
         all IPv4 addresses bound to local network interfaces
     """
 
-    result: List[ipaddress.IPv4Address] = []
+    result: list[ipaddress.IPv4Address] = []
 
     for interface in netifaces.interfaces():
         ifaddresses = netifaces.ifaddresses(interface)
 
         if netifaces.AF_INET in ifaddresses:
             # IPv4 address is bound to NIC
             ifaddress = ifaddresses[netifaces.AF_INET][0]
@@ -106,15 +104,15 @@
 
     ipv4_address = ipaddress.ip_address(socket.gethostbyname(hostname))
     local_ipv4_addresses = get_local_ipv4_addresses()
 
     return ipv4_address in local_ipv4_addresses
 
 
-def parse_hostname_result(hostname_result: str) -> List[ipaddress.IPv4Address]:
+def parse_hostname_result(hostname_result: str) -> list[ipaddress.IPv4Address]:
     """Parses the output of the hostname command (Linux)
 
     Parameters
     ----------
     hostname_result
         output of the hostname command (Linux)
 
@@ -122,14 +120,14 @@
     -------
     list[ipaddress.IPv4Address]
         all IPv4 addresses bound to local network interfaces
     """
 
     hostnames = hostname_result.rstrip().split(" ")
     ip_addresses = list(map(lambda str: ipaddress.ip_address(str), hostnames))
-    ipv4_addresses: List[ipaddress.IPv4Address] = []
+    ipv4_addresses: list[ipaddress.IPv4Address] = []
 
     for ip_address in ip_addresses:
         if isinstance(ip_address, ipaddress.IPv4Address):
             ipv4_addresses.append(ip_address)
 
     return ipv4_addresses
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/operating_system.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/operating_system.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/path.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/path.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/process.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,23 +13,23 @@
 #  limitations under the License.
 
 import asyncio
 import logging
 import os
 import pathlib
 
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Optional
 
 import click
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 class ProcessResult:
-    def __init__(self, command: List[str], return_code: int, stderr: List[str], stdout: List[str]):
+    def __init__(self, command: list[str], return_code: int, stderr: list[str], stdout: list[str]):
         self.command = command
         self.return_code = return_code
         self._stderr = stderr
         self._stdout = stdout
 
     def raise_for_status(self):
         if self.return_code != 0:
@@ -48,16 +48,16 @@
     @property
     def stdout(self) -> str:
         return "\n".join(self._stdout)
 
 
 def execute_command(
     program: pathlib.Path,
-    args: List[str],
-    env: Dict[str, str] = os.environ.copy(),
+    args: list[str],
+    env: dict[str, str] = os.environ.copy(),
     capture_output=False,
     check=True,
     print_captured_output=False,
 ) -> ProcessResult:
     """Executes a process
 
     Parameters
@@ -85,16 +85,16 @@
     """
 
     command = [str(program)] + args
 
     logging.debug(f"Executing command: {' '.join(command)}")
 
     return_code: Optional[int] = None
-    stderr_buffer: List[str] = []
-    stdout_buffer: List[str] = []
+    stderr_buffer: list[str] = []
+    stdout_buffer: list[str] = []
 
     if capture_output:
         return_code = asyncio.run(
             _create_subprocess_and_capture_output(
                 program,
                 args,
                 env,
@@ -110,15 +110,15 @@
     if check:
         result.raise_for_status()
 
     return result
 
 
 def execute_command_without_check(
-    program: pathlib.Path, args: List[str], capture_output=True, print_captured_output=False
+    program: pathlib.Path, args: list[str], capture_output=True, print_captured_output=False
 ) -> ProcessResult:
     """Executes a process without checking its return code
 
     Parameters
     ----------
     program
         path of the executable
@@ -142,15 +142,15 @@
         args,
         capture_output=capture_output,
         check=False,
         print_captured_output=print_captured_output,
     )
 
 
-async def _create_subprocess(program: pathlib.Path, args: List[str], env: Dict[str, str]) -> int:
+async def _create_subprocess(program: pathlib.Path, args: list[str], env: dict[str, str]) -> int:
     """Executes a process
 
     Parameters
     ----------
     program
         path of the executable
     args
@@ -166,15 +166,15 @@
 
     process = await asyncio.create_subprocess_exec(*([str(program)] + args), env=env)
 
     return await process.wait()
 
 
 async def _create_subprocess_and_capture_output(
-    program: pathlib.Path, args: List[str], env: Dict[str, str], stdout_callback, stderr_callback
+    program: pathlib.Path, args: list[str], env: dict[str, str], stdout_callback, stderr_callback
 ) -> int:
     """Executes a process and captures its output to stdout/stderr
 
     Parameters
     ----------
     program
         path of the executable
@@ -206,22 +206,22 @@
             asyncio.create_task(_read_stream(process.stdout, stdout_callback)),
         ]
     )
 
     return await process.wait()
 
 
-def _process_stderr_output(line: str, buffer: List[str], print_captured_output: bool):
+def _process_stderr_output(line: str, buffer: list[str], print_captured_output: bool):
     if print_captured_output:
         click.echo(click.style(line, fg="red"), err=True, nl=False)
 
     buffer.append(line.rstrip())
 
 
-def _process_stdout_output(line: str, buffer: List[str], print_captured_output: bool):
+def _process_stdout_output(line: str, buffer: list[str], print_captured_output: bool):
     if print_captured_output:
         click.echo(line, nl=False)
 
     buffer.append(line.rstrip())
 
 
 async def _read_stream(stream: Optional[asyncio.StreamReader], callback: Callable[[str], None]):
```

### Comparing `cloud-pak-operations-cli-0.3.6/cpo/utils/ssh.py` & `cloud-pak-operations-cli-0.4.0/cpo/utils/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import pathlib
 
 from abc import ABC, abstractmethod
-from typing import Optional, Type
+from typing import Optional
 
 import asyncssh
 import click
 import colorama
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
@@ -114,15 +114,15 @@
 
         if self._connection is None:
             raise CloudPakOperationsCLIException("Not connected to " + self._hostname)
 
         await asyncssh.scp(str(path), self._connection)
 
 
-def create_remote_client_ssh_session(print_output: bool) -> Type[asyncssh.SSHClientSession]:
+def create_remote_client_ssh_session(print_output: bool) -> type[asyncssh.SSHClientSession]:
     """Returns a parameterized subclass of asyncssh.SSHClientSession that
     may be passed to asyncssh.SSHClientConnection.create_session()
 
     Parameters
     ----------
     print_output
         flag indicating whether output to stdout and stderr of a command
```

### Comparing `cloud-pak-operations-cli-0.3.6/pyproject.toml` & `cloud-pak-operations-cli-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,42 +6,43 @@
 authors = [{ email = "db2datagate@ibm.com", name = "IBM Corporation" }]
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"License :: OSI Approved :: Apache Software License",
 	"Operating System :: MacOS",
 	"Operating System :: Microsoft :: Windows",
 	"Operating System :: POSIX :: Linux",
-	"Programming Language :: Python :: 3.8"
+	"Programming Language :: Python :: 3.10"
 ]
 dependencies = [
 	"ansible",
 	"ansible_runner",
 	"asyncssh",
 	"click",
 	"click-option-group",
 	"colorama",
 	"halo",
 	"jmespath",
 	"jsonschema",
 	"kubernetes >= 12",
 	"netifaces",
+	"pypi_simple",
 	"pytest",
 	"pyyaml",
 	"q",
 	"requests",
 	"semver",
 	"tabulate",
 	"tqdm",
 	"urllib3"
 ]
 description = "IBM Cloud Pak Operations CLI"
 dynamic = ["version"]
 name = "cloud-pak-operations-cli"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 [project.scripts]
 cpo = "cpo.cpo:cli"
 cpo-get-current-cluster-alias = "cpo.scripts.get_current_cluster_alias:get_current_cluster_alias"
 
 [project.urls]
 repository = "https://github.com/IBM/cloud-pak-operations-cli"
```

