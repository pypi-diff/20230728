# Comparing `tmp/djangoldp_application-2.0.0.tar.gz` & `tmp/djangoldp_application-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_application-2.0.0.tar", last modified: Thu Jul 27 15:06:37 2023, max compression
+gzip compressed data, was "djangoldp_application-2.0.1.tar", last modified: Fri Jul 28 12:52:54 2023, max compression
```

## Comparing `djangoldp_application-2.0.0.tar` & `djangoldp_application-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.527599 djangoldp_application-2.0.0/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-27 15:06:35.000000 djangoldp_application-2.0.0/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0006_applicationservice.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19843 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    26614 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.527599 djangoldp_application-2.0.0/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:52:54.014203 djangoldp_application-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 12:52:54.014203 djangoldp_application-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:52:54.010203 djangoldp_application-2.0.1/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-28 12:52:51.000000 djangoldp_application-2.0.1/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:52:54.014203 djangoldp_application-2.0.1/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0006_applicationservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21594 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    26529 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/djangoldp_application/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 12:52:54.010203 djangoldp_application-2.0.1/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 12:52:53.000000 djangoldp_application-2.0.1/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-07-28 12:52:53.000000 djangoldp_application-2.0.1/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 12:52:53.000000 djangoldp_application-2.0.1/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-28 12:52:53.000000 djangoldp_application-2.0.1/djangoldp_application.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 12:52:53.000000 djangoldp_application-2.0.1/djangoldp_application.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-28 12:52:54.014203 djangoldp_application-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-28 12:52:35.000000 djangoldp_application-2.0.1/setup.py
```

### Comparing `djangoldp_application-2.0.0/README.md` & `djangoldp_application-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/admin.py` & `djangoldp_application-2.0.1/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-2.0.1/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-2.0.1/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/djangoldp_application/models.py` & `djangoldp_application-2.0.1/djangoldp_application/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import uuid
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.core.mail import send_mail
 from django.db import models
 from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
+from django.template import loader
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 from djangoldp.models import Model
 from djangoldp_component.models import Component, Package
 from rest_framework.exceptions import ValidationError
 
+EMAIL_FROM = getattr(settings, "DEFAULT_FROM_EMAIL", False) or getattr(
+    settings, "EMAIL_HOST_USER", False
+)
+
 
 class Application(Model):
     repository = models.CharField(max_length=255, blank=True, null=True)
     friendly_name = models.CharField(max_length=255, blank=True, null=True)
     short_description = models.CharField(max_length=255, blank=True, null=True)
     creator = models.ForeignKey(
         get_user_model(),
@@ -605,7 +611,43 @@
             setattr(
                 instance, Model.slug_field(instance), slugify(instance.friendly_name)
             )
             setattr(instance, "urlid", "")
     else:
         # Is a distant object, generate a random slug
         setattr(instance, Model.slug_field(instance), uuid.uuid4().hex.upper()[0:8])
+
+@receiver(post_save, sender=Application)
+def post_create_mail_admins(created, instance, **kwargs):
+    if created:
+        if instance.client_url.endswith(".otc.startinblox.com"):
+            html_message = loader.render_to_string(
+                "djangoldp_application/email.html",
+                {
+                    "message": "{} {}\n{} {}".format(
+                        _("A new application have been created:"),
+                        instance.client_url,
+                        _("Created by:"),
+                        instance.creator.get_full_name(),
+                    ),
+                    "link": (getattr(settings, 'INSTANCE_DEFAULT_CLIENT', False) or getattr(settings, 'JABBER_DEFAULT_HOST')),
+                    "object": "{} (https://{})".format(
+                        _("A new application have been created"),
+                        instance.client_url
+                    ),
+                },
+            )
+
+            send_mail(
+                "{} (https://{})".format(
+                    _("A new application have been created ") + instance.application_title,
+                    instance.client_url,
+                ),
+                "{} (https://{})".format(
+                    _("A new application have been created ") + instance.application_title,
+                    instance.client_url,
+                ),
+                EMAIL_FROM,
+                get_user_model().objects.filter(is_superuser=True).values_list('email'),
+                fail_silently=True,
+                html_message=html_message,
+            )
```

### Comparing `djangoldp_application-2.0.0/djangoldp_application/views.py` & `djangoldp_application-2.0.1/djangoldp_application/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,31 +549,29 @@
             if deploy.requester:
                 requester = deploy.requester
             else:
                 requester = application.creator
 
             if application.deployments.count() == 1:
                 html_message = loader.render_to_string(
-                    "email.html",
+                    "djangoldp_application/email.html",
                     {
-                        "on": application.client_url,
-                        "instance": {"summary": _("Deployment done. You can use the default account: admin/admin. Don't forget to create your own account.")},
-                        "author": requester.get_full_name(),
+                        "message": _("Deployment done. You can use the default account: admin/admin. Don't forget to create your own account."),
+                        "link": application.client_url,
                         "object": "{} https://{}".format(
                             _("About your deployment of"), application.client_url
                         ),
                     },
                 )
             else :
                 html_message = loader.render_to_string(
-                    "email.html",
+                    "djangoldp_application/email.html",
                     {
-                        "on": application.client_url,
-                        "instance": {"summary": _("Deployment done.")},
-                        "author": requester.get_full_name(),
+                        "message": _("Deployment done."),
+                        "link": application.client_url,
                         "object": "{} https://{}".format(
                             _("About your deployment of"), application.client_url
                         ),
                     },
                 )
 
             send_mail(
@@ -597,19 +595,18 @@
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Failed"
             deploy.save()
             if deploy.requester:
                 html_message = loader.render_to_string(
-                    "email.html",
+                    "djangoldp_application/email.html",
                     {
-                        "on": application.client_url,
-                        "instance": {"summary": _("Deployment failed")},
-                        "author": deploy.requester.get_full_name(),
+                        "message": _("Deployment failed"),
+                        "link": (getattr(settings, 'INSTANCE_DEFAULT_CLIENT', False) or getattr(settings, 'JABBER_DEFAULT_HOST')),
                         "object": "{} https://{}".format(
                             _("About your deployment of"), application.client_url
                         ),
                     },
                 )
 
                 send_mail(
```

### Comparing `djangoldp_application-2.0.0/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-2.0.1/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.0/setup.cfg` & `djangoldp_application-2.0.1/setup.cfg`

 * *Files identical despite different names*

