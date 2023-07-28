# Comparing `tmp/emark-1.1rc3.tar.gz` & `tmp/emark-1.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emark-1.1rc3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "emark-1.1rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `emark-1.1rc3.tar` & `emark-1.1rc4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1518 2023-07-21 11:26:22.438302 emark-1.1rc3/LICENSE
--rw-r--r--   0        0        0     5944 2023-07-21 11:26:22.438302 emark-1.1rc3/README.md
--rw-r--r--   0        0        0      152 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/__init__.py
--rw-r--r--   0        0        0      158 2023-07-21 11:26:48.790992 emark-1.1rc3/emark/_version.py
--rw-r--r--   0        0        0     4282 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/backends.py
--rw-r--r--   0        0        0     1030 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/buildapi.py
--rw-r--r--   0        0        0      309 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/conf.py
--rw-r--r--   0        0        0      535 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9005 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/message.py
--rw-r--r--   0        0        0     3483 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/migrations/__init__.py
--rw-r--r--   0        0        0     2247 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/models.py
--rw-r--r--   0        0        0     3259 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/templates/emark/base.html
--rw-r--r--   0        0        0     1081 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/templates/emark/license.txt
--rw-r--r--   0        0        0     5945 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/templates/emark/styles.css
--rw-r--r--   0        0        0      325 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/urls.py
--rw-r--r--   0        0        0     3796 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/utils.py
--rw-r--r--   0        0        0     2505 2023-07-21 11:26:22.438302 emark-1.1rc3/emark/views.py
--rw-r--r--   0        0        0     2302 2023-07-21 11:26:22.438302 emark-1.1rc3/pyproject.toml
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc3/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-07-28 11:46:22.188819 emark-1.1rc4/LICENSE
+-rw-r--r--   0        0        0     5944 2023-07-28 11:46:22.188819 emark-1.1rc4/README.md
+-rw-r--r--   0        0        0      152 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-28 11:46:46.424820 emark-1.1rc4/emark/_version.py
+-rw-r--r--   0        0        0     4282 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/backends.py
+-rw-r--r--   0        0        0     1030 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/buildapi.py
+-rw-r--r--   0        0        0      309 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/conf.py
+-rw-r--r--   0        0        0      535 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9005 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/message.py
+-rw-r--r--   0        0        0     3483 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/migrations/__init__.py
+-rw-r--r--   0        0        0     2247 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/models.py
+-rw-r--r--   0        0        0     3259 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/base.html
+-rw-r--r--   0        0        0     1081 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/license.txt
+-rw-r--r--   0        0        0     5945 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/styles.css
+-rw-r--r--   0        0        0      325 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/urls.py
+-rw-r--r--   0        0        0     3796 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/utils.py
+-rw-r--r--   0        0        0     3040 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/views.py
+-rw-r--r--   0        0        0     2302 2023-07-28 11:46:22.188819 emark-1.1rc4/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc4/PKG-INFO
```

### Comparing `emark-1.1rc3/LICENSE` & `emark-1.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/README.md` & `emark-1.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/backends.py` & `emark-1.1rc4/emark/backends.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/buildapi.py` & `emark-1.1rc4/emark/buildapi.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/locale/de/LC_MESSAGES/django.po` & `emark-1.1rc4/emark/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/message.py` & `emark-1.1rc4/emark/message.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/migrations/0001_initial.py` & `emark-1.1rc4/emark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/models.py` & `emark-1.1rc4/emark/models.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/templates/emark/base.html` & `emark-1.1rc4/emark/templates/emark/base.html`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/templates/emark/license.txt` & `emark-1.1rc4/emark/templates/emark/license.txt`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/templates/emark/styles.css` & `emark-1.1rc4/emark/templates/emark/styles.css`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/utils.py` & `emark-1.1rc4/emark/utils.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/emark/views.py` & `emark-1.1rc4/emark/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from urllib.parse import urlparse
+
 from django import http
-from django.utils.http import url_has_allowed_host_and_scheme
+from django.conf import settings
+from django.http.request import split_domain_port, validate_host
 from django.views import View
 from django.views.generic.detail import SingleObjectMixin
 
 from . import models
 
 # white 1x1 pixel JPEG in bytes:
 #
@@ -41,18 +44,32 @@
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
 
         redirect_to = request.GET.get("url")
         # The redirect_to URL is user-provided, so it might be malicious
         # or malformed. We use Django's URL validation to ensure that it
         # is safe to redirect to.
-        if not url_has_allowed_host_and_scheme(
-            url=redirect_to,
-            allowed_hosts=request.get_host(),
-            require_https=request.is_secure(),
+        parsed_url = urlparse(redirect_to)
+        if not parsed_url.netloc:
+            return http.HttpResponseBadRequest("Missing url or malformed parameter")
+
+        domain, _port = split_domain_port(parsed_url.netloc)
+        allowed_hosts = settings.ALLOWED_HOSTS
+        if settings.DEBUG:
+            allowed_hosts = settings.ALLOWED_HOSTS + [
+                ".localhost",
+                "127.0.0.1",
+                "[::1]",
+            ]
+        if any(
+            [
+                not domain,
+                not validate_host(domain, allowed_hosts),
+                request.scheme != parsed_url.scheme,
+            ]
         ):
             return http.HttpResponseBadRequest("Missing url or malformed parameter")
 
         models.Click.objects.create_for_request(
             request, email=self.object, redirect_url=redirect_to
         )
         return http.HttpResponseRedirect(redirect_to)
```

### Comparing `emark-1.1rc3/pyproject.toml` & `emark-1.1rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emark-1.1rc3/PKG-INFO` & `emark-1.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emark
-Version: 1.1rc3
+Version: 1.1rc4
 Summary: Markdown template based HTML and text emails for Django.
 Keywords: Markdown,Django,email,templates,HTML
 Author-email: Rust Saiargaliev <fly.amureki@gmail.com>, Johannes Maron <johannes@maron.family>, Mostafa Mohamed <mostafa.anm91@gmail.com>, Jacqueline Kraus <jacquelinekraus1992@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

