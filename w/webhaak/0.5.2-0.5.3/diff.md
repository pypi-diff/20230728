# Comparing `tmp/webhaak-0.5.2.tar.gz` & `tmp/webhaak-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhaak-0.5.2.tar", last modified: Fri Jun  9 19:54:29 2023, max compression
+gzip compressed data, was "webhaak-0.5.3.tar", last modified: Fri Jul 28 11:27:00 2023, max compression
```

## Comparing `webhaak-0.5.2.tar` & `webhaak-0.5.3.tar`

### file list

```diff
@@ -1,58 +1,20 @@
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.182563 webhaak-0.5.2/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      936 2023-04-06 07:21:19.000000 webhaak-0.5.2/.gitignore
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4810 2023-06-09 19:53:46.000000 webhaak-0.5.2/CHANGELOG.md
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-07-07 08:00:19.000000 webhaak-0.5.2/LICENSE
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-06-09 19:54:29.178563 webhaak-0.5.2/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-06-09 18:11:07.000000 webhaak-0.5.2/README.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2021-07-07 08:00:19.000000 webhaak-0.5.2/__init__.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.174564 webhaak-0.5.2/docs/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      707 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/Makefile
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      791 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/make.bat
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/docs/source/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4810 2023-06-09 19:53:46.000000 webhaak-0.5.2/docs/source/CHANGELOG.md
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-06-09 18:11:07.000000 webhaak-0.5.2/docs/source/README.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     6219 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/conf.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     2218 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/exampleconfig.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      514 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/source/index.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       58 2021-07-07 08:00:19.000000 webhaak-0.5.2/docs/source/modules.rst
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      557 2023-04-29 18:49:36.000000 webhaak-0.5.2/docs/source/webhaak.rst
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     3351 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/examples.yaml
--rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      824 2023-04-29 18:49:36.000000 webhaak-0.5.2/example_config/flake8diff.sh
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      293 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/gunicorn_webhaak_conf.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/nginx/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1049 2023-03-31 18:46:56.000000 webhaak-0.5.2/example_config/nginx/hook.example.com.conf
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      593 2023-04-06 07:21:19.000000 webhaak-0.5.2/example_config/rq_settings.example.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1237 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/sentry_to_telegram.sh
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/supervisord/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1112 2023-04-28 07:25:54.000000 webhaak-0.5.2/example_config/supervisord/webhaak_rq_worker.conf
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/example_config/systemd/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      887 2023-04-29 18:49:36.000000 webhaak-0.5.2/example_config/systemd/webhaak.service
--rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      631 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/update_flask.sh
--rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      987 2021-07-07 08:00:19.000000 webhaak-0.5.2/example_config/update_virtualenv.sh
--rwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)      628 2023-03-31 18:46:56.000000 webhaak-0.5.2/example_config/update_webapp.sh
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      353 2023-04-06 07:21:19.000000 webhaak-0.5.2/pylintrc
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      936 2023-06-09 19:43:45.000000 webhaak-0.5.2/pyproject.toml
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       98 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-dev.in
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     4809 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-dev.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       29 2023-03-31 18:46:56.000000 webhaak-0.5.2/requirements-server.in
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1972 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements-server.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      175 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements.in
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1859 2023-06-06 16:20:17.000000 webhaak-0.5.2/requirements.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-09 19:54:29.182563 webhaak-0.5.2/setup.cfg
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-04-06 07:21:19.000000 webhaak-0.5.2/setup.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      346 2018-10-03 09:36:45.000000 webhaak-0.5.2/src/settings.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/webhaak/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-04-06 09:50:43.000000 webhaak-0.5.2/src/webhaak/__init__.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10139 2023-03-31 18:46:56.000000 webhaak-0.5.2/src/webhaak/incoming.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9724 2023-04-28 07:25:54.000000 webhaak-0.5.2/src/webhaak/main.py
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16655 2023-06-09 18:58:03.000000 webhaak-0.5.2/src/webhaak/tasks.py
-drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-06-09 19:54:29.178563 webhaak-0.5.2/src/webhaak.egg-info/
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/PKG-INFO
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1133 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/SOURCES.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/dependency_links.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/entry_points.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       92 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/requires.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       17 2023-06-09 19:54:29.000000 webhaak-0.5.2/src/webhaak.egg-info/top_level.txt
--rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      380 2023-04-06 07:21:19.000000 webhaak-0.5.2/tox.ini
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    11357 2021-10-12 17:55:24.000000 webhaak-0.5.3/LICENSE
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:27:00.001183 webhaak-0.5.3/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5034 2023-07-03 15:05:41.000000 webhaak-0.5.3/README.rst
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     1327 2023-07-28 11:25:54.000000 webhaak-0.5.3/pyproject.toml
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-07-28 11:27:00.001183 webhaak-0.5.3/setup.cfg
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      189 2023-07-03 15:05:41.000000 webhaak-0.5.3/setup.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:26:59.997183 webhaak-0.5.3/src/
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/src/webhaak/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-03 15:05:41.000000 webhaak-0.5.3/src/webhaak/__init__.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    10158 2023-07-03 15:27:27.000000 webhaak-0.5.3/src/webhaak/incoming.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     9937 2023-07-03 19:59:32.000000 webhaak-0.5.3/src/webhaak/main.py
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)    16684 2023-07-28 11:24:04.000000 webhaak-0.5.3/src/webhaak/tasks.py
+drwxrwxr-x   0 mbscholt  (1000) mbscholt  (1000)        0 2023-07-28 11:27:00.001183 webhaak-0.5.3/src/webhaak.egg-info/
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)     5651 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/PKG-INFO
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      343 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        1 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)       38 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/entry_points.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)      105 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/requires.txt
+-rw-rw-r--   0 mbscholt  (1000) mbscholt  (1000)        8 2023-07-28 11:26:59.000000 webhaak-0.5.3/src/webhaak.egg-info/top_level.txt
```

### Comparing `webhaak-0.5.2/LICENSE` & `webhaak-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.2/PKG-INFO` & `webhaak-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webhaak
-Version: 0.5.2
+Version: 0.5.3
 Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
 Author-email: Michiel Scholten <michiel@diginaut.net>
 License: Apache
 Project-URL: Homepage, https://github.com/aquatix/webhaak
 Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
 Keywords: webhook,api,automation,CI/CD
 Classifier: Framework :: FastAPI
```

### Comparing `webhaak-0.5.2/README.rst` & `webhaak-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `webhaak-0.5.2/docs/source/README.rst` & `webhaak-0.5.3/src/webhaak.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: webhaak
+Version: 0.5.3
+Summary: Simple webhook service to update and deploy sites and do other maintenance and automatic tasks
+Author-email: Michiel Scholten <michiel@diginaut.net>
+License: Apache
+Project-URL: Homepage, https://github.com/aquatix/webhaak
+Project-URL: Bug Tracker, https://github.com/aquatix/webhaak/issues
+Keywords: webhook,api,automation,CI/CD
+Classifier: Framework :: FastAPI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 webhaak
 =======
 
 |PyPI version| |PyPI downloads| |PyPI license| |Code quality| |Known vulnerabilities|
 
 `webhaak`_ is a simple `webhook`_ service to update and deploy sites and do
 other maintenance without having to ssh to a node.
```

### Comparing `webhaak-0.5.2/src/webhaak/incoming.py` & `webhaak-0.5.3/src/webhaak/incoming.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,21 @@
     if payload['push']['changes'][0]['new']:
         # Info about the (merge) commit is known
         hook_info['commit_after'] = payload['push']['changes'][0]['new']['target']['hash']
     else:
         # Likely a 'None' merge commit, so get the info from the branch that is getting merged
         hook_info['commit_after'] = payload['push']['changes'][0]['old']['target']['hash']
 
-    if 'links' in payload['push']['changes'][0]:
+    if 'links' in payload['push']['changes'][0] and 'html' in payload['push']['changes'][0]['links']:
         hook_info['compare_url'] = payload['push']['changes'][0]['links']['html']['href']
-    elif payload['push']['changes'][0]['old'] and 'links' in payload['push']['changes'][0]['old']:
+    elif (
+        payload['push']['changes'][0]['old']
+        and 'links' in payload['push']['changes'][0]['old']
+        and 'html' in payload['push']['changes'][0]['old']['links']
+    ):
         hook_info['compare_url'] = payload['push']['changes'][0]['old']['links']['html']['href']
     else:
         hook_info['compare_url'] = ''
 
     # Whether branch was closed; most likely after a merge
     hook_info['closed'] = payload['push']['changes'][0].get('closed', False)
     hook_info['commits'] = []
@@ -161,16 +165,14 @@
     """Parse the incoming webhook information and assemble the hook_info
 
     :param dict config: the projects configuration
     :param dict payload: dictionary containing the incoming webhook payload
     :param dict hook_info: dictionary containing the webhook configuration
     :param str event_info: message containing information about the event, to be used to log and as feedback to user
     """
-    sentry_message = False
-
     if 'push' in payload:
         # BitBucket, which has a completely different format
         handle_bitbucket_push(payload, hook_info)
 
     if 'pullrequest' in payload:
         # BitBucket pullrequest event
         handle_bitbucket_pullrequest(payload, hook_info)
@@ -202,14 +204,12 @@
     if 'before' in payload:
         hook_info['commit_before'] = payload['before']
     if 'after' in payload:
         hook_info['commit_after'] = payload['after']
     if 'commits' in payload:
         # Gather info on the commits included in this push
         get_commits_info(payload, hook_info)
-    if sentry_message:
-        event_info = handle_sentry_message(payload, hook_info, event_info)
 
     logger.debug(hook_info)
     logger.info(event_info)
 
     return event_info
```

### Comparing `webhaak-0.5.2/src/webhaak/main.py` & `webhaak-0.5.3/src/webhaak/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,20 +173,23 @@
         if not payload:
             logger.error(
                 '%s unknown, as no json was received. Check that %s webhook content type is application/json',
                 str(event_info),
                 vcs_source
             )
 
-        event_info = incoming.determine_task(config, payload, hook_info, event_info)
+        if sentry_message:
+            event_info = incoming.handle_sentry_message(payload, hook_info, event_info)
+        else:
+            event_info = incoming.determine_task(config, payload, hook_info, event_info)
         # Write event_info to task log
 
     # Create RQ job (task) for this request
     redis_conn = Redis()
-    q = Queue(connection=redis_conn)  # no args implies the default queue
+    q = Queue(connection=redis_conn, queue='webhaak')  # use named queue to prevent clashes with other RQ workers
 
     # Delay execution of count_words_at_url('http://nvie.com')
     job = q.enqueue(tasks.do_pull_andor_command, args=(config, hook_info,))
     logger.info('Enqueued job with id: %s', job.id)
 
     if not os.path.isdir(settings.jobs_log_dir):
         os.makedirs(settings.jobs_log_dir)
@@ -208,15 +211,15 @@
 
     :param str job_id:
     :return: dictionary with a task `status` and a `result`, including a relevant `message` on failure
     :rtype: json
     """
     logger.info('Status requested for job %s', job_id)
     redis_conn = Redis()
-    q = Queue(connection=redis_conn)  # no args implies the default queue
+    q = Queue(connection=redis_conn, queue='webhaak')  # use named queue to prevent clashes with other RQ workers
     job = q.fetch_job(job_id)
     if job is None:
         response = {'status': 'unknown'}
     else:
         log_contents = ''
         job_logfile_name = os.path.join(settings.jobs_log_dir, f'{job_id}.log')
         if os.path.isfile(job_logfile_name):
```

### Comparing `webhaak-0.5.2/src/webhaak/tasks.py` & `webhaak-0.5.3/src/webhaak/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import subprocess
 import time
 from datetime import datetime
 
 import git
 import requests
 import strictyaml
-from pydantic import BaseSettings, DirectoryPath, FilePath, validator
+from pydantic import DirectoryPath, FilePath, validator
+from pydantic_settings import BaseSettings
 from rq import get_current_job
 from strictyaml import Bool, Map, MapPattern, Optional, Seq, Str
 
 
 class Settings(BaseSettings):
     """
     Configuration needed for webhaak to do its tasks, using environment variables
```

