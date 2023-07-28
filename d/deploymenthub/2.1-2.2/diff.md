# Comparing `tmp/deploymenthub-2.1.tar.gz` & `tmp/deploymenthub-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.1.tar", last modified: Fri Jul 28 18:23:39 2023, max compression
+gzip compressed data, was "deploymenthub-2.2.tar", last modified: Fri Jul 28 18:38:39 2023, max compression
```

## Comparing `deploymenthub-2.1.tar` & `deploymenthub-2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.567682 deploymenthub-2.1/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.1/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:23:39.567565 deploymenthub-2.1/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.1/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.566928 deploymenthub-2.1/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1313 2023-07-28 18:22:59.000000 deploymenthub-2.1/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.567386 deploymenthub-2.1/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-28 18:23:39.567715 deploymenthub-2.1/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-28 18:22:59.000000 deploymenthub-2.1/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.422835 deploymenthub-2.2/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.2/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:38:39.422712 deploymenthub-2.2/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.2/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.421990 deploymenthub-2.2/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1313 2023-07-28 18:35:59.000000 deploymenthub-2.2/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:38:39.422552 deploymenthub-2.2/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:38:39.000000 deploymenthub-2.2/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-28 18:38:39.422874 deploymenthub-2.2/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-28 18:38:27.000000 deploymenthub-2.2/setup.py
```

### Comparing `deploymenthub-2.1/LICENSE.txt` & `deploymenthub-2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.1/bin/deploymenthub` & `deploymenthub-2.2/bin/deploymenthub`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.1/setup.py` & `deploymenthub-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.1",
+    version="2.2",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

