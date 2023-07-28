# Comparing `tmp/django-migration-rollback-1.0.4.tar.gz` & `tmp/django-migration-rollback-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-migration-rollback-1.0.4.tar", last modified: Wed Feb 15 02:11:04 2023, max compression
+gzip compressed data, was "django-migration-rollback-1.0.5.tar", last modified: Fri Jul 28 02:50:49 2023, max compression
```

## Comparing `django-migration-rollback-1.0.4.tar` & `django-migration-rollback-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.708413 django-migration-rollback-1.0.4/
--rw-r--r--   0 jeffreyb   (501) staff       (20)     1064 2022-07-27 00:23:28.000000 django-migration-rollback-1.0.4/LICENSE
--rw-r--r--   0 jeffreyb   (501) staff       (20)       84 2022-09-16 01:14:15.000000 django-migration-rollback-1.0.4/MANIFEST.in
--rw-r--r--   0 jeffreyb   (501) staff       (20)     4148 2023-02-15 02:11:04.708482 django-migration-rollback-1.0.4/PKG-INFO
--rw-r--r--   0 jeffreyb   (501) staff       (20)     2955 2023-02-15 02:04:07.000000 django-migration-rollback-1.0.4/README.md
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.707327 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/
--rw-r--r--   0 jeffreyb   (501) staff       (20)     4148 2023-02-15 02:11:04.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/PKG-INFO
--rw-r--r--   0 jeffreyb   (501) staff       (20)      720 2023-02-15 02:11:04.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreyb   (501) staff       (20)        1 2023-02-15 02:11:04.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreyb   (501) staff       (20)        1 2022-09-17 00:57:09.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/not-zip-safe
--rw-r--r--   0 jeffreyb   (501) staff       (20)       15 2023-02-15 02:11:04.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/requires.txt
--rw-r--r--   0 jeffreyb   (501) staff       (20)       19 2023-02-15 02:11:04.000000 django-migration-rollback-1.0.4/django_migration_rollback.egg-info/top_level.txt
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.707595 django-migration-rollback-1.0.4/migration_rollback/
--rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 00:43:00.000000 django-migration-rollback-1.0.4/migration_rollback/__init__.py
--rw-r--r--   0 jeffreyb   (501) staff       (20)      110 2022-09-15 01:15:53.000000 django-migration-rollback-1.0.4/migration_rollback/apps.py
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.707724 django-migration-rollback-1.0.4/migration_rollback/management/
--rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 01:00:29.000000 django-migration-rollback-1.0.4/migration_rollback/management/__init__.py
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.708063 django-migration-rollback-1.0.4/migration_rollback/management/commands/
--rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 01:00:36.000000 django-migration-rollback-1.0.4/migration_rollback/management/commands/__init__.py
--rw-r--r--   0 jeffreyb   (501) staff       (20)     1012 2022-09-23 01:12:32.000000 django-migration-rollback-1.0.4/migration_rollback/management/commands/migrateprevious.py
--rw-r--r--   0 jeffreyb   (501) staff       (20)     1310 2022-09-17 00:54:09.000000 django-migration-rollback-1.0.4/migration_rollback/management/commands/migraterollback.py
-drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-02-15 02:11:04.708299 django-migration-rollback-1.0.4/migration_rollback/utils/
--rw-r--r--   0 jeffreyb   (501) staff       (20)       61 2022-09-15 01:15:53.000000 django-migration-rollback-1.0.4/migration_rollback/utils/__init__.py
--rw-r--r--   0 jeffreyb   (501) staff       (20)     1398 2023-02-15 02:03:57.000000 django-migration-rollback-1.0.4/migration_rollback/utils/migration_utils.py
--rw-r--r--   0 jeffreyb   (501) staff       (20)      541 2023-02-15 02:04:07.000000 django-migration-rollback-1.0.4/pyproject.toml
--rw-r--r--   0 jeffreyb   (501) staff       (20)       15 2022-09-23 01:13:10.000000 django-migration-rollback-1.0.4/requirements.txt
--rw-r--r--   0 jeffreyb   (501) staff       (20)       79 2023-02-15 02:11:04.708694 django-migration-rollback-1.0.4/setup.cfg
--rw-r--r--   0 jeffreyb   (501) staff       (20)     1777 2023-02-15 02:04:07.000000 django-migration-rollback-1.0.4/setup.py
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.776877 django-migration-rollback-1.0.5/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     1064 2022-07-27 00:23:28.000000 django-migration-rollback-1.0.5/LICENSE
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       84 2022-09-16 01:14:15.000000 django-migration-rollback-1.0.5/MANIFEST.in
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     4152 2023-07-28 02:50:49.776998 django-migration-rollback-1.0.5/PKG-INFO
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     2957 2023-07-28 02:29:24.000000 django-migration-rollback-1.0.5/README.md
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.775539 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     4152 2023-07-28 02:50:49.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreyb   (501) staff       (20)      720 2023-07-28 02:50:49.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreyb   (501) staff       (20)        1 2023-07-28 02:50:49.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreyb   (501) staff       (20)        1 2022-09-17 00:57:09.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/not-zip-safe
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       15 2023-07-28 02:50:49.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/requires.txt
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       19 2023-07-28 02:50:49.000000 django-migration-rollback-1.0.5/django_migration_rollback.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.775796 django-migration-rollback-1.0.5/migration_rollback/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 00:43:00.000000 django-migration-rollback-1.0.5/migration_rollback/__init__.py
+-rw-r--r--   0 jeffreyb   (501) staff       (20)      110 2022-09-15 01:15:53.000000 django-migration-rollback-1.0.5/migration_rollback/apps.py
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.776024 django-migration-rollback-1.0.5/migration_rollback/management/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 01:00:29.000000 django-migration-rollback-1.0.5/migration_rollback/management/__init__.py
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.776388 django-migration-rollback-1.0.5/migration_rollback/management/commands/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)        0 2022-07-27 01:00:36.000000 django-migration-rollback-1.0.5/migration_rollback/management/commands/__init__.py
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     1012 2022-09-23 01:12:32.000000 django-migration-rollback-1.0.5/migration_rollback/management/commands/migrateprevious.py
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     1310 2022-09-17 00:54:09.000000 django-migration-rollback-1.0.5/migration_rollback/management/commands/migraterollback.py
+drwxr-xr-x   0 jeffreyb   (501) staff       (20)        0 2023-07-28 02:50:49.776627 django-migration-rollback-1.0.5/migration_rollback/utils/
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       61 2022-09-15 01:15:53.000000 django-migration-rollback-1.0.5/migration_rollback/utils/__init__.py
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     1410 2023-07-28 02:43:50.000000 django-migration-rollback-1.0.5/migration_rollback/utils/migration_utils.py
+-rw-r--r--   0 jeffreyb   (501) staff       (20)      541 2023-07-28 02:27:17.000000 django-migration-rollback-1.0.5/pyproject.toml
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       15 2022-09-23 01:13:10.000000 django-migration-rollback-1.0.5/requirements.txt
+-rw-r--r--   0 jeffreyb   (501) staff       (20)       79 2023-07-28 02:50:49.777488 django-migration-rollback-1.0.5/setup.cfg
+-rw-r--r--   0 jeffreyb   (501) staff       (20)     1777 2023-07-28 02:27:17.000000 django-migration-rollback-1.0.5/setup.py
```

### Comparing `django-migration-rollback-1.0.4/LICENSE` & `django-migration-rollback-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-migration-rollback-1.0.4/PKG-INFO` & `django-migration-rollback-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-migration-rollback
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple Django app to be able to migrate back to a previous migration or to migrate back to a migration in a specific branch in a git repository or locally.
 Home-page: https://github.com/jdboisvert/django-migration-rollback
-Download-URL: https://github.com/jdboisvert/django-migration-rollback/archive/refs/tags/v1.0.4.zip
 Author: Jeffrey Boisvert
 Author-email: info.jeffreyboisvert@gmail.com
 License: MIT License
+Download-URL: https://github.com/jdboisvert/django-migration-rollback/archive/refs/tags/v1.0.5.zip
 Project-URL: Repository, https://github.com/jdboisvert/django-migration-rollback
 Project-URL: Bug Reports, https://github.com/jdboisvert/django-migration-rollback/issues
 Keywords: django,migration,rollback,git
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Django Migration Rollback v1.0.4
+# Django Migration Rollback v1.0.5
 A Django package used to just make the `python manage.py migrate` a little easier for Django apps that commit their migrations and want a way to rollback to a previous migration without needing to check what the which one it is via `python manage.py showmigrations` or in the project's git repository.
 
 ## Features
 Able to set which branch in a git repository to rollback to using the custom command `migraterollback` or if you wish to just rollback to a previous migration only via `migrateprevious`. Note in order to use the rollback with a git repository's branch feature with git the project must have a `.git` file present.
 
 ### Django `migraterollback` command
     ❯ python manage.py migraterollback polls feature/really-cool-branch
@@ -91,20 +91,22 @@
 eval "$(pyenv init --path)"
 eval "$(pyenv init -)"
 eval "$(pyenv virtualenv-init -)"
 """ > ~/.zshrc
 source ~/.zshrc
 
 # create a virtualenv
-pyenv install 1.0.4
-pyenv virtualenv 1.0.4 django_migration_rollback
+pyenv install 3.10.5
+pyenv virtualenv 3.10.5 django_migration_rollback
 pyenv activate django_migration_rollback
 
 # install dependencies
 pip install -U pip
 pip install -r requirements.txt -r requirements_dev.txt
 ```
 
 ## Installing pre-commit hooks
 ```bash
 pre-commit install
 ```
+
+
```

### Comparing `django-migration-rollback-1.0.4/README.md` & `django-migration-rollback-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Django Migration Rollback v1.0.4
+# Django Migration Rollback v1.0.5
 A Django package used to just make the `python manage.py migrate` a little easier for Django apps that commit their migrations and want a way to rollback to a previous migration without needing to check what the which one it is via `python manage.py showmigrations` or in the project's git repository.
 
 ## Features
 Able to set which branch in a git repository to rollback to using the custom command `migraterollback` or if you wish to just rollback to a previous migration only via `migrateprevious`. Note in order to use the rollback with a git repository's branch feature with git the project must have a `.git` file present.
 
 ### Django `migraterollback` command
     ❯ python manage.py migraterollback polls feature/really-cool-branch
@@ -66,16 +66,16 @@
 eval "$(pyenv init --path)"
 eval "$(pyenv init -)"
 eval "$(pyenv virtualenv-init -)"
 """ > ~/.zshrc
 source ~/.zshrc
 
 # create a virtualenv
-pyenv install 1.0.4
-pyenv virtualenv 1.0.4 django_migration_rollback
+pyenv install 3.10.5
+pyenv virtualenv 3.10.5 django_migration_rollback
 pyenv activate django_migration_rollback
 
 # install dependencies
 pip install -U pip
 pip install -r requirements.txt -r requirements_dev.txt
 ```
```

### Comparing `django-migration-rollback-1.0.4/django_migration_rollback.egg-info/PKG-INFO` & `django-migration-rollback-1.0.5/django_migration_rollback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-migration-rollback
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple Django app to be able to migrate back to a previous migration or to migrate back to a migration in a specific branch in a git repository or locally.
 Home-page: https://github.com/jdboisvert/django-migration-rollback
-Download-URL: https://github.com/jdboisvert/django-migration-rollback/archive/refs/tags/v1.0.4.zip
 Author: Jeffrey Boisvert
 Author-email: info.jeffreyboisvert@gmail.com
 License: MIT License
+Download-URL: https://github.com/jdboisvert/django-migration-rollback/archive/refs/tags/v1.0.5.zip
 Project-URL: Repository, https://github.com/jdboisvert/django-migration-rollback
 Project-URL: Bug Reports, https://github.com/jdboisvert/django-migration-rollback/issues
 Keywords: django,migration,rollback,git
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Django Migration Rollback v1.0.4
+# Django Migration Rollback v1.0.5
 A Django package used to just make the `python manage.py migrate` a little easier for Django apps that commit their migrations and want a way to rollback to a previous migration without needing to check what the which one it is via `python manage.py showmigrations` or in the project's git repository.
 
 ## Features
 Able to set which branch in a git repository to rollback to using the custom command `migraterollback` or if you wish to just rollback to a previous migration only via `migrateprevious`. Note in order to use the rollback with a git repository's branch feature with git the project must have a `.git` file present.
 
 ### Django `migraterollback` command
     ❯ python manage.py migraterollback polls feature/really-cool-branch
@@ -91,20 +91,22 @@
 eval "$(pyenv init --path)"
 eval "$(pyenv init -)"
 eval "$(pyenv virtualenv-init -)"
 """ > ~/.zshrc
 source ~/.zshrc
 
 # create a virtualenv
-pyenv install 1.0.4
-pyenv virtualenv 1.0.4 django_migration_rollback
+pyenv install 3.10.5
+pyenv virtualenv 3.10.5 django_migration_rollback
 pyenv activate django_migration_rollback
 
 # install dependencies
 pip install -U pip
 pip install -r requirements.txt -r requirements_dev.txt
 ```
 
 ## Installing pre-commit hooks
 ```bash
 pre-commit install
 ```
+
+
```

### Comparing `django-migration-rollback-1.0.4/django_migration_rollback.egg-info/SOURCES.txt` & `django-migration-rollback-1.0.5/django_migration_rollback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-migration-rollback-1.0.4/migration_rollback/management/commands/migrateprevious.py` & `django-migration-rollback-1.0.5/migration_rollback/management/commands/migrateprevious.py`

 * *Files identical despite different names*

### Comparing `django-migration-rollback-1.0.4/migration_rollback/management/commands/migraterollback.py` & `django-migration-rollback-1.0.5/migration_rollback/management/commands/migraterollback.py`

 * *Files identical despite different names*

### Comparing `django-migration-rollback-1.0.4/migration_rollback/utils/migration_utils.py` & `django-migration-rollback-1.0.5/migration_rollback/utils/migration_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 def get_previous_migration(app_name: str) -> str:
     """
     Gets the previous migration present in an app's migration directory in the database
 
     :param app_name: The name of the app to get the previous migration for
     :return: The previous migration number (ex: 0001 for 0001_initial.py)
     """
-    command = f"python manage.py showmigrations {app_name} | sort -r | grep '\[X\]' | head -2 | tail -1 | cut -d ' ' -f 3"
+    command = f"python manage.py showmigrations {app_name} 2>/dev/null | sort -r | grep '\[X\]' | head -2 | tail -1 | cut -d ' ' -f 3"
     command_pipe = Popen(command, shell=True, stdin=PIPE, stdout=PIPE, stderr=STDOUT, close_fds=True)
 
     return command_pipe.stdout.read().decode("utf-8").split("_")[0]
```

### Comparing `django-migration-rollback-1.0.4/pyproject.toml` & `django-migration-rollback-1.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311"]
 extend-exclude = '__pycache__'
 line-length = 140
 
 # Docs: https://gitlab.com/mbarkhau/pycalver
 [bumpver]
-current_version = "1.0.4"
+current_version = "1.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[RELEASE] {new_version}"
 commit = true
 tag = false
 push = false
 
 [bumpver.file_patterns]
```

### Comparing `django-migration-rollback-1.0.4/setup.py` & `django-migration-rollback-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os.path import dirname, join
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 GITHUB_URL = "https://github.com/jdboisvert/django-migration-rollback"
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 
 def read(fname):
     """Read content of a file and return as a string."""
     return Path(join(dirname(__file__), fname)).read_text()
```

