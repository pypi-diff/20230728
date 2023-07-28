# Comparing `tmp/semgrep_rules_manager-0.1.0.tar.gz` & `tmp/semgrep_rules_manager-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semgrep_rules_manager-0.1.0.tar", max compression
+gzip compressed data, was "semgrep_rules_manager-0.1.0.post1.tar", max compression
```

## Comparing `semgrep_rules_manager-0.1.0.tar` & `semgrep_rules_manager-0.1.0.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     1711 2023-07-28 10:09:03.889111 semgrep_rules_manager-0.1.0/README.pypi.md
--rw-r--r--   0        0        0     1434 2023-07-28 12:23:37.019755 semgrep_rules_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.1.0/semgrep_rules_manager/__init__.py
--rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.1.0/semgrep_rules_manager/cli.py
--rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.1.0/semgrep_rules_manager/core.py
--rw-r--r--   0        0        0     1426 2023-07-28 07:44:40.423516 semgrep_rules_manager-0.1.0/semgrep_rules_manager/data/sources.yaml
--rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.1.0/semgrep_rules_manager/exception.py
--rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.1.0/semgrep_rules_manager/sources.py
--rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-27 09:28:13.660884 semgrep_rules_manager-0.1.0.post1/LICENSE
+-rw-r--r--   0        0        0     1710 2023-07-28 12:26:40.315877 semgrep_rules_manager-0.1.0.post1/README.pypi.md
+-rw-r--r--   0        0        0     1440 2023-07-28 12:28:53.575978 semgrep_rules_manager-0.1.0.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 10:09:41.096768 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/__init__.py
+-rw-r--r--   0        0        0     4994 2023-07-27 15:23:18.259554 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/cli.py
+-rw-r--r--   0        0        0     1440 2023-07-27 15:12:22.885391 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/core.py
+-rw-r--r--   0        0        0     1426 2023-07-28 07:44:40.423516 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/data/sources.yaml
+-rw-r--r--   0        0        0      284 2023-07-27 13:50:03.352821 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/exception.py
+-rw-r--r--   0        0        0     4902 2023-07-28 12:12:53.103670 semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/sources.py
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 semgrep_rules_manager-0.1.0.post1/PKG-INFO
```

### Comparing `semgrep_rules_manager-0.1.0/LICENSE` & `semgrep_rules_manager-0.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0/README.pypi.md` & `semgrep_rules_manager-0.1.0.post1/README.pypi.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <img src="https://raw.githubusercontent.com/returntocorp/semgrep/develop/images/semgrep-logo-light.svg" height="100" alt="Semgrep logo"/>
 </p>
 
 ## Description
 
 Despite the fact that there is an open source repository containing community rules, some Semgrep users prefer to keep their custom rules in repositories that they manage.
 
-The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager`` can handle deletion procedures.
+The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager` can handle deletion procedures.
 
 ## Included Sources
 
 | Identifier    | Repository URL                                             | Author        | License   |
 |---------------|------------------------------------------------------------|---------------|-----------|
 | `community`   | https://github.com/returntocorp/semgrep-rules              | Semgrep       | LGPL 2.1  |
 | `gitlab`      | https://gitlab.com/gitlab-org/security-products/sast-rules | GitLab        | MIT       |
```

### Comparing `semgrep_rules_manager-0.1.0/pyproject.toml` & `semgrep_rules_manager-0.1.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semgrep_rules_manager"
-version = "0.1.0"
+version = "0.1.0.post1"
 description = "Manager of third-party Semgrep rules"
 keywords = ["semgrep", "semgrep-rules", "semgrep-rules-manager", "sast"]
 authors = ["George-Andrei Iosif <andrei.iosif@canonical.com>"]
 readme = "README.pypi.md"
 license = "MIT"
 packages = [{include = "semgrep_rules_manager"}]
 repository = "https://github.com/iosifache/semgrep-rules-manager"
```

### Comparing `semgrep_rules_manager-0.1.0/semgrep_rules_manager/cli.py` & `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/cli.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0/semgrep_rules_manager/core.py` & `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/core.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0/semgrep_rules_manager/data/sources.yaml` & `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/data/sources.yaml`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0/semgrep_rules_manager/sources.py` & `semgrep_rules_manager-0.1.0.post1/semgrep_rules_manager/sources.py`

 * *Files identical despite different names*

### Comparing `semgrep_rules_manager-0.1.0/PKG-INFO` & `semgrep_rules_manager-0.1.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semgrep-rules-manager
-Version: 0.1.0
+Version: 0.1.0.post1
 Summary: Manager of third-party Semgrep rules
 Home-page: https://github.com/iosifache/semgrep-rules-manager
 License: MIT
 Keywords: semgrep,semgrep-rules,semgrep-rules-manager,sast
 Author: George-Andrei Iosif
 Author-email: andrei.iosif@canonical.com
 Requires-Python: >=3.10,<4.0
@@ -29,15 +29,15 @@
     <img src="https://raw.githubusercontent.com/returntocorp/semgrep/develop/images/semgrep-logo-light.svg" height="100" alt="Semgrep logo"/>
 </p>
 
 ## Description
 
 Despite the fact that there is an open source repository containing community rules, some Semgrep users prefer to keep their custom rules in repositories that they manage.
 
-The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager`` can handle deletion procedures.
+The goal of **`semgrep-rules-manager`** is to collect **high-quality Semgrep rules from third-party sources**. It allows you to examine information about a source, download it, and check for and retrieve remote updates. If a downloaded source no longer meets your requirements, `semgrep-rules-manager` can handle deletion procedures.
 
 ## Included Sources
 
 | Identifier    | Repository URL                                             | Author        | License   |
 |---------------|------------------------------------------------------------|---------------|-----------|
 | `community`   | https://github.com/returntocorp/semgrep-rules              | Semgrep       | LGPL 2.1  |
 | `gitlab`      | https://gitlab.com/gitlab-org/security-products/sast-rules | GitLab        | MIT       |
```

