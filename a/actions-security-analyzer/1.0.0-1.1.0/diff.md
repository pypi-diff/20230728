# Comparing `tmp/actions_security_analyzer-1.0.0.tar.gz` & `tmp/actions_security_analyzer-1.1.0.tar.gz`

## Comparing `actions_security_analyzer-1.0.0.tar` & `actions_security_analyzer-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/__about__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/colors.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/requirements.txt
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/analyzer/__init__.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/analyzer/analyzer.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/analyzer/analyzer_test.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/images/asa-stdout.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/LICENSE
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/README.md
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 actions_security_analyzer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/__about__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/colors.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/__init__.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/analyzer.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/images/asa-stdout.png
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/README.md
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 actions_security_analyzer-1.1.0/PKG-INFO
```

### Comparing `actions_security_analyzer-1.0.0/colors.py` & `actions_security_analyzer-1.1.0/colors.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/main.py` & `actions_security_analyzer-1.1.0/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,26 +40,28 @@
     parser.add_argument("--verbose", "-v", action="store_true", help="increase tool verbosity")
     parser.add_argument(
         "--ignore-warnings",
         "-i",
         action="store_true",
         help="ignore checks labeled as warning",
     )
+    parser.add_argument("--no-summary", "-n", action="store_true", help="don't show tool summary section")
     return parser.parse_args()
 
 
 def _main():
     _rewrite_pyyaml_boolean_recognition_rules()
     args = _parse_args()
 
     file_ = args.file
     dir_ = args.dir
     list_checks = args.list_checks
     verbose = args.verbose
     ignore_warnings = args.ignore_warnings
+    no_summary = args.no_summary
 
     analyzer = Analyzer(ignore_warnings=ignore_warnings, verbose=verbose)
 
     errored = False
     failed_actions = []
     try:
         if file_:
@@ -103,23 +105,24 @@
             errored = True
             print(f"[{Colors.LIGHT_GRAY}INFO{Colors.END}] must provide `--file` or `--dir`")
 
     except (FileNotFoundError, KeyError, YAMLError) as exception:
         errored = True
         print(f"[{Colors.RED}ERROR{Colors.END}] {exception}")
     finally:
-        if not errored and not list_checks:
-            if failed_actions:
-                print(
-                    f"{Colors.PURPLE}{Colors.UNDERLINE}Summary{Colors.END}"
-                    "\nThe following Actions failed to pass one or more checks:"
-                )
-                for action in failed_actions:
-                    print(f" \u2022 {Colors.BOLD}{action}{Colors.END}")
-                exit(FAILED)
-            else:
-                print(f"{Colors.PURPLE}Summary{Colors.END}: Passed all checks \U0001F44D")
-                exit(SUCCESS)
+        if not no_summary:
+            if not errored and not list_checks:
+                if failed_actions:
+                    print(
+                        f"{Colors.PURPLE}{Colors.UNDERLINE}Summary{Colors.END}"
+                        "\nThe following Actions failed to pass one or more checks:"
+                    )
+                    for action in failed_actions:
+                        print(f" \u2022 {Colors.BOLD}{action}{Colors.END}")
+                    exit(FAILED)
+                else:
+                    print(f"{Colors.PURPLE}Summary{Colors.END}: Passed all checks \U0001F44D")
+                    exit(SUCCESS)
 
 
 if __name__ == "__main__":
     _main()
```

### Comparing `actions_security_analyzer-1.0.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `actions_security_analyzer-1.1.0/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/analyzer/analyzer.py` & `actions_security_analyzer-1.1.0/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/images/asa-stdout.png` & `actions_security_analyzer-1.1.0/images/asa-stdout.png`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/.gitignore` & `actions_security_analyzer-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/LICENSE` & `actions_security_analyzer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/README.md` & `actions_security_analyzer-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # asa
 asa (actions-security-analzyer) is a tool to analyze the security posture of your GitHub Actions.
 
 ![asa-stdout](/images/asa-stdout.png)
 
 ### Installation
 
-> Make sure you have `~/.local/bin` in your PATH
+> Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
 pip3 install actions-security-analzyer
 ```
 
 ### Usage
```

### Comparing `actions_security_analyzer-1.0.0/pyproject.toml` & `actions_security_analyzer-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actions_security_analyzer-1.0.0/PKG-INFO` & `actions_security_analyzer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actions-security-analyzer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Analyze the security posture of one or more GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/asa#readme
 Project-URL: Issues, https://github.com/bin3xish477/asa/issues
 Project-URL: Source, https://github.com/bin3xish477/asa
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -28,15 +28,15 @@
 # asa
 asa (actions-security-analzyer) is a tool to analyze the security posture of your GitHub Actions.
 
 ![asa-stdout](/images/asa-stdout.png)
 
 ### Installation
 
-> Make sure you have `~/.local/bin` in your PATH
+> Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
 pip3 install actions-security-analzyer
 ```
 
 ### Usage
```

