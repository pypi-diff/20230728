# Comparing `tmp/python_aap-0.0.1.tar.gz` & `tmp/python_aap-0.0.2.tar.gz`

## Comparing `python_aap-0.0.1.tar` & `python_aap-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 python_aap-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_aap-0.0.1/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 python_aap-0.0.1/src/aap/__init__.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 python_aap-0.0.1/src/aap/base.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 python_aap-0.0.1/src/aap/endpoints.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 python_aap-0.0.1/src/aap/mixins.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 python_aap-0.0.1/.gitignore
--rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.1/LICENSE
--rw-r--r--   0        0        0     6195 2020-02-02 00:00:00.000000 python_aap-0.0.1/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 python_aap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 python_aap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 python_aap-0.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 python_aap-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/__init__.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/__main__.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/base.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/endpoints.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 python_aap-0.0.2/src/aap/mixins.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 python_aap-0.0.2/.gitignore
+-rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 python_aap-0.0.2/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_aap-0.0.2/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 python_aap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 python_aap-0.0.2/PKG-INFO
```

### Comparing `python_aap-0.0.1/.gitlab-ci.yml` & `python_aap-0.0.2/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -13,36 +13,45 @@
   cache:
     paths:
       - venv
 
 code style check:
   extends: .base
   stage: validate
-  image: python3.8
   script:
-   - pip3 install --upgrade pep8
-   - pep8 src/aap
+   - pip3 install --upgrade pycodestyle
+   - pycodestyle --max-line-length=120 src/aap
   allow_failure: true
   rules:
     - if: $CI_PIPELINE_SOURCE == "merge_request_event"
       changes:
         paths:
-          - src/*
+          - src/aap/*
 
 basic tests:
   extends: .base
   stage: test
-  image: python3.8
   script:
    - echo "Not yet implemented"
   rules:
     - if: $CI_PIPELINE_SOURCE == "merge_request_event"
       changes:
         paths:
-          - src/*
+          - src/aap/*
+
+example test:
+  extends: .base
+  stage: test
+  script:
+   - PYTHONPATH="$(pwd)/src" python3 -m aap --id 7848 -l sw01-dist.itdev --insecure run-job --ignore-fail
+  rules:
+    - if: $CI_PIPELINE_SOURCE == "merge_request_event"
+      changes:
+        paths:
+          - src/aap/*
 
 build job:
   extends: .base
   stage: build
   script:
    - pip3 install --upgrade build[virtualenv]
    - python3 -m build
@@ -75,10 +84,11 @@
   extends: .base
   stage: publish
   dependencies:
     - build job
   script:
    - pip3 install --upgrade twine
    - python3 -m twine upload  -u __token__ -p $PYPI_TOKEN dist/*
+  when: manual
   rules:
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
       when: on_success
```

### Comparing `python_aap-0.0.1/src/aap/base.py` & `python_aap-0.0.2/src/aap/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import requests
 import time
 
+
 class APIError(Exception):
     pass
 
+
 class API:
     _obj = None  # Warning: use on own risk
 
-    def __init__(self, url, user, password, version = 2, retries=0, ssl_verify=False, retry_timeout=1) -> None:
+    def __init__(self, url, user, password, version=2, retries=0,
+                 ssl_verify=False, retry_timeout=1) -> None:
         self.url = url
-        self.vstr  = f'/api/v{version}'
+        self.vstr = f'/api/v{version}'
         self.session = requests.Session()
         self.session.auth = (user, password)
         self.session.verify = ssl_verify
         self.timeout = retry_timeout
         self.retries = retries
         API._obj = self
 
@@ -31,27 +34,27 @@
             # retry on server error
             time.sleep(self.timeout)
             return self.request(method, path, json, retries - 1, parse)
         if not 200 <= response.status_code < 300:
             raise APIError(path, response.text)
         return response.json() if parse else response
 
-
     def load(self, path):
         p = path
         while p:
             resp = self.request('GET', p)
             p = resp.get('next')
             for i in resp['results']:
                 yield i
 
 
 class APIObject:
     _related = {}
     _sub = {}
+    _on_demand = {}
     _actions = []
     _path = None
     _map = {}
     _cache = {}
     _display = 'name'
 
     def __init_subclass__(cls) -> None:
@@ -59,93 +62,113 @@
 
     def __init__(self, data, api) -> None:
         self._data = data
         self.api = api
         self._cache[data['id']] = self
 
     def _reload(self):
-        del self._cache[self._data['id']] 
+        del self._cache[self._data['id']]
         self._data = self.load(self._data['id'], self.api)._data
 
     def delete(self):
         # Invalidates object
-        self.api.request('DELETE', self._path + str(self._data['id']) +'/', parse=False)
+        self.api.request('DELETE', self._path +
+                         str(self._data['id']) + '/', parse=False)
+
     def get_sub(self, path, obj_type):
         for obj in self.api.load(self._path + f'{self.id}/{path}/'):
             yield obj_type(obj, self.api)
+
     def _action(self, action, method="POST"):
         def foo(**kwargs):
-            self.api.request(method, self._path + f'{self.id}/{action}/', kwargs)
+            self.api.request(method, self._path +
+                             f'{self.id}/{action}/', kwargs)
         return foo
+
+    def __on_demand(self, path):
+        return self.api.request("GET", self.url + path, parse=False).text
+
     def __getattribute__(self, __name: str):
         if __name.startswith('_'):
             return super().__getattribute__(__name)
         if __name in self._sub:
             return self.get_sub(__name, self._sub[__name])
         if __name in self._related:
             return self._related[__name](self, __name)
+        if __name in self._on_demand:
+            return self.__on_demand(self._on_demand[__name])
         if __name in self._actions:
             return self._action(__name)
         if __name in self._map:
             return self._map[__name](self._data[__name])
         if __name in self._data:
             return self._data[__name]
         return super().__getattribute__(__name)
+
     @classmethod
     def find(cls, query, order_by=None, api=None):
         url = cls._path + '?search=' + query
         if order_by:
             url += '&order_by=' + ','.join(order_by)
         if not api:
             api = API._obj
         yield from map(lambda x: cls(x, api), api.load(url))
+
     @classmethod
     def find_first(cls, query, order_by=None, api=None):
         for i in cls.find(query, order_by, api):
             return i
         return None
+
     @classmethod
     def load(cls, oid, api=None):
         if oid in cls._cache:
             return cls._cache[oid]
         if not api:
             api = API._obj
         return cls(api.request('GET', cls._path + f'{oid}/'), api)
+
     @property
     def name(self):
         return self._data.get(self._display, None)
+
     def __repr__(self) -> str:
         name = self._data.get(self._display, '-')
         return f'<{type(self).__name__} {name} {self.id}>'
 
+
 class Related:
-    def __init__(self, obj_type, *key, iterable=False, prefix=None, allow_none=True) -> None:
+    def __init__(self, obj_type, *key, iterable=False,
+                 prefix=None, allow_none=True) -> None:
         self.key = key
         self.obj = obj_type
         self.iterable = iterable
         self.prefix = prefix
         self.none = allow_none
+
     def __get_attr(self, key, obj):
         if not key:
             return obj
         head, *key = key
         return self.__get_attr(key, obj[head])
+
     def __iter(self, obj, path):
         for i in obj.api.load(path):
             yield self.obj(i, obj.api)
+
     def __call__(self, obj, k):
         key = self.key
         if not key:
             key = [k]
         path = str(self.__get_attr(key, obj._data))
         if self.none and path is None:
             return
         if self.prefix:
             path = self.prefix + path
         if not self.iterable:
             return self.obj(
                 obj.api.request('GET',
-                    path
-                ),
+                                path
+                                ),
                 obj.api
             )
-        return self.__iter(obj, path)
+        return self.__iter(obj, path)
```

### Comparing `python_aap-0.0.1/src/aap/endpoints.py` & `python_aap-0.0.2/src/aap/endpoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,111 +1,132 @@
 import os
 import datetime
 
-import base
-import mixins
+from .base import APIObject, Related
+from .mixins import LaunchableMixin, WaitableMixin
 
 
-class Schedule(base.APIObject):
+class Schedule(APIObject):
     _path = 'schedules/'
     _action = {}
     _map = {
-        'dtstart': lambda x: datetime.datetime.fromisoformat(x.replace("Z", "")),  # unsuported ISO format until 3.11
-        'dtend': lambda x: datetime.datetime.fromisoformat(x.replace("Z", ""))   # unsuported ISO format until 3.11
+        # unsuported ISO format until 3.11
+        'dtstart': lambda x: datetime.datetime.fromisoformat(x.replace("Z", "")),
+        # unsuported ISO format until 3.11
+        'dtend': lambda x: datetime.datetime.fromisoformat(x.replace("Z", ""))
     }
 
-base.__schedule_class = Schedule
 
+LaunchableMixin.__schedule_class = Schedule
 
-class JobEvent(base.APIObject):
+
+class JobEvent(APIObject):
     _display = "event"
 
-class Job(base.APIObject, mixins.WaitableMixin):
+
+class Job(APIObject, WaitableMixin):
     _path = 'jobs/'
     _sub = {
         'job_events': JobEvent
     }
+    _on_demand = {'stdout': "stdout/?format=txt"}
+
     @property
     def artifacts(self):
         if self.status not in self._states:
             return None
         for event in self.job_events:
             if event.event == "playbook_on_stats":
                 return event.get('artifact_data', {})
+
     @property
     def web_url(self):
-        return os.path.join(self.api.url.strip(self.api.vstr) +f"/#/jobs/playbook/{self.id}/details")
+        return os.path.join(self.api.url.strip(self.api.vstr) + f"/#/jobs/playbook/{self.id}/details")
 
-class WorkflowNode(base.APIObject):
+
+class WorkflowNode(APIObject):
     _path = "workflow_nodes"
     _related = {
-        'job': base.Related(Job, 'summary_fields', 'job', 'id', iterable=False, prefix='jobs/')
+        'job': Related(Job, 'summary_fields', 'job', 'id', iterable=False, prefix='jobs/')
     }
+
     @property
     def is_executed(self):
         return self._data.get('job') is not None
-class WorkflowJob(base.APIObject, mixins.WaitableMixin):
+
+
+class WorkflowJob(APIObject, WaitableMixin):
     _path = 'workflow_jobs/'
     _related = {
-        'workflow_nodes': base.Related(WorkflowNode, 'related', 'workflow_nodes', iterable=True)
+        'workflow_nodes': Related(WorkflowNode, 'related', 'workflow_nodes', iterable=True)
     }
+
     @property
     def web_url(self):
-        return os.path.join(self.api.url.strip(self.api.vstr) +f"/#/jobs/workflow/{self.id}/output")
+        return os.path.join(self.api.url.strip(self.api.vstr) + f"/#/jobs/workflow/{self.id}/output")
 
     def job_nodes(self):
         for workflow_node in self.workflow_nodes:
             if workflow_node._data.get('summary_fields', {}).get('job', {}).get('type') == 'job':
                 yield workflow_node
 
-class WorkflowJobTemplate(base.APIObject, mixins.LaunchableMixin):
+
+class WorkflowJobTemplate(APIObject, LaunchableMixin):
     _creates = WorkflowJob
     _related = {
 
     }
     _sub = {
         'workflow_jobs': WorkflowJob,
         'schedules': Schedule
     }
     _path = 'workflow_job_templates/'
+
     @property
     def web_url(self):
-        return os.path.join(self.api.url.strip(self.api.vstr) +f"/#/templates/workflow_job_template/{self.id}/details")
+        return os.path.join(
+            self.api.url.strip(self.api.vstr) +
+            f"/#/templates/workflow_job_template/{self.id}/details"
+        )
 
 
-class JobTemplate(base.APIObject, mixins.LaunchableMixin):
+class JobTemplate(APIObject, LaunchableMixin):
     _creates = Job
     _related = {
 
     }
     _sub = {
         'jobs': Job,
         'schedules': Schedule
     }
     _path = 'job_templates/'
+
     @property
     def web_url(self):
-        return os.path.join(self.api.url.strip(self.api.vstr) +f"/#/templates/job_template/{self.id}/details")
+        return os.path.join(self.api.url.strip(self.api.vstr) + f"/#/templates/job_template/{self.id}/details")
 
 
-class Organization(base.APIObject):
+class Organization(APIObject):
     _related = {
 
     }
     _sub = {
         'workflow_job_templates': WorkflowJobTemplate,
         'job_templates': JobTemplate
     }
     _path = 'organizations/'
 
-class Group(base.APIObject):
+
+class Group(APIObject):
     _path = "groups/"
 
-class Host(base.APIObject):
+
+class Host(APIObject):
     _path = "hosts/"
 
-class Inventory(base.APIObject):
-    _path='inventories/'
+
+class Inventory(APIObject):
+    _path = 'inventories/'
     _sub = {
         'hosts': Host,
         'groups': Group
     }
```

### Comparing `python_aap-0.0.1/src/aap/mixins.py` & `python_aap-0.0.2/src/aap/mixins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 import time
 
+
 class WaitableMixin:
     _states = {
         'successful': True,
         'failed': False,
         'canceled': False,
         'error': False,
         'never_updated': False
-    }    
+    }
+
+    @property
+    def is_running(self):
+        return self.status == "running"
+
     @property
-    def finished(self):
+    def is_finished(self):
         return self.status in self._states
+
+    @property
+    def is_successfull(self):
+        return self._states.get(self.status)
+
     def wait(self, timeout=None, poll=1):
         started = time.time()
-        while not self.finished:
+        while not self.is_finished:
             if timeout and time.time() - started > timeout:
                 break
             time.sleep(poll)
             self._reload()
         return self._states.get(self.status)
 
+
 class LaunchableMixin:
     def launch(self, extra_vars={}, limit=[]):
         data = {'extra_vars': extra_vars}
         if limit:
             data['limit'] = ','.join(limit)
-        result = self.api.request('POST', self._path + f"{self.id}/launch/", data)
+        result = self.api.request(
+            'POST', self._path + f"{self.id}/launch/", data)
         return self._creates.load(result[self._creates._path.strip('/').rstrip('s')], self.api)
+
     def schedule(self, name, rrule, **kwargs):
         """
         Schedule launch
         required:
          name: Name of this schedule. (string, required)
          rrule: A value representing the schedules iCal recurrence rule. (string, required)
         optional:
@@ -39,12 +53,13 @@
          limit: list/str
         """
         if type(kwargs.get('limit')) == list:
             kwargs['limit'] = ",".join(kwargs['limit'])
 
         if type(kwargs.get('job_tags')) == list:
             kwargs['job_tags'] = ",".join(kwargs['job_tags'])
-        
+
         kwargs['name'] = name
         kwargs['rrule'] = rrule
-        response = self.api.request("POST", self._path + f"{self.id}/schedules/", kwargs)
-        return self.__schedule_class(response, self.api)
+        response = self.api.request(
+            "POST", self._path + f"{self.id}/schedules/", kwargs)
+        return self.__schedule_class(response, self.api)
```

### Comparing `python_aap-0.0.1/.gitignore` & `python_aap-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+*.env
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
```

### Comparing `python_aap-0.0.1/LICENSE` & `python_aap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_aap-0.0.1/pyproject.toml` & `python_aap-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-aap"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ivan Mitruk", email="imitruk@redhat.com" },
 ]
 description = "Unofficial python wrapper over Ansible Automation Platform REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

