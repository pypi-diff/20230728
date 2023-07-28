# Comparing `tmp/gen3users-0.8.0.tar.gz` & `tmp/gen3users-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3users-0.8.0.tar", last modified: Thu Mar 10 22:31:15 2022, max compression
+gzip compressed data, was "gen3users-1.0.0.tar", max compression
```

## Comparing `gen3users-0.8.0.tar` & `gen3users-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,10 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-10 22:31:15.616672 gen3users-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2022-03-10 22:30:32.000000 gen3users-0.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2022-03-10 22:30:32.000000 gen3users-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2022-03-10 22:30:32.000000 gen3users-0.8.0/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2022-03-10 22:31:15.616672 gen3users-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2022-03-10 22:30:32.000000 gen3users-0.8.0/Pipfile
--rw-rw-r--   0 travis    (2000) travis    (2000)     3879 2022-03-10 22:30:32.000000 gen3users-0.8.0/Pipfile.lock
--rw-rw-r--   0 travis    (2000) travis    (2000)     1101 2022-03-10 22:30:32.000000 gen3users-0.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-10 22:31:15.616672 gen3users-0.8.0/gen3users/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-03-10 22:30:32.000000 gen3users-0.8.0/gen3users/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2303 2022-03-10 22:30:32.000000 gen3users-0.8.0/gen3users/base_abac.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8663 2022-03-10 22:30:32.000000 gen3users-0.8.0/gen3users/conversion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2022-03-10 22:30:32.000000 gen3users-0.8.0/gen3users/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20289 2022-03-10 22:30:32.000000 gen3users-0.8.0/gen3users/validation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-03-10 22:31:15.616672 gen3users-0.8.0/gen3users.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1370 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      379 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2022-03-10 22:31:15.000000 gen3users-0.8.0/gen3users.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-03-10 22:31:15.616672 gen3users-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2022-03-10 22:30:58.000000 gen3users-0.8.0/setup.py
+-rw-r--r--   0        0        0    11358 2023-07-28 20:10:49.637672 gen3users-1.0.0/LICENSE
+-rw-r--r--   0        0        0      558 2023-07-28 20:10:49.637672 gen3users-1.0.0/NOTICE
+-rw-r--r--   0        0        0     1101 2023-07-28 20:10:49.637672 gen3users-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/__init__.py
+-rw-r--r--   0        0        0     2303 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/base_abac.json
+-rw-r--r--   0        0        0     8661 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/conversion.py
+-rw-r--r--   0        0        0     1438 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/main.py
+-rw-r--r--   0        0        0    22130 2023-07-28 20:10:49.637672 gen3users-1.0.0/gen3users/validation.py
+-rw-r--r--   0        0        0      566 2023-07-28 20:10:49.637672 gen3users-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 gen3users-1.0.0/PKG-INFO
```

### Comparing `gen3users-0.8.0/LICENSE` & `gen3users-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3users-0.8.0/NOTICE` & `gen3users-1.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3users-0.8.0/PKG-INFO` & `gen3users-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: gen3users
-Version: 0.8.0
-Summary: Utils for Gen3 commons user management
-Home-page: https://github.com/uc-cdis/gen3users
-License: Apache
-Platform: UNKNOWN
+Version: 1.0.0
+Summary: Utils for Gen3 Commons user management
+Home-page: https://github.com/uc-cdis/gen3utils
+License: Apache-2.0
+Author: CTDS UChicago
+Author-email: cdis@uchicago.edu
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cdislogging (>=1,<2)
+Requires-Dist: click
+Requires-Dist: pyyaml (>=6,<7)
+Project-URL: Repository, https://github.com/uc-cdis/gen3utils
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
 
 # gen3users
 
 Utils for Gen3 commons user management.
 
 ## user.yaml validation
 
@@ -49,8 +58,7 @@
 dst_file_name = "my-gen3-commons/new_user.yaml"
 with open (src_file_name, "r") as f:
         user_yaml = f.read()
         convert_old_user_yaml_to_new_user_yaml(user_yaml, dst_file_name)
 
 ```
 
-
```

### Comparing `gen3users-0.8.0/README.md` & `gen3users-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gen3users-0.8.0/gen3users/base_abac.json` & `gen3users-1.0.0/gen3users/base_abac.json`

 * *Files identical despite different names*

### Comparing `gen3users-0.8.0/gen3users/conversion.py` & `gen3users-1.0.0/gen3users/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,18 +184,16 @@
             )
         elif resource["name"] not in existing_resources:
             logger.warning("Ignoring resource {}".format(resource["name"]))
 
     # convert user privileges into roles and policies
     existing_policies = [item.get("id") for item in new_user_yaml["authz"]["policies"]]
     for user_email, user_access in old_user_yaml.get("users", {}).items():
-
         # generate user policies
         for project in user_access.get("projects", []):
-
             # get the resource path.
             # if no resource path is specified, use the auth_id
             if "resource" not in project:
                 resource_path = auth_id_to_resource_path(
                     new_user_yaml, project["auth_id"]
                 )
                 if not resource_path:
```

### Comparing `gen3users-0.8.0/gen3users/main.py` & `gen3users-1.0.0/gen3users/main.py`

 * *Files identical despite different names*

### Comparing `gen3users-0.8.0/gen3users/validation.py` & `gen3users-1.0.0/gen3users/validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 logger = get_logger("gen3users")
 logging.basicConfig()
 
 
 def assert_and_log(assertion_success, error_message):
     """
-    If an assertion fails, logs the provided error message and updates
-    the global variable "failed_validation" for future use.
+    If an assertion fails, logs the provided error message.
 
     Args:
         assertion_success (bool): result of an assertion.
         error_message (str): message to display if the assertion failed.
 
     Return:
         assertion_success(bool): result of the assertion.
@@ -49,14 +48,15 @@
     ok = validate_syntax(user_yaml_dict)
     ok = validate_groups(user_yaml_dict) and ok
     ok = validate_policies(user_yaml_dict, existing_resources) and ok
     ok = validate_clients(user_yaml_dict) and ok
     ok = validate_user_project_to_resource(user_yaml_dict, existing_resources) and ok
     ok = validate_users(user_yaml_dict, existing_resources) and ok
     ok = validate_roles(user_yaml_dict) and ok
+    ok = check_broad_roles(user_yaml_dict) and ok
 
     if not ok:
         raise AssertionError(
             "user.yaml validation failed. See errors in previous logs."
         )
     else:
         logger.info("OK")
@@ -380,15 +380,14 @@
         ok(bool): whether the validation succeeded.
     """
     logger.info("- Validating policies")
     ok = True
 
     existing_roles = get_field_from_list(user_yaml_dict["authz"].get("roles", []), "id")
     for policy in user_yaml_dict["authz"].get("policies", []):
-
         # check resource paths in "authz.policies" are valid
         # given "authz.resources" resource tree
         for resource_path in policy["resource_paths"]:
             ok = (
                 assert_and_log(
                     resource_path.startswith("/"),
                     'Resource path "{}" in policy "{}" should start with a "/"'.format(
@@ -504,15 +503,14 @@
 
     existing_policies = get_field_from_list(
         user_yaml_dict["authz"].get("policies", []), "id"
     )
     allowed_auth_ids = get_allowed_auth_ids(user_yaml_dict)
 
     for user_email, user_access in user_yaml_dict["users"].items():
-
         # check policies are defined
         user_policies = user_access.get("policies", [])
         invalid_policies = set(user_policies).difference(existing_policies)
         ok = (
             assert_and_log(
                 len(invalid_policies) == 0,
                 'Policies {} for user "{}" are not defined in list of policies'.format(
@@ -626,7 +624,41 @@
                     "method is not specified for permission {} in role {}".format(
                         perm_id, role_id
                     ),
                 )
                 and ok
             )
     return ok
+
+
+def check_broad_roles(user_yaml_dict):
+    """
+    Make sure 'service = *' is not used for anonymous or all_users policies. This is dangerous because it
+    may allow users to access things in services that were not intended to be accessible. For example:
+    - Anonymous users have access to public project "projectA". We use a "reader" role with "service = *".
+    - If a user has "read" access for service "requestor" in a project, the Requestor service allows them
+    to see access requests for the project.
+    - Because of "service = *", anonymous users can see who requested access to "projectA", and whether their
+    access was approved!
+    """
+    ok = True
+
+    all_policies_dict = {
+        e["id"]: e for e in user_yaml_dict["authz"].get("policies", [])
+    }
+    all_roles_dict = {e["id"]: e for e in user_yaml_dict["authz"].get("roles", [])}
+
+    an_policies = user_yaml_dict["authz"].get("anonymous_policies", [])
+    al_policies = user_yaml_dict["authz"].get("all_users_policies", [])
+    for group_name, policies in [
+        ("anonymous_policies", an_policies),
+        ("all_users_policies", al_policies),
+    ]:
+        for policy_name in policies:
+            role_names = all_policies_dict[policy_name]["role_ids"]
+            for role_name in role_names:
+                role = all_roles_dict[role_name]
+                for perm in role["permissions"]:
+                    msg = f"Permission '{perm['id']}' in role '{role_name}' in policy '{policy_name}' has 'service = *'. This is unsecure because policy '{policy_name}' is granted to public group '{group_name}'. Fix suggestion: restrict this policy to specific methods and services, for example for public datasets, 'read in peregrine' + 'read in guppy' + 'read-storage in fence'."
+                    ok = assert_and_log(perm["action"]["service"] != "*", msg) and ok
+
+    return ok
```

