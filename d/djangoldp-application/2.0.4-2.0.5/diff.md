# Comparing `tmp/djangoldp_application-2.0.4.tar.gz` & `tmp/djangoldp_application-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_application-2.0.4.tar", last modified: Fri Jul 28 13:58:38 2023, max compression
+gzip compressed data, was "djangoldp_application-2.0.5.tar", last modified: Fri Jul 28 15:11:09 2023, max compression
```

## Comparing `djangoldp_application-2.0.4.tar` & `djangoldp_application-2.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-28 13:58:35.000000 djangoldp_application-2.0.4/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0006_applicationservice.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21594 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.524931 djangoldp_application-2.0.4/djangoldp_application/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/email.html
--rw-rw-rw-   0 root         (0) root         (0)    26529 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/djangoldp_application/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1425 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 13:58:38.000000 djangoldp_application-2.0.4/djangoldp_application.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-28 13:58:38.528931 djangoldp_application-2.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-28 13:58:20.000000 djangoldp_application-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.831611 djangoldp_application-2.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 15:11:09.831611 djangoldp_application-2.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.827611 djangoldp_application-2.0.5/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-28 15:11:05.000000 djangoldp_application-2.0.5/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.831611 djangoldp_application-2.0.5/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0006_applicationservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21599 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.827611 djangoldp_application-2.0.5/djangoldp_application/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.831611 djangoldp_application-2.0.5/djangoldp_application/templates/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/templates/djangoldp_application/email.html
+-rw-rw-rw-   0 root         (0) root         (0)    26529 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/djangoldp_application/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:11:09.827611 djangoldp_application-2.0.5/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-28 15:11:09.000000 djangoldp_application-2.0.5/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-28 15:11:09.000000 djangoldp_application-2.0.5/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 15:11:09.000000 djangoldp_application-2.0.5/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-28 15:11:09.000000 djangoldp_application-2.0.5/djangoldp_application.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-28 15:11:09.000000 djangoldp_application-2.0.5/djangoldp_application.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-07-28 15:11:09.835612 djangoldp_application-2.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-28 15:10:44.000000 djangoldp_application-2.0.5/setup.py
```

### Comparing `djangoldp_application-2.0.4/README.md` & `djangoldp_application-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/admin.py` & `djangoldp_application-2.0.5/djangoldp_application/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-2.0.5/djangoldp_application/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-2.0.5/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application/models.py` & `djangoldp_application-2.0.5/djangoldp_application/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,18 +625,18 @@
                 {
                     "message": "{} {}\n{} {}".format(
                         _("A new application have been created:"),
                         instance.client_url,
                         _("Created by:"),
                         instance.creator.get_full_name(),
                     ),
-                    "link": (getattr(settings, 'INSTANCE_DEFAULT_CLIENT', False) or getattr(settings, 'JABBER_DEFAULT_HOST')),
+                    "link": (getattr(settings, 'INSTANCE_DEFAULT_CLIENT', False) or getattr(settings, 'JABBER_DEFAULT_HOST', "")),
                     "object": "{} (https://{})".format(
                         _("A new application have been created"),
-                        instance.client_url
+                        instance.client_url,
                     ),
                 },
             )
 
             send_mail(
                 "{} (https://{})".format(
                     _("A new application have been created ") + instance.application_title,
```

### Comparing `djangoldp_application-2.0.4/djangoldp_application/templates/djangoldp_application/email.html` & `djangoldp_application-2.0.5/djangoldp_application/templates/djangoldp_application/email.html`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <table role="presentation" border="0" cellpadding="0" cellspacing="0" class="btn btn-primary" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; box-sizing: border-box; width: 100%;" width="100%">
   <tbody>
     <tr>
       <td align="center" style="font-family: sans-serif; font-size: 14px; vertical-align: top; padding-bottom: 15px; padding-top: 15px" valign="top">
         <table role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate; mso-table-lspace: 0pt; mso-table-rspace: 0pt; width: auto;">
           <tbody>
             <tr>
-              <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; border-radius: 5px; text-align: center; background-color: #3498db;" valign="top" align="center" bgcolor="#3498db"> <a href="{% link %}" target="_blank" style="border: solid 1px #3498db; border-radius: 5px; box-sizing: border-box; cursor: pointer; display: inline-block; font-size: 14px; font-weight: bold; margin: 0; padding: 12px 25px; text-decoration: none; background-color: #3498db; border-color: #3498db; color: #ffffff;">{% trans "Accéder à l'application" %}</a> </td>
+              <td style="font-family: sans-serif; font-size: 14px; vertical-align: top; border-radius: 5px; text-align: center; background-color: #3498db;" valign="top" align="center" bgcolor="#3498db"> <a href="{{ link }}" target="_blank" style="border: solid 1px #3498db; border-radius: 5px; box-sizing: border-box; cursor: pointer; display: inline-block; font-size: 14px; font-weight: bold; margin: 0; padding: 12px 25px; text-decoration: none; background-color: #3498db; border-color: #3498db; color: #ffffff;">{% trans "Accéder à l'application" %}</a> </td>
             </tr>
           </tbody>
         </table>
       </td>
     </tr>
   </tbody>
 </table>
```

### Comparing `djangoldp_application-2.0.4/djangoldp_application/views.py` & `djangoldp_application-2.0.5/djangoldp_application/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-2.0.5/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-2.0.4/setup.cfg` & `djangoldp_application-2.0.5/setup.cfg`

 * *Files identical despite different names*

