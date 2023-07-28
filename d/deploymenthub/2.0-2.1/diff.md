# Comparing `tmp/deploymenthub-2.0.tar.gz` & `tmp/deploymenthub-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-2.0.tar", last modified: Fri Jul 28 18:21:17 2023, max compression
+gzip compressed data, was "deploymenthub-2.1.tar", last modified: Fri Jul 28 18:23:39 2023, max compression
```

## Comparing `deploymenthub-2.0.tar` & `deploymenthub-2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:21:17.051112 deploymenthub-2.0/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.0/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:21:17.050999 deploymenthub-2.0/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.0/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:21:17.050254 deploymenthub-2.0/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1341 2023-07-28 18:02:16.000000 deploymenthub-2.0/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:21:17.050839 deploymenthub-2.0/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:21:17.000000 deploymenthub-2.0/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-28 18:21:17.000000 deploymenthub-2.0/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:21:17.000000 deploymenthub-2.0/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:21:17.000000 deploymenthub-2.0/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-28 18:21:17.051146 deploymenthub-2.0/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-28 18:21:15.000000 deploymenthub-2.0/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.567682 deploymenthub-2.1/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-2.1/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:23:39.567565 deploymenthub-2.1/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-2.1/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.566928 deploymenthub-2.1/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1313 2023-07-28 18:22:59.000000 deploymenthub-2.1/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-28 18:23:39.567386 deploymenthub-2.1/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-28 18:23:39.000000 deploymenthub-2.1/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-28 18:23:39.567715 deploymenthub-2.1/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      685 2023-07-28 18:22:59.000000 deploymenthub-2.1/setup.py
```

### Comparing `deploymenthub-2.0/LICENSE.txt` & `deploymenthub-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-2.0/bin/deploymenthub` & `deploymenthub-2.1/bin/deploymenthub`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
             command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
 
         command_list = json.loads(os.popen(command).read())
 
-        print(command_list)
         for command in command_list:
             print(command)
 
     else:
         print("Project does not exist!")
```

### Comparing `deploymenthub-2.0/setup.py` & `deploymenthub-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version="2.0",
+    version="2.1",
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```

