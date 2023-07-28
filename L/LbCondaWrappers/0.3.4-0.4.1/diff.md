# Comparing `tmp/LbCondaWrappers-0.3.4.tar.gz` & `tmp/LbCondaWrappers-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbCondaWrappers-0.3.4.tar", last modified: Wed Jul 26 12:48:33 2023, max compression
+gzip compressed data, was "LbCondaWrappers-0.4.1.tar", last modified: Fri Jul 28 04:05:46 2023, max compression
```

## Comparing `LbCondaWrappers-0.3.4.tar` & `LbCondaWrappers-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1823 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5960 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5097 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/README.md
--rw-r--r--   0 root         (0) root         (0)      309 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2469 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers/
--rw-r--r--   0 root         (0) root         (0)    19359 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5960 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 12:48:33.000000 LbCondaWrappers-0.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/tests/test_platforms.py
--rw-r--r--   0 root         (0) root         (0)     7105 2023-07-26 12:48:32.000000 LbCondaWrappers-0.3.4/tests/test_running.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:05:46.504000 LbCondaWrappers-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-07-28 04:05:46.504000 LbCondaWrappers-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 04:05:46.504000 LbCondaWrappers-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:05:46.500000 LbCondaWrappers-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:05:46.500000 LbCondaWrappers-0.4.1/src/LbCondaWrappers/
+-rw-r--r--   0 root         (0) root         (0)    20222 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:05:46.504000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      462 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 04:05:46.000000 LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 04:05:46.504000 LbCondaWrappers-0.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/tests/test_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-07-28 04:05:37.000000 LbCondaWrappers-0.4.1/tests/test_running.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `LbCondaWrappers-0.3.4/.gitignore` & `LbCondaWrappers-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.4/.gitlab-ci.yml` & `LbCondaWrappers-0.4.1/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 stages:
   - test
+  - build
   - deploy
 
 pre-commit:
   stage: test
   image: registry.cern.ch/docker.io/library/python:3.9
-  rules:
-    - when: always
   before_script:
     - pip install pre-commit
   script:
     - pre-commit run --all-files
   variables:
     PRE_COMMIT_HOME: ${CI_PROJECT_DIR}/.cache/pre-commit
   cache:
@@ -34,21 +33,33 @@
     - cvmfs
   script:
     - python --version
     - pip install --upgrade setuptools
     - pip install '.[testing]'
     - pytest -vvv
 
+package:
+  stage: build
+  image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.9
+  script:
+    - python -m build
+  artifacts:
+    paths:
+      - dist
+    expire_in: 1 week
+  before_script:
+    - pip install build
+  after_script: []
+
 # Packaging step
 deploy-packages:
   stage: deploy
+  image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.9
   only:
     - tags
-  dependencies: []
-  image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.7
+  dependencies:
+    - package
   script:
-    - python setup.py sdist --dist-dir public/
-    - python setup.py bdist_wheel --dist-dir public/
     - if [ -z "$TWINE_PASSWORD" ] ; then echo "Set TWINE_PASSWORD in CI variables" ; exit 1 ; fi
-    - twine upload -u __token__ public/*
+    - twine upload -u __token__ dist/*
   before_script: []
   after_script: []
```

### Comparing `LbCondaWrappers-0.3.4/LICENSE` & `LbCondaWrappers-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.4/PKG-INFO` & `LbCondaWrappers-0.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: LbCondaWrappers
-Version: 0.3.4
-Summary: Wrappers for using LHCb CVMFS conda installations
-Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
-Author: LHCb
-Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
-Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
-Keywords: LHCb Core task runner
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # LHCb Conda Wrappers
 
 Wrapper scripts for providing access to conda environments which are installed on CVMFS.
 
 ## Standard Usage
 
 The main environment provided is named `default` and aims to provide most software tools that will be needed for analaysis that is performed outside of the standard LHCb software stack.
```

### Comparing `LbCondaWrappers-0.3.4/README.md` & `LbCondaWrappers-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: LbCondaWrappers
+Version: 0.4.1
+Summary: Wrappers for using LHCb CVMFS conda installations
+Author: LHCb
+Project-URL: Homepage, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
+Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
+Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
+Keywords: LHCb,Core,task,runner
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 # LHCb Conda Wrappers
 
 Wrapper scripts for providing access to conda environments which are installed on CVMFS.
 
 ## Standard Usage
 
 The main environment provided is named `default` and aims to provide most software tools that will be needed for analaysis that is performed outside of the standard LHCb software stack.
```

### Comparing `LbCondaWrappers-0.3.4/src/LbCondaWrappers/__init__.py` & `LbCondaWrappers-0.4.1/src/LbCondaWrappers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,36 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-
 import argparse
 import difflib
+import json
 import logging
 import os
-import pipes
 import platform
 import re
+import shlex
 import stat
 import subprocess
 import sys
 import tempfile
+import uuid
 from collections import defaultdict
 from datetime import datetime
 from os.path import basename, isdir, join, relpath
 
 from lb_telemetry import Logger
 
+TELEMETRY_TABLE = "lbconda2"
+TELEMETRY_TAGS = ["conda_subdir", "env_name", "env_version", "latest", "with_texlive"]
+
 
 def compute_conda_subdir():
     if "CONDA_SUBDIR" in os.environ:
         return os.environ["CONDA_SUBDIR"]
     conda_platform = platform.system().lower()
     conda_platform = {"darwin": "osx"}.get(conda_platform, conda_platform)
     conda_arch = platform.machine()
@@ -93,15 +97,15 @@
                 pass
     return sorted(versions)
 
 
 def list_environments(subdir=None):
     if subdir is None:
         subdir = compute_conda_subdir()
-    envs = defaultdict(dict)
+    envs: defaultdict[str, dict[str, str]] = defaultdict(dict)
     for dirpath, dirnames, _ in os.walk(ENVS_ROOT, topdown=True):
         if any(d in dirnames for d in KNOWN_CONDA_SUBDIRS):
             if subdir not in dirnames:
                 # Avoid searching any deeper in the tree
                 dirnames[:] = []
                 continue
             split_dirpath = relpath(dirpath, ENVS_ROOT).split(os.sep)
@@ -175,17 +179,14 @@
     env_name, env_version, _ = get_env_details(env_string)
     return CONDA_ENVIRONMENTS[env_name][env_version]
 
 
 def call_in_conda(
     command,
     env_prefix,
-    env_name,
-    env_version,
-    latest,
     *,
     with_venv=None,
     texlive=None,
     extravars=None,
 ):
     """Replace the current process with a command in the conda environment
 
@@ -212,19 +213,19 @@
                     ]
                 )
             )
 
         bashrc.write(
             "\n".join(
                 [
-                    f'eval "$({pipes.quote(conda_cmd())} shell.bash hook)"',
-                    f"conda activate {pipes.quote(env_prefix)}",
+                    f'eval "$({shlex.quote(conda_cmd())} shell.bash hook)"',
+                    f"conda activate {shlex.quote(env_prefix)}",
                     "unset BASH_ENV",
-                    f"source {pipes.quote(with_venv)}" if with_venv else "",
-                    f"rm {pipes.quote(bashrc.name)}",
+                    f"source {shlex.quote(with_venv)}" if with_venv else "",
+                    f"rm {shlex.quote(bashrc.name)}",
                     # Always end with a new line
                     "",
                 ]
             )
         )
 
     env["BASH_ENV"] = bashrc.name
@@ -237,37 +238,22 @@
     # Now adding the extra variables requested on the command line
     for v in extravars or []:
         env[v] = extravars[v]
 
     if basename(command[0]) == "bash":
         exec_command = "exec bash --norc --noprofile"
         for c in command[1:]:
-            exec_command += " " + pipes.quote(c)
+            exec_command += " " + shlex.quote(c)
     elif basename(command[0]) in ["sh", "ksh", "csh", "tcsh", "zsh", "fish"]:
         raise NotImplementedError(
             "Unable to launch %s as only bash is supported for now"
             % basename(command[0]),
         )
     else:
-        exec_command = " ".join(pipes.quote(x) for x in command)
-
-    telemetry = {
-        "conda_subdir": compute_conda_subdir(),
-        "env_name": env_name,
-        "env_version": env_version,
-        "latest": bool(latest),
-        "with_texlive": bool(texlive),
-    }
-
-    Logger().log_to_monit(
-        "LbCondaT2",
-        telemetry,
-        tags=["conda_subdir", "env_name", "env_version", "latest", "with_texlive"],
-        include_host_info=True,
-    )
+        exec_command = " ".join(shlex.quote(x) for x in command)
 
     logging.debug("Running command %s", exec_command)
     sys.stdout.flush()
     sys.stderr.flush()
     os.execvpe("bash", ["bash", "--norc", "--noprofile", "-c", exec_command], env)
 
 
@@ -365,32 +351,45 @@
             'Did you mean "lb-conda default"?\n'
         )
         sys.exit(3)
 
     if args.export or (len(args.command) >= 2 and args.command[1] == "--export"):
         with open(env_prefix + ".yaml", encoding="utf-8") as fp:
             print(fp.read())
-            sys.exit(0)
         sys.exit(0)
 
     # Checking the variables to be added
     # Splitting by the first '='
     extravars = {}
     for newvar in args.environment_variables or []:
         newvarname, newvarval = newvar.split("=", 1)
         extravars[newvarname] = newvarval
 
+    # Send telemetry
+    telemetry = {
+        "conda_subdir": compute_conda_subdir(),
+        "env_name": env_name,
+        "env_version": env_version,
+        "latest": bool(latest),
+        "with_texlive": bool(texlive),
+        "env_type": "release",
+        "dev_id": "none",
+    }
+    Logger().log_to_monit(
+        TELEMETRY_TABLE,
+        telemetry,
+        tags=TELEMETRY_TAGS,
+        include_host_info=True,
+    )
+
     # Try to replace the current process with the desired command
     try:
         call_in_conda(
             command,
             env_prefix,
-            env_name,
-            env_version,
-            latest,
             texlive=texlive,
             extravars=extravars,
         )
     except Exception as e:
         sys.stderr.write("ERROR: %s\n" % e)
         sys.exit(1)
 
@@ -416,15 +415,15 @@
     parser.add_argument(
         "-e",
         "--env",
         action="append",
         dest="environment_variables",
         help="Specify an variable to be set in the environment",
     )
-    subparsers = parser.add_subparsers(help="sub-command help")
+    subparsers = parser.add_subparsers(dest="env_type", help="sub-command help")
     venv_parser = subparsers.add_parser(
         "virtual-env",
         help="Create an copy of the environment for use with pip "
         "(recommended, minimal disk requirements)",
     )
     venv_parser.set_defaults(func=_lb_conda_dev_venv)
 
@@ -479,16 +478,16 @@
                 texlive=texlive,
                 extravars=extravars,
             )
         except Exception as e:
             sys.stderr.write("ERROR: %s\n" % e)
             sys.exit(20)
     elif hasattr(args, "func"):
-        env_name = args.env_name
-        env_prefix = get_env_prefix(args.env_name)
+        env_name, env_version, latest = get_env_details(args.env_name)
+        env_prefix = get_env_prefix(env_name)
 
         directory = args.directory
         if directory is None:
             directory = env_name.replace("/", "-") + "_dev"
         directory = os.path.abspath(directory)
 
         if isdir(directory):
@@ -515,28 +514,39 @@
             sys.exit(11)
         else:
             if python_version < 3:
                 sys.stderr.write(
                     "ERROR: Python 2 is not supported but was found in %s\n" % env_name
                 )
                 sys.exit(12)
-        args.func(env_name, env_prefix, directory, texlive=texlive)
+
+        telemetry = {
+            "conda_subdir": compute_conda_subdir(),
+            "env_name": env_name,
+            "env_version": env_version,
+            "latest": bool(latest),
+            "with_texlive": bool(texlive),
+            "env_type": args.env_type,
+            "dev_id": str(uuid.uuid4()),
+        }
+
+        args.func(env_name, env_prefix, directory, telemetry, texlive=texlive)
         sys.stderr.write("Environment created in %s\n" % directory)
         sys.stderr.write(
             '   Execute "%s/run" to launch a shell inside the environment\n' % directory
         )
         sys.stderr.write(
             '   Execute "%s/run my_command" to launch "my_command" inside the environment\n'
             % directory
         )
     else:
         parser.error('Either "virtual-env" or "clone" must be specified')
 
 
-def _lb_conda_dev_venv(env_name, env_prefix, directory, *, texlive=None):
+def _lb_conda_dev_venv(env_name, env_prefix, directory, telemetry, *, texlive=None):
     subprocess.check_output(
         [
             "lb-conda",
             env_name,
             "python",
             "-m",
             "venv",
@@ -544,45 +554,61 @@
             directory,
         ],
         text=True,
     )
     write_run_script(
         join(directory, "run"),
         env_prefix,
+        telemetry,
         with_venv=join(directory, "bin", "activate"),
         texlive=texlive,
     )
 
 
-def _lb_conda_dev_clone(env_name, env_prefix, directory, *, texlive=None):
+def _lb_conda_dev_clone(env_name, env_prefix, directory, telemetry, *, texlive=None):
     subprocess.check_output(
         [
             "lb-conda",
             env_name,
             "conda",
             "create",
             "--clone",
             env_prefix,
             "--prefix",
             directory,
         ],
         text=True,
     )
-    write_run_script(join(directory, "run"), env_prefix, texlive=texlive)
+    write_run_script(join(directory, "run"), env_prefix, telemetry, texlive=texlive)
 
 
-def write_run_script(fn, env_prefix, *, with_venv=None, texlive=None):
+def write_run_script(fn, env_prefix, telemetry, *, with_venv=None, texlive=None):
     lb_conda_dev_executable = sys.argv[0]
     if basename(lb_conda_dev_executable) != "lb-conda-dev":
         raise NotImplementedError(sys.argv)
 
+    telemetry_command = shlex.join(
+        [
+            sys.executable,
+            "-m",
+            "lb_telemetry",
+            "send",
+            "-t",
+            TELEMETRY_TABLE,
+            "--tags",
+            *TELEMETRY_TAGS,
+            "--include-host-info",
+            json.dumps(telemetry),
+        ]
+    )
+
     cmd = ["exec"]
     cmd += [lb_conda_dev_executable]
     if with_venv:
         cmd += ["--with-venv", with_venv]
     if texlive:
         cmd += ["--texlive-version", str(texlive)]
     cmd += ["--execute", env_prefix]
-    cmd = " ".join([pipes.quote(s) for s in cmd])
+    cmd = " ".join([shlex.quote(s) for s in cmd])
     with open(fn, "w") as fp:
-        fp.write(f'#!/usr/bin/env bash\n{cmd} "$@"')
+        fp.write(f'#!/usr/bin/env bash\n{telemetry_command} || true\n{cmd} "$@"')
     os.chmod(fn, os.stat(fn).st_mode | stat.S_IEXEC)
```

### Comparing `LbCondaWrappers-0.3.4/src/LbCondaWrappers.egg-info/PKG-INFO` & `LbCondaWrappers-0.4.1/src/LbCondaWrappers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.4
+Version: 0.4.1
 Summary: Wrappers for using LHCb CVMFS conda installations
-Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
+Project-URL: Homepage, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
-Keywords: LHCb Core task runner
+Keywords: LHCb,Core,task,runner
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # LHCb Conda Wrappers
 
 Wrapper scripts for providing access to conda environments which are installed on CVMFS.
```

### Comparing `LbCondaWrappers-0.3.4/tests/test_platforms.py` & `LbCondaWrappers-0.4.1/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.4/tests/test_running.py` & `LbCondaWrappers-0.4.1/tests/test_running.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     [
         ["--list", get_random_env()[0]],
         ["--list", get_random_env()[0], "bash"],
         ["--list", get_random_env()[0], "exit", "100"],
     ],
 )
 def test_lb_conda_list_versions(cmd, require_cvmfs_lhcbdev):
-    stdout, stderr = check_output(["lb-conda"] + cmd)
+    stdout, stderr = check_output(["lb-conda", *cmd])
     env_name, env_version = get_random_env()
     for version in CONDA_ENVIRONMENTS[cmd[1]]:
         assert version in stdout or version.split("_")[0] in stdout
 
 
 def test_lb_conda_echo_list(require_cvmfs_lhcbdev):
     env_name, env_version = get_random_env()
@@ -97,15 +97,15 @@
         ["--export", get_random_env()[0]],
         [get_random_env()[0], "--export"],
         ["--export", get_random_env()[0], "bash"],
         ["--export", get_random_env()[0], "exit", "100"],
     ],
 )
 def test_lb_conda_export(cmd, require_cvmfs_lhcbdev):
-    stdout, stderr = check_output(["lb-conda"] + cmd)
+    stdout, stderr = check_output(["lb-conda", *cmd])
     assert "channels:" in stdout
     assert "dependencies:" in stdout
 
 
 def test_lb_conda_command(require_cvmfs_lhcbdev):
     env_name, env_version = get_random_env()
 
@@ -125,20 +125,20 @@
     ],
 )
 def test_lb_conda_command_texlive(require_cvmfs_lhcbdev, texlive_arg):
     env_name, env_version = get_random_env()
     year = "2020"
     arch = "x86_64-linux"
     path_to_latex = f"/cvmfs/lhcbdev.cern.ch/tools/texlive/{year}/bin/{arch}/latex"
-    lb_conda_cmd = ["lb-conda"] + texlive_arg + [env_name]
+    lb_conda_cmd = ["lb-conda", *texlive_arg, env_name]
 
-    stdout, stderr = check_output(lb_conda_cmd + ["which", "latex"])
+    stdout, stderr = check_output([*lb_conda_cmd, "which", "latex"])
     assert stdout.strip() == path_to_latex
 
-    stdout, stderr = check_output(lb_conda_cmd + ["latex", "--version"])
+    stdout, stderr = check_output([*lb_conda_cmd, "latex", "--version"])
     assert f"TeX Live {year}" in stdout.strip()
 
 
 # def test_lb_conda_shells(require_cvmfs_lhcbdev):
 #     stdout, stderr = check_output(["lb-conda", "bash", "-c", "env"])
 #     assert "DIRAC=" in stdout
```

