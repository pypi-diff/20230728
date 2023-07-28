# Comparing `tmp/badsecrets-0.4.398.tar.gz` & `tmp/badsecrets-0.4.402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.4.398.tar", max compression
+gzip compressed data, was "badsecrets-0.4.402.tar", max compression
```

## Comparing `badsecrets-0.4.398.tar` & `badsecrets-0.4.402.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    35149 2023-07-21 20:37:42.332475 badsecrets-0.4.398/LICENSE
--rw-r--r--   0        0        0    32418 2023-07-21 20:37:42.332475 badsecrets-0.4.398/README.md
--rw-r--r--   0        0        0      711 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/__init__.py
--rw-r--r--   0        0        0     7763 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4210 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7939 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     5076 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0    10468 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1006 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2867 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/express_signedcookies_cs.py
--rw-r--r--   0        0        0     2287 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/express_signedcookies_es.py
--rw-r--r--   0        0        0     1120 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4087 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14881 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2192 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1958 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3097 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2963 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     5002 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3776 2023-07-21 20:37:42.332475 badsecrets-0.4.398/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654096 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-07-21 20:37:42.336475 badsecrets-0.4.398/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-07-21 20:37:42.356476 badsecrets-0.4.398/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-07-21 20:37:42.360476 badsecrets-0.4.398/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-07-21 20:37:42.360476 badsecrets-0.4.398/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-07-21 20:38:10.452760 badsecrets-0.4.398/pyproject.toml
--rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.398/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-28 19:44:29.402510 badsecrets-0.4.402/LICENSE
+-rw-r--r--   0        0        0    32418 2023-07-28 19:44:29.402510 badsecrets-0.4.402/README.md
+-rw-r--r--   0        0        0      711 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/__init__.py
+-rw-r--r--   0        0        0     7763 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7939 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10468 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0     1006 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2867 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/express_signedcookies_cs.py
+-rw-r--r--   0        0        0     2287 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/express_signedcookies_es.py
+-rw-r--r--   0        0        0     1120 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4087 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14881 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2192 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1958 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3097 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2963 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     5002 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3776 2023-07-28 19:44:29.402510 badsecrets-0.4.402/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-07-28 19:44:29.410510 badsecrets-0.4.402/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-07-28 19:44:29.430510 badsecrets-0.4.402/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-07-28 19:44:29.434510 badsecrets-0.4.402/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-07-28 19:44:29.434510 badsecrets-0.4.402/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-07-28 19:44:54.770801 badsecrets-0.4.402/pyproject.toml
+-rw-r--r--   0        0        0    33272 1970-01-01 00:00:00.000000 badsecrets-0.4.402/PKG-INFO
```

### Comparing `badsecrets-0.4.398/LICENSE` & `badsecrets-0.4.402/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/README.md` & `badsecrets-0.4.402/README.md`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/__init__.py` & `badsecrets-0.4.402/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/base.py` & `badsecrets-0.4.402/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/examples/blacklist3r.py` & `badsecrets-0.4.402/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/examples/cli.py` & `badsecrets-0.4.402/badsecrets/examples/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,22 +49,22 @@
 
     def print_report(self, report_message):
         print(report_message)
         print(f"Detecting Module: {self.x['detecting_module']}\n")
         print(f"Product Type: {self.x['description']['product']}")
         print(f"Product: {self.x['product']}")
         print(f"Secret Type: {self.x['description']['secret']}")
-        print(f"Severity: {self.x['description']['severity']}")
         print(f"Location: {self.x['location']}")
 
 
 class ReportSecret(BaseReport):
     def report(self):
         self.print_report(print_status("Known Secret Found!\n", color=Fore.GREEN, passthru=True))
         print_status(f"Secret: {self.x['secret']}", color=Fore.GREEN)
+        print(f"Severity: {self.x['description']['severity']}")
         print(f"Details: {self.x['details']}")
 
 
 class ReportIdentify(BaseReport):
     def report(self):
         self.print_report(
             print_status("Cryptographic Product Identified (no vulnerability)\n", color=Fore.YELLOW, passthru=True)
```

### Comparing `badsecrets-0.4.398/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.4.402/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.4.402/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/helpers.py` & `badsecrets-0.4.402/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.4.402/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.4.402/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/express_signedcookies_cs.py` & `badsecrets-0.4.402/badsecrets/modules/express_signedcookies_cs.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/express_signedcookies_es.py` & `badsecrets-0.4.402/badsecrets/modules/express_signedcookies_es.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.4.402/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/generic_jwt.py` & `badsecrets-0.4.402/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.4.402/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.4.402/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.4.402/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.4.402/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.4.402/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.4.402/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.4.402/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.4.402/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.4.402/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.4.402/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.4.402/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.4.402/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.4.402/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.4.402/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.4.402/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.4.402/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.4.402/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.4.402/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.4.402/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.4.402/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.4.398/pyproject.toml` & `badsecrets-0.4.402/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.4.398"
+version = "v0.4.402"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.4.398/PKG-INFO` & `badsecrets-0.4.402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.4.398
+Version: 0.4.402
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

