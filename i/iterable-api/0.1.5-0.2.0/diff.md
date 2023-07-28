# Comparing `tmp/iterable-api-0.1.5.tar.gz` & `tmp/iterable-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable-api-0.1.5.tar", max compression
+gzip compressed data, was "iterable-api-0.2.0.tar", max compression
```

## Comparing `iterable-api-0.1.5.tar` & `iterable-api-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35147 2021-06-27 15:07:12.400044 iterable-api-0.1.5/LICENSE
--rw-r--r--   0        0        0     1910 2022-09-06 21:28:07.086804 iterable-api-0.1.5/README.md
--rw-r--r--   0        0        0      847 2022-12-01 04:48:30.958082 iterable-api-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       54 2021-06-27 15:07:12.400528 iterable-api-0.1.5/src/iterable/__init__.py
--rw-r--r--   0        0        0     4620 2021-11-25 20:57:27.190846 iterable-api-0.1.5/src/iterable/client.py
--rw-r--r--   0        0        0      257 2021-06-27 15:07:12.401082 iterable-api-0.1.5/src/iterable/exceptions.py
--rw-r--r--   0        0        0     1151 2021-06-27 15:07:12.401521 iterable-api-0.1.5/src/iterable/helpers.py
--rw-r--r--   0        0        0      862 2021-06-27 15:07:12.401906 iterable-api-0.1.5/src/iterable/resources/__init__.py
--rw-r--r--   0        0        0       77 2021-06-27 15:07:12.402097 iterable-api-0.1.5/src/iterable/resources/base.py
--rw-r--r--   0        0        0     3016 2021-06-27 15:07:12.402248 iterable-api-0.1.5/src/iterable/resources/campaigns.py
--rw-r--r--   0        0        0      939 2021-06-27 15:07:12.402373 iterable-api-0.1.5/src/iterable/resources/channels.py
--rw-r--r--   0        0        0     1128 2021-06-27 15:07:12.402504 iterable-api-0.1.5/src/iterable/resources/commerce.py
--rw-r--r--   0        0        0      884 2021-06-27 15:07:12.402639 iterable-api-0.1.5/src/iterable/resources/email.py
--rw-r--r--   0        0        0     3279 2022-12-01 03:15:50.039436 iterable-api-0.1.5/src/iterable/resources/events.py
--rw-r--r--   0        0        0      676 2021-06-27 15:07:12.402927 iterable-api-0.1.5/src/iterable/resources/experiments.py
--rw-r--r--   0        0        0     1324 2021-06-27 15:07:12.403057 iterable-api-0.1.5/src/iterable/resources/export.py
--rw-r--r--   0        0        0     1093 2021-06-27 15:07:12.403182 iterable-api-0.1.5/src/iterable/resources/in_app.py
--rw-r--r--   0        0        0     1770 2021-06-27 15:07:12.403307 iterable-api-0.1.5/src/iterable/resources/lists.py
--rw-r--r--   0        0        0      160 2021-06-27 15:07:12.403435 iterable-api-0.1.5/src/iterable/resources/message_types.py
--rw-r--r--   0        0        0     1274 2021-06-27 15:07:12.403557 iterable-api-0.1.5/src/iterable/resources/metadata.py
--rw-r--r--   0        0        0     1076 2021-06-27 15:07:12.403682 iterable-api-0.1.5/src/iterable/resources/push.py
--rw-r--r--   0        0        0      976 2021-06-27 15:07:12.403821 iterable-api-0.1.5/src/iterable/resources/sms.py
--rw-r--r--   0        0        0     7635 2022-12-01 03:12:23.422315 iterable-api-0.1.5/src/iterable/resources/templates.py
--rw-r--r--   0        0        0     6964 2021-06-27 15:07:12.404251 iterable-api-0.1.5/src/iterable/resources/users.py
--rw-r--r--   0        0        0      736 2021-06-27 15:07:12.404436 iterable-api-0.1.5/src/iterable/resources/utils.py
--rw-r--r--   0        0        0      698 2021-06-27 15:07:12.404623 iterable-api-0.1.5/src/iterable/resources/web_push.py
--rw-r--r--   0        0        0      559 2021-06-27 15:07:12.404808 iterable-api-0.1.5/src/iterable/resources/workflows.py
--rw-r--r--   0        0        0     2727 2022-12-01 04:48:55.600928 iterable-api-0.1.5/setup.py
--rw-r--r--   0        0        0     2806 2022-12-01 04:48:55.601307 iterable-api-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-06-27 15:07:12.400044 iterable-api-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1910 2022-09-06 21:28:07.086804 iterable-api-0.2.0/README.md
+-rw-r--r--   0        0        0      847 2023-07-28 00:32:02.536864 iterable-api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2021-06-27 15:07:12.400528 iterable-api-0.2.0/src/iterable/__init__.py
+-rw-r--r--   0        0        0     4620 2021-11-25 20:57:27.190846 iterable-api-0.2.0/src/iterable/client.py
+-rw-r--r--   0        0        0      257 2021-06-27 15:07:12.401082 iterable-api-0.2.0/src/iterable/exceptions.py
+-rw-r--r--   0        0        0     1151 2021-06-27 15:07:12.401521 iterable-api-0.2.0/src/iterable/helpers.py
+-rw-r--r--   0        0        0      862 2021-06-27 15:07:12.401906 iterable-api-0.2.0/src/iterable/resources/__init__.py
+-rw-r--r--   0        0        0       77 2021-06-27 15:07:12.402097 iterable-api-0.2.0/src/iterable/resources/base.py
+-rw-r--r--   0        0        0     3016 2021-06-27 15:07:12.402248 iterable-api-0.2.0/src/iterable/resources/campaigns.py
+-rw-r--r--   0        0        0      939 2021-06-27 15:07:12.402373 iterable-api-0.2.0/src/iterable/resources/channels.py
+-rw-r--r--   0        0        0     1127 2023-07-28 00:29:37.382340 iterable-api-0.2.0/src/iterable/resources/commerce.py
+-rw-r--r--   0        0        0      884 2021-06-27 15:07:12.402639 iterable-api-0.2.0/src/iterable/resources/email.py
+-rw-r--r--   0        0        0     3279 2022-12-01 03:15:50.039436 iterable-api-0.2.0/src/iterable/resources/events.py
+-rw-r--r--   0        0        0      676 2021-06-27 15:07:12.402927 iterable-api-0.2.0/src/iterable/resources/experiments.py
+-rw-r--r--   0        0        0     1324 2021-06-27 15:07:12.403057 iterable-api-0.2.0/src/iterable/resources/export.py
+-rw-r--r--   0        0        0     1093 2021-06-27 15:07:12.403182 iterable-api-0.2.0/src/iterable/resources/in_app.py
+-rw-r--r--   0        0        0     1770 2021-06-27 15:07:12.403307 iterable-api-0.2.0/src/iterable/resources/lists.py
+-rw-r--r--   0        0        0      160 2021-06-27 15:07:12.403435 iterable-api-0.2.0/src/iterable/resources/message_types.py
+-rw-r--r--   0        0        0     1274 2021-06-27 15:07:12.403557 iterable-api-0.2.0/src/iterable/resources/metadata.py
+-rw-r--r--   0        0        0     1076 2021-06-27 15:07:12.403682 iterable-api-0.2.0/src/iterable/resources/push.py
+-rw-r--r--   0        0        0      976 2021-06-27 15:07:12.403821 iterable-api-0.2.0/src/iterable/resources/sms.py
+-rw-r--r--   0        0        0     7635 2022-12-01 03:12:23.422315 iterable-api-0.2.0/src/iterable/resources/templates.py
+-rw-r--r--   0        0        0     7086 2023-07-28 00:29:37.382678 iterable-api-0.2.0/src/iterable/resources/users.py
+-rw-r--r--   0        0        0      736 2021-06-27 15:07:12.404436 iterable-api-0.2.0/src/iterable/resources/utils.py
+-rw-r--r--   0        0        0      698 2021-06-27 15:07:12.404623 iterable-api-0.2.0/src/iterable/resources/web_push.py
+-rw-r--r--   0        0        0      559 2021-06-27 15:07:12.404808 iterable-api-0.2.0/src/iterable/resources/workflows.py
+-rw-r--r--   0        0        0     2727 2023-07-28 00:34:20.207703 iterable-api-0.2.0/setup.py
+-rw-r--r--   0        0        0     2806 2023-07-28 00:34:20.208075 iterable-api-0.2.0/PKG-INFO
```

### Comparing `iterable-api-0.1.5/LICENSE` & `iterable-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/README.md` & `iterable-api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/pyproject.toml` & `iterable-api-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterable-api"
-version = "0.1.5"
+version = "0.2.0"
 description = "Iterable API wrapper"
 readme = "README.md"
 authors = ["Alex Kahn <alexkahn@users.noreply.github.com>"]
 license = "GPL-3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `iterable-api-0.1.5/src/iterable/client.py` & `iterable-api-0.2.0/src/iterable/client.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/helpers.py` & `iterable-api-0.2.0/src/iterable/helpers.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/__init__.py` & `iterable-api-0.2.0/src/iterable/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/campaigns.py` & `iterable-api-0.2.0/src/iterable/resources/campaigns.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/channels.py` & `iterable-api-0.2.0/src/iterable/resources/channels.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/commerce.py` & `iterable-api-0.2.0/src/iterable/resources/commerce.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if not isinstance(items, (list, tuple)):
             items = [items]
         payload["items"] = items
         payload["total"] = total
         payload["campaignId"] = campaign_id
         payload["templateId"] = template_id
         payload["createdAt"] = created_at
-        payload["data_fields"] = data_fields
+        payload["dataFields"] = data_fields
         return self.client.post(resource, data=payload)
 
     def update_cart(self, user=None, items=None):
         resource = "/api/commerce/updateCart"
         payload = {}
         payload["user"] = user
         if not isinstance(items, (list, tuple)):
```

### Comparing `iterable-api-0.1.5/src/iterable/resources/email.py` & `iterable-api-0.2.0/src/iterable/resources/email.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/events.py` & `iterable-api-0.2.0/src/iterable/resources/events.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/experiments.py` & `iterable-api-0.2.0/src/iterable/resources/experiments.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/export.py` & `iterable-api-0.2.0/src/iterable/resources/export.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/in_app.py` & `iterable-api-0.2.0/src/iterable/resources/in_app.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/lists.py` & `iterable-api-0.2.0/src/iterable/resources/lists.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/metadata.py` & `iterable-api-0.2.0/src/iterable/resources/metadata.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/push.py` & `iterable-api-0.2.0/src/iterable/resources/push.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/sms.py` & `iterable-api-0.2.0/src/iterable/resources/sms.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/templates.py` & `iterable-api-0.2.0/src/iterable/resources/templates.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/users.py` & `iterable-api-0.2.0/src/iterable/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,25 +118,28 @@
                 of the user.
             4. mergeNestedObjects-- in the form of an object-- used to merge top level
                 objects instead of overwriting.
         """
 
         resource = "/api/users/update"
         payload = {}
-        payload["email"] = str(email)
+        if email is not None:
+            payload["email"] = str(email)
         payload["dataFields"] = data_fields
-        payload["userId"] = str(user_id)
+        if user_id is not None:
+            payload["userId"] = str(user_id)
         payload["mergeNestedObjects"] = merge_nested_objects
         return self.client.post(resource, data=payload)
 
-    def update_email(self, current_email, new_email):
+    def update_email(self, current_email, new_email, merge=False):
         resource = "/api/users/updateEmail"
         payload = {}
         payload["currentEmail"] = str(current_email)
         payload["newEmail"] = str(new_email)
+        payload["merge"] = bool(merge)
         return self.client.post(resource, data=payload)
 
     def bulk_update(self, users):
         """
         The Iterable 'Bulk User Update' api Bulk update user data or adds
         it if does not exist. Data is merged - missing fields are not deleted
```

### Comparing `iterable-api-0.1.5/src/iterable/resources/utils.py` & `iterable-api-0.2.0/src/iterable/resources/utils.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/web_push.py` & `iterable-api-0.2.0/src/iterable/resources/web_push.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/src/iterable/resources/workflows.py` & `iterable-api-0.2.0/src/iterable/resources/workflows.py`

 * *Files identical despite different names*

### Comparing `iterable-api-0.1.5/setup.py` & `iterable-api-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'iterable-api',
-    'version': '0.1.5',
+    'version': '0.2.0',
     'description': 'Iterable API wrapper',
     'long_description': "# Iterable API\n\nThis is a mostly complete wrapper of the Iterable API built with Python.\n\nThe interface is still in a state of flux, some methods will be renamed but the signatures should stay the same.\n\n## User Docs\n\nThis is a pure python development kit for interacting with the Iterable API. If you find anything to be out of date or are looking for support, you can file an issue on Github.\n\n### Installation\n\nYou can download and install the package from the Python Package Index with:\n\n```\npip install iterable-api\n```\n\n### Quickstart\n\n```py\nfrom iterable import Iterable\n\napi = Iterable('YOUR_API_KEY')\n\napi.events.track(event_name='hello_iterable', user_id=42, created_at=datetime.now().to_timestamp())\n```\n\nIf you're familiar with environment variables, you can set `ITERABLE_API_KEY`. In that case you can set up the api client like so:\n\n```py\nfrom os import getenv\nfrom iterable import Iterable\n\napi = Iterable(getenv('ITERABLE_API_KEY'))\n```\n\n### Data exports\n\nIf you're interested in getting data out of your Iterable account, you can use the `export_data_api` method on the API client.\n\n### Dropping down\n\nThe API client is a requests.Session under the hood with HTTP method names as top level functions in the wrapper.\n\nIf you want to drop down to the client, you only need to provide the resource path, e.g.:\n\n```py\napi.get('/events/track')\n```\n\nThis might be useful for exploring the API or debugging an issue.\n\n## Development Docs\n\nIf you're interested in extending this library, please follow these guidelines:\n\n1. Please file an issue first describing what you want to add or change.\n2. Fork the repository and submit a pull request.\n\n### Installation for development\n\nThis project uses poetry for now, so follow your preferred procedure for that.\n\n```\npoetry install\n```\n\n### Testing\n\nThe library uses pytest - you can run the tests by invoking the following:\n\n```py\npoetry run pytest\n```\n",
     'author': 'Alex Kahn',
     'author_email': 'alexkahn@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alexkahn/iterable-api',
```

### Comparing `iterable-api-0.1.5/PKG-INFO` & `iterable-api-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable-api
-Version: 0.1.5
+Version: 0.2.0
 Summary: Iterable API wrapper
 Home-page: https://github.com/alexkahn/iterable-api
 License: GPL-3.0
 Author: Alex Kahn
 Author-email: alexkahn@users.noreply.github.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

