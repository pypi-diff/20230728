# Comparing `tmp/heat-agents-6.0.0.tar.gz` & `tmp/heat-agents-6.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-agents-6.0.0.tar", last modified: Wed Mar 22 12:20:44 2023, max compression
+gzip compressed data, was "heat-agents-6.0.0.0rc1.tar", last modified: Thu Mar  2 11:37:46 2023, max compression
```

## Comparing `heat-agents-6.0.0.tar` & `heat-agents-6.0.0.0rc1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.568376 heat-agents-6.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-03-22 12:20:15.000000 heat-agents-6.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-22 12:20:15.000000 heat-agents-6.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-03-22 12:20:44.000000 heat-agents-6.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-03-22 12:20:15.000000 heat-agents-6.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8333 2023-03-22 12:20:44.000000 heat-agents-6.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-22 12:20:15.000000 heat-agents-6.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-03-22 12:20:15.000000 heat-agents-6.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2023-03-22 12:20:44.568376 heat-agents-6.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-03-22 12:20:15.000000 heat-agents-6.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.536369 heat-agents-6.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.536369 heat-agents-6.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5639 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.536369 heat-agents-6.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.536369 heat-agents-6.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/building_image.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/doc/source/install/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/ansible.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/apply-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/cfn-init.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/chef.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/docker-cmd.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/docker-compose.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/hiera.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/json-file.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/kubelet.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/puppet.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/salt.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks/script.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/hooks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-22 12:20:15.000000 heat-agents-6.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5899 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/bin/heat-config-notify
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1397 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/bin/heat-config-rebuild-deployed
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.528367 heat-agents-6.0.0/heat-config/install.d/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config/install.d/heat-config-package-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       76 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/install.d/heat-config-package-install/50-heat-config-package
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config/install.d/heat-config-source-install/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      779 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/install.d/heat-config-source-install/50-heat-config-soure
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.532368 heat-agents-6.0.0/heat-config/os-apply-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config/os-apply-config/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/os-apply-config/etc/os-collect-config.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.532368 heat-agents-6.0.0/heat-config/os-apply-config/var/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.532368 heat-agents-6.0.0/heat-config/os-apply-config/var/run/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.556374 heat-agents-6.0.0/heat-config/os-apply-config/var/run/heat-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/os-apply-config/var/run/heat-config/heat-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.532368 heat-agents-6.0.0/heat-config/os-refresh-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.556374 heat-agents-6.0.0/heat-config/os-refresh-config/configure.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       42 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/os-refresh-config/configure.d/20-os-apply-config
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7556 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config/os-refresh-config/configure.d/55-heat-config
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-ansible/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-ansible/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-ansible/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      169 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-ansible/install.d/50-heat-config-hook-ansible
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4625 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-ansible/install.d/hook-ansible.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-apply-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-apply-config/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-apply-config/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      154 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-apply-config/install.d/50-heat-config-apply-config
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1787 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-apply-config/install.d/hook-apply-config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-cfn-init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-cfn-init/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.540370 heat-agents-6.0.0/heat-config-cfn-init/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      146 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-cfn-init/install.d/50-heat-config-hook-cfn-init
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2581 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-cfn-init/install.d/hook-cfn-init.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-chef/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-chef/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-chef/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      164 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-chef/install.d/50-heat-config-hook-chef
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6020 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-chef/install.d/hook-chef.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-cmd/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-cmd/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      150 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-cmd/install.d/50-heat-config-hook-docker-cmd
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7382 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-cmd/install.d/hook-docker-cmd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.528367 heat-agents-6.0.0/heat-config-docker-cmd/os-refresh-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-cmd/os-refresh-config/configure.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4440 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-cmd/os-refresh-config/configure.d/50-heat-config-docker-cmd
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-compose/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-compose/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-compose/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      406 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-compose/install.d/50-heat-config-hook-docker-compose
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3734 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-compose/install.d/hook-docker-compose.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.528367 heat-agents-6.0.0/heat-config-docker-compose/os-refresh-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-docker-compose/os-refresh-config/configure.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3484 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-docker-compose/os-refresh-config/configure.d/50-heat-config-docker-compose
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.544371 heat-agents-6.0.0/heat-config-hiera/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-hiera/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-hiera/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      212 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-hiera/install.d/50-heat-config-hook-hiera
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3929 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-hiera/install.d/hook-hiera.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-json-file/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-json-file/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-json-file/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      148 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-json-file/install.d/50-heat-config-hook-json-file
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1537 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-json-file/install.d/hook-json-file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-kubelet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-kubelet/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-kubelet/extra-data.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      307 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-kubelet/extra-data.d/50-docker-images
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-kubelet/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4491 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-kubelet/install.d/50-heat-config-kubelet
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6200 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-kubelet/install.d/hook-kubelet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.528367 heat-agents-6.0.0/heat-config-kubelet/os-refresh-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-kubelet/os-refresh-config/configure.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2132 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-kubelet/os-refresh-config/configure.d/50-heat-config-kubelet
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.548372 heat-agents-6.0.0/heat-config-puppet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-puppet/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config-puppet/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      166 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-puppet/install.d/50-heat-config-hook-puppet
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5976 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-puppet/install.d/hook-puppet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config-salt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-salt/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config-salt/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      168 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-salt/install.d/50-heat-config-hook-salt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3744 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-salt/install.d/hook-salt.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config-script/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-script/element-deps
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.552373 heat-agents-6.0.0/heat-config-script/install.d/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-script/install.d/50-heat-config-hook-script
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2998 2023-03-22 12:20:15.000000 heat-agents-6.0.0/heat-config-script/install.d/hook-script.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.556374 heat-agents-6.0.0/heat_agents.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:20:44.000000 heat-agents-6.0.0/heat_agents.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.532368 heat-agents-6.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.560375 heat-agents-6.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/docker-cmd-paunch-0a674fc1b84b2dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/drop-python-3-6-and-3-7-17dd2c0ff96ee806.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/heat-config-notify-retry-e01b995d239bb1fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/hook_docker_envfile-bc9eb287d854e1e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/notes/switch-docker-cmd-hook-to-docker-cli-5d8f6deee2125d65.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.564375 heat-agents-6.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5699 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-22 12:20:15.000000 heat-agents-6.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-22 12:20:15.000000 heat-agents-6.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-03-22 12:20:44.572377 heat-agents-6.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-03-22 12:20:15.000000 heat-agents-6.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-03-22 12:20:15.000000 heat-agents-6.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:44.568376 heat-agents-6.0.0/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1948 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/config-tool-fake.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5899 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/heat_config_notify.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1249 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/hook-fake-raises.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1920 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/hook-fake.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7382 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/hook_docker_cmd.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6200 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/hook_kubelet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10394 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_heat_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_heat_config_docker_compose.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_heat_config_kubelet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8471 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_heat_config_notify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9665 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_ansible.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_apply_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3653 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_cfn_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_chef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25130 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_docker_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5247 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_docker_compose.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_hiera.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2020 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_json_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4065 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_kubelet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_puppet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_salt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4777 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tests/test_hook_script.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-03-22 12:20:15.000000 heat-agents-6.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.356319 heat-agents-6.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8343 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2023-03-02 11:37:46.356319 heat-agents-6.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5639 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/building_image.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/doc/source/install/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/ansible.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/apply-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/cfn-init.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/chef.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/docker-cmd.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/docker-compose.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/hiera.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/json-file.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/kubelet.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/puppet.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/salt.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks/script.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/hooks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/heat-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5899 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/bin/heat-config-notify
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1397 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/bin/heat-config-rebuild-deployed
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config/install.d/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/install.d/heat-config-package-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       76 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/install.d/heat-config-package-install/50-heat-config-package
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/install.d/heat-config-source-install/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      779 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/install.d/heat-config-source-install/50-heat-config-soure
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/etc/os-collect-config.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/var/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/var/run/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/var/run/heat-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/os-apply-config/var/run/heat-config/heat-config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config/os-refresh-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config/os-refresh-config/configure.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       42 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/os-refresh-config/configure.d/20-os-apply-config
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7556 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config/os-refresh-config/configure.d/55-heat-config
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.340319 heat-agents-6.0.0.0rc1/heat-config-ansible/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-ansible/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-ansible/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      169 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-ansible/install.d/50-heat-config-hook-ansible
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4625 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-ansible/install.d/hook-ansible.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-apply-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-apply-config/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-apply-config/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      154 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-apply-config/install.d/50-heat-config-apply-config
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1787 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-apply-config/install.d/hook-apply-config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-cfn-init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-cfn-init/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-cfn-init/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      146 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-cfn-init/install.d/50-heat-config-hook-cfn-init
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2581 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-cfn-init/install.d/hook-cfn-init.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-chef/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-chef/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-chef/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      164 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-chef/install.d/50-heat-config-hook-chef
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6020 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-chef/install.d/hook-chef.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      150 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/install.d/50-heat-config-hook-docker-cmd
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7382 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/install.d/hook-docker-cmd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/os-refresh-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/os-refresh-config/configure.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4440 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-cmd/os-refresh-config/configure.d/50-heat-config-docker-cmd
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-compose/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-compose/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-compose/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      406 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-compose/install.d/50-heat-config-hook-docker-compose
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3734 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-compose/install.d/hook-docker-compose.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config-docker-compose/os-refresh-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-docker-compose/os-refresh-config/configure.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3484 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-docker-compose/os-refresh-config/configure.d/50-heat-config-docker-compose
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-hiera/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-hiera/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-hiera/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      212 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-hiera/install.d/50-heat-config-hook-hiera
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3929 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-hiera/install.d/hook-hiera.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-json-file/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-json-file/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-json-file/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      148 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-json-file/install.d/50-heat-config-hook-json-file
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1537 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-json-file/install.d/hook-json-file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-kubelet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-kubelet/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-kubelet/extra-data.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      307 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-kubelet/extra-data.d/50-docker-images
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-kubelet/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4491 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-kubelet/install.d/50-heat-config-kubelet
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6200 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-kubelet/install.d/hook-kubelet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/heat-config-kubelet/os-refresh-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-kubelet/os-refresh-config/configure.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2132 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-kubelet/os-refresh-config/configure.d/50-heat-config-kubelet
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.344318 heat-agents-6.0.0.0rc1/heat-config-puppet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-puppet/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config-puppet/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      166 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-puppet/install.d/50-heat-config-hook-puppet
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5976 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-puppet/install.d/hook-puppet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config-salt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-salt/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config-salt/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      168 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-salt/install.d/50-heat-config-hook-salt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3744 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-salt/install.d/hook-salt.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config-script/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-script/element-deps
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat-config-script/install.d/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      142 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-script/install.d/50-heat-config-hook-script
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2998 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/heat-config-script/install.d/hook-script.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/heat_agents.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:37:46.000000 heat-agents-6.0.0.0rc1/heat_agents.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.336318 heat-agents-6.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.348319 heat-agents-6.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/docker-cmd-paunch-0a674fc1b84b2dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-17dd2c0ff96ee806.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/heat-config-notify-retry-e01b995d239bb1fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/hook_docker_envfile-bc9eb287d854e1e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/notes/switch-docker-cmd-hook-to-docker-cli-5d8f6deee2125d65.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.352319 heat-agents-6.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5699 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-03-02 11:37:46.356319 heat-agents-6.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:46.356319 heat-agents-6.0.0.0rc1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1948 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/config-tool-fake.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5899 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/heat_config_notify.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1249 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/hook-fake-raises.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1920 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/hook-fake.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7382 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/hook_docker_cmd.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6200 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/hook_kubelet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10394 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_heat_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_heat_config_docker_compose.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_heat_config_kubelet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8471 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_heat_config_notify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9665 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_ansible.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_apply_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3653 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_cfn_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_chef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25130 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_docker_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5247 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_docker_compose.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_hiera.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2020 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_json_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4065 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_kubelet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_puppet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_salt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4777 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tests/test_hook_script.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-03-02 11:37:19.000000 heat-agents-6.0.0.0rc1/tox.ini
```

### Comparing `heat-agents-6.0.0/AUTHORS` & `heat-agents-6.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/CONTRIBUTING.rst` & `heat-agents-6.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/ChangeLog` & `heat-agents-6.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-6.0.0
------
+6.0.0.0rc1
+----------
 
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
 
 5.0.0
 -----
```

### Comparing `heat-agents-6.0.0/LICENSE` & `heat-agents-6.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/MANIFEST.in` & `heat-agents-6.0.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/PKG-INFO` & `heat-agents-6.0.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-agents
-Version: 6.0.0
+Version: 6.0.0.0rc1
 Summary: heat-agents
 Home-page: https://docs.openstack.org/heat/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `heat-agents-6.0.0/doc/source/conf.py` & `heat-agents-6.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/contributor/contributing.rst` & `heat-agents-6.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/index.rst` & `heat-agents-6.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/building_image.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/building_image.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/apply-config.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/apply-config.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/chef.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/chef.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/docker-cmd.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/docker-cmd.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/docker-compose.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/docker-compose.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/hiera.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/hiera.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/json-file.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/json-file.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/kubelet.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/kubelet.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/doc/source/install/hooks/puppet.rst` & `heat-agents-6.0.0.0rc1/doc/source/install/hooks/puppet.rst`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config/bin/heat-config-notify` & `heat-agents-6.0.0.0rc1/heat-config/bin/heat-config-notify`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config/bin/heat-config-rebuild-deployed` & `heat-agents-6.0.0.0rc1/heat-config/bin/heat-config-rebuild-deployed`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config/install.d/heat-config-source-install/50-heat-config-soure` & `heat-agents-6.0.0.0rc1/heat-config/install.d/heat-config-source-install/50-heat-config-soure`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config/os-apply-config/etc/os-collect-config.conf` & `heat-agents-6.0.0.0rc1/heat-config/os-apply-config/etc/os-collect-config.conf`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config/os-refresh-config/configure.d/55-heat-config` & `heat-agents-6.0.0.0rc1/heat-config/os-refresh-config/configure.d/55-heat-config`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-ansible/install.d/hook-ansible.py` & `heat-agents-6.0.0.0rc1/heat-config-ansible/install.d/hook-ansible.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-apply-config/install.d/hook-apply-config.py` & `heat-agents-6.0.0.0rc1/heat-config-apply-config/install.d/hook-apply-config.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-cfn-init/install.d/hook-cfn-init.py` & `heat-agents-6.0.0.0rc1/heat-config-cfn-init/install.d/hook-cfn-init.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-chef/install.d/hook-chef.py` & `heat-agents-6.0.0.0rc1/heat-config-chef/install.d/hook-chef.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-docker-cmd/install.d/hook-docker-cmd.py` & `heat-agents-6.0.0.0rc1/heat-config-docker-cmd/install.d/hook-docker-cmd.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-docker-cmd/os-refresh-config/configure.d/50-heat-config-docker-cmd` & `heat-agents-6.0.0.0rc1/heat-config-docker-cmd/os-refresh-config/configure.d/50-heat-config-docker-cmd`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-docker-compose/install.d/hook-docker-compose.py` & `heat-agents-6.0.0.0rc1/heat-config-docker-compose/install.d/hook-docker-compose.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-docker-compose/os-refresh-config/configure.d/50-heat-config-docker-compose` & `heat-agents-6.0.0.0rc1/heat-config-docker-compose/os-refresh-config/configure.d/50-heat-config-docker-compose`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-hiera/install.d/hook-hiera.py` & `heat-agents-6.0.0.0rc1/heat-config-hiera/install.d/hook-hiera.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-json-file/install.d/hook-json-file.py` & `heat-agents-6.0.0.0rc1/heat-config-json-file/install.d/hook-json-file.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-kubelet/install.d/50-heat-config-kubelet` & `heat-agents-6.0.0.0rc1/heat-config-kubelet/install.d/50-heat-config-kubelet`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-kubelet/install.d/hook-kubelet.py` & `heat-agents-6.0.0.0rc1/heat-config-kubelet/install.d/hook-kubelet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-kubelet/os-refresh-config/configure.d/50-heat-config-kubelet` & `heat-agents-6.0.0.0rc1/heat-config-kubelet/os-refresh-config/configure.d/50-heat-config-kubelet`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-puppet/install.d/hook-puppet.py` & `heat-agents-6.0.0.0rc1/heat-config-puppet/install.d/hook-puppet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-salt/install.d/hook-salt.py` & `heat-agents-6.0.0.0rc1/heat-config-salt/install.d/hook-salt.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat-config-script/install.d/hook-script.py` & `heat-agents-6.0.0.0rc1/heat-config-script/install.d/hook-script.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/heat_agents.egg-info/PKG-INFO` & `heat-agents-6.0.0.0rc1/heat_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-agents
-Version: 6.0.0
+Version: 6.0.0.0rc1
 Summary: heat-agents
 Home-page: https://docs.openstack.org/heat/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `heat-agents-6.0.0/heat_agents.egg-info/SOURCES.txt` & `heat-agents-6.0.0.0rc1/heat_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/releasenotes/source/conf.py` & `heat-agents-6.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/setup.cfg` & `heat-agents-6.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/setup.py` & `heat-agents-6.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/test-requirements.txt` & `heat-agents-6.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/common.py` & `heat-agents-6.0.0.0rc1/tests/common.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/config-tool-fake.py` & `heat-agents-6.0.0.0rc1/tests/config-tool-fake.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/heat_config_notify.py` & `heat-agents-6.0.0.0rc1/tests/heat_config_notify.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/hook-fake-raises.py` & `heat-agents-6.0.0.0rc1/tests/hook-fake-raises.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/hook-fake.py` & `heat-agents-6.0.0.0rc1/tests/hook-fake.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/hook_docker_cmd.py` & `heat-agents-6.0.0.0rc1/tests/hook_docker_cmd.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/hook_kubelet.py` & `heat-agents-6.0.0.0rc1/tests/hook_kubelet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_heat_config.py` & `heat-agents-6.0.0.0rc1/tests/test_heat_config.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_heat_config_docker_compose.py` & `heat-agents-6.0.0.0rc1/tests/test_heat_config_docker_compose.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_heat_config_kubelet.py` & `heat-agents-6.0.0.0rc1/tests/test_heat_config_kubelet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_heat_config_notify.py` & `heat-agents-6.0.0.0rc1/tests/test_heat_config_notify.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_ansible.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_ansible.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_apply_config.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_apply_config.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_cfn_init.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_cfn_init.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_chef.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_chef.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_docker_cmd.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_docker_cmd.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_docker_compose.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_docker_compose.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_hiera.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_hiera.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_json_file.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_json_file.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_kubelet.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_kubelet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_puppet.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_puppet.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_salt.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_salt.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tests/test_hook_script.py` & `heat-agents-6.0.0.0rc1/tests/test_hook_script.py`

 * *Files identical despite different names*

### Comparing `heat-agents-6.0.0/tox.ini` & `heat-agents-6.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

