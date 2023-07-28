# Comparing `tmp/django-feed-reader-1.0.5.tar.gz` & `tmp/django-feed-reader-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-feed-reader-1.0.5.tar", last modified: Mon Feb 20 01:36:53 2023, max compression
+gzip compressed data, was "django-feed-reader-1.0.6.tar", last modified: Fri Jul 28 05:50:28 2023, max compression
```

## Comparing `django-feed-reader-1.0.5.tar` & `django-feed-reader-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.430980 django-feed-reader-1.0.5/
--rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-1.0.5/LICENSE
--rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-1.0.5/MANIFEST.in
--rw-r--r--   0 g          (501) staff       (20)     4513 2023-02-20 01:36:53.431030 django-feed-reader-1.0.5/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)     4074 2023-01-28 17:47:47.000000 django-feed-reader-1.0.5/README.md
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.427975 django-feed-reader-1.0.5/django_feed_reader.egg-info/
--rw-r--r--   0 g          (501) staff       (20)     4513 2023-02-20 01:36:53.000000 django-feed-reader-1.0.5/django_feed_reader.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)      933 2023-02-20 01:36:53.000000 django-feed-reader-1.0.5/django_feed_reader.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2023-02-20 01:36:53.000000 django-feed-reader-1.0.5/django_feed_reader.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)       74 2023-02-20 01:36:53.000000 django-feed-reader-1.0.5/django_feed_reader.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        6 2023-02-20 01:36:53.000000 django-feed-reader-1.0.5/django_feed_reader.egg-info/top_level.txt
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.429187 django-feed-reader-1.0.5/feeds/
--rw-r--r--   0 g          (501) staff       (20)      454 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1520 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/admin.py
--rw-r--r--   0 g          (501) staff       (20)      139 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/apps.py
--rw-r--r--   0 g          (501) staff       (20)       17 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/cloudflare.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.429322 django-feed-reader-1.0.5/feeds/management/
--rw-r--r--   0 g          (501) staff       (20)        1 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/management/__init__.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.429571 django-feed-reader-1.0.5/feeds/management/commands/
--rw-r--r--   0 g          (501) staff       (20)        1 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/management/commands/__init__.py
--rw-r--r--   0 g          (501) staff       (20)      310 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/management/commands/refreshfeeds.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2023-02-20 01:36:53.430884 django-feed-reader-1.0.5/feeds/migrations/
--rw-r--r--   0 g          (501) staff       (20)     3384 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0001_initial.py
--rw-r--r--   0 g          (501) staff       (20)      395 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0002_auto_20190604_0845.py
--rw-r--r--   0 g          (501) staff       (20)      407 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0003_post_image_url.py
--rw-r--r--   0 g          (501) staff       (20)      513 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0004_webproxy.py
--rw-r--r--   0 g          (501) staff       (20)      385 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0005_source_description.py
--rw-r--r--   0 g          (501) staff       (20)      921 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0006_auto_20190901_1644.py
--rw-r--r--   0 g          (501) staff       (20)     1098 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0007_auto_20210502_0716.py
--rw-r--r--   0 g          (501) staff       (20)      419 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0008_allow_longer_post_guid.py
--rw-r--r--   0 g          (501) staff       (20)      576 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
--rw-r--r--   0 g          (501) staff       (20)        0 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/migrations/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     6180 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/models.py
--rw-r--r--   0 g          (501) staff       (20)    16817 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/tests.py
--rw-r--r--   0 g          (501) staff       (20)    32728 2023-02-20 01:36:33.000000 django-feed-reader-1.0.5/feeds/utils.py
--rw-r--r--   0 g          (501) staff       (20)       63 2023-02-17 10:11:46.000000 django-feed-reader-1.0.5/feeds/views.py
--rw-r--r--   0 g          (501) staff       (20)       38 2023-02-20 01:36:53.431193 django-feed-reader-1.0.5/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      869 2023-02-20 01:36:33.000000 django-feed-reader-1.0.5/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.962802 django-feed-reader-1.0.6/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)       87 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/MANIFEST.in
+-rw-r--r--   0 g          (501) staff       (20)     4513 2023-07-28 05:50:28.962852 django-feed-reader-1.0.6/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     4074 2023-01-28 17:47:47.000000 django-feed-reader-1.0.6/README.md
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.960308 django-feed-reader-1.0.6/django_feed_reader.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)     4513 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)      997 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)       74 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        6 2023-07-28 05:50:28.000000 django-feed-reader-1.0.6/django_feed_reader.egg-info/top_level.txt
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961192 django-feed-reader-1.0.6/feeds/
+-rw-r--r--   0 g          (501) staff       (20)      454 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     1520 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/admin.py
+-rw-r--r--   0 g          (501) staff       (20)      139 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/apps.py
+-rw-r--r--   0 g          (501) staff       (20)       17 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/cloudflare.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961309 django-feed-reader-1.0.6/feeds/management/
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/__init__.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.961510 django-feed-reader-1.0.6/feeds/management/commands/
+-rw-r--r--   0 g          (501) staff       (20)        1 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/commands/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)      310 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/management/commands/refreshfeeds.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2023-07-28 05:50:28.962725 django-feed-reader-1.0.6/feeds/migrations/
+-rw-r--r--   0 g          (501) staff       (20)     3384 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0001_initial.py
+-rw-r--r--   0 g          (501) staff       (20)      395 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0002_auto_20190604_0845.py
+-rw-r--r--   0 g          (501) staff       (20)      407 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0003_post_image_url.py
+-rw-r--r--   0 g          (501) staff       (20)      513 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0004_webproxy.py
+-rw-r--r--   0 g          (501) staff       (20)      385 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0005_source_description.py
+-rw-r--r--   0 g          (501) staff       (20)      921 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0006_auto_20190901_1644.py
+-rw-r--r--   0 g          (501) staff       (20)     1098 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0007_auto_20210502_0716.py
+-rw-r--r--   0 g          (501) staff       (20)      419 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0008_allow_longer_post_guid.py
+-rw-r--r--   0 g          (501) staff       (20)      576 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+-rw-r--r--   0 g          (501) staff       (20)      626 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/migrations/0010_enclosure_description_enclosure_medium.py
+-rw-r--r--   0 g          (501) staff       (20)        0 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/migrations/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     6322 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/models.py
+-rw-r--r--   0 g          (501) staff       (20)    16817 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/tests.py
+-rw-r--r--   0 g          (501) staff       (20)    33338 2023-07-28 05:42:06.000000 django-feed-reader-1.0.6/feeds/utils.py
+-rw-r--r--   0 g          (501) staff       (20)       63 2023-07-27 22:04:19.000000 django-feed-reader-1.0.6/feeds/views.py
+-rw-r--r--   0 g          (501) staff       (20)       38 2023-07-28 05:50:28.962999 django-feed-reader-1.0.6/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      869 2023-07-28 05:45:12.000000 django-feed-reader-1.0.6/setup.py
```

### Comparing `django-feed-reader-1.0.5/LICENSE` & `django-feed-reader-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/PKG-INFO` & `django-feed-reader-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 1.0.5
+Version: 1.0.6
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-feed-reader-1.0.5/README.md` & `django-feed-reader-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/django_feed_reader.egg-info/PKG-INFO` & `django-feed-reader-1.0.6/django_feed_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feed-reader
-Version: 1.0.5
+Version: 1.0.6
 Summary: An RSS feed reading library for Django.
 Home-page: https://github.com/xurble/django-feed-reader
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-feed-reader-1.0.5/django_feed_reader.egg-info/SOURCES.txt` & `django-feed-reader-1.0.6/django_feed_reader.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 feeds/migrations/0003_post_image_url.py
 feeds/migrations/0004_webproxy.py
 feeds/migrations/0005_source_description.py
 feeds/migrations/0006_auto_20190901_1644.py
 feeds/migrations/0007_auto_20210502_0716.py
 feeds/migrations/0008_allow_longer_post_guid.py
 feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py
+feeds/migrations/0010_enclosure_description_enclosure_medium.py
 feeds/migrations/__init__.py
```

### Comparing `django-feed-reader-1.0.5/feeds/admin.py` & `django-feed-reader-1.0.6/feeds/admin.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/migrations/0001_initial.py` & `django-feed-reader-1.0.6/feeds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/migrations/0004_webproxy.py` & `django-feed-reader-1.0.6/feeds/migrations/0004_webproxy.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/migrations/0006_auto_20190901_1644.py` & `django-feed-reader-1.0.6/feeds/migrations/0006_auto_20190901_1644.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/migrations/0007_auto_20210502_0716.py` & `django-feed-reader-1.0.6/feeds/migrations/0007_auto_20210502_0716.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py` & `django-feed-reader-1.0.6/feeds/migrations/0009_allow_source_last_change_and_last_success_to_be_blank.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/models.py` & `django-feed-reader-1.0.6/feeds/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,17 @@
         ordering = ["index"]
         
 class Enclosure(models.Model):
 
     post   = models.ForeignKey(Post, on_delete=models.CASCADE, related_name='enclosures')
     length = models.IntegerField(default=0)
     href   = models.CharField(max_length=512)
-    type   = models.CharField(max_length=256) 
+    type   = models.CharField(max_length=256)
+    medium = models.CharField(max_length=25, null=True, blank=True)
+    description = models.CharField(max_length=512, null= True, blank=True)
     
     @property
     def recast_link(self):
     
         # TODO: This needs to come out, it's just for recast
 
         #if "?" in self.href:
```

### Comparing `django-feed-reader-1.0.5/feeds/tests.py` & `django-feed-reader-1.0.6/feeds/tests.py`

 * *Files identical despite different names*

### Comparing `django-feed-reader-1.0.5/feeds/utils.py` & `django-feed-reader-1.0.6/feeds/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -605,28 +605,37 @@
                             href = "url"
 
                         length = "length"
                         if length not in pe:
                             length = "filesize"
                     
                     
-                        if pe["href"] == ee.href and ee.href not in seen_files:
+                        if pe[href] == ee.href and ee.href not in seen_files:
                             found_enclosure = True
                         
                             try:
                                 ee.length = int(pe[length])
                             except:
                                 ee.length = 0
 
                             try:
                                 type = pe["type"]
                             except:
                                 type = "audio/mpeg"  # we are assuming podcasts here but that's probably not safe
 
                             ee.type = type
+
+                            
+                            if "medium" in pe:
+                                ee.medium = pe["medium"]
+                            
+                            if "description" in pe:
+                                ee.description = pe["description"][:512]
+                                
+                            
                             ee.save()
                             break
                     if not found_enclosure:
                         ee.delete()
                     seen_files.append(ee.href)
     
                 for pe in post_files:
@@ -649,14 +658,23 @@
                             
                             try:
                                 type = pe["type"]
                             except:
                                 type = "audio/mpeg"
                     
                             ee = Enclosure(post=p, href=pe[href], length=length, type=type)
+
+                            if "medium" in pe:
+                                ee.medium = pe["medium"]
+                            
+                            if "description" in pe:
+                                ee.description = pe["description"][:512]
+
+
+
                             ee.save()
                     except Exception as ex:
                         pass
             except Exception as ex:
                 if output:
                     output.write("No enclosures - " + str(ex))
```

### Comparing `django-feed-reader-1.0.5/setup.py` & `django-feed-reader-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('readme.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='django-feed-reader',
-    version='1.0.5',
+    version='1.0.6',
     description='An RSS feed reading library for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/django-feed-reader',
     license='MIT',
```

