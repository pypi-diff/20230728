# Comparing `tmp/wagtail-cache-2.2.0.tar.gz` & `tmp/wagtail-cache-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cache-2.2.0.tar", last modified: Wed Oct 19 23:18:20 2022, max compression
+gzip compressed data, was "wagtail-cache-2.3.0.tar", last modified: Thu Jul 27 22:48:02 2023, max compression
```

## Comparing `wagtail-cache-2.2.0.tar` & `wagtail-cache-2.3.0.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.915282 wagtail-cache-2.2.0/
--rw-rw-rw-   0        0        0     1921 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       96 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3815 2022-10-19 23:18:20.915282 wagtail-cache-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2988 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/README.md
--rw-rw-rw-   0        0        0      187 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      412 2022-10-19 23:18:20.915282 wagtail-cache-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1060 2022-10-19 23:09:55.000000 wagtail-cache-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtail_cache.egg-info/
--rw-rw-rw-   0        0        0     3815 2022-10-19 23:18:20.000000 wagtail-cache-2.2.0/wagtail_cache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2022-10-19 23:18:20.000000 wagtail-cache-2.2.0/wagtail_cache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-19 23:18:20.000000 wagtail-cache-2.2.0/wagtail_cache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-10-19 23:18:20.000000 wagtail-cache-2.2.0/wagtail_cache.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-10-19 23:18:20.000000 wagtail-cache-2.2.0/wagtail_cache.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtailcache/
--rw-rw-rw-   0        0        0      157 2022-10-19 23:10:24.000000 wagtail-cache-2.2.0/wagtailcache/__init__.py
--rw-rw-rw-   0        0        0      222 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/apps.py
--rw-rw-rw-   0        0        0    15620 2022-10-19 23:09:55.000000 wagtail-cache-2.2.0/wagtailcache/cache.py
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtailcache/compat_backends/
--rw-rw-rw-   0        0        0        0 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/compat_backends/__init__.py
--rw-rw-rw-   0        0        0      408 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/compat_backends/django_redis.py
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtailcache/management/
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtailcache/management/commands/
--rw-rw-rw-   0        0        0      278 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/management/commands/clear_wagtail_cache.py
--rw-rw-rw-   0        0        0     1370 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/settings.py
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.899681 wagtail-cache-2.2.0/wagtailcache/templates/
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.915282 wagtail-cache-2.2.0/wagtailcache/templates/wagtailcache/
--rw-rw-rw-   0        0        0     1757 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/wagtailcache/templates/wagtailcache/index.html
--rw-rw-rw-   0        0        0      332 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/wagtailcache/templates/wagtailcache/wagtailcache-bolt.svg
-drwxrwxrwx   0        0        0        0 2022-10-19 23:18:20.915282 wagtail-cache-2.2.0/wagtailcache/templatetags/
--rw-rw-rw-   0        0        0        0 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1578 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/templatetags/wagtailcache_tags.py
--rw-rw-rw-   0        0        0      225 2022-08-05 16:48:51.000000 wagtail-cache-2.2.0/wagtailcache/urls.py
--rw-rw-rw-   0        0        0      901 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/wagtailcache/views.py
--rw-rw-rw-   0        0        0     1397 2022-10-19 23:07:03.000000 wagtail-cache-2.2.0/wagtailcache/wagtail_hooks.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.017834 wagtail-cache-2.3.0/
+-rw-rw-rw-   0        0        0     1921 2022-10-19 23:07:03.000000 wagtail-cache-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0       96 2022-08-05 16:48:51.000000 wagtail-cache-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3870 2023-07-27 22:48:02.017834 wagtail-cache-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2988 2022-10-19 23:07:03.000000 wagtail-cache-2.3.0/README.md
+-rw-rw-rw-   0        0        0      532 2023-06-14 17:43:12.000000 wagtail-cache-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-07-27 22:48:02.017834 wagtail-cache-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.002213 wagtail-cache-2.3.0/wagtail_cache.egg-info/
+-rw-rw-rw-   0        0        0     3870 2023-07-27 22:48:01.000000 wagtail-cache-2.3.0/wagtail_cache.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-07-27 22:48:01.000000 wagtail-cache-2.3.0/wagtail_cache.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 22:48:01.000000 wagtail-cache-2.3.0/wagtail_cache.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 22:48:01.000000 wagtail-cache-2.3.0/wagtail_cache.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 22:48:01.000000 wagtail-cache-2.3.0/wagtail_cache.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.002213 wagtail-cache-2.3.0/wagtailcache/
+-rw-rw-rw-   0        0        0      157 2023-06-14 16:59:52.000000 wagtail-cache-2.3.0/wagtailcache/__init__.py
+-rw-rw-rw-   0        0        0      222 2022-08-05 16:48:51.000000 wagtail-cache-2.3.0/wagtailcache/apps.py
+-rw-rw-rw-   0        0        0    15825 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:01.986571 wagtail-cache-2.3.0/wagtailcache/management/
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.002213 wagtail-cache-2.3.0/wagtailcache/management/commands/
+-rw-rw-rw-   0        0        0      278 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/management/commands/clear_wagtail_cache.py
+-rw-rw-rw-   0        0        0     1369 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:01.986571 wagtail-cache-2.3.0/wagtailcache/templates/
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.017834 wagtail-cache-2.3.0/wagtailcache/templates/wagtailcache/
+-rw-rw-rw-   0        0        0     1757 2022-10-19 23:07:03.000000 wagtail-cache-2.3.0/wagtailcache/templates/wagtailcache/index.html
+-rw-rw-rw-   0        0        0      332 2022-10-19 23:07:03.000000 wagtail-cache-2.3.0/wagtailcache/templates/wagtailcache/wagtailcache-bolt.svg
+drwxrwxrwx   0        0        0        0 2023-07-27 22:48:02.017834 wagtail-cache-2.3.0/wagtailcache/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-08-05 16:48:51.000000 wagtail-cache-2.3.0/wagtailcache/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1580 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/templatetags/wagtailcache_tags.py
+-rw-rw-rw-   0        0        0      255 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/urls.py
+-rw-rw-rw-   0        0        0      919 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/views.py
+-rw-rw-rw-   0        0        0     1442 2023-06-14 17:43:17.000000 wagtail-cache-2.3.0/wagtailcache/wagtail_hooks.py
```

### Comparing `wagtail-cache-2.2.0/LICENSE` & `wagtail-cache-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cache-2.2.0/PKG-INFO` & `wagtail-cache-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: wagtail-cache
-Version: 2.2.0
+Version: 2.3.0
 Summary: A simple page cache for Wagtail based on the Django cache middleware.
 Home-page: https://github.com/coderedcorp/wagtail-cache
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD license
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Wagtail Cache
 =============
 
 A fast and simple page cache for Wagtail, inspired by the Django cache
@@ -79,9 +80,7 @@
 * Was sourced from the Fork Awesome project at
    https://github.com/ForkAwesome/Fork-Awesome.
 
 * Is licensed under the Creative Commons Attribution 3.0 Unported license,
    a copy of which is available at https://creativecommons.org/licenses/by/3.0/
 
 * Has been modified from the original sources.
-
-
```

### Comparing `wagtail-cache-2.2.0/README.md` & `wagtail-cache-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cache-2.2.0/setup.py` & `wagtail-cache-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
+
 from wagtailcache import __version__
 
+
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="wagtail-cache",
     version=__version__,
     author="CodeRed LLC",
@@ -12,20 +15,22 @@
     url="https://github.com/coderedcorp/wagtail-cache",
     description="A simple page cache for Wagtail based on the Django cache middleware.",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="BSD license",
     include_package_data=True,
     packages=find_packages(),
-    install_requires=["wagtail>=3.0,<5.0"],
+    install_requires=["wagtail>=3.0,<6"],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Framework :: Django",
         "Framework :: Wagtail",
         "Framework :: Wagtail :: 3",
+        "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
     ],
 )
```

### Comparing `wagtail-cache-2.2.0/wagtail_cache.egg-info/PKG-INFO` & `wagtail-cache-2.3.0/wagtail_cache.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: wagtail-cache
-Version: 2.2.0
+Version: 2.3.0
 Summary: A simple page cache for Wagtail based on the Django cache middleware.
 Home-page: https://github.com/coderedcorp/wagtail-cache
 Author: CodeRed LLC
 Author-email: info@coderedcorp.com
 License: BSD license
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Wagtail Cache
 =============
 
 A fast and simple page cache for Wagtail, inspired by the Django cache
@@ -79,9 +80,7 @@
 * Was sourced from the Fork Awesome project at
    https://github.com/ForkAwesome/Fork-Awesome.
 
 * Is licensed under the Creative Commons Attribution 3.0 Unported license,
    a copy of which is available at https://creativecommons.org/licenses/by/3.0/
 
 * Has been modified from the original sources.
-
-
```

### Comparing `wagtail-cache-2.2.0/wagtail_cache.egg-info/SOURCES.txt` & `wagtail-cache-2.3.0/wagtail_cache.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,12 @@
 wagtailcache/__init__.py
 wagtailcache/apps.py
 wagtailcache/cache.py
 wagtailcache/settings.py
 wagtailcache/urls.py
 wagtailcache/views.py
 wagtailcache/wagtail_hooks.py
-wagtailcache/compat_backends/__init__.py
-wagtailcache/compat_backends/django_redis.py
 wagtailcache/management/commands/clear_wagtail_cache.py
 wagtailcache/templates/wagtailcache/index.html
 wagtailcache/templates/wagtailcache/wagtailcache-bolt.svg
 wagtailcache/templatetags/__init__.py
 wagtailcache/templatetags/wagtailcache_tags.py
```

### Comparing `wagtail-cache-2.2.0/wagtailcache/cache.py` & `wagtail-cache-2.3.0/wagtailcache/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 Functionality to set, serve from, and clear the cache.
 """
 import re
 from enum import Enum
 from functools import wraps
-from typing import Callable, Optional, List
+from typing import Callable
+from typing import List
+from typing import Optional
 from urllib.parse import unquote
+
 from django.conf import settings
 from django.core.cache import caches
 from django.core.cache.backends.base import BaseCache
 from django.core.handlers.wsgi import WSGIRequest
 from django.http.response import HttpResponse
 from django.template.response import SimpleTemplateResponse
-from django.utils.cache import (
-    cc_delim_re,
-    get_cache_key,
-    get_max_age,
-    has_vary_header,
-    learn_cache_key,
-    patch_response_headers,
-)
+from django.utils.cache import cc_delim_re
+from django.utils.cache import get_cache_key
+from django.utils.cache import get_max_age
+from django.utils.cache import has_vary_header
+from django.utils.cache import learn_cache_key
+from django.utils.cache import patch_response_headers
 from django.utils.deprecation import MiddlewareMixin
 from wagtail import hooks
 
 from wagtailcache.settings import wagtailcache_settings
 
 
 class CacheControl(Enum):
@@ -180,50 +181,46 @@
         self._wagcache = caches[wagtailcache_settings.WAGTAIL_CACHE_BACKEND]
         self.get_response = get_response
         self._async_check()
 
     def process_request(self, request: WSGIRequest) -> Optional[HttpResponse]:
         if not wagtailcache_settings.WAGTAIL_CACHE:
             return None
-
         # Check if request is cacheable
         # Only cache GET and HEAD requests.
         # Don't cache requests that are previews.
         # Don't cache requests that have a logged in user.
         # NOTE: Wagtail manually adds `is_preview` to the request object.
         #       This is not normally part of a request object.
         is_cacheable = (
             request.method in ("GET", "HEAD")
             and not getattr(request, "is_preview", False)
             and not (hasattr(request, "user") and request.user.is_authenticated)
         )
-
         # Allow the user to override our caching decision.
         for fn in hooks.get_hooks("is_request_cacheable"):
             result = fn(request, is_cacheable)
             if isinstance(result, bool):
                 is_cacheable = result
 
         if not is_cacheable:
             setattr(request, "_wagtailcache_update", False)
             setattr(request, "_wagtailcache_skip", True)
             return None  # Don't bother checking the cache.
-
         # Try and get the cached response.
         cache_key = _get_cache_key(request, self._wagcache)
         if cache_key is None:
             setattr(request, "_wagtailcache_update", True)
             return None  # No cache information available, need to rebuild.
 
         response = self._wagcache.get(cache_key)
 
         if response is None:
             setattr(request, "_wagtailcache_update", True)
             return None  # No cache information available, need to rebuild.
-
         # Hit. Return cached response.
         setattr(request, "_wagtailcache_update", False)
         return response
 
 
 class UpdateCacheMiddleware(MiddlewareMixin):
     """
@@ -256,15 +253,14 @@
         ):
             # Add a response header to indicate this was a cache hit.
             _patch_header(response, Status.HIT)
             # Potentially remove the ``Vary: Cookie`` header.
             _chop_response_vary(request, response)
             # We don't need to update the cache, just return.
             return response
-
         # Check if the response is cacheable
         # Don't cache private or no-cache responses.
         # Do cache 200, 301, 302, 304, and 404 codes so that wagtail doesn't
         #   have to repeatedly look up these URLs in the database.
         # Don't cache streaming responses.
         # Don't cache responses that set a user-specific cookie in response
         #   to a cookie-less request (e.g. CSRF tokens).
@@ -276,102 +272,94 @@
             and not response.streaming
             and not (
                 not request.COOKIES
                 and response.cookies
                 and has_vary_header(response, "Cookie")
             )
         )
-
         # Allow the user to override our caching decision.
         for fn in hooks.get_hooks("is_response_cacheable"):
             result = fn(response, is_cacheable)
             if isinstance(result, bool):
                 is_cacheable = result
-
         # If we are not allowed to cache the response, just return.
         if not is_cacheable:
             # Add response header to indicate this was intentionally not cached.
             _patch_header(response, Status.SKIP)
             return response
-
         # Potentially remove the ``Vary: Cookie`` header.
         _chop_response_vary(request, response)
-
         # Try to get the timeout from the ``max-age`` section of the
         # ``Cache-Control`` header before reverting to using the cache's
         # default.
         timeout = get_max_age(response)
         if timeout is None:
             timeout = self._wagcache.default_timeout
         patch_response_headers(response, timeout)
         if timeout:
             cache_key = _learn_cache_key(
                 request, response, timeout, self._wagcache
             )
-
             # Track cache keys based on URI.
             # (of the chopped request, not the real one).
             cr = _chop_querystring(request)
             uri = unquote(cr.build_absolute_uri())
             keyring = self._wagcache.get("keyring", {})
             # Get current cache keys belonging to this URI.
             # This should be a list of keys.
             uri_keys: List[str] = keyring.get(uri, [])
             # Append the key to this list and save.
             uri_keys.append(cache_key)
             keyring[uri] = uri_keys
             self._wagcache.set("keyring", keyring)
 
             if isinstance(response, SimpleTemplateResponse):
-                response.add_post_render_callback(
-                    lambda r: self._wagcache.set(cache_key, r, timeout)
-                )
+
+                def callback(r):
+                    self._wagcache.set(cache_key, r, timeout)
+
+                response.add_post_render_callback(callback)
             else:
                 self._wagcache.set(cache_key, response, timeout)
-
             # Add a response header to indicate this was a cache miss.
             _patch_header(response, Status.MISS)
 
         return response
 
 
-def clear_cache(urls: List[str] = None) -> None:
+def clear_cache(urls: List[str] = []) -> None:
     """
     Clears the Wagtail cache backend.
 
     :param urls: An optional list of strings, representing regular expressions
     to match against the list of URLs in the cache. If a URL matches, it is
     deleted from the cache. If ``urls`` is ``None`` the entire cache is cleared.
     """
 
     if not wagtailcache_settings.WAGTAIL_CACHE:
         return
 
     _wagcache = caches[wagtailcache_settings.WAGTAIL_CACHE_BACKEND]
     if urls and "keyring" in _wagcache:
         keyring = _wagcache.get("keyring")
-
         # Check the provided URL matches a key in our keyring.
         matched_urls = []
         for regex in urls:
             for key in keyring:
                 if re.match(regex, key):
                     matched_urls.append(key)
-
         # If it matches, delete each entry from the cache,
         # and delete the URL from the keyring.
         for url in matched_urls:
             entries = keyring.get(url, [])
             for cache_key in entries:
                 _wagcache.delete(cache_key)
             del keyring[url]
-
         # Save the keyring.
         _wagcache.set("keyring", keyring)
-
     # Clears the entire cache backend used by wagtail-cache.
     else:
         _wagcache.clear()
 
 
 def cache_page(view_func: Callable[..., HttpResponse]):
     """
@@ -420,27 +408,27 @@
     Add cache-control headers to various Page responses that could be returned.
     """
 
     def serve_password_required_response(self, request, form, action_url):
         """
         Add a cache-control header if the page requires a password.
         """
-        response = super().serve_password_required_response(
+        response = super().serve_password_required_response(  # type: ignore
             request, form, action_url
         )
         response["Cache-Control"] = CacheControl.PRIVATE.value
         return response
 
     def serve(self, request, *args, **kwargs):
         """
         Add a custom cache-control header, or set to private if the page is
         being served behind a view restriction.
         """
-        response = super().serve(request, *args, **kwargs)
-        if self.get_view_restrictions():
+        response = super().serve(request, *args, **kwargs)  # type: ignore
+        if self.get_view_restrictions():  # type: ignore
             response["Cache-Control"] = CacheControl.PRIVATE.value
         elif hasattr(self, "cache_control"):
             if callable(self.cache_control):
                 response["Cache-Control"] = self.cache_control()
             else:
                 response["Cache-Control"] = self.cache_control
         return response
```

### Comparing `wagtail-cache-2.2.0/wagtailcache/settings.py` & `wagtail-cache-2.3.0/wagtailcache/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Default django settings for wagtail-cache.
 """
-
 from typing import Text
+
 from django.conf import settings
 
 
 class _DefaultSettings:
-
     WAGTAIL_CACHE = True
     WAGTAIL_CACHE_BACKEND = "default"
     WAGTAIL_CACHE_HEADER = "X-Wagtail-Cache"
     WAGTAIL_CACHE_IGNORE_COOKIES = True
     WAGTAIL_CACHE_IGNORE_QS = [
         r"^_bta_.*$",  # Bronto
         r"^_ga$",  # Google Analytics
```

### Comparing `wagtail-cache-2.2.0/wagtailcache/templates/wagtailcache/index.html` & `wagtail-cache-2.3.0/wagtailcache/templates/wagtailcache/index.html`

 * *Files identical despite different names*

### Comparing `wagtail-cache-2.2.0/wagtailcache/templatetags/wagtailcache_tags.py` & `wagtail-cache-2.3.0/wagtailcache/templatetags/wagtailcache_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional
+
 from django import template
 from django.core.cache import caches
 from django.utils.translation import gettext_lazy as _
+
 from wagtailcache.settings import wagtailcache_settings
 
 
 register = template.Library()
 
 
 def seconds_to_readable(seconds: int) -> str:
```

### Comparing `wagtail-cache-2.2.0/wagtailcache/views.py` & `wagtail-cache-2.3.0/wagtailcache/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Views for the wagtail admin dashboard.
 """
-from typing import Dict, List
+from typing import Dict
+from typing import List
 
 from django.core.cache import caches
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.urls import reverse
 
 from wagtailcache.cache import clear_cache
```

### Comparing `wagtail-cache-2.2.0/wagtailcache/wagtail_hooks.py` & `wagtail-cache-2.3.0/wagtailcache/wagtail_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Registers wagtail-cache in the wagtail admin dashboard.
 """
-
-from django.urls import include, path, reverse
+from django.urls import include
+from django.urls import path
+from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
-from wagtail.admin.menu import MenuItem
 from wagtail import hooks
+from wagtail.admin.menu import MenuItem
 
 from wagtailcache import urls
 
 
 class CacheMenuItem(MenuItem):
     """
     Registers wagtail-cache in wagtail admin for superusers.
```

