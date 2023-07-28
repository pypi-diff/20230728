# Comparing `tmp/emark-1.1rc4.tar.gz` & `tmp/emark-2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emark-1.1rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "emark-2.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `emark-1.1rc4.tar` & `emark-2.0rc1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1518 2023-07-28 11:46:22.188819 emark-1.1rc4/LICENSE
--rw-r--r--   0        0        0     5944 2023-07-28 11:46:22.188819 emark-1.1rc4/README.md
--rw-r--r--   0        0        0      152 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/__init__.py
--rw-r--r--   0        0        0      158 2023-07-28 11:46:46.424820 emark-1.1rc4/emark/_version.py
--rw-r--r--   0        0        0     4282 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/backends.py
--rw-r--r--   0        0        0     1030 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/buildapi.py
--rw-r--r--   0        0        0      309 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/conf.py
--rw-r--r--   0        0        0      535 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9005 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/message.py
--rw-r--r--   0        0        0     3483 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/migrations/__init__.py
--rw-r--r--   0        0        0     2247 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/models.py
--rw-r--r--   0        0        0     3259 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/base.html
--rw-r--r--   0        0        0     1081 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/license.txt
--rw-r--r--   0        0        0     5945 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/templates/emark/styles.css
--rw-r--r--   0        0        0      325 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/urls.py
--rw-r--r--   0        0        0     3796 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/utils.py
--rw-r--r--   0        0        0     3040 2023-07-28 11:46:22.188819 emark-1.1rc4/emark/views.py
--rw-r--r--   0        0        0     2302 2023-07-28 11:46:22.188819 emark-1.1rc4/pyproject.toml
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc4/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-07-28 13:43:07.232656 emark-2.0rc1/LICENSE
+-rw-r--r--   0        0        0     5944 2023-07-28 13:43:07.232656 emark-2.0rc1/README.md
+-rw-r--r--   0        0        0      152 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-28 13:43:33.321516 emark-2.0rc1/emark/_version.py
+-rw-r--r--   0        0        0     4231 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/backends.py
+-rw-r--r--   0        0        0     1030 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/buildapi.py
+-rw-r--r--   0        0        0      309 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/conf.py
+-rw-r--r--   0        0        0      535 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9106 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/message.py
+-rw-r--r--   0        0        0     3483 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1495 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/migrations/0002_rename_from_address_send_from_email_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/migrations/__init__.py
+-rw-r--r--   0        0        0     2465 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/models.py
+-rw-r--r--   0        0        0     3259 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/templates/emark/base.html
+-rw-r--r--   0        0        0     1081 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/templates/emark/license.txt
+-rw-r--r--   0        0        0     5945 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/templates/emark/styles.css
+-rw-r--r--   0        0        0      325 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/urls.py
+-rw-r--r--   0        0        0     3796 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/utils.py
+-rw-r--r--   0        0        0     3040 2023-07-28 13:43:07.232656 emark-2.0rc1/emark/views.py
+-rw-r--r--   0        0        0     2302 2023-07-28 13:43:07.232656 emark-2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-2.0rc1/PKG-INFO
```

### Comparing `emark-1.1rc4/LICENSE` & `emark-2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/README.md` & `emark-2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/buildapi.py` & `emark-2.0rc1/emark/buildapi.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/locale/de/LC_MESSAGES/django.po` & `emark-2.0rc1/emark/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/message.py` & `emark-2.0rc1/emark/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     text body, which extracts a Gmail style plain text version of the fully rendered
     HTML email.
     """
 
     base_html_template = "emark/base.html"
     template = None
     subject = None
-    _tracking_uuid = False
+    uuid = False
 
     def __init__(
         self,
         language: str,
         subject: str = "",
         context: dict = None,
         utm_params=None,
@@ -56,67 +56,54 @@
     ):
         """Initialize an email message and attach a rendered HTML version of it."""
         self.template = template or self.template
         self.context = context or {}
         self.language = language
         self.utm_params = utm_params or {}
         self.subject = subject or self.subject
+        self.html = None
+        self.markdown = None
         super().__init__(subject=self.subject, **kwargs)
 
-    def get_html(self):
-        """Return the rendered HTML version of the email."""
-        with translation.override(self.language):
-            utm_params = self.get_utm_params()
-            context = self.get_context_data(**utm_params)
-            context |= utm_params
-            template = self.get_template()
-            subject = self.get_subject(**context)
-
-            markdown_string = self.get_markdown_string(template, context, utm_params)
-
-            return self.render_html(
-                markdown_string=markdown_string,
-                context={
-                    "subject": subject,
-                    **context,
-                },
-            )
-
-    def get_body(self, html):
-        """Return the parsed plain text version of the rendered HTML email."""
-        parser = utils.HTML2TextParser()
-        parser.feed(html)
-        parser.close()
-        body = str(parser)
-        if self._tracking_uuid:
-            href = reverse("emark:email-detail", kwargs={"pk": self._tracking_uuid})
-            href = parse.urljoin(self.get_site_url(), href)
-            txt = capfirst(gettext("view in browser"))
-            body = f"{txt} <{href}>\n\n" + body
-        return body
+    @classmethod
+    def to_user(cls, user=None, context=None, language=None, **kwargs):
+        """Return email with user specific language, context and recipient."""
+        if not user.email:
+            raise ValueError("User has no email address")
+        if not user.is_active:
+            raise ValueError("User is not active")
+        if settings.USE_I18N:
+            try:
+                language = language or user.language
+            except AttributeError as e:
+                raise ValueError(
+                    "If your user model does not have a language field,"
+                    " you must provide a language."
+                ) from e
+        context = context or {}
+        context |= {
+            "short_name": user.get_short_name(),
+            "user": user,
+        }
+        obj = cls(
+            **{
+                "to": [f'"{user.get_full_name()}" <{user.email}>'],
+                "context": context,
+                "language": language,
+            }
+            | kwargs
+        )
+        obj.user = user
+        return obj
 
     def message(self):
         # The connection will call .message while sending the email.
-        self.subject = self.get_subject(**self.get_context_data())
-        self.html = self.get_html()
-        self.body = self.get_body(self.html)
-        self.attach_alternative(self.html, "text/html")
+        self.render()
         return super().message()
 
-    def get_utm_params(self, **params: {str: str}) -> {str: str}:
-        """Return a dictionary of UTM parameters."""
-        return (
-            conf.get_settings().UTM_PARAMS
-            | {
-                "utm_campaign": self.get_utm_campaign_name(),
-            }
-            | self.utm_params
-            | params
-        )
-
     @classmethod
     def get_utm_campaign_name(cls):
         """Return the UTM campaign name for this email."""
         return "_".join(
             (m.group(0) for m in CLS_NAME_TO_CAMPAIGN_RE.finditer(cls.__qualname__))
         ).upper()
 
@@ -124,64 +111,38 @@
         """Add UTM parameters to a URL and add the click tracking URL."""
         redirect_url_parts = parse.urlparse(url)
         url_params = dict(parse.parse_qsl(redirect_url_parts.query))
         params.update(url_params)
         url_new_query = parse.urlencode(params)
         redirect_url_parts = redirect_url_parts._replace(query=url_new_query)
         redirect_url = parse.urlunparse(redirect_url_parts)
-        if not self._tracking_uuid:
+        if not self.uuid:
+            return redirect_url
+        site_url = self.get_site_url()
+        # external links should not be tracked
+        top_level_domain = ".".join(site_url.split(".")[-2:])
+        if not redirect_url_parts.netloc.endswith(top_level_domain):
             return redirect_url
-        tracking_url = reverse("emark:email-click", kwargs={"pk": self._tracking_uuid})
-        tracking_url = parse.urljoin(self.get_site_url(), tracking_url)
+        tracking_url = reverse("emark:email-click", kwargs={"pk": self.uuid})
+        tracking_url = parse.urljoin(site_url, tracking_url)
         tracking_url_parts = parse.urlparse(tracking_url)
         tracking_url_parts = tracking_url_parts._replace(
             query=parse.urlencode({"url": redirect_url})
         )
         return parse.urlunparse(tracking_url_parts)
 
-    def set_utm_attributes(self, md, **utm):
+    def inject_utm_params(self, md, **utm):
         for url in INLINE_LINK_RE.findall(md):
             md = md.replace(f"({url})", f"({self.update_url_params(url, **utm)})")
         for url in INLINE_HTML_LINK_RE.findall(md):
             md = md.replace(
                 f'href="{url}"', f'href="{self.update_url_params(url, **utm)}"'
             )
         return md
 
-    @classmethod
-    def to_user(cls, user=None, context=None, language=None, **kwargs):
-        """Return email with user specific language, context and recipient."""
-        if not user.email:
-            raise ValueError("User has no email address")
-        if not user.is_active:
-            raise ValueError("User is not active")
-        if settings.USE_I18N:
-            try:
-                language = language or user.language
-            except AttributeError as e:
-                raise ValueError(
-                    "If your user model does not have a language field,"
-                    " you must provide a language."
-                ) from e
-        context = context or {}
-        context |= {
-            "short_name": user.get_short_name(),
-            "user": user,
-        }
-        obj = cls(
-            **{
-                "to": [f'"{user.get_full_name()}" <{user.email}>'],
-                "context": context,
-                "language": language,
-            }
-            | kwargs
-        )
-        obj.user = user
-        return obj
-
     def get_template(self):
         if not self.template:
             raise ImproperlyConfigured(
                 f"{self.__class__.__qualname__} is missing a template."
             )
         return self.template
 
@@ -192,44 +153,56 @@
         elif apps.is_installed("django.contrib.sites"):
             from django.contrib.sites.models import Site
 
             domain = Site.objects.get_current().domain
 
         return parse.urlunparse((protocol, domain, "", "", "", ""))
 
-    def get_context_data(self, **context):
+    def get_utm_params(self) -> {str: str}:
+        """Return a dictionary of UTM parameters."""
+        return (
+            conf.get_settings().UTM_PARAMS
+            | {
+                "utm_campaign": self.get_utm_campaign_name(),
+            }
+            | self.utm_params
+        )
+
+    def get_context_data(self):
         """Return the context data for the email."""
-        if self._tracking_uuid:
+        context = {}
+        if self.uuid:
             context |= {
-                "tracking_uuid": self._tracking_uuid,
+                "tracking_uuid": self.uuid,
                 "view_in_browser_url": parse.urljoin(
                     self.get_site_url(),
-                    reverse("emark:email-detail", kwargs={"pk": self._tracking_uuid}),
+                    reverse("emark:email-detail", kwargs={"pk": self.uuid}),
                 ),
                 "tracking_pixel_url": parse.urljoin(
                     self.get_site_url(),
-                    reverse("emark:email-open", kwargs={"pk": self._tracking_uuid}),
+                    reverse("emark:email-open", kwargs={"pk": self.uuid}),
                 ),
             }
 
-        return self.context | context
+        return context | self.context
 
     def get_subject(self, **context):
         """Return the email's subject."""
         if not self.subject:
             raise ImproperlyConfigured(
                 f"{self.__class__.__qualname__} is missing a subject."
             )
-        return self.subject
+        return self.subject % context
 
-    def get_markdown_string(self, template, context, utm):
+    def get_markdown(self, context, utm):
+        template = self.get_template()
         markdown_string = loader.get_template(template).render(context)
-        return self.set_utm_attributes(markdown_string, **self.get_utm_params(**utm))
+        return self.inject_utm_params(markdown_string, **utm)
 
-    def render_html(self, markdown_string, context):
+    def get_html(self, markdown_string, context):
         html_message = markdown.markdown(
             markdown_string,
             extensions=[
                 "markdown.extensions.meta",
                 "markdown.extensions.tables",
                 "markdown.extensions.extra",
             ],
@@ -242,7 +215,38 @@
         inlined_html = premailer.transform(
             html=rendered_html,
             strip_important=False,
             keep_style_tags=True,
             cssutils_logging_level=logging.WARNING,
         )
         return inlined_html
+
+    def get_body(self, html):
+        """Return the parsed plain text version of the rendered HTML email."""
+        parser = utils.HTML2TextParser()
+        parser.feed(html)
+        parser.close()
+        body = str(parser)
+        if self.uuid:
+            href = reverse("emark:email-detail", kwargs={"pk": self.uuid})
+            href = parse.urljoin(self.get_site_url(), href)
+            txt = capfirst(gettext("view in browser"))
+            body = f"{txt} <{href}>\n\n" + body
+        return body
+
+    def render(self, tracking_uuid=None):
+        """Render the email."""
+        if self.html is None:
+            self.uuid = tracking_uuid
+            with translation.override(self.language):
+                utm_params = self.get_utm_params()
+                context = self.get_context_data()
+                context |= utm_params
+                self.subject = self.get_subject(**context)
+                context["subject"] = self.subject
+                self.markdown = self.get_markdown(context, utm_params)
+                self.html = self.get_html(
+                    markdown_string=self.markdown,
+                    context=context,
+                )
+                self.body = self.get_body(self.html)
+                self.attach_alternative(self.html, "text/html")
```

### Comparing `emark-1.1rc4/emark/migrations/0001_initial.py` & `emark-2.0rc1/emark/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/models.py` & `emark-2.0rc1/emark/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 
     user = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.SET_NULL,
         related_name="emark_emails",
         null=True,
     )
-    from_address = models.EmailField()
-    to_address = models.EmailField()
+    # In RFC 2822 "from" is a mailbox-list, but Django only support a single
+    from_email = models.TextField(max_length=998)
+    to = models.JSONField(default=list)
+    cc = models.JSONField(default=list)
+    bcc = models.JSONField(default=list)
+    reply_to = models.JSONField(default=list)
     subject = models.TextField(max_length=998)  # RFC 2822
     body = models.TextField()
     html = models.TextField(null=True)
     utm = models.JSONField(default=dict)
     created_at = models.DateTimeField(auto_now_add=True)
 
     def get_absolute_url(self):
```

### Comparing `emark-1.1rc4/emark/templates/emark/base.html` & `emark-2.0rc1/emark/templates/emark/base.html`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/templates/emark/license.txt` & `emark-2.0rc1/emark/templates/emark/license.txt`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/templates/emark/styles.css` & `emark-2.0rc1/emark/templates/emark/styles.css`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/utils.py` & `emark-2.0rc1/emark/utils.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/emark/views.py` & `emark-2.0rc1/emark/views.py`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/pyproject.toml` & `emark-2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emark-1.1rc4/PKG-INFO` & `emark-2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emark
-Version: 1.1rc4
+Version: 2.0rc1
 Summary: Markdown template based HTML and text emails for Django.
 Keywords: Markdown,Django,email,templates,HTML
 Author-email: Rust Saiargaliev <fly.amureki@gmail.com>, Johannes Maron <johannes@maron.family>, Mostafa Mohamed <mostafa.anm91@gmail.com>, Jacqueline Kraus <jacquelinekraus1992@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

