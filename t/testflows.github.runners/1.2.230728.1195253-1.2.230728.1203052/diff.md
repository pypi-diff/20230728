# Comparing `tmp/testflows.github.runners-1.2.230728.1195253.tar.gz` & `tmp/testflows.github.runners-1.2.230728.1203052.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230728.1195253.tar", last modified: Fri Jul 28 19:52:53 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230728.1203052.tar", last modified: Fri Jul 28 20:30:52 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230728.1195253.tar` & `testflows.github.runners-1.2.230728.1203052.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1195253/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    38097 2023-07-27 18:44:42.000000 testflows.github.runners-1.2.230728.1195253/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.463779 testflows.github.runners-1.2.230728.1195253/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.463779 testflows.github.runners-1.2.230728.1195253/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    12069 2023-07-28 19:51:52.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1195253/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 19:52:53.467779 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    38689 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 19:52:53.000000 testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230728.1203052/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    39717 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    39125 2023-07-28 20:30:27.000000 testflows.github.runners-1.2.230728.1203052/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-28 12:15:47.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22684 2023-07-28 12:17:00.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12755 2023-07-28 15:03:49.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-07-28 14:48:45.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-28 12:15:58.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9760 2023-07-28 16:35:01.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12069 2023-07-28 19:51:52.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.474443 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230728.1203052/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 20:30:52.470443 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    39717 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 20:30:52.000000 testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230728.1195253/LICENSE` & `testflows.github.runners-1.2.230728.1203052/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/PKG-INFO` & `testflows.github.runners-1.2.230728.1203052/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1195253
+Version: 1.2.230728.1203052
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -17,17 +17,20 @@
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :align: left
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
-.. image:: https://badge.fury.io/py/testflows.github.runners.svg
-    :target: https://pypi.org/project/testflows.github.runners/
-    :align: right
+----
+
+:PyPi:
+   `Versions <https://pypi.org/project/testflows.github.runners/>`_
+:License:
+   `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
@@ -49,32 +52,56 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 
 .. contents:: Read more about:
    :backlinks: top
    :depth: 4
 
+----
+
 --------
 Features
 --------
 
-* cost efficient on-demand runners using Hetzner Cloud
+* very cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
-* supports specifying custom runner types using job labels
+* supports specifying custom runner server types, images, and locations using job labels
 * simple configuration
-* self-contained and can deploy and manage itself on a cloud instance
+* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+
+----
+
+-----------
+Limitations
+-----------
+
+* *Group runners are not supported*
+
+  However, you can run individual services for each repository using different Hetzner Cloud projects.
+
+* *Unique Hetzner Cloud project must be used for each repository*
+
+  However, unique projects allow to easily keep track of runner costs per repository.
+
+* *Idle runner pool is not supported*
+
+  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+
+----
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
+----
+
 ------------
 Quick Start
 ------------
 
 Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
 
 .. code-block:: bash
@@ -101,25 +128,29 @@
 
 or you can pass the required options inline as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
+----
+
 -------------------------
 Installation From Sources
 -------------------------
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
+----
+
 -------------------
 Basic Configuration
 -------------------
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
@@ -128,24 +159,28 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+----
+
 ------------------------------------
 Specifying Maximum Number of Runners
 ------------------------------------
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -179,14 +214,16 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
+----
+
 ---------------------------
 Specifying Runner Location
 ---------------------------
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
@@ -197,14 +234,15 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
+----
 
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
@@ -219,28 +257,33 @@
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 
 :docker-ce app:
+   :✋ Note:
+      Currently Docker CE application does not support ARM64 architecture.
+
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
 
+----
+
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
@@ -263,14 +306,16 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -291,23 +336,27 @@
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
+----
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
+----
+
 Installing and Uninstalling
 ===========================
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
@@ -343,28 +392,31 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
+----
+
 Modifying Program Options
 =========================
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
+----
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -389,14 +441,16 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
+----
+
 Manual Start and Stop
 =====================
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
@@ -406,14 +460,16 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
+----
+
 Checking Logs
 =============
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
@@ -458,14 +514,16 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+----
+
 --------------------------
 Running as a Cloud Service
 --------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
@@ -476,14 +534,16 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
+----
+
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -565,14 +625,16 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+----
+
 Redeploying Cloud Service
 =========================
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
@@ -581,14 +643,16 @@
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
+----
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -601,44 +665,52 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
+----
+
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
+----
+
 Stopping Cloud Service
 ======================
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
+----
+
 Starting Cloud Service
 ======================
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
+----
+
 Installing Cloud Service
 ========================
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
@@ -648,25 +720,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
+----
 
 Uninstalling Cloud Service
 ==========================
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
+----
+
 Upgrading Cloud Service Package
 ===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
@@ -680,14 +755,16 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
+----
+
 Changing Cloud Service Options
 ==============================
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
@@ -704,14 +781,15 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
+----
 
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
@@ -729,14 +807,16 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+----
+
 SSH in to Cloud Service
 ==============================
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
@@ -751,14 +831,16 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
+----
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -778,24 +860,27 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
+----
+
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
+----
 
 New Server
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
@@ -828,14 +913,16 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
+----
+
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
@@ -847,20 +934,25 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
+----
+
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
+:✋ Note:
+   The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
+
 The x64 **startup** script installs and configures x64 version of the runner.
 
 :x64:
 
    .. code-block:: bash
 
      set -x
@@ -893,14 +985,16 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
+----
+
 --------------------
 Scaling Down Runners
 --------------------
 
 Powered Off Servers
 ===================
 
@@ -922,14 +1016,16 @@
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
+----
+
 ---------------------------
 Handling Failing Conditions
 ---------------------------
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
@@ -947,14 +1043,16 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
+----
+
 ---------------
 Program Options
 ---------------
 
 The following options are supported:
 
 * **-h, --help**
```

### Comparing `testflows.github.runners-1.2.230728.1195253/README.rst` & `testflows.github.runners-1.2.230728.1203052/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :align: left
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
-.. image:: https://badge.fury.io/py/testflows.github.runners.svg
-    :target: https://pypi.org/project/testflows.github.runners/
-    :align: right
+----
+
+:PyPi:
+   `Versions <https://pypi.org/project/testflows.github.runners/>`_
+:License:
+   `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
@@ -32,32 +35,56 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 
 .. contents:: Read more about:
    :backlinks: top
    :depth: 4
 
+----
+
 --------
 Features
 --------
 
-* cost efficient on-demand runners using Hetzner Cloud
+* very cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
-* supports specifying custom runner types using job labels
+* supports specifying custom runner server types, images, and locations using job labels
 * simple configuration
-* self-contained and can deploy and manage itself on a cloud instance
+* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+
+----
+
+-----------
+Limitations
+-----------
+
+* *Group runners are not supported*
+
+  However, you can run individual services for each repository using different Hetzner Cloud projects.
+
+* *Unique Hetzner Cloud project must be used for each repository*
+
+  However, unique projects allow to easily keep track of runner costs per repository.
+
+* *Idle runner pool is not supported*
+
+  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+
+----
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
+----
+
 ------------
 Quick Start
 ------------
 
 Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
 
 .. code-block:: bash
@@ -84,25 +111,29 @@
 
 or you can pass the required options inline as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
+----
+
 -------------------------
 Installation From Sources
 -------------------------
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
+----
+
 -------------------
 Basic Configuration
 -------------------
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
@@ -111,24 +142,28 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+----
+
 ------------------------------------
 Specifying Maximum Number of Runners
 ------------------------------------
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -162,14 +197,16 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
+----
+
 ---------------------------
 Specifying Runner Location
 ---------------------------
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
@@ -180,14 +217,15 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
+----
 
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
@@ -202,28 +240,33 @@
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 
 :docker-ce app:
+   :✋ Note:
+      Currently Docker CE application does not support ARM64 architecture.
+
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
 
+----
+
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
@@ -246,14 +289,16 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -274,23 +319,27 @@
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
+----
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
+----
+
 Installing and Uninstalling
 ===========================
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
@@ -326,28 +375,31 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
+----
+
 Modifying Program Options
 =========================
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
+----
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -372,14 +424,16 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
+----
+
 Manual Start and Stop
 =====================
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
@@ -389,14 +443,16 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
+----
+
 Checking Logs
 =============
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
@@ -441,14 +497,16 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+----
+
 --------------------------
 Running as a Cloud Service
 --------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
@@ -459,14 +517,16 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
+----
+
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -548,14 +608,16 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+----
+
 Redeploying Cloud Service
 =========================
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
@@ -564,14 +626,16 @@
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
+----
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -584,44 +648,52 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
+----
+
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
+----
+
 Stopping Cloud Service
 ======================
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
+----
+
 Starting Cloud Service
 ======================
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
+----
+
 Installing Cloud Service
 ========================
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
@@ -631,25 +703,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
+----
 
 Uninstalling Cloud Service
 ==========================
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
+----
+
 Upgrading Cloud Service Package
 ===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
@@ -663,14 +738,16 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
+----
+
 Changing Cloud Service Options
 ==============================
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
@@ -687,14 +764,15 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
+----
 
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
@@ -712,14 +790,16 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+----
+
 SSH in to Cloud Service
 ==============================
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
@@ -734,14 +814,16 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
+----
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -761,24 +843,27 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
+----
+
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
+----
 
 New Server
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
@@ -811,14 +896,16 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
+----
+
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
@@ -830,20 +917,25 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
+----
+
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
+:✋ Note:
+   The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
+
 The x64 **startup** script installs and configures x64 version of the runner.
 
 :x64:
 
    .. code-block:: bash
 
      set -x
@@ -876,14 +968,16 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
+----
+
 --------------------
 Scaling Down Runners
 --------------------
 
 Powered Off Servers
 ===================
 
@@ -905,14 +999,16 @@
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
+----
+
 ---------------------------
 Handling Failing Conditions
 ---------------------------
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
@@ -930,14 +1026,16 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
+----
+
 ---------------
 Program Options
 ---------------
 
 The following options are supported:
 
 * **-h, --help**
```

### Comparing `testflows.github.runners-1.2.230728.1195253/setup.py` & `testflows.github.runners-1.2.230728.1203052/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230728.1195253",
+    version="1.2.230728.1203052",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230728.1195253"
+__version__ = "1.2.230728.1203052"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/config.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/logger.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230728.1203052/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230728.1195253
+Version: 1.2.230728.1203052
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -17,17 +17,20 @@
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :align: left
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
-.. image:: https://badge.fury.io/py/testflows.github.runners.svg
-    :target: https://pypi.org/project/testflows.github.runners/
-    :align: right
+----
+
+:PyPi:
+   `Versions <https://pypi.org/project/testflows.github.runners/>`_
+:License:
+   `Apache-2.0 <https://github.com/testflows/TestFlows-GitHub-Runners/blob/main/LICENSE>`_
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
 ======================================================
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
@@ -49,32 +52,56 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 
 .. contents:: Read more about:
    :backlinks: top
    :depth: 4
 
+----
+
 --------
 Features
 --------
 
-* cost efficient on-demand runners using Hetzner Cloud
+* very cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
-* supports specifying custom runner types using job labels
+* supports specifying custom runner server types, images, and locations using job labels
 * simple configuration
-* self-contained and can deploy and manage itself on a cloud instance
+* self-contained and it can deploy, redeploy, and manage itself on a cloud instance
+
+----
+
+-----------
+Limitations
+-----------
+
+* *Group runners are not supported*
+
+  However, you can run individual services for each repository using different Hetzner Cloud projects.
+
+* *Unique Hetzner Cloud project must be used for each repository*
+
+  However, unique projects allow to easily keep track of runner costs per repository.
+
+* *Idle runner pool is not supported*
+
+  Given that runner servers are created for each job, currently, idle runner pool is not supported.. 
+
+----
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
    pip3 install testflows.github.runners
 
+----
+
 ------------
 Quick Start
 ------------
 
 Set environment variables corresponding to your GitHub repository and Hetzner Cloud project
 
 .. code-block:: bash
@@ -101,25 +128,29 @@
 
 or you can pass the required options inline as follows:
 
 .. code-block:: bash
 
    github-runners --github-token <GITHUB_TOKEN> --github-repository <GITHUB_REPOSITORY> --hetzner-token <HETZNER_TOKEN>
 
+----
+
 -------------------------
 Installation From Sources
 -------------------------
 
 For development, you can install from sources as follows:
 
 .. code-block:: bash
 
    git clone https://github.com/testflows/Github-Runners.git
    ./package && ./install
 
+----
+
 -------------------
 Basic Configuration
 -------------------
 
 By default, the program uses the following environment variables:
 
 * **GITHUB_TOKEN**
@@ -128,24 +159,28 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+----
+
 ------------------------------------
 Specifying Maximum Number of Runners
 ------------------------------------
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -179,14 +214,16 @@
 as follows:
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cax21]
 
+----
+
 ---------------------------
 Specifying Runner Location
 ---------------------------
 
 By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
 option to force specific default server location.
 
@@ -197,14 +234,15 @@
 For example,
 
 .. code-block:: yaml
 
    job-name:
       runs-on: [self-hosted, type-cx11, in-ash]
 
+----
 
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
@@ -219,28 +257,33 @@
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 
 :docker-ce app:
+   :✋ Note:
+      Currently Docker CE application does not support ARM64 architecture.
+
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
          runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
 
+----
+
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
@@ -263,14 +306,16 @@
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
 
+----
+
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
 
@@ -291,23 +336,27 @@
 
 If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
 after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
 auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
 is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
 added to your project using the MD5 hash of the public key as the SSH key name.
 
+----
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
    In order to install the service, the user that installed the module must have **sudo** privileges.
 
+----
+
 Installing and Uninstalling
 ===========================
 
 After installation, you can use **service install** and **service uninstall** commands to install and
 uninstall the service.
 
 :✋ Note:
@@ -343,28 +392,31 @@
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
+----
+
 Modifying Program Options
 =========================
 
 If you want to modify service program options you can stop the service,
 edit the **/etc/systemd/system/github-runners.service** file by hand, then reload service daemon,
 and start the service back up.
 
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
+----
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -389,14 +441,16 @@
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to Hetzner >
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Logging in to GitHub
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Getting repository vza>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale up serv>
       Jul 24 14:38:33 user-node github-runners[66188]: 07/24/2023 02:38:33 PM   INFO MainThread            main 🍀 Creating scale down se>
       lines 1-16/16 (END)
 
+----
+
 Manual Start and Stop
 =====================
 
 You can start and stop the service using the **service start** and **service stop** commands as follows:
 
 .. code-block:: bash
 
@@ -406,14 +460,16 @@
 or using **service** system utility
 
 .. code-block:: bash
 
    sudo service github-runners start
    sudo service github-runners stop
 
+----
+
 Checking Logs
 =============
 
 You can get the logs for the service using the **service logs** command.
 
 Use **-f, --follow** option to follow logs journal.
 
@@ -458,14 +514,16 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+----
+
 --------------------------
 Running as a Cloud Service
 --------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
@@ -476,14 +534,16 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
+----
+
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -565,14 +625,16 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+----
+
 Redeploying Cloud Service
 =========================
 
 You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
 using the **cloud redeploy** command.
 
 .. code-block:: bash
@@ -581,14 +643,16 @@
 
 :✋ Note:
    The options that are passed to the **github-runners <options> cloud redeploy** command
    will be the same options with which the service will be executed.
 
 You can specify the version of the package to be installed using the **--version** option.
 
+----
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -601,44 +665,52 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
+----
+
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
 .. code-block:: bash
 
    github-runners cloud status
 
+----
+
 Stopping Cloud Service
 ======================
 
 You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
 
 .. code-block:: bash
 
    github-runners cloud stop
 
+----
+
 Starting Cloud Service
 ======================
 
 You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
 using the **github-runners cloud start** command.
 
 .. code-block:: bash
 
    github-runners cloud start
 
+----
+
 Installing Cloud Service
 ========================
 
 You can manually force installation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud install** command.
 
 :✋ Note:
@@ -648,25 +720,28 @@
 
 You can specify **-f, --force** option to force service re-installation if it is already installed.
 
 .. code-block:: bash
 
    github-runners <options> cloud install -f
 
+----
 
 Uninstalling Cloud Service
 ==========================
 
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
+----
+
 Upgrading Cloud Service Package
 ===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
@@ -680,14 +755,16 @@
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
 The service is not re-installed during the package upgrade process.
 Instead, it is stopped before the upgrade and then started back up
 
+----
+
 Changing Cloud Service Options
 ==============================
 
 If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
 you can keep the existing server and use **cloud redeploy** command.
 
 .. code-block:: bash
@@ -704,14 +781,15 @@
    github-runners <options> cloud deploy --version latest
 
 :✋ Note:
    Complete teardown will not affect any current jobs as the service is designed to
    be restartable. However, some servers might be left in an unfinished state
    but they will be cleaned up when the service is restarted.
 
+----
 
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
@@ -729,14 +807,16 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+----
+
 SSH in to Cloud Service
 ==============================
 
 You can open SSH client to the cloud service using the **cloud ssh** command. For example,
 
 .. code-block:: bash
 
@@ -751,14 +831,16 @@
 
 The output will contain the full **ssh** command including the IP address of the cloud service server.
 
 ::
 
    ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
 
+----
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -778,24 +860,27 @@
 Also,
 
 :Note:
    There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
+----
+
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
+----
 
 New Server
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
@@ -828,14 +913,16 @@
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
+----
+
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
@@ -847,20 +934,25 @@
 
         adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
         usermod -aG wheel ubuntu
         usermod -aG sudo ubuntu
 
+----
+
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
+:✋ Note:
+   The **startup** script is executed as **ubuntu** user and therefore you must use **sudo** for any commands that need *root* privileges.
+
 The x64 **startup** script installs and configures x64 version of the runner.
 
 :x64:
 
    .. code-block:: bash
 
      set -x
@@ -893,14 +985,16 @@
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
      echo "Start runner"
      bash -c "screen -d -m bash -c './run.sh; sudo poweroff'"
 
+----
+
 --------------------
 Scaling Down Runners
 --------------------
 
 Powered Off Servers
 ===================
 
@@ -922,14 +1016,16 @@
 Zombie Servers
 ==============
 
 The scale down service will delete any zombie servers. A zombie server is defined as as any server that fails to register its runner within
 the **max-runner-registration-time**. The **max-runner-registration-time** can be specified using the **--max-runner-registration-time** option
 which by default is set to *60* sec.
 
+----
+
 ---------------------------
 Handling Failing Conditions
 ---------------------------
 
 The program is designed to handle the following failing conditions:
 
 :Server Never Registers a Runner:
@@ -947,14 +1043,16 @@
 
 :Runner Never Gets a Job Assigned:
    If the runner never gets a job assigned, then the scale down service will remove the runner and delete its server after the **max-idle-runner-time** period.
 
 :Runner Created With a Mismatched Labels:
    The behavior will be the same as for the **Runner Never Gets a Job Assigned** case above.
 
+----
+
 ---------------
 Program Options
 ---------------
 
 The following options are supported:
 
 * **-h, --help**
```

### Comparing `testflows.github.runners-1.2.230728.1195253/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230728.1203052/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

