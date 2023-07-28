# Comparing `tmp/nextline_schedule-0.2.2.tar.gz` & `tmp/nextline_schedule-0.2.3.tar.gz`

## Comparing `nextline_schedule-0.2.2.tar` & `nextline_schedule-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/auto/factory.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/auto/machine.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/queries/AutoMode.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/test_fsm.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/test_request.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/test_scratch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/auto/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/schema/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/schema/conftest.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/tests/schema/test_run.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/README.md
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 nextline_schedule-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/auto/factory.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/auto/machine.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/queries/AutoMode.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/test_fsm.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/test_request.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/test_scratch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/schema/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/schema/conftest.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/tests/schema/test_run.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/README.md
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 nextline_schedule-0.2.3/PKG-INFO
```

### Comparing `nextline_schedule-0.2.2/.github/workflows/pypi.yml` & `nextline_schedule-0.2.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/.github/workflows/type-check.yml` & `nextline_schedule-0.2.3/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/.github/workflows/unit-test.yml` & `nextline_schedule-0.2.3/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/.vscode/settings.json` & `nextline_schedule-0.2.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/plugin.py` & `nextline_schedule-0.2.3/src/nextline_schedule/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/scheduler.py` & `nextline_schedule-0.2.3/src/nextline_schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/auto/callback.py` & `nextline_schedule-0.2.3/src/nextline_schedule/auto/callback.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,21 +56,14 @@
             await self._nextline.reset(statement=statement)
             await self.auto_mode.run()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.pull() cancelled')
 
     async def run(self, started: asyncio.Event) -> None:
         try:
-            async with self._nextline.run_session():
-                async for prompt in self._nextline.prompts():
-                    await self._nextline.send_pdb_command(
-                        command='continue',
-                        prompt_no=prompt.prompt_no,
-                        trace_no=prompt.trace_no,
-                    )
-                    started.set()
+            await self._nextline.run_continue_and_wait(started)
             if self._nextline.exception() is not None:
                 await self.auto_mode.on_raised()  # type: ignore
                 return
             await self.auto_mode.on_finished()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.run() cancelled')
```

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/auto/factory.py` & `nextline_schedule-0.2.3/src/nextline_schedule/auto/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/auto/machine.py` & `nextline_schedule-0.2.3/src/nextline_schedule/auto/machine.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/schema/mutation.py` & `nextline_schedule-0.2.3/src/nextline_schedule/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.2.3/src/nextline_schedule/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/test_fsm.py` & `nextline_schedule-0.2.3/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/test_request.py` & `nextline_schedule-0.2.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/test_scratch.py` & `nextline_schedule-0.2.3/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/auto/test_auto.py` & `nextline_schedule-0.2.3/tests/auto/test_auto.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/auto/test_auto_on_raised.py` & `nextline_schedule-0.2.3/tests/auto/test_auto_on_raised.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/auto/test_auto_turn_off.py` & `nextline_schedule-0.2.3/tests/auto/test_auto_turn_off.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/tests/schema/test_run.py` & `nextline_schedule-0.2.3/tests/schema/test_run.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/.gitignore` & `nextline_schedule-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/LICENSE.txt` & `nextline_schedule-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/README.md` & `nextline_schedule-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.2/pyproject.toml` & `nextline_schedule-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = ["transitions>=0.9", "httpx>=0.23"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-host = ["nextline-graphql>=0.4.8"]
+host = ["nextline-graphql>=0.5.5"]
 tests = [
   "async-asgi-testclient>=1.4",
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
   "hypothesis>=6.65",
```

### Comparing `nextline_schedule-0.2.2/PKG-INFO` & `nextline_schedule-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextline-schedule
-Version: 0.2.2
+Version: 0.2.3
 Summary: A plugin of nextline-graphql. An interface to the SO scheduler.
 Project-URL: Documentation, https://github.com/simonsobs/nextline-schedule#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-schedule/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-schedule
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: httpx>=0.23
 Requires-Dist: transitions>=0.9
 Provides-Extra: host
-Requires-Dist: nextline-graphql>=0.4.8; extra == 'host'
+Requires-Dist: nextline-graphql>=0.5.5; extra == 'host'
 Provides-Extra: tests
 Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: hypothesis>=6.65; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-httpx>=0.21; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
```

