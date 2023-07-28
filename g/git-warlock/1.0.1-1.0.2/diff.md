# Comparing `tmp/git-warlock-1.0.1.tar.gz` & `tmp/git-warlock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-warlock-1.0.1.tar", last modified: Fri Jul 28 14:13:24 2023, max compression
+gzip compressed data, was "git-warlock-1.0.2.tar", last modified: Fri Jul 28 14:18:11 2023, max compression
```

## Comparing `git-warlock-1.0.1.tar` & `git-warlock-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:13:24.345957 git-warlock-1.0.1/
--rw-r--r--   0 willy      (501) staff       (20)      136 2023-07-28 14:13:24.345802 git-warlock-1.0.1/PKG-INFO
--rw-r--r--   0 willy      (501) staff       (20)     2680 2023-07-28 13:50:24.000000 git-warlock-1.0.1/README.md
-drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:13:24.344585 git-warlock-1.0.1/git_warlock/
--rw-r--r--   0 willy      (501) staff       (20)        0 2023-07-28 13:28:29.000000 git-warlock-1.0.1/git_warlock/__init__.py
--rwxr-xr-x   0 willy      (501) staff       (20)     3618 2023-07-28 13:29:23.000000 git-warlock-1.0.1/git_warlock/git-warlock.py
--rw-r--r--   0 willy      (501) staff       (20)     3994 2023-07-28 13:33:23.000000 git-warlock-1.0.1/git_warlock/git_warlock.py
--rw-r--r--   0 willy      (501) staff       (20)     3994 2023-07-28 14:09:34.000000 git-warlock-1.0.1/git_warlock/main.py
-drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:13:24.345586 git-warlock-1.0.1/git_warlock.egg-info/
--rw-r--r--   0 willy      (501) staff       (20)      136 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/PKG-INFO
--rw-r--r--   0 willy      (501) staff       (20)      328 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/SOURCES.txt
--rw-r--r--   0 willy      (501) staff       (20)        1 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/dependency_links.txt
--rw-r--r--   0 willy      (501) staff       (20)       54 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/entry_points.txt
--rw-r--r--   0 willy      (501) staff       (20)        5 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/requires.txt
--rw-r--r--   0 willy      (501) staff       (20)       12 2023-07-28 14:13:24.000000 git-warlock-1.0.1/git_warlock.egg-info/top_level.txt
--rw-r--r--   0 willy      (501) staff       (20)       38 2023-07-28 14:13:24.346001 git-warlock-1.0.1/setup.cfg
--rw-r--r--   0 willy      (501) staff       (20)      425 2023-07-28 14:12:39.000000 git-warlock-1.0.1/setup.py
+drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:18:11.977895 git-warlock-1.0.2/
+-rw-r--r--   0 willy      (501) staff       (20)      136 2023-07-28 14:18:11.977719 git-warlock-1.0.2/PKG-INFO
+-rw-r--r--   0 willy      (501) staff       (20)     2680 2023-07-28 13:50:24.000000 git-warlock-1.0.2/README.md
+drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:18:11.976523 git-warlock-1.0.2/git_warlock/
+-rw-r--r--   0 willy      (501) staff       (20)        0 2023-07-28 13:28:29.000000 git-warlock-1.0.2/git_warlock/__init__.py
+-rwxr-xr-x   0 willy      (501) staff       (20)     3618 2023-07-28 13:29:23.000000 git-warlock-1.0.2/git_warlock/git-warlock.py
+-rw-r--r--   0 willy      (501) staff       (20)     3994 2023-07-28 14:09:34.000000 git-warlock-1.0.2/git_warlock/main.py
+drwxr-xr-x   0 willy      (501) staff       (20)        0 2023-07-28 14:18:11.977503 git-warlock-1.0.2/git_warlock.egg-info/
+-rw-r--r--   0 willy      (501) staff       (20)      136 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/PKG-INFO
+-rw-r--r--   0 willy      (501) staff       (20)      301 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/SOURCES.txt
+-rw-r--r--   0 willy      (501) staff       (20)        1 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/dependency_links.txt
+-rw-r--r--   0 willy      (501) staff       (20)       54 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/entry_points.txt
+-rw-r--r--   0 willy      (501) staff       (20)        5 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/requires.txt
+-rw-r--r--   0 willy      (501) staff       (20)       12 2023-07-28 14:18:11.000000 git-warlock-1.0.2/git_warlock.egg-info/top_level.txt
+-rw-r--r--   0 willy      (501) staff       (20)       38 2023-07-28 14:18:11.977943 git-warlock-1.0.2/setup.cfg
+-rw-r--r--   0 willy      (501) staff       (20)      425 2023-07-28 14:16:33.000000 git-warlock-1.0.2/setup.py
```

### Comparing `git-warlock-1.0.1/README.md` & `git-warlock-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `git-warlock-1.0.1/git_warlock/git-warlock.py` & `git-warlock-1.0.2/git_warlock/git-warlock.py`

 * *Files identical despite different names*

### Comparing `git-warlock-1.0.1/git_warlock/git_warlock.py` & `git-warlock-1.0.2/git_warlock/main.py`

 * *Files identical despite different names*

