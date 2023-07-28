# Comparing `tmp/nextline-0.5.4.tar.gz` & `tmp/nextline-0.5.5.tar.gz`

## Comparing `nextline-0.5.4.tar` & `nextline-0.5.5.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/__about__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/count.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/disable.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/py.typed
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/types.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/fsm/__init__.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/fsm/factory.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/fsm/state.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/hook.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/spec.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/argument.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/__init__.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/prompt_info.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/prompt_notice.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/run_info.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/run_no.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/script.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/state_name.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/stdout.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/trace_info.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/registrars/trace_nos.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/session/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/session/monitor.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/session/session.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/plugin/plugins/session/spawn.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/call.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/commands.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/events.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/exc.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/runner.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/types.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/hook.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/skip.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/spec.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/_script.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/compose.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/concurrency.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/filter.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/global_.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/local_.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/peek.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/repeat.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/__init__.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/custom.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/factory.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/prompt.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/stream.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/test/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/test/py38.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/__init__.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/func.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/multiprocessing_logging.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/path.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/peek.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/profile.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/run.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/thread_exception.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/thread_task_id.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/done_callback/__init__.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/done_callback/task.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/done_callback/thread.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/done_callback/union.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/pubsub/__init__.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/pubsub/broker.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 nextline-0.5.4/nextline/utils/pubsub/item.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.5.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.5.4/LICENSE
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 nextline-0.5.4/README.md
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 nextline-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nextline-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/__about__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/__init__.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/continuous.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/count.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/disable.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/py.typed
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/types.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/fsm/__init__.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/fsm/factory.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/fsm/state.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/hook.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/spec.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/argument.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/__init__.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/prompt_info.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/prompt_notice.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/run_info.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/run_no.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/script.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/state_name.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/stdout.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/trace_info.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/registrars/trace_nos.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/session/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/session/monitor.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/session/session.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/plugin/plugins/session/spawn.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/call.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/commands.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/events.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/exc.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/runner.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/types.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/hook.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/skip.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/spec.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/_script.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/compose.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/concurrency.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/filter.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/global_.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/local_.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/peek.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/repeat.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/__init__.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/custom.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/factory.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/prompt.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/stream.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/test/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/test/py38.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/__init__.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/func.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/multiprocessing_logging.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/path.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/peek.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/profile.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/run.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/thread_exception.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/thread_task_id.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/done_callback/__init__.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/done_callback/task.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/done_callback/thread.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/done_callback/union.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/pubsub/__init__.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/pubsub/broker.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 nextline-0.5.5/nextline/utils/pubsub/item.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 nextline-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nextline-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 nextline-0.5.5/README.md
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 nextline-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nextline-0.5.5/PKG-INFO
```

### Comparing `nextline-0.5.4/nextline/count.py` & `nextline-0.5.5/nextline/count.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/main.py` & `nextline-0.5.5/nextline/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import reprlib
 from contextlib import asynccontextmanager
 from logging import getLogger
 from pathlib import Path
 from types import CodeType
 from typing import Any, AsyncIterator, Callable, Optional, Tuple, Union
 
+from .continuous import Continuous
 from .fsm import Machine
 from .spawned import PdbCommand
 from .types import (
     PromptInfo,
     PromptNo,
     PromptNotice,
     RunInfo,
@@ -44,19 +45,20 @@
 
     def __init__(
         self,
         statement: Union[str, Path, CodeType, Callable[[], Any]],
         run_no_start_from: int = 1,
         timeout_on_exit: float = 3,
     ):
-
         logger = getLogger(__name__)
         logger.debug(f'statement: {reprlib.repr(statement)}')
         logger.debug(f"The run number starts from {run_no_start_from}")
 
+        self._continuous = Continuous(self)
+
         self._machine = Machine(
             run_no_start_from=run_no_start_from,
             statement=statement,
         )
         self._timeout_on_exit = timeout_on_exit
         self._registry = self._machine.registry
 
@@ -67,21 +69,23 @@
         # e.g., "<Nextline 'running'>"
         return f'<{self.__class__.__name__} {self.state!r}>'
 
     async def start(self) -> None:
         if self._started:
             return
         self._started = True
+        await self._continuous.start()
         await self._machine.initialize()  # type: ignore
 
     async def close(self) -> None:
         if self._closed:
             return
         self._closed = True
         await self._machine.close()  # type: ignore
+        await self._continuous.close()
 
     async def __aenter__(self):
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         del exc_type, exc_value, traceback
@@ -96,14 +100,29 @@
         '''Yield when the script execution is started and exit when it has finished.'''
         await self._machine.run()  # type: ignore
         try:
             yield self
         finally:
             await self._machine.wait()
 
+    async def run_and_continue(self) -> None:
+        '''Start the script execution in the non-interactive mode.
+
+        Returns when the run has started.
+        '''
+        await self._continuous.run_and_continue()
+
+    async def run_continue_and_wait(self, started: asyncio.Event) -> None:
+        '''Start the script execution in the non-interactive mode and wait until end.
+
+        Similar to run_and_continue() but returns when the run has finished.
+        The event started is set when the run has started.
+        '''
+        await self._continuous.run_continue_and_wait(started)
+
     async def send_pdb_command(
         self, command: str, prompt_no: int, trace_no: int
     ) -> None:
         logger = getLogger(__name__)
         logger.debug(f'send_pdb_command({command!r}, {prompt_no!r}, {trace_no!r})')
         item = PdbCommand(
             trace_no=TraceNo(trace_no),
@@ -204,15 +223,14 @@
 
         # Alternative implementation under development
         # return self._subscribe_prompt_info_for(trace_no)
 
     async def _subscribe_prompt_info_for(
         self, trace_no: int
     ) -> AsyncIterator[PromptInfo]:
-
         merged = merge_aiters(
             self.subscribe_prompt_info(),
             self.subscribe_trace_info(),
         )
         async for _, info in merged:
             if not info.trace_no == trace_no:  # type: ignore
                 continue
@@ -228,7 +246,14 @@
         return self._registry.latest(key)
 
     def subscribe(self, key, last: Optional[bool] = True) -> AsyncIterator[Any]:
         return self._registry.subscribe(key, last=last)
 
     def subscribe_stdout(self) -> AsyncIterator[StdoutInfo]:
         return self.subscribe("stdout", last=False)
+
+    @property
+    def continuous_enabled(self) -> bool:
+        return self._continuous.enabled
+
+    def subscribe_continuous_enabled(self) -> AsyncIterator[bool]:
+        return self._continuous.subscribe_enabled()
```

### Comparing `nextline-0.5.4/nextline/types.py` & `nextline-0.5.5/nextline/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/fsm/factory.py` & `nextline-0.5.5/nextline/fsm/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/fsm/state.py` & `nextline-0.5.5/nextline/fsm/state.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/spec.py` & `nextline-0.5.5/nextline/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/__init__.py` & `nextline-0.5.5/nextline/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/argument.py` & `nextline-0.5.5/nextline/plugin/plugins/argument.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/__init__.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/prompt_info.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/prompt_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/prompt_notice.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/prompt_notice.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/run_info.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/run_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/stdout.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/stdout.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/trace_info.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/trace_info.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/registrars/trace_nos.py` & `nextline-0.5.5/nextline/plugin/plugins/registrars/trace_nos.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/session/monitor.py` & `nextline-0.5.5/nextline/plugin/plugins/session/monitor.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/session/session.py` & `nextline-0.5.5/nextline/plugin/plugins/session/session.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/plugin/plugins/session/spawn.py` & `nextline-0.5.5/nextline/plugin/plugins/session/spawn.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/__init__.py` & `nextline-0.5.5/nextline/spawned/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/call.py` & `nextline-0.5.5/nextline/spawned/call.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/events.py` & `nextline-0.5.5/nextline/spawned/events.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/runner.py` & `nextline-0.5.5/nextline/spawned/runner.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/types.py` & `nextline-0.5.5/nextline/spawned/types.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/utils.py` & `nextline-0.5.5/nextline/spawned/utils.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/hook.py` & `nextline-0.5.5/nextline/spawned/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/skip.py` & `nextline-0.5.5/nextline/spawned/plugin/skip.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/spec.py` & `nextline-0.5.5/nextline/spawned/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/__init__.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/_script.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/_script.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/compose.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/compose.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/concurrency.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/concurrency.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/filter.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/global_.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/global_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/local_.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/local_.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/peek.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/repeat.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/repeat.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/custom.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/custom.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/factory.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/factory.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/prompt.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/prompt.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/spawned/plugin/plugins/pdb_/stream.py` & `nextline-0.5.5/nextline/spawned/plugin/plugins/pdb_/stream.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/test/py38.py` & `nextline-0.5.5/nextline/test/py38.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/__init__.py` & `nextline-0.5.5/nextline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/func.py` & `nextline-0.5.5/nextline/utils/func.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/multiprocessing_logging.py` & `nextline-0.5.5/nextline/utils/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/peek.py` & `nextline-0.5.5/nextline/utils/peek.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/run.py` & `nextline-0.5.5/nextline/utils/run.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/thread_task_id.py` & `nextline-0.5.5/nextline/utils/thread_task_id.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/done_callback/task.py` & `nextline-0.5.5/nextline/utils/done_callback/task.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/done_callback/thread.py` & `nextline-0.5.5/nextline/utils/done_callback/thread.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/done_callback/union.py` & `nextline-0.5.5/nextline/utils/done_callback/union.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/pubsub/broker.py` & `nextline-0.5.5/nextline/utils/pubsub/broker.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/nextline/utils/pubsub/item.py` & `nextline-0.5.5/nextline/utils/pubsub/item.py`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/.gitignore` & `nextline-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/LICENSE` & `nextline-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/README.md` & `nextline-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/pyproject.toml` & `nextline-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextline-0.5.4/PKG-INFO` & `nextline-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextline
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Python library for controlling Python scripts execution
 Project-URL: Homepage, https://github.com/simonsobs/nextline#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline/issues
 Project-URL: Source, https://github.com/simonsobs/nextline
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
```

