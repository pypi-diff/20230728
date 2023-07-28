# Comparing `tmp/nextline_graphql-0.5.4.tar.gz` & `tmp/nextline_graphql-0.5.5.tar.gz`

## Comparing `nextline_graphql-0.5.4.tar` & `nextline_graphql-0.5.5.tar`

### file list

```diff
@@ -1,55 +1,49 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/__about__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/py.typed
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/config/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/config/default.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/custom/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/custom/strawberry.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/hook/__init__.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/hook/spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/__init__.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/types.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/schema/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/schema/mutation.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/schema/query.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/continuous/schema/subscription.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/__init__.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/test.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/script.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/script2.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/__init__.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/mutation.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/query.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/subscription.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/plugin.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/graphql/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/schema/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/schema/query.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/test/__init__.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/test/funcs.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/LICENSE
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 nextline_graphql-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/__about__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/py.typed
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/config/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/config/default.toml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/custom/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/custom/strawberry.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/hook/__init__.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/hook/spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/__init__.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/test.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/script.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/script2.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/script_asyncio.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/script_scratch.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/example_script/script_threading.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/mutations/Exec.gql
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/mutations/Reset.gql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/mutations/SendPdbCommand.gql
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/queries/Exception.gql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/queries/Source.gql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/queries/SourceLine.gql
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/queries/State.gql
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Counter.gql
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Prompting.gql
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/subscriptions/State.gql
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/subscriptions/Stdout.gql
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/subscriptions/TraceIds.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/__init__.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/mutation.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/query.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/subscription.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/plugin.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/graphql/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/graphql/queries/Settings.gql
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/schema/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/schema/query.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/test/__init__.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/test/funcs.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/LICENSE
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/README.md
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 nextline_graphql-0.5.5/PKG-INFO
```

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/factory.py` & `nextline_graphql-0.5.5/nextlinegraphql/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/config/__init__.py` & `nextline_graphql-0.5.5/nextlinegraphql/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/config/default.toml` & `nextline_graphql-0.5.5/nextlinegraphql/config/default.toml`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/custom/strawberry.py` & `nextline_graphql-0.5.5/nextlinegraphql/custom/strawberry.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/hook/__init__.py` & `nextline_graphql-0.5.5/nextlinegraphql/hook/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 __all__ = ['spec', 'load_plugins']
 
 from apluggy import PluginManager
 
-from nextlinegraphql.plugins import ctrl, graphql, continuous
+from nextlinegraphql.plugins import ctrl, graphql
 
 from . import spec
 
 
 def load_plugins() -> PluginManager:
     '''Return a pluggy PluginManager with the plugins registered'''
 
     pm = PluginManager(spec.PROJECT_NAME)
     pm.add_hookspecs(spec)
 
     # The hooks are called in the reverse order of the plugin registration.
     # https://pluggy.readthedocs.io/en/stable/#call-time-order
-    pm.register(continuous.Plugin(), name='continuous')
     pm.register(graphql.Plugin(), name='graphql')
     pm.register(ctrl.Plugin(), name='ctrl')
     # pm.set_blocked('schedule')
     pm.load_setuptools_entrypoints(spec.PROJECT_NAME)
 
     return pm
```

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/hook/spec.py` & `nextline_graphql-0.5.5/nextlinegraphql/hook/spec.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/__init__.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/test.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/test.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/graphql/__init__.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/mutation.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/mutation.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 async def mutate_exec(info: Info) -> bool:
     nextline: Nextline = info.context["nextline"]
     await nextline.run()
     return True
 
 
+async def mutate_run_and_continue(info: Info) -> bool:
+    nextline: Nextline = info.context["nextline"]
+    await nextline.run_and_continue()
+    return True
+
+
 async def mutate_reset(info: Info, statement: Optional[str] = None):
     nextline: Nextline = info.context["nextline"]
     await nextline.reset(statement=statement)
     return True
 
 
 async def mutate_send_pdb_command(
@@ -46,12 +52,13 @@
     await nextline.kill()
     return True
 
 
 @strawberry.type
 class Mutation:
     exec: bool = strawberry.field(resolver=mutate_exec)
+    run_and_continue: bool = strawberry.field(resolver=mutate_run_and_continue)
     reset: bool = strawberry.field(resolver=mutate_reset)
     send_pdb_command: bool = strawberry.field(resolver=mutate_send_pdb_command)
     interrupt: bool = strawberry.field(resolver=mutate_interrupt)
     terminate: bool = strawberry.field(resolver=mutate_terminate)
     kill: bool = strawberry.field(resolver=mutate_kill)
```

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/query.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,21 @@
 def query_exception(info: Info) -> Optional[str]:
     nextline: Nextline = info.context["nextline"]
     if exc := nextline.exception():
         return "".join(traceback.format_exception(type(exc), exc, exc.__traceback__))
     return None
 
 
+def query_continuous_enabled(info: Info) -> bool:
+    nextline: Nextline = info.context["nextline"]
+    return nextline.continuous_enabled
+
+
 @strawberry.type
 class Query:
     hello: str = strawberry.field(resolver=query_hello)
     state: str = strawberry.field(resolver=query_state)
     run_no: int = strawberry.field(resolver=query_run_no)
     source: List[str] = strawberry.field(resolver=query_source)
     source_line: str = strawberry.field(resolver=query_source_line)
     exception: Optional[str] = strawberry.field(resolver=query_exception)
+    continuous_enabled: bool = strawberry.field(resolver=query_continuous_enabled)
```

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/ctrl/schema/subscription.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/ctrl/schema/subscription.py`

 * *Files 21% similar despite different names*

```diff
@@ -61,14 +61,19 @@
 async def subscribe_stdout(info: Info) -> AsyncIterator[str]:
     nextline: Nextline = info.context["nextline"]
     async for i in nextline.subscribe_stdout():
         assert i.text is not None
         yield i.text
 
 
+def subscribe_continuous_enabled(info: Info) -> AsyncIterator[bool]:
+    nextline: Nextline = info.context["nextline"]
+    return nextline.subscribe_continuous_enabled()
+
+
 @strawberry.type
 class Subscription:
     counter: AsyncIterator[int] = strawberry.field(
         is_subscription=True, resolver=subscribe_counter
     )
     state: AsyncIterator[str] = strawberry.field(
         is_subscription=True, resolver=subscribe_state
@@ -81,7 +86,10 @@
     )
     prompting: AsyncIterator[PromptingData] = strawberry.field(
         is_subscription=True, resolver=subscribe_prompting
     )
     stdout: AsyncIterator[str] = strawberry.field(
         is_subscription=True, resolver=subscribe_stdout
     )
+    continuous_enabled: AsyncIterator[bool] = strawberry.field(
+        is_subscription=True, resolver=subscribe_continuous_enabled
+    )
```

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/plugin.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/nextlinegraphql/plugins/graphql/test/funcs.py` & `nextline_graphql-0.5.5/nextlinegraphql/plugins/graphql/test/funcs.py`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/.gitignore` & `nextline_graphql-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/LICENSE` & `nextline_graphql-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/README.md` & `nextline_graphql-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nextline_graphql-0.5.4/pyproject.toml` & `nextline_graphql-0.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "nextline==0.5.4",
+    "nextline>=0.5.5",
     "nextline-rdb>=0.2",
     "apluggy>=0.9.0",
     "dynaconf>=3.1",
     "starlette>=0.26",
     "strawberry-graphql>=0.168",
     "websockets>=10.2",
     "rich>=13.3",
```

### Comparing `nextline_graphql-0.5.4/PKG-INFO` & `nextline_graphql-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextline-graphql
-Version: 0.5.4
+Version: 0.5.5
 Summary: A GraphQL API for Nextline
 Project-URL: Homepage, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apluggy>=0.9.0
 Requires-Dist: dynaconf>=3.1
 Requires-Dist: nextline-rdb>=0.2
-Requires-Dist: nextline==0.5.4
+Requires-Dist: nextline>=0.5.5
 Requires-Dist: rich>=13.3
 Requires-Dist: starlette>=0.26
 Requires-Dist: strawberry-graphql>=0.168
 Requires-Dist: websockets>=10.2
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
```

