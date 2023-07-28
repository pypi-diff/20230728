# Comparing `tmp/multimcts-0.4.tar.gz` & `tmp/multimcts-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.4.tar", last modified: Wed Jul 26 20:09:30 2023, max compression
+gzip compressed data, was "multimcts-0.4.1.tar", last modified: Fri Jul 28 21:07:22 2023, max compression
```

## Comparing `multimcts-0.4.tar` & `multimcts-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.548791 multimcts-0.4/
--rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.4/LICENSE
--rw-r--r--   0 taylorvance   (501) staff       (20)     2988 2023-07-26 20:09:30.548644 multimcts-0.4/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     2674 2023-07-26 13:34:49.000000 multimcts-0.4/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.547936 multimcts-0.4/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.4/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   543355 2023-07-26 20:06:50.000000 multimcts-0.4/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)   544050 2023-07-26 20:06:46.000000 multimcts-0.4/multimcts/mcts.cpp
--rw-r--r--   0 taylorvance   (501) staff       (20)    11549 2023-07-26 20:06:41.000000 multimcts-0.4/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-26 20:09:30.548455 multimcts-0.4/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2988 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      250 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-26 20:09:30.000000 multimcts-0.4/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.4/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-26 20:09:30.548837 multimcts-0.4/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      617 2023-07-26 20:09:15.000000 multimcts-0.4/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.694677 multimcts-0.4.1/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.4.1/LICENSE
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:07:22.694542 multimcts-0.4.1/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2673 2023-07-28 21:05:02.000000 multimcts-0.4.1/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.693800 multimcts-0.4.1/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.4.1/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   529256 2023-07-27 19:57:49.000000 multimcts-0.4.1/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)   529951 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts/mcts.cpp
+-rw-r--r--   0 taylorvance   (501) staff       (20)    10793 2023-07-28 14:44:52.000000 multimcts-0.4.1/multimcts/mcts.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)    11224 2023-07-28 13:26:02.000000 multimcts-0.4.1/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.694335 multimcts-0.4.1/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      268 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.4.1/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-28 21:07:22.694740 multimcts-0.4.1/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      619 2023-07-27 02:14:35.000000 multimcts-0.4.1/setup.py
```

### Comparing `multimcts-0.4/LICENSE` & `multimcts-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multimcts-0.4/PKG-INFO` & `multimcts-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.4
+Version: 0.4.1
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,53 +13,44 @@
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
 
 
 ## Features
 
-- Efficient MCTS implementation
+- Efficient (largely C-compiled) MCTS implementation
 - Support for any number of players/teams
 - Easily create AI for any board game
 
 
-## Game Implementation
+## Usage
 
 ### For your game, you will need to:
-- Represent the game state in code
+- Represent a game state in code
 - Identify all legal moves
 - Determine if the game is over and who won
 
 ### You do NOT need to:
 - Understand strategy
 - Have domain knowledge
 - Evaluate the favorability of a game state
 
-
-## Installation
-
+You can install with pip.
 ```bash
 pip install multimcts
 ```
 
-
-## Usage
-
-To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see the [Tic-Tac-Toe](https://github.com/taylorvance/multimcts/blob/main/examples/tictactoe.py) example):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
-Then you can use MCTS to search for the best move. It will search until some limit is reached.
-```python
-state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
-```
-
+Then you can use MCTS to search for the best move. It will search until your defined limit is reached. The following shows how to simulate a game using MCTS:
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
```

### Comparing `multimcts-0.4/README.md` & `multimcts-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
 
 
 ## Features
 
-- Efficient MCTS implementation
+- Efficient (largely C-compiled) MCTS implementation
 - Support for any number of players/teams
 - Easily create AI for any board game
 
 
-## Game Implementation
+## Usage
 
 ### For your game, you will need to:
-- Represent the game state in code
+- Represent a game state in code
 - Identify all legal moves
 - Determine if the game is over and who won
 
 ### You do NOT need to:
 - Understand strategy
 - Have domain knowledge
 - Evaluate the favorability of a game state
 
-
-## Installation
-
+You can install with pip.
 ```bash
 pip install multimcts
 ```
 
-
-## Usage
-
-To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see the [Tic-Tac-Toe](https://github.com/taylorvance/multimcts/blob/main/examples/tictactoe.py) example):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
-Then you can use MCTS to search for the best move. It will search until some limit is reached.
-```python
-state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
-```
-
+Then you can use MCTS to search for the best move. It will search until your defined limit is reached. The following shows how to simulate a game using MCTS:
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
```

### Comparing `multimcts-0.4/multimcts/mcts.c` & `multimcts-0.4.1/multimcts/mcts.c`

 * *Files 2% similar despite different names*

```diff
@@ -980,51 +980,102 @@
   "multimcts/mcts.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9multimcts_4mcts_Node;
 struct __pyx_obj_9multimcts_4mcts_MCTS;
+struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate;
+
+/* "multimcts/mcts.pyx":225
+ *         return child
+ * 
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
+ *         """Step 3: Simulation (aka playout/rollout)
+ *         Play out a game, from the given node to termination, and return the final reward.
+ */
+struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate {
+  int __pyx_n;
+  PyObject *heuristic;
+};
 
 /* "multimcts/mcts.pyx":49
  * 
  * 
  * cdef class Node:             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
- * 
+ *     Args:
  */
 struct __pyx_obj_9multimcts_4mcts_Node {
   PyObject_HEAD
-  PyObject *_state;
-  PyObject *_move;
-  std::string _team;
-  struct __pyx_obj_9multimcts_4mcts_Node *_parent;
-  PyObject *_children;
-  PyObject *_remaining_moves;
-  std::map<std::string,float>  _total_reward;
-  int _num_visits;
-  double log_visits;
-  int _is_terminal;
-  int _is_fully_expanded;
+  struct __pyx_vtabstruct_9multimcts_4mcts_Node *__pyx_vtab;
+  PyObject *state;
+  PyObject *move;
+  PyObject *team;
+  std::string cteam;
+  struct __pyx_obj_9multimcts_4mcts_Node *parent;
+  PyObject *children;
+  PyObject *remaining_moves;
+  std::map<std::string,double>  rewards;
+  int visits;
+  int is_terminal;
+  int is_fully_expanded;
+  double avg_reward;
+  double sqrtlog_visits;
+  double invsqrt_visits;
 };
 
 
-/* "multimcts/mcts.pyx":114
+/* "multimcts/mcts.pyx":134
  * 
  * 
  * cdef class MCTS:             # <<<<<<<<<<<<<<
  *     cdef double exploration_bias
  * 
  */
 struct __pyx_obj_9multimcts_4mcts_MCTS {
   PyObject_HEAD
+  struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *__pyx_vtab;
   double exploration_bias;
 };
 
 
+
+/* "multimcts/mcts.pyx":49
+ * 
+ * 
+ * cdef class Node:             # <<<<<<<<<<<<<<
+ *     """Represents a game state node in the MCTS search tree.
+ *     Args:
+ */
+
+struct __pyx_vtabstruct_9multimcts_4mcts_Node {
+  PyObject *(*apply_rewards)(struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> );
+  double (*ucb)(struct __pyx_obj_9multimcts_4mcts_Node *, double, double);
+};
+static struct __pyx_vtabstruct_9multimcts_4mcts_Node *__pyx_vtabptr_9multimcts_4mcts_Node;
+
+
+/* "multimcts/mcts.pyx":134
+ * 
+ * 
+ * cdef class MCTS:             # <<<<<<<<<<<<<<
+ *     cdef double exploration_bias
+ * 
+ */
+
+struct __pyx_vtabstruct_9multimcts_4mcts_MCTS {
+  struct __pyx_obj_9multimcts_4mcts_Node *(*select)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+  struct __pyx_obj_9multimcts_4mcts_Node *(*expand)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+  std::map<std::string,double>  (*simulate)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args);
+  PyObject *(*backpropagate)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> );
+  struct __pyx_obj_9multimcts_4mcts_Node *(*get_best_child)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+};
+static struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *__pyx_vtabptr_9multimcts_4mcts_MCTS;
+
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
@@ -1091,21 +1142,14 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1134,14 +1178,253 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
+/* Profile.proto */
+#ifndef CYTHON_PROFILE
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+  #define CYTHON_PROFILE 0
+#else
+  #define CYTHON_PROFILE 1
+#endif
+#endif
+#ifndef CYTHON_TRACE_NOGIL
+  #define CYTHON_TRACE_NOGIL 0
+#else
+  #if CYTHON_TRACE_NOGIL && !defined(CYTHON_TRACE)
+    #define CYTHON_TRACE 1
+  #endif
+#endif
+#ifndef CYTHON_TRACE
+  #define CYTHON_TRACE 0
+#endif
+#if CYTHON_TRACE
+  #undef CYTHON_PROFILE_REUSE_FRAME
+#endif
+#ifndef CYTHON_PROFILE_REUSE_FRAME
+  #define CYTHON_PROFILE_REUSE_FRAME 0
+#endif
+#if CYTHON_PROFILE || CYTHON_TRACE
+  #include "compile.h"
+  #include "frameobject.h"
+  #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #if CYTHON_PROFILE_REUSE_FRAME
+    #define CYTHON_FRAME_MODIFIER static
+    #define CYTHON_FRAME_DEL(frame)
+  #else
+    #define CYTHON_FRAME_MODIFIER
+    #define CYTHON_FRAME_DEL(frame) Py_CLEAR(frame)
+  #endif
+  #define __Pyx_TraceDeclarations\
+      static PyCodeObject *__pyx_frame_code = NULL;\
+      CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
+      int __Pyx_use_tracing = 0;
+  #define __Pyx_TraceFrameInit(codeobj)\
+      if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
+#if PY_VERSION_HEX >= 0x030b00a2
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+#elif PY_VERSION_HEX >= 0x030a00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->cframe->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                 || tstate->c_profilefunc != NULL);\
+      } while (0)
+#else
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                         || tstate->c_profilefunc != NULL);\
+      } while (0)
+#endif
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  if (nogil) {\
+      if (CYTHON_TRACE_NOGIL) {\
+          PyThreadState *tstate;\
+          PyGILState_STATE state = PyGILState_Ensure();\
+          tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 1, 1)) {\
+              __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          }\
+          PyGILState_Release(state);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  } else {\
+      PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #else
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  {   PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #endif
+  #define __Pyx_TraceException()\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 1)) {\
+          __Pyx_EnterTracing(tstate);\
+          PyObject *exc_info = __Pyx_GetExceptionTuple(tstate);\
+          if (exc_info) {\
+              if (CYTHON_TRACE && tstate->c_tracefunc)\
+                  tstate->c_tracefunc(\
+                      tstate->c_traceobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              tstate->c_profilefunc(\
+                  tstate->c_profileobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              Py_DECREF(exc_info);\
+          }\
+          __Pyx_LeaveTracing(tstate);\
+      }\
+  }
+  static void __Pyx_call_return_trace_func(PyThreadState *tstate, PyFrameObject *frame, PyObject *result) {
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_EnterTracing(tstate);
+      if (CYTHON_TRACE && tstate->c_tracefunc)
+          tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_RETURN, result);
+      if (tstate->c_profilefunc)
+          tstate->c_profilefunc(tstate->c_profileobj, frame, PyTrace_RETURN, result);
+      CYTHON_FRAME_DEL(frame);
+      __Pyx_LeaveTracing(tstate);
+      __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0)) {\
+                  __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+              }\
+              PyGILState_Release(state);\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0)) {\
+              __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0)) {\
+          __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+      }\
+  }
+  #endif
+  static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno);
+  static int __Pyx_TraceSetupAndCall(PyCodeObject** code, PyFrameObject** frame, PyThreadState* tstate, const char *funcname, const char *srcfile, int firstlineno);
+#else
+  #define __Pyx_TraceDeclarations
+  #define __Pyx_TraceFrameInit(codeobj)
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)   if ((1)); else goto_error;
+  #define __Pyx_TraceException()
+  #define __Pyx_TraceReturn(result, nogil)
+#endif
+#if CYTHON_TRACE
+  static int __Pyx_call_line_trace_func(PyThreadState *tstate, PyFrameObject *frame, int lineno) {
+      int ret;
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_PyFrame_SetLineNumber(frame, lineno);
+      __Pyx_EnterTracing(tstate);
+      ret = tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_LINE, NULL);
+      __Pyx_LeaveTracing(tstate);
+      if (likely(!ret)) {
+          __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+      } else {
+          Py_XDECREF(type);
+          Py_XDECREF(value);
+          Py_XDECREF(traceback);
+      }
+      return ret;
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              int ret = 0;\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+                  ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              }\
+              PyGILState_Release(state);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+              int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+          int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+          if (unlikely(ret)) goto_error;\
+      }\
+  }
+  #endif
+#else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)   if ((1)); else goto_error;
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
@@ -1258,14 +1541,19 @@
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1316,17 +1604,14 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* pop.proto */
@@ -1365,38 +1650,14 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -1412,16 +1673,76 @@
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* append.proto */
 static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
 
-/* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
+/* PyIntCompare.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
+/* pyobject_as_double.proto */
+static double __Pyx__PyObject_AsDouble(PyObject* obj);
+#if CYTHON_COMPILING_IN_PYPY
+#define __Pyx_PyObject_AsDouble(obj)\
+(likely(PyFloat_CheckExact(obj)) ? PyFloat_AS_DOUBLE(obj) :\
+ likely(PyInt_CheckExact(obj)) ?\
+ PyFloat_AsDouble(obj) : __Pyx__PyObject_AsDouble(obj))
+#else
+#define __Pyx_PyObject_AsDouble(obj)\
+((likely(PyFloat_CheckExact(obj))) ?\
+ PyFloat_AS_DOUBLE(obj) : __Pyx__PyObject_AsDouble(obj))
+#endif
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
@@ -1451,78 +1772,37 @@
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
-
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
-/* HasAttr.proto */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
-
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
+/* SetVTable.proto */
+static int __Pyx_SetVtable(PyObject *dict, void *vtable);
+
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
-/* ObjectGetItem.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
-#else
-#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
-#endif
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1598,18 +1878,14 @@
 
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
-/* GetNameInClass.proto */
-#define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
-static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1709,14 +1985,21 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+static PyObject *__pyx_f_9multimcts_4mcts_4Node_apply_rewards(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, std::map<std::string,double>  __pyx_v_crewards); /* proto*/
+static double __pyx_f_9multimcts_4mcts_4Node_ucb(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, double __pyx_v_exploration_bias, double __pyx_v_parent_sqrtlog_visits); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_expand(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
+static std::map<std::string,double>  __pyx_f_9multimcts_4mcts_4MCTS_simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args); /* proto*/
+static PyObject *__pyx_f_9multimcts_4mcts_4MCTS_backpropagate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, std::map<std::string,double>  __pyx_v_crewards); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_get_best_child(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
 
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'libcpp.utility' */
 
 /* Module declarations from 'libcpp.map' */
 
@@ -1735,105 +2018,86 @@
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *, PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
-static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &); /*proto*/
-static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *); /*proto*/
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____double(std::map<std::string,double>  const &); /*proto*/
+static std::map<std::string,double>  __pyx_convert_map_from_py_std_3a__3a_string__and_double(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "multimcts.mcts"
 extern int __pyx_module_is_main_multimcts__mcts;
 int __pyx_module_is_main_multimcts__mcts = 0;
 
 /* Implementation of 'multimcts.mcts' */
-static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_pop[] = "pop";
-static const char __pyx_k_val[] = "val";
 static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_List[] = "List";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Move[] = "Move";
 static const char __pyx_k_Node[] = "Node";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_Team[] = "Team";
-static const char __pyx_k_ckey[] = "ckey";
 static const char __pyx_k_dict[] = "__dict__";
-static const char __pyx_k_item[] = "item";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_move[] = "move";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Union[] = "Union";
-static const char __pyx_k_child[] = "child";
-static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_state[] = "state";
-static const char __pyx_k_visit[] = "visit";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_choice[] = "choice";
-static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_parent[] = "parent";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
-static const char __pyx_k_reward[] = "reward";
-static const char __pyx_k_select[] = "select";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Rewards[] = "Rewards";
-static const char __pyx_k_creward[] = "creward";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_shuffle[] = "shuffle";
-static const char __pyx_k_children[] = "children";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_max_time[] = "max_time";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_GameState[] = "GameState";
 static const char __pyx_k_heuristic[] = "heuristic";
 static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_make_move[] = "make_move";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
-static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_get_reward[] = "get_reward";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_is_terminal[] = "is_terminal";
 static const char __pyx_k_return_type[] = "return_type";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
-static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_stringsource[] = "stringsource";
-static const char __pyx_k_backpropagate[] = "backpropagate";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
-static const char __pyx_k_get_best_child[] = "get_best_child";
 static const char __pyx_k_max_iterations[] = "max_iterations";
 static const char __pyx_k_multimcts_mcts[] = "multimcts.mcts";
 static const char __pyx_k_must_be_one_of[] = ", must be one of ";
 static const char __pyx_k_get_legal_moves[] = "get_legal_moves";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
-static const char __pyx_k_remaining_moves[] = "remaining_moves";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_exploration_bias[] = "exploration_bias";
 static const char __pyx_k_get_current_team[] = "get_current_team";
 static const char __pyx_k_pyx_unpickle_MCTS[] = "__pyx_unpickle_MCTS";
 static const char __pyx_k_pyx_unpickle_Node[] = "__pyx_unpickle_Node";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_multimcts_mcts_pyx[] = "multimcts/mcts.pyx";
@@ -1845,17 +2109,16 @@
 static const char __pyx_k_GameState_get_legal_moves[] = "GameState.get_legal_moves";
 static const char __pyx_k_GameState_get_current_team[] = "GameState.get_current_team";
 static const char __pyx_k_GameState_must_implement_get_cur[] = "GameState must implement get_current_team.";
 static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
 static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
 static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
 static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
-static const char __pyx_k_Tried_to_expand_a_node_with_no_r[] = "Tried to expand a node with no remaining moves.";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))";
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_GameState;
 static PyObject *__pyx_n_u_GameState;
 static PyObject *__pyx_n_s_GameState_get_current_team;
 static PyObject *__pyx_n_s_GameState_get_legal_moves;
@@ -1865,167 +2128,135 @@
 static PyObject *__pyx_kp_u_GameState_must_implement_get_cur;
 static PyObject *__pyx_kp_u_GameState_must_implement_get_leg;
 static PyObject *__pyx_kp_u_GameState_must_implement_get_rew;
 static PyObject *__pyx_kp_u_GameState_must_implement_is_term;
 static PyObject *__pyx_kp_u_GameState_must_implement_make_mo;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
-static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_u_Invalid_return_type;
 static PyObject *__pyx_n_s_List;
 static PyObject *__pyx_n_s_MCTS;
 static PyObject *__pyx_n_s_Move;
 static PyObject *__pyx_n_s_Node;
 static PyObject *__pyx_kp_u_None;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_kp_u_One_or_more_of_max_time_max_iter;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Rewards;
 static PyObject *__pyx_n_s_Team;
-static PyObject *__pyx_kp_u_Tried_to_expand_a_node_with_no_r;
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_append;
-static PyObject *__pyx_n_s_backpropagate;
-static PyObject *__pyx_n_s_child;
-static PyObject *__pyx_n_s_children;
 static PyObject *__pyx_n_s_choice;
-static PyObject *__pyx_n_s_ckey;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_creward;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_expand;
 static PyObject *__pyx_n_s_exploration_bias;
-static PyObject *__pyx_n_s_get_best_child;
 static PyObject *__pyx_n_s_get_current_team;
 static PyObject *__pyx_n_s_get_legal_moves;
 static PyObject *__pyx_n_s_get_reward;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_heuristic;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_is_terminal;
-static PyObject *__pyx_n_s_item;
-static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_iteritems;
-static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_make_move;
 static PyObject *__pyx_n_s_max_iterations;
 static PyObject *__pyx_n_s_max_time;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_move;
 static PyObject *__pyx_n_u_move;
 static PyObject *__pyx_n_s_multimcts_mcts;
 static PyObject *__pyx_kp_s_multimcts_mcts_pyx;
 static PyObject *__pyx_kp_u_must_be_one_of;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
-static PyObject *__pyx_n_s_node;
 static PyObject *__pyx_n_u_node;
 static PyObject *__pyx_n_s_parent;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pop;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_MCTS;
 static PyObject *__pyx_n_s_pyx_unpickle_Node;
+static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_random;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_remaining_moves;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_return_type;
-static PyObject *__pyx_n_s_reward;
-static PyObject *__pyx_n_s_select;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shuffle;
-static PyObject *__pyx_n_s_simulate;
 static PyObject *__pyx_n_s_state;
 static PyObject *__pyx_n_u_state;
-static PyObject *__pyx_n_s_staticmethod;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_s_update;
-static PyObject *__pyx_n_s_val;
-static PyObject *__pyx_n_s_visit;
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
-static PyObject *__pyx_int_24284988;
-static PyObject *__pyx_int_53904430;
+static PyObject *__pyx_int_0;
+static PyObject *__pyx_int_56097295;
+static PyObject *__pyx_int_59888949;
 static PyObject *__pyx_int_82662024;
+static PyObject *__pyx_int_99932858;
 static PyObject *__pyx_int_203704333;
-static PyObject *__pyx_int_227935910;
 static PyObject *__pyx_int_231097371;
-static PyObject *__pyx_tuple_;
+static PyObject *__pyx_codeobj_;
 static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
+static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
+static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__3;
+static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
 /* Late includes */
 
 /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
@@ -2045,29 +2276,32 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj_)
   __Pyx_RefNannySetupContext("get_current_team", 0);
+  __Pyx_TraceCall("get_current_team", __pyx_f[0], 22, 0, __PYX_ERR(0, 22, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 24, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":22
  * 
@@ -2079,92 +2313,97 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves[] = "Returns a list of all legal moves from this state.";
+static char __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves[] = "List of all legal moves from this state.";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves = {"get_legal_moves", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_legal_moves (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__3)
   __Pyx_RefNannySetupContext("get_legal_moves", 0);
+  __Pyx_TraceCall("get_legal_moves", __pyx_f[0], 26, 0, __PYX_ERR(0, 26, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 28, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_4make_move[] = "Returns a new GameState, which is the result of applying the given move to this state.\n        Note: The current state (self) should NOT be modified. Rather, modify a copy of it.\n        ";
+static char __pyx_doc_9multimcts_4mcts_9GameState_4make_move[] = "A new GameState--the result of applying the given move to this state.\n        Note: The current state (self) should NOT be modified. Rather, modify a copy of it.\n        ";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_5make_move = {"make_move", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_9GameState_5make_move, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_9GameState_4make_move};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   CYTHON_UNUSED PyObject *__pyx_v_move = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -2222,184 +2461,196 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__5)
   __Pyx_RefNannySetupContext("make_move", 0);
+  __Pyx_TraceCall("make_move", __pyx_f[0], 30, 0, __PYX_ERR(0, 30, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 34, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal[] = "Checks if the game is over.";
+static char __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal[] = "Is the game over?";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal = {"is_terminal", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_terminal (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__7)
   __Pyx_RefNannySetupContext("is_terminal", 0);
+  __Pyx_TraceCall("is_terminal", __pyx_f[0], 36, 0, __PYX_ERR(0, 36, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_8get_reward[] = "Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}\n        Note: This method is only called on terminal states.\n        ";
+static char __pyx_doc_9multimcts_4mcts_9GameState_8get_reward[] = "The reward earned by the team that played the game-ending move (the \"terminal team\", or the team from the previous state).\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}\n        Note: This method is only called on terminal states.\n        ";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_9get_reward = {"get_reward", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_9get_reward, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_8get_reward};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_reward (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_8get_reward(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__9)
   __Pyx_RefNannySetupContext("get_reward", 0);
+  __Pyx_TraceCall("get_reward", __pyx_f[0], 40, 0, __PYX_ERR(0, 40, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":75
- *     cdef bint _is_fully_expanded
+/* "multimcts/mcts.pyx":72
+ *     cdef double avg_reward, sqrtlog_visits, invsqrt_visits
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self._state = state
- *         self._parent = parent
+ *         self.state = state
+ *         self.parent = parent
  */
 
 /* Python wrapper */
 static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent = 0;
@@ -2443,15 +2694,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2462,335 +2713,390 @@
     }
     __pyx_v_state = values[0];
     __pyx_v_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[1]);
     __pyx_v_move = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 72, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parent), __pyx_ptype_9multimcts_4mcts_Node, 1, "parent", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parent), __pyx_ptype_9multimcts_4mcts_Node, 1, "parent", 0))) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), __pyx_v_state, __pyx_v_parent, __pyx_v_move);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  std::map<std::string,double>  __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  std::string __pyx_t_4;
-  std::map<std::string,float>  __pyx_t_5;
-  int __pyx_t_6;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  std::string __pyx_t_6;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_TraceCall("__init__", __pyx_f[0], 72, 0, __PYX_ERR(0, 72, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":76
+  /* "multimcts/mcts.pyx":73
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self._state = state             # <<<<<<<<<<<<<<
- *         self._parent = parent
- *         self._move = move
+ *         self.state = state             # <<<<<<<<<<<<<<
+ *         self.parent = parent
+ *         self.move = move
  */
   __Pyx_INCREF(__pyx_v_state);
   __Pyx_GIVEREF(__pyx_v_state);
-  __Pyx_GOTREF(__pyx_v_self->_state);
-  __Pyx_DECREF(__pyx_v_self->_state);
-  __pyx_v_self->_state = __pyx_v_state;
+  __Pyx_GOTREF(__pyx_v_self->state);
+  __Pyx_DECREF(__pyx_v_self->state);
+  __pyx_v_self->state = __pyx_v_state;
 
-  /* "multimcts/mcts.pyx":77
+  /* "multimcts/mcts.pyx":74
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self._state = state
- *         self._parent = parent             # <<<<<<<<<<<<<<
- *         self._move = move
- *         self._team = str(self._state.get_current_team()).encode()
+ *         self.state = state
+ *         self.parent = parent             # <<<<<<<<<<<<<<
+ *         self.move = move
+ * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_parent));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_parent));
-  __Pyx_GOTREF(__pyx_v_self->_parent);
-  __Pyx_DECREF(((PyObject *)__pyx_v_self->_parent));
-  __pyx_v_self->_parent = __pyx_v_parent;
+  __Pyx_GOTREF(__pyx_v_self->parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v_self->parent));
+  __pyx_v_self->parent = __pyx_v_parent;
 
-  /* "multimcts/mcts.pyx":78
- *         self._state = state
- *         self._parent = parent
- *         self._move = move             # <<<<<<<<<<<<<<
- *         self._team = str(self._state.get_current_team()).encode()
+  /* "multimcts/mcts.pyx":75
+ *         self.state = state
+ *         self.parent = parent
+ *         self.move = move             # <<<<<<<<<<<<<<
  * 
+ *         self.children:List['Node'] = []
  */
   __Pyx_INCREF(__pyx_v_move);
   __Pyx_GIVEREF(__pyx_v_move);
-  __Pyx_GOTREF(__pyx_v_self->_move);
-  __Pyx_DECREF(__pyx_v_self->_move);
-  __pyx_v_self->_move = __pyx_v_move;
-
-  /* "multimcts/mcts.pyx":79
- *         self._parent = parent
- *         self._move = move
- *         self._team = str(self._state.get_current_team()).encode()             # <<<<<<<<<<<<<<
- * 
- *         self._children:List['Node'] = []
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_2), NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_self->_team = __pyx_t_4;
+  __Pyx_GOTREF(__pyx_v_self->move);
+  __Pyx_DECREF(__pyx_v_self->move);
+  __pyx_v_self->move = __pyx_v_move;
 
-  /* "multimcts/mcts.pyx":81
- *         self._team = str(self._state.get_current_team()).encode()
+  /* "multimcts/mcts.pyx":77
+ *         self.move = move
  * 
- *         self._children:List['Node'] = []             # <<<<<<<<<<<<<<
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY
+ *         self.children:List['Node'] = []             # <<<<<<<<<<<<<<
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v_self->_children);
-  __Pyx_DECREF(__pyx_v_self->_children);
-  __pyx_v_self->_children = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v_self->children);
+  __Pyx_DECREF(__pyx_v_self->children);
+  __pyx_v_self->children = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":82
- * 
- *         self._children:List['Node'] = []
- *         self._num_visits = 0             # <<<<<<<<<<<<<<
- *         self.log_visits = -INFINITY
- *         self._total_reward = map[string,float]()
- */
-  __pyx_v_self->_num_visits = 0;
-
-  /* "multimcts/mcts.pyx":83
- *         self._children:List['Node'] = []
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY             # <<<<<<<<<<<<<<
- *         self._total_reward = map[string,float]()
+  /* "multimcts/mcts.pyx":78
  * 
+ *         self.children:List['Node'] = []
+ *         self.visits = 0             # <<<<<<<<<<<<<<
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()
  */
-  __pyx_v_self->log_visits = (-INFINITY);
+  __pyx_v_self->visits = 0;
 
-  /* "multimcts/mcts.pyx":84
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY
- *         self._total_reward = map[string,float]()             # <<<<<<<<<<<<<<
- * 
- *         self._is_terminal = self._state.is_terminal()
+  /* "multimcts/mcts.pyx":79
+ *         self.children:List['Node'] = []
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()             # <<<<<<<<<<<<<<
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
  */
   try {
-    __pyx_t_5 = std::map<std::string,float> ();
+    __pyx_t_2 = std::map<std::string,double> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 84, __pyx_L1_error)
+    __PYX_ERR(0, 79, __pyx_L1_error)
   }
-  __pyx_v_self->_total_reward = __pyx_t_5;
+  __pyx_v_self->rewards = __pyx_t_2;
 
-  /* "multimcts/mcts.pyx":86
- *         self._total_reward = map[string,float]()
- * 
- *         self._is_terminal = self._state.is_terminal()             # <<<<<<<<<<<<<<
- *         if self._is_terminal:
- *             self._is_fully_expanded = True
+  /* "multimcts/mcts.pyx":80
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()             # <<<<<<<<<<<<<<
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_self->_is_terminal = __pyx_t_6;
+  __pyx_v_self->is_terminal = __pyx_t_5;
 
-  /* "multimcts/mcts.pyx":87
- * 
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:             # <<<<<<<<<<<<<<
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []
- */
-  __pyx_t_6 = (__pyx_v_self->_is_terminal != 0);
-  if (__pyx_t_6) {
-
-    /* "multimcts/mcts.pyx":88
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:
- *             self._is_fully_expanded = True             # <<<<<<<<<<<<<<
- *             self._remaining_moves = []
+  /* "multimcts/mcts.pyx":81
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal             # <<<<<<<<<<<<<<
+ *         if self.is_fully_expanded:
+ *             self.remaining_moves = []
+ */
+  __pyx_t_5 = __pyx_v_self->is_terminal;
+  __pyx_v_self->is_fully_expanded = __pyx_t_5;
+
+  /* "multimcts/mcts.pyx":82
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *             self.remaining_moves = []
  *         else:
  */
-    __pyx_v_self->_is_fully_expanded = 1;
+  __pyx_t_5 = (__pyx_v_self->is_fully_expanded != 0);
+  if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":89
- *         if self._is_terminal:
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":83
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:
+ *             self.remaining_moves = []             # <<<<<<<<<<<<<<
  *         else:
- *             self._is_fully_expanded = False
+ *             self.remaining_moves = self.state.get_legal_moves()
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
-    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
-    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
-    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __Pyx_GOTREF(__pyx_v_self->remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->remaining_moves);
+    __pyx_v_self->remaining_moves = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":87
- * 
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:             # <<<<<<<<<<<<<<
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []
+    /* "multimcts/mcts.pyx":82
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *             self.remaining_moves = []
+ *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":91
- *             self._remaining_moves = []
- *         else:
- *             self._is_fully_expanded = False             # <<<<<<<<<<<<<<
- *             self._remaining_moves = self._state.get_legal_moves()
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
- */
-  /*else*/ {
-    __pyx_v_self->_is_fully_expanded = 0;
-
-    /* "multimcts/mcts.pyx":92
+  /* "multimcts/mcts.pyx":85
+ *             self.remaining_moves = []
  *         else:
- *             self._is_fully_expanded = False
- *             self._remaining_moves = self._state.get_legal_moves()             # <<<<<<<<<<<<<<
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
+ *             self.remaining_moves = self.state.get_legal_moves()             # <<<<<<<<<<<<<<
+ *             shuffle(self.remaining_moves)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
+  /*else*/ {
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_1);
-    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
-    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
-    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __Pyx_GOTREF(__pyx_v_self->remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->remaining_moves);
+    __pyx_v_self->remaining_moves = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":93
- *             self._is_fully_expanded = False
- *             self._remaining_moves = self._state.get_legal_moves()
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":86
+ *         else:
+ *             self.remaining_moves = self.state.get_legal_moves()
+ *             shuffle(self.remaining_moves)             # <<<<<<<<<<<<<<
  * 
- *     @property
+ *         # The following are cached for performance.
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_remaining_moves) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_remaining_moves);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_self->remaining_moves) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_self->remaining_moves);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":75
- *     cdef bint _is_fully_expanded
+  /* "multimcts/mcts.pyx":89
+ * 
+ *         # The following are cached for performance.
+ *         self.team = self.state.get_current_team()             # <<<<<<<<<<<<<<
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->team);
+  __Pyx_DECREF(__pyx_v_self->team);
+  __pyx_v_self->team = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "multimcts/mcts.pyx":90
+ *         # The following are cached for performance.
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()             # <<<<<<<<<<<<<<
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0
+ */
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_self->team); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_1), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_self->cteam = __pyx_t_6;
+
+  /* "multimcts/mcts.pyx":91
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ */
+  __pyx_t_5 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+  __pyx_t_7 = (__pyx_t_5 != 0);
+  if (__pyx_t_7) {
+
+    /* "multimcts/mcts.pyx":92
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0             # <<<<<<<<<<<<<<
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0
+ */
+    (__pyx_v_self->rewards[__pyx_v_self->parent->cteam]) = 0.0;
+
+    /* "multimcts/mcts.pyx":91
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ */
+  }
+
+  /* "multimcts/mcts.pyx":93
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0             # <<<<<<<<<<<<<<
+ *         self.invsqrt_visits = 0
+ *         self.avg_reward = 0
+ */
+  __pyx_v_self->sqrtlog_visits = 0.0;
+
+  /* "multimcts/mcts.pyx":94
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0             # <<<<<<<<<<<<<<
+ *         self.avg_reward = 0
+ * 
+ */
+  __pyx_v_self->invsqrt_visits = 0.0;
+
+  /* "multimcts/mcts.pyx":95
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0
+ *         self.avg_reward = 0             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  __pyx_v_self->avg_reward = 0.0;
+
+  /* "multimcts/mcts.pyx":72
+ *     cdef double avg_reward, sqrtlog_visits, invsqrt_visits
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self._state = state
- *         self._parent = parent
+ *         self.state = state
+ *         self.parent = parent
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":96
+/* "multimcts/mcts.pyx":98
  * 
  *     @property
- *     def state(self) -> GameState: return self._state             # <<<<<<<<<<<<<<
+ *     def state(self) -> GameState: return self.state             # <<<<<<<<<<<<<<
  *     @property
- *     def parent(self) -> 'Node': return self._parent
+ *     def rewards(self): return self.rewards
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2800,523 +3106,626 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_TraceCall("__get__", __pyx_f[0], 98, 0, __PYX_ERR(0, 98, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_state);
-  __pyx_r = __pyx_v_self->_state;
+  __Pyx_INCREF(__pyx_v_self->state);
+  __pyx_r = __pyx_v_self->state;
   goto __pyx_L0;
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.Node.state.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":98
- *     def state(self) -> GameState: return self._state
- *     @property
- *     def parent(self) -> 'Node': return self._parent             # <<<<<<<<<<<<<<
+/* "multimcts/mcts.pyx":100
+ *     def state(self) -> GameState: return self.state
  *     @property
- *     def move(self) -> Move: return self._move
+ *     def rewards(self): return self.rewards             # <<<<<<<<<<<<<<
+ * 
+ *     @cython.cdivision(True)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6parent___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_TraceCall("__get__", __pyx_f[0], 100, 0, __PYX_ERR(0, 100, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
-  __pyx_r = ((PyObject *)__pyx_v_self->_parent);
+  __pyx_t_1 = __pyx_convert_map_to_py_std_3a__3a_string____double(__pyx_v_self->rewards); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.Node.rewards.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":100
- *     def parent(self) -> 'Node': return self._parent
- *     @property
- *     def move(self) -> Move: return self._move             # <<<<<<<<<<<<<<
- *     @property
- *     def children(self) -> List['Node']: return self._children
+/* "multimcts/mcts.pyx":103
+ * 
+ *     @cython.cdivision(True)
+ *     cdef apply_rewards(self, map[string,double] crewards):             # <<<<<<<<<<<<<<
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4move___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_f_9multimcts_4mcts_4Node_apply_rewards(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, std::map<std::string,double>  __pyx_v_crewards) {
+  std::pair<std::string,double>  __pyx_v_item;
+  double __pyx_v_total_rewards;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_move);
-  __pyx_r = __pyx_v_self->_move;
-  goto __pyx_L0;
+  std::map<std::string,double> ::iterator __pyx_t_1;
+  std::pair<std::string,double>  __pyx_t_2;
+  int __pyx_t_3;
+  std::string __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("apply_rewards", 0);
+  __Pyx_TraceCall("apply_rewards", __pyx_f[0], 103, 0, __PYX_ERR(0, 103, __pyx_L1_error));
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+  /* "multimcts/mcts.pyx":105
+ *     cdef apply_rewards(self, map[string,double] crewards):
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1             # <<<<<<<<<<<<<<
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))
+ */
+  __pyx_v_self->visits = (__pyx_v_self->visits + 1);
 
-/* "multimcts/mcts.pyx":102
- *     def move(self) -> Move: return self._move
- *     @property
- *     def children(self) -> List['Node']: return self._children             # <<<<<<<<<<<<<<
- *     @property
- *     def remaining_moves(self) -> List[Move]: return self._remaining_moves
+  /* "multimcts/mcts.pyx":107
+ *         self.visits += 1
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))             # <<<<<<<<<<<<<<
+ *         self.invsqrt_visits = 1 / sqrt(self.visits)
+ * 
  */
+  __pyx_v_self->sqrtlog_visits = sqrt(log(__pyx_v_self->visits));
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_8children___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  /* "multimcts/mcts.pyx":108
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))
+ *         self.invsqrt_visits = 1 / sqrt(self.visits)             # <<<<<<<<<<<<<<
+ * 
+ *         cdef pair[string,double] item
+ */
+  __pyx_v_self->invsqrt_visits = (1.0 / sqrt(__pyx_v_self->visits));
 
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+  /* "multimcts/mcts.pyx":111
+ * 
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0             # <<<<<<<<<<<<<<
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:
+ */
+  __pyx_v_total_rewards = 0.0;
+
+  /* "multimcts/mcts.pyx":112
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0
+ *         for item in crewards:             # <<<<<<<<<<<<<<
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ */
+  __pyx_t_1 = __pyx_v_crewards.begin();
+  for (;;) {
+    if (!(__pyx_t_1 != __pyx_v_crewards.end())) break;
+    __pyx_t_2 = *__pyx_t_1;
+    ++__pyx_t_1;
+    __pyx_v_item = __pyx_t_2;
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_children);
-  __pyx_r = __pyx_v_self->_children;
-  goto __pyx_L0;
+    /* "multimcts/mcts.pyx":113
+ *         cdef double total_rewards = 0
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:             # <<<<<<<<<<<<<<
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ */
+    __pyx_t_3 = ((__pyx_v_self->rewards.count(__pyx_v_item.first) == 0) != 0);
+    if (__pyx_t_3) {
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+      /* "multimcts/mcts.pyx":114
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0             # <<<<<<<<<<<<<<
+ *             self.rewards[item.first] += item.second
+ *             total_rewards += self.rewards[item.first]
+ */
+      (__pyx_v_self->rewards[__pyx_v_item.first]) = 0.0;
 
-/* "multimcts/mcts.pyx":104
- *     def children(self) -> List['Node']: return self._children
- *     @property
- *     def remaining_moves(self) -> List[Move]: return self._remaining_moves             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":113
+ *         cdef double total_rewards = 0
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:             # <<<<<<<<<<<<<<
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ */
+    }
+
+    /* "multimcts/mcts.pyx":115
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second             # <<<<<<<<<<<<<<
+ *             total_rewards += self.rewards[item.first]
  * 
- *     @cython.cdivision(True)
  */
+    __pyx_t_4 = __pyx_v_item.first;
+    (__pyx_v_self->rewards[__pyx_t_4]) = ((__pyx_v_self->rewards[__pyx_t_4]) + __pyx_v_item.second);
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+    /* "multimcts/mcts.pyx":116
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ *             total_rewards += self.rewards[item.first]             # <<<<<<<<<<<<<<
+ * 
+ *         if self.parent is not None:
+ */
+    __pyx_v_total_rewards = (__pyx_v_total_rewards + (__pyx_v_self->rewards[__pyx_v_item.first]));
 
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+    /* "multimcts/mcts.pyx":112
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0
+ *         for item in crewards:             # <<<<<<<<<<<<<<
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ */
+  }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
-  __pyx_r = __pyx_v_self->_remaining_moves;
-  goto __pyx_L0;
+  /* "multimcts/mcts.pyx":118
+ *             total_rewards += self.rewards[item.first]
+ * 
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
+ */
+  __pyx_t_3 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+  __pyx_t_5 = (__pyx_t_3 != 0);
+  if (__pyx_t_5) {
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+    /* "multimcts/mcts.pyx":120
+ *         if self.parent is not None:
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits             # <<<<<<<<<<<<<<
+ * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):
+ */
+    __pyx_v_self->avg_reward = (((2.0 * (__pyx_v_self->rewards[__pyx_v_self->parent->cteam])) - __pyx_v_total_rewards) / ((double)__pyx_v_self->visits));
 
-/* "multimcts/mcts.pyx":109
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def visit(self):             # <<<<<<<<<<<<<<
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)
+    /* "multimcts/mcts.pyx":118
+ *             total_rewards += self.rewards[item.first]
+ * 
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
  */
+  }
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("visit (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_2visit(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  /* "multimcts/mcts.pyx":103
+ * 
+ *     @cython.cdivision(True)
+ *     cdef apply_rewards(self, map[string,double] crewards):             # <<<<<<<<<<<<<<
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1
+ */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.Node.apply_rewards", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("visit", 0);
-
-  /* "multimcts/mcts.pyx":110
- *     @cython.wraparound(False)
- *     def visit(self):
- *         self._num_visits += 1             # <<<<<<<<<<<<<<
- *         self.log_visits = log(self._num_visits)
+/* "multimcts/mcts.pyx":122
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
  * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
+ *         """Upper Confidence Bound
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
-  __pyx_v_self->_num_visits = (__pyx_v_self->_num_visits + 1);
 
-  /* "multimcts/mcts.pyx":111
- *     def visit(self):
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)             # <<<<<<<<<<<<<<
+static double __pyx_f_9multimcts_4mcts_4Node_ucb(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, double __pyx_v_exploration_bias, double __pyx_v_parent_sqrtlog_visits) {
+  double __pyx_r;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("ucb", 0);
+  __Pyx_TraceCall("ucb", __pyx_f[0], 122, 0, __PYX_ERR(0, 122, __pyx_L1_error));
+
+  /* "multimcts/mcts.pyx":131
+ *         """
+ *         # ucb = avgR + C * sqrt(ln(N)) * (1/sqrt(n))
+ *         return self.avg_reward + exploration_bias * parent_sqrtlog_visits * self.invsqrt_visits             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_v_self->log_visits = log(__pyx_v_self->_num_visits);
+  __pyx_r = (__pyx_v_self->avg_reward + ((__pyx_v_exploration_bias * __pyx_v_parent_sqrtlog_visits) * __pyx_v_self->invsqrt_visits));
+  goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":109
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def visit(self):             # <<<<<<<<<<<<<<
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)
+  /* "multimcts/mcts.pyx":122
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
+ * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
+ *         """Upper Confidence Bound
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("multimcts.mcts.Node.ucb", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  int __pyx_t_9;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
+  int __pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)             # <<<<<<<<<<<<<<
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->avg_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_self->cteam); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->invsqrt_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_self->_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_self->is_fully_expanded); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __pyx_convert_map_to_py_std_3a__3a_string____float(__pyx_v_self->_total_reward); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_self->is_terminal); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_self->log_visits); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_map_to_py_std_3a__3a_string____double(__pyx_v_self->rewards); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyTuple_New(11); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_self->sqrtlog_visits); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_INCREF(__pyx_v_self->_children);
-  __Pyx_GIVEREF(__pyx_v_self->_children);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_self->_children);
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->visits); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_9 = PyTuple_New(14); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self->children);
+  __Pyx_GIVEREF(__pyx_v_self->children);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_self->children);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2);
-  __Pyx_INCREF(__pyx_v_self->_move);
-  __Pyx_GIVEREF(__pyx_v_self->_move);
-  PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_v_self->_move);
+  PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_t_3);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->_parent));
-  PyTuple_SET_ITEM(__pyx_t_7, 5, ((PyObject *)__pyx_v_self->_parent));
-  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
-  __Pyx_GIVEREF(__pyx_v_self->_remaining_moves);
-  PyTuple_SET_ITEM(__pyx_t_7, 6, __pyx_v_self->_remaining_moves);
-  __Pyx_INCREF(__pyx_v_self->_state);
-  __Pyx_GIVEREF(__pyx_v_self->_state);
-  PyTuple_SET_ITEM(__pyx_t_7, 7, __pyx_v_self->_state);
+  PyTuple_SET_ITEM(__pyx_t_9, 3, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_7, 8, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_9, 4, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_7, 9, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_9, 5, __pyx_t_5);
+  __Pyx_INCREF(__pyx_v_self->move);
+  __Pyx_GIVEREF(__pyx_v_self->move);
+  PyTuple_SET_ITEM(__pyx_t_9, 6, __pyx_v_self->move);
+  __Pyx_INCREF(((PyObject *)__pyx_v_self->parent));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->parent));
+  PyTuple_SET_ITEM(__pyx_t_9, 7, ((PyObject *)__pyx_v_self->parent));
+  __Pyx_INCREF(__pyx_v_self->remaining_moves);
+  __Pyx_GIVEREF(__pyx_v_self->remaining_moves);
+  PyTuple_SET_ITEM(__pyx_t_9, 8, __pyx_v_self->remaining_moves);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_7, 10, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_9, 9, __pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_9, 10, __pyx_t_7);
+  __Pyx_INCREF(__pyx_v_self->state);
+  __Pyx_GIVEREF(__pyx_v_self->state);
+  PyTuple_SET_ITEM(__pyx_t_9, 11, __pyx_v_self->state);
+  __Pyx_INCREF(__pyx_v_self->team);
+  __Pyx_GIVEREF(__pyx_v_self->team);
+  PyTuple_SET_ITEM(__pyx_t_9, 12, __pyx_v_self->team);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_9, 13, __pyx_t_8);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
-  __pyx_v_state = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
+  __pyx_t_8 = 0;
+  __pyx_v_state = ((PyObject*)__pyx_t_9);
+  __pyx_t_9 = 0;
 
   /* "(tree fragment)":6
  *     cdef bint use_setstate
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_7 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_v__dict = __pyx_t_7;
-  __pyx_t_7 = 0;
+  __pyx_t_9 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_v__dict = __pyx_t_9;
+  __pyx_t_9 = 0;
 
   /* "(tree fragment)":7
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
-  __pyx_t_8 = (__pyx_v__dict != Py_None);
-  __pyx_t_9 = (__pyx_t_8 != 0);
-  if (__pyx_t_9) {
+  __pyx_t_10 = (__pyx_v__dict != Py_None);
+  __pyx_t_11 = (__pyx_t_10 != 0);
+  if (__pyx_t_11) {
 
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v__dict);
-    __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_6));
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v__dict);
+    __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_8));
+    __pyx_t_8 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
  *         state += (_dict,)
  *         use_setstate = True             # <<<<<<<<<<<<<<
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  */
     __pyx_v_use_setstate = 1;
 
     /* "(tree fragment)":7
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
     goto __pyx_L3;
   }
 
   /* "(tree fragment)":11
  *         use_setstate = True
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None             # <<<<<<<<<<<<<<
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None             # <<<<<<<<<<<<<<
  *     if use_setstate:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  */
   /*else*/ {
-    __pyx_t_8 = (__pyx_v_self->_children != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
+    __pyx_t_10 = (__pyx_v_self->children != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
+    } else {
+      __pyx_t_11 = __pyx_t_12;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_12 = (__pyx_v_self->move != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
     if (!__pyx_t_10) {
     } else {
-      __pyx_t_9 = __pyx_t_10;
+      __pyx_t_11 = __pyx_t_10;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_10 = (__pyx_v_self->_move != Py_None);
-    __pyx_t_8 = (__pyx_t_10 != 0);
-    if (!__pyx_t_8) {
+    __pyx_t_10 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
     } else {
-      __pyx_t_9 = __pyx_t_8;
+      __pyx_t_11 = __pyx_t_12;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_8 = (((PyObject *)__pyx_v_self->_parent) != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
+    __pyx_t_12 = (__pyx_v_self->remaining_moves != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
     if (!__pyx_t_10) {
     } else {
-      __pyx_t_9 = __pyx_t_10;
+      __pyx_t_11 = __pyx_t_10;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_10 = (__pyx_v_self->_remaining_moves != Py_None);
-    __pyx_t_8 = (__pyx_t_10 != 0);
-    if (!__pyx_t_8) {
+    __pyx_t_10 = (__pyx_v_self->state != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
     } else {
-      __pyx_t_9 = __pyx_t_8;
+      __pyx_t_11 = __pyx_t_12;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_8 = (__pyx_v_self->_state != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
-    __pyx_t_9 = __pyx_t_10;
+    __pyx_t_12 = (__pyx_v_self->team != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
+    __pyx_t_11 = __pyx_t_10;
     __pyx_L4_bool_binop_done:;
-    __pyx_v_use_setstate = __pyx_t_9;
+    __pyx_v_use_setstate = __pyx_t_11;
   }
   __pyx_L3:;
 
   /* "(tree fragment)":12
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
  */
-  __pyx_t_9 = (__pyx_v_use_setstate != 0);
-  if (__pyx_t_9) {
+  __pyx_t_11 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_11) {
 
     /* "(tree fragment)":13
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state             # <<<<<<<<<<<<<<
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_24284988);
-    __Pyx_GIVEREF(__pyx_int_24284988);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_56097295);
+    __Pyx_GIVEREF(__pyx_int_56097295);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_int_56097295);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_7, 2, Py_None);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_9, 2, Py_None);
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_9);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_state);
+    __pyx_t_8 = 0;
+    __pyx_t_9 = 0;
+    __pyx_r = __pyx_t_7;
     __pyx_t_7 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
  */
   }
 
   /* "(tree fragment)":15
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_24284988);
-    __Pyx_GIVEREF(__pyx_int_24284988);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_56097295);
+    __Pyx_GIVEREF(__pyx_int_56097295);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_int_56097295);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_state);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_v_state);
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
-    __pyx_t_5 = 0;
+    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_9);
     __pyx_t_7 = 0;
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_9 = 0;
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
   }
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
@@ -3327,94 +3736,100 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.Node.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.Node.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":117
+/* "multimcts/mcts.pyx":137
  *     cdef double exploration_bias
  * 
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
- * 
+ *         Args:
  */
 
 /* Python wrapper */
 static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n\n        Args:\n            exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.\n                It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).\n                The default \342\210\2322 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.\n        ";
+static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n        Args:\n            exploration_bias (float): The exploration bias, which balances exploration (favoring untested moves) and exploitation (favoring good moves).\n                The default \342\210\2322 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.\n        ";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
 #endif
 static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_exploration_bias;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -3439,79 +3854,90 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 137, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 137, __pyx_L3_error)
     } else {
       __pyx_v_exploration_bias = ((double)1.414);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 137, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_exploration_bias);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_TraceCall("__init__", __pyx_f[0], 137, 0, __PYX_ERR(0, 137, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":125
+  /* "multimcts/mcts.pyx":143
  *                 The default 2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
  *         """
  *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->exploration_bias = __pyx_v_exploration_bias;
 
-  /* "multimcts/mcts.pyx":117
+  /* "multimcts/mcts.pyx":137
  *     cdef double exploration_bias
  * 
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
- * 
+ *         Args:
  */
 
   /* function exit code */
   __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":128
+/* "multimcts/mcts.pyx":146
  * 
  *     @property
- *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
- *         return self.exploration_bias
+ *     def exploration_bias(self) -> float: return self.exploration_bias             # <<<<<<<<<<<<<<
  * 
+ *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3521,65 +3947,52 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "multimcts/mcts.pyx":129
- *     @property
- *     def exploration_bias(self) -> float:
- *         return self.exploration_bias             # <<<<<<<<<<<<<<
- * 
- *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
- */
+  __Pyx_TraceCall("__get__", __pyx_f[0], 146, 0, __PYX_ERR(0, 146, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":128
- * 
- *     @property
- *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
- *         return self.exploration_bias
- * 
- */
-
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.exploration_bias.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":131
- *         return self.exploration_bias
+/* "multimcts/mcts.pyx":148
+ *     def exploration_bias(self) -> float: return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
- * 
+ *         Args:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_2search[] = "Searches for this state's best move until some limit has been reached.\n\n        Args:\n            state (GameState): The game state for which to find the best move.\n            max_time (int|float): The maximum time to search, in seconds.\n            max_iterations (int): The maximum number of selections/simulations to perform.\n            heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.\n            return_type (str): One of \"state\", \"move\", or \"node\".\n        Returns:\n            GameState: A new game state which is the result of applying the best move to the given state.\n        ";
+static char __pyx_doc_9multimcts_4mcts_4MCTS_2search[] = "Searches for this state's best move until some limit has been reached.\n        Args:\n            state (GameState): The game state for which to find the best move.\n            max_time (int|float): The maximum time to search, in seconds.\n            max_iterations (int): The maximum number of selections/simulations to perform.\n            heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.\n            return_type (str): One of \"state\", \"move\", or \"node\".\n        Returns:\n            GameState: A new game state which is the result of applying the best move to the given state.\n        ";
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v_max_time = 0;
   PyObject *__pyx_v_max_iterations = 0;
   PyObject *__pyx_v_heuristic = 0;
   PyObject *__pyx_v_return_type = 0;
   int __pyx_lineno = 0;
@@ -3614,183 +4027,183 @@
         Py_ssize_t index;
         for (index = 1; index < 5 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 131, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_state = values[0];
     __pyx_v_max_time = values[1];
     __pyx_v_max_iterations = values[2];
     __pyx_v_heuristic = values[3];
     __pyx_v_return_type = ((PyObject*)values[4]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 131, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyUnicode_Type), 1, "return_type", 1))) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyUnicode_Type), 1, "return_type", 1))) __PYX_ERR(0, 148, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_state, __pyx_v_max_time, __pyx_v_max_iterations, __pyx_v_heuristic, __pyx_v_return_type);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type) {
   PyObject *__pyx_v_VALID_RETURN_TYPES = NULL;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = NULL;
-  double __pyx_v_exploration_bias;
   double __pyx_v_end_time;
   int __pyx_v_i;
-  PyObject *__pyx_v_child = NULL;
-  PyObject *__pyx_v_reward = NULL;
-  PyObject *__pyx_v_best = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
+  std::map<std::string,double>  __pyx_v_rewards;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   int __pyx_t_8;
   double __pyx_t_9;
-  int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
+  std::map<std::string,double>  __pyx_t_10;
+  struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
+  __Pyx_TraceCall("search", __pyx_f[0], 148, 0, __PYX_ERR(0, 148, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_return_type);
 
-  /* "multimcts/mcts.pyx":143
+  /* "multimcts/mcts.pyx":159
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         return_type = return_type.lower()             # <<<<<<<<<<<<<<
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_return_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_return_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_return_type, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":144
+  /* "multimcts/mcts.pyx":160
  *         """
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}             # <<<<<<<<<<<<<<
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_state) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_move) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_node) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_state) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_move) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_node) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __pyx_v_VALID_RETURN_TYPES = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":145
+  /* "multimcts/mcts.pyx":161
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
-  __pyx_t_4 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 161, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":146
+    /* "multimcts/mcts.pyx":162
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')             # <<<<<<<<<<<<<<
  * 
  *         if max_time is None and max_iterations is None:
  */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_return_type);
     __pyx_t_6 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_return_type);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_return_type);
-    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_return_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_return_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_must_be_one_of);
     __pyx_t_6 += 17;
     __Pyx_GIVEREF(__pyx_kp_u_must_be_one_of);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_must_be_one_of);
-    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 146, __pyx_L1_error)
+    __PYX_ERR(0, 162, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":145
+    /* "multimcts/mcts.pyx":161
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":148
+  /* "multimcts/mcts.pyx":164
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   __pyx_t_4 = (__pyx_v_max_time == Py_None);
@@ -3802,1386 +4215,896 @@
   }
   __pyx_t_8 = (__pyx_v_max_iterations == Py_None);
   __pyx_t_4 = (__pyx_t_8 != 0);
   __pyx_t_5 = __pyx_t_4;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":149
+    /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 149, __pyx_L1_error)
+    __PYX_ERR(0, 165, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":148
+    /* "multimcts/mcts.pyx":164
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":151
+  /* "multimcts/mcts.pyx":167
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
- *         cdef double exploration_bias = self.exploration_bias
+ *         cdef double end_time
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_v_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_v_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":153
- *         node = Node(state)
- * 
- *         cdef double exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":170
  * 
  *         cdef double end_time
+ *         cdef int i = 0             # <<<<<<<<<<<<<<
+ *         if max_time is not None:
+ *             end_time = time() + max_time
  */
-  __pyx_t_9 = __pyx_v_self->exploration_bias;
-  __pyx_v_exploration_bias = __pyx_t_9;
+  __pyx_v_i = 0;
 
-  /* "multimcts/mcts.pyx":157
+  /* "multimcts/mcts.pyx":171
  *         cdef double end_time
- *         cdef int i
+ *         cdef int i = 0
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
- *         if max_iterations is not None:
+ * 
  */
   __pyx_t_5 = (__pyx_v_max_time != Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":158
- *         cdef int i
+    /* "multimcts/mcts.pyx":172
+ *         cdef int i = 0
  *         if max_time is not None:
  *             end_time = time() + max_time             # <<<<<<<<<<<<<<
- *         if max_iterations is not None:
- *             i = max_iterations
+ * 
+ *         while True:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_end_time = __pyx_t_9;
 
-    /* "multimcts/mcts.pyx":157
+    /* "multimcts/mcts.pyx":171
  *         cdef double end_time
- *         cdef int i
+ *         cdef int i = 0
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
- *         if max_iterations is not None:
+ * 
  */
   }
 
-  /* "multimcts/mcts.pyx":159
- *         if max_time is not None:
+  /* "multimcts/mcts.pyx":174
  *             end_time = time() + max_time
- *         if max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = max_iterations
  * 
+ *         while True:             # <<<<<<<<<<<<<<
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)
  */
-  __pyx_t_4 = (__pyx_v_max_iterations != Py_None);
-  __pyx_t_5 = (__pyx_t_4 != 0);
-  if (__pyx_t_5) {
+  while (1) {
 
-    /* "multimcts/mcts.pyx":160
- *             end_time = time() + max_time
- *         if max_iterations is not None:
- *             i = max_iterations             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":175
  * 
  *         while True:
+ *             child = self.select(node)             # <<<<<<<<<<<<<<
+ *             rewards = self.simulate(child, heuristic=heuristic)
+ *             self.backpropagate(child, rewards)
  */
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
-    __pyx_v_i = __pyx_t_10;
+    __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->select(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
+    __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":159
- *         if max_time is not None:
- *             end_time = time() + max_time
- *         if max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = max_iterations
+    /* "multimcts/mcts.pyx":176
+ *         while True:
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
+ *             self.backpropagate(child, rewards)
  * 
  */
-  }
+    __pyx_t_11.__pyx_n = 1;
+    __pyx_t_11.heuristic = __pyx_v_heuristic;
+    __pyx_t_10 = ((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->simulate(__pyx_v_self, __pyx_v_child, &__pyx_t_11); 
+    __pyx_v_rewards = __pyx_t_10;
 
-  /* "multimcts/mcts.pyx":162
- *             i = max_iterations
+    /* "multimcts/mcts.pyx":177
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)
+ *             self.backpropagate(child, rewards)             # <<<<<<<<<<<<<<
  * 
- *         while True:             # <<<<<<<<<<<<<<
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)
+ *             # If there is only one legal move, we don't need to search.
  */
-  while (1) {
+    __pyx_t_2 = ((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->backpropagate(__pyx_v_self, __pyx_v_child, __pyx_v_rewards); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":163
+    /* "multimcts/mcts.pyx":180
+ * 
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:             # <<<<<<<<<<<<<<
+ *                 break
  * 
- *         while True:
- *             child = self.select(node, exploration_bias)             # <<<<<<<<<<<<<<
- *             reward = self.simulate(child, heuristic=heuristic)
- *             self.backpropagate(child, reward)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_select); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_11 = NULL;
-    __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_11)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_11);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_10 = 1;
-      }
+    __pyx_t_5 = (__pyx_v_node->is_fully_expanded != 0);
+    if (__pyx_t_5) {
+    } else {
+      __pyx_t_4 = __pyx_t_5;
+      goto __pyx_L11_bool_binop_done;
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_12 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      if (__pyx_t_11) {
-        __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
-      }
-      __Pyx_INCREF(((PyObject *)__pyx_v_node));
-      __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
-      __Pyx_GIVEREF(__pyx_t_3);
-      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_10, __pyx_t_3);
-      __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_2 = __pyx_v_node->children;
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_5 = ((__pyx_t_6 == 1) != 0);
+    __pyx_t_4 = __pyx_t_5;
+    __pyx_L11_bool_binop_done:;
+    if (__pyx_t_4) {
+
+      /* "multimcts/mcts.pyx":181
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *             if max_time is not None:
+ */
+      goto __pyx_L9_break;
+
+      /* "multimcts/mcts.pyx":180
+ * 
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
     }
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_2);
-    __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":164
- *         while True:
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
- *             self.backpropagate(child, reward)
+    /* "multimcts/mcts.pyx":183
+ *                 break
  * 
+ *             if max_time is not None:             # <<<<<<<<<<<<<<
+ *                 if time() >= end_time:
+ *                     break
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simulate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_v_child);
-    __Pyx_GIVEREF(__pyx_v_child);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_child);
-    __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_4 = (__pyx_v_max_time != Py_None);
+    __pyx_t_5 = (__pyx_t_4 != 0);
+    if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":165
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)
- *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
- * 
- *             if max_time is not None and time() >= end_time:
- */
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_1 = NULL;
-    __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
-        __pyx_t_10 = 1;
+      /* "multimcts/mcts.pyx":184
+ * 
+ *             if max_time is not None:
+ *                 if time() >= end_time:             # <<<<<<<<<<<<<<
+ *                     break
+ *             if max_iterations is not None:
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+        }
       }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_12)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_3);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_3);
-    } else
-    #endif
-    {
-      __pyx_t_2 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (__pyx_t_1) {
-        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1); __pyx_t_1 = NULL;
-      }
-      __Pyx_INCREF(__pyx_v_child);
-      __Pyx_GIVEREF(__pyx_v_child);
-      PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_10, __pyx_v_child);
-      __Pyx_INCREF(__pyx_v_reward);
-      __Pyx_GIVEREF(__pyx_v_reward);
-      PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_10, __pyx_v_reward);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_GE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":167
- *             self.backpropagate(child, reward)
- * 
- *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
- *                 break
+        /* "multimcts/mcts.pyx":185
+ *             if max_time is not None:
+ *                 if time() >= end_time:
+ *                     break             # <<<<<<<<<<<<<<
  *             if max_iterations is not None:
+ *                 i += 1
  */
-    __pyx_t_4 = (__pyx_v_max_time != Py_None);
-    __pyx_t_8 = (__pyx_t_4 != 0);
-    if (__pyx_t_8) {
-    } else {
-      __pyx_t_5 = __pyx_t_8;
-      goto __pyx_L12_bool_binop_done;
-    }
-    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_12);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
-      }
-    }
-    __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_12, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = __pyx_t_8;
-    __pyx_L12_bool_binop_done:;
-    if (__pyx_t_5) {
+        goto __pyx_L9_break;
 
-      /* "multimcts/mcts.pyx":168
+        /* "multimcts/mcts.pyx":184
  * 
- *             if max_time is not None and time() >= end_time:
- *                 break             # <<<<<<<<<<<<<<
+ *             if max_time is not None:
+ *                 if time() >= end_time:             # <<<<<<<<<<<<<<
+ *                     break
  *             if max_iterations is not None:
- *                 i -= 1
  */
-      goto __pyx_L10_break;
+      }
 
-      /* "multimcts/mcts.pyx":167
- *             self.backpropagate(child, reward)
- * 
- *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":183
  *                 break
- *             if max_iterations is not None:
+ * 
+ *             if max_time is not None:             # <<<<<<<<<<<<<<
+ *                 if time() >= end_time:
+ *                     break
  */
     }
 
-    /* "multimcts/mcts.pyx":169
- *             if max_time is not None and time() >= end_time:
- *                 break
+    /* "multimcts/mcts.pyx":186
+ *                 if time() >= end_time:
+ *                     break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i -= 1
- *                 if i <= 0:
+ *                 i += 1
+ *                 if i >= max_iterations:
  */
     __pyx_t_5 = (__pyx_v_max_iterations != Py_None);
-    __pyx_t_8 = (__pyx_t_5 != 0);
-    if (__pyx_t_8) {
+    __pyx_t_4 = (__pyx_t_5 != 0);
+    if (__pyx_t_4) {
 
-      /* "multimcts/mcts.pyx":170
- *                 break
+      /* "multimcts/mcts.pyx":187
+ *                     break
  *             if max_iterations is not None:
- *                 i -= 1             # <<<<<<<<<<<<<<
- *                 if i <= 0:
+ *                 i += 1             # <<<<<<<<<<<<<<
+ *                 if i >= max_iterations:
  *                     break
  */
-      __pyx_v_i = (__pyx_v_i - 1);
+      __pyx_v_i = (__pyx_v_i + 1);
 
-      /* "multimcts/mcts.pyx":171
+      /* "multimcts/mcts.pyx":188
  *             if max_iterations is not None:
- *                 i -= 1
- *                 if i <= 0:             # <<<<<<<<<<<<<<
+ *                 i += 1
+ *                 if i >= max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
-      __pyx_t_8 = ((__pyx_v_i <= 0) != 0);
-      if (__pyx_t_8) {
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_v_max_iterations, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (__pyx_t_4) {
 
-        /* "multimcts/mcts.pyx":172
- *                 i -= 1
- *                 if i <= 0:
+        /* "multimcts/mcts.pyx":189
+ *                 i += 1
+ *                 if i >= max_iterations:
  *                     break             # <<<<<<<<<<<<<<
  * 
- *         best = self.get_best_child(node, exploration_bias)
+ *         cdef Node best = self.get_best_child(node)
  */
-        goto __pyx_L10_break;
+        goto __pyx_L9_break;
 
-        /* "multimcts/mcts.pyx":171
+        /* "multimcts/mcts.pyx":188
  *             if max_iterations is not None:
- *                 i -= 1
- *                 if i <= 0:             # <<<<<<<<<<<<<<
+ *                 i += 1
+ *                 if i >= max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":169
- *             if max_time is not None and time() >= end_time:
- *                 break
+      /* "multimcts/mcts.pyx":186
+ *                 if time() >= end_time:
+ *                     break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i -= 1
- *                 if i <= 0:
+ *                 i += 1
+ *                 if i >= max_iterations:
  */
     }
   }
-  __pyx_L10_break:;
+  __pyx_L9_break:;
 
-  /* "multimcts/mcts.pyx":174
+  /* "multimcts/mcts.pyx":191
  *                     break
  * 
- *         best = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
+ *         cdef Node best = self.get_best_child(node)             # <<<<<<<<<<<<<<
  * 
  *         if return_type == "state":
  */
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 174, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = NULL;
-  __pyx_t_10 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
-    if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-      __Pyx_INCREF(__pyx_t_1);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_12, function);
-      __pyx_t_10 = 1;
-    }
-  }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_12)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    if (__pyx_t_1) {
-      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_1); __pyx_t_1 = NULL;
-    }
-    __Pyx_INCREF(((PyObject *)__pyx_v_node));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_v_best = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->get_best_child(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_best = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":176
- *         best = self.get_best_child(node, exploration_bias)
+  /* "multimcts/mcts.pyx":193
+ *         cdef Node best = self.get_best_child(node)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_state, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_5 = (__pyx_t_8 != 0);
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_state, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":177
+    /* "multimcts/mcts.pyx":194
  * 
  *         if return_type == "state":
  *             return best.state             # <<<<<<<<<<<<<<
  *         elif return_type == "move":
  *             return best.move
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v_best->state);
+    __pyx_r = __pyx_v_best->state;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":176
- *         best = self.get_best_child(node, exploration_bias)
+    /* "multimcts/mcts.pyx":193
+ *         cdef Node best = self.get_best_child(node)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
   }
 
-  /* "multimcts/mcts.pyx":178
+  /* "multimcts/mcts.pyx":195
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_move, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __pyx_t_8 = (__pyx_t_5 != 0);
-  if (__pyx_t_8) {
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_move, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_5 != 0);
+  if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":179
+    /* "multimcts/mcts.pyx":196
  *             return best.state
  *         elif return_type == "move":
  *             return best.move             # <<<<<<<<<<<<<<
  *         elif return_type == "node":
  *             return best
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_move); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v_best->move);
+    __pyx_r = __pyx_v_best->move;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":178
+    /* "multimcts/mcts.pyx":195
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
   }
 
-  /* "multimcts/mcts.pyx":180
+  /* "multimcts/mcts.pyx":197
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_node, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_t_5 = (__pyx_t_8 != 0);
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_node, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":181
+    /* "multimcts/mcts.pyx":198
  *             return best.move
  *         elif return_type == "node":
  *             return best             # <<<<<<<<<<<<<<
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:
+ *     cdef Node select(self, Node node):
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_v_best);
-    __pyx_r = __pyx_v_best;
+    __Pyx_INCREF(((PyObject *)__pyx_v_best));
+    __pyx_r = ((PyObject *)__pyx_v_best);
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":180
+    /* "multimcts/mcts.pyx":197
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":131
- *         return self.exploration_bias
+  /* "multimcts/mcts.pyx":148
+ *     def exploration_bias(self) -> float: return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
- * 
+ *         Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_VALID_RETURN_TYPES);
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
-  __Pyx_XDECREF(__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_reward);
-  __Pyx_XDECREF(__pyx_v_best);
+  __Pyx_XDECREF((PyObject *)__pyx_v_child);
+  __Pyx_XDECREF((PyObject *)__pyx_v_best);
   __Pyx_XDECREF(__pyx_v_return_type);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":183
+/* "multimcts/mcts.pyx":200
  *             return best
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node select(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_4select[] = "Step 1: Selection\n        Traverse the tree for the node we most want to simulate.\n        Looks for an unexplored child of this node's best child's best child's...best child.\n        ";
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  double __pyx_v_exploration_bias;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("select (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 183, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
+  __Pyx_TraceCall("select", __pyx_f[0], 200, 0, __PYX_ERR(0, 200, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":188
+  /* "multimcts/mcts.pyx":205
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
- *         while not node._is_terminal:             # <<<<<<<<<<<<<<
- *             if not node._is_fully_expanded:
+ *         while not node.is_terminal:             # <<<<<<<<<<<<<<
+ *             if not node.is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = ((!(__pyx_v_node->_is_terminal != 0)) != 0);
+    __pyx_t_1 = ((!(__pyx_v_node->is_terminal != 0)) != 0);
     if (!__pyx_t_1) break;
 
-    /* "multimcts/mcts.pyx":189
+    /* "multimcts/mcts.pyx":206
  *         """
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = ((!(__pyx_v_node->_is_fully_expanded != 0)) != 0);
+    __pyx_t_1 = ((!(__pyx_v_node->is_fully_expanded != 0)) != 0);
     if (__pyx_t_1) {
 
-      /* "multimcts/mcts.pyx":190
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:
+      /* "multimcts/mcts.pyx":207
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
- *                 node = self.get_best_child(node, exploration_bias)
+ *                 node = self.get_best_child(node)
  */
       __Pyx_XDECREF(((PyObject *)__pyx_r));
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_expand); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_4);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
-        }
-      }
-      __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_node)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_node));
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->expand(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 190, __pyx_L1_error)
       __pyx_r = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2);
       __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":189
+      /* "multimcts/mcts.pyx":206
  *         """
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":192
+    /* "multimcts/mcts.pyx":209
  *                 return self.expand(node)
  *             else:
- *                 node = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
- * 
+ *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
  *         return node
+ * 
  */
     /*else*/ {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = NULL;
-      __pyx_t_6 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_5);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
-          __pyx_t_6 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__pyx_t_5) {
-          __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-        }
-        __Pyx_INCREF(((PyObject *)__pyx_v_node));
-        __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, ((PyObject *)__pyx_v_node));
-        __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-        __pyx_t_4 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 192, __pyx_L1_error)
+      __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->get_best_child(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
       __pyx_t_2 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":194
- *                 node = self.get_best_child(node, exploration_bias)
- * 
+  /* "multimcts/mcts.pyx":210
+ *             else:
+ *                 node = self.get_best_child(node)
  *         return node             # <<<<<<<<<<<<<<
  * 
- *     @staticmethod
+ *     cdef Node expand(self, Node node):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_node));
   __pyx_r = __pyx_v_node;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":183
+  /* "multimcts/mcts.pyx":200
  *             return best
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node select(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":197
+/* "multimcts/mcts.pyx":212
+ *         return node
  * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node expand(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_6expand[] = "Step 2: Expansion\n        Add a new child to this node.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_7expand = {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand};
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("expand (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,0};
-    PyObject* values[1] = {0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expand") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expand", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 197, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6expand(__pyx_v_node);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_expand(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   PyObject *__pyx_v_move = NULL;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  int __pyx_t_11;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
+  __Pyx_TraceCall("expand", __pyx_f[0], 212, 0, __PYX_ERR(0, 212, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":201
+  /* "multimcts/mcts.pyx":216
  *         Add a new child to this node.
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
+ *         move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
+ *         if len(node.remaining_moves) == 0:
+ *             node.is_fully_expanded = True
  */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "multimcts/mcts.pyx":202
- *         """
- *         try:
- *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")
- */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 202, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_v_move = __pyx_t_5;
-      __pyx_t_5 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Pop(__pyx_v_node->remaining_moves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_move = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":201
- *         Add a new child to this node.
+  /* "multimcts/mcts.pyx":217
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
+ *             node.is_fully_expanded = True
+ * 
  */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_1 = __pyx_v_node->remaining_moves;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 217, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = ((__pyx_t_2 == 0) != 0);
+  if (__pyx_t_3) {
 
-    /* "multimcts/mcts.pyx":203
- *         try:
- *             move = node.remaining_moves.pop()
- *         except IndexError:             # <<<<<<<<<<<<<<
- *             raise IndexError("Tried to expand a node with no remaining moves.")
+    /* "multimcts/mcts.pyx":218
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:
+ *             node.is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)
  */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 203, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GOTREF(__pyx_t_7);
+    __pyx_v_node->is_fully_expanded = 1;
 
-      /* "multimcts/mcts.pyx":204
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
- * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 204, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 204, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "multimcts/mcts.pyx":201
- *         Add a new child to this node.
+    /* "multimcts/mcts.pyx":217
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
+ *             node.is_fully_expanded = True
+ * 
+ */
   }
 
-  /* "multimcts/mcts.pyx":206
- *             raise IndexError("Tried to expand a node with no remaining moves.")
+  /* "multimcts/mcts.pyx":220
+ *             node.is_fully_expanded = True
  * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)             # <<<<<<<<<<<<<<
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)             # <<<<<<<<<<<<<<
  *         node.children.append(child)
  * 
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node->state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_move);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_move);
+  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_parent, ((PyObject *)__pyx_v_node)) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_parent, ((PyObject *)__pyx_v_node)) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_child = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":207
+  /* "multimcts/mcts.pyx":221
  * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)
  *         node.children.append(child)             # <<<<<<<<<<<<<<
  * 
- *         if len(node.remaining_moves) == 0:
- */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_Append(__pyx_t_4, ((PyObject *)__pyx_v_child)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "multimcts/mcts.pyx":209
- *         node.children.append(child)
- * 
- *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node._is_fully_expanded = True
- * 
- */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 209, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_11 = ((__pyx_t_10 == 0) != 0);
-  if (__pyx_t_11) {
-
-    /* "multimcts/mcts.pyx":210
- * 
- *         if len(node.remaining_moves) == 0:
- *             node._is_fully_expanded = True             # <<<<<<<<<<<<<<
- * 
  *         return child
  */
-    __pyx_v_node->_is_fully_expanded = 1;
+  __pyx_t_7 = __Pyx_PyObject_Append(__pyx_v_node->children, ((PyObject *)__pyx_v_child)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 221, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":209
+  /* "multimcts/mcts.pyx":223
  *         node.children.append(child)
  * 
- *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node._is_fully_expanded = True
- * 
- */
-  }
-
-  /* "multimcts/mcts.pyx":212
- *             node._is_fully_expanded = True
- * 
  *         return child             # <<<<<<<<<<<<<<
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_child));
   __pyx_r = __pyx_v_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":197
+  /* "multimcts/mcts.pyx":212
+ *         return node
  * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node expand(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":214
+/* "multimcts/mcts.pyx":225
  *         return child
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_8simulate[] = "Step 3: Simulation (aka playout/rollout)\n        Play out a game, from the given node to termination, and return the final reward.\n        A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.\n\n        Args:\n            node (Node): The node from which to begin the simulation.\n            heuristic (callable): A function that takes a state and returns a move.\n        ";
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  PyObject *__pyx_v_heuristic = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("simulate (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_heuristic,0};
-    PyObject* values[2] = {0,0};
-    values[1] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (kw_args == 1) {
-        const Py_ssize_t index = 1;
-        PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
-        if (value) { values[index] = value; kw_args--; }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_heuristic = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 214, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 214, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_heuristic);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic) {
+static std::map<std::string,double>  __pyx_f_9multimcts_4mcts_4MCTS_simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args) {
+  PyObject *__pyx_v_heuristic = ((PyObject *)Py_None);
   PyObject *__pyx_v_state = NULL;
   PyObject *__pyx_v_terminal_team = NULL;
   PyObject *__pyx_v_move = NULL;
   PyObject *__pyx_v_reward = NULL;
-  PyObject *__pyx_r = NULL;
+  std::map<std::string,double>  __pyx_v_crewards;
+  PyObject *__pyx_v_team = NULL;
+  std::map<std::string,double>  __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
+  std::map<std::string,double>  __pyx_t_8;
+  Py_ssize_t __pyx_t_9;
+  PyObject *(*__pyx_t_10)(PyObject *);
+  double __pyx_t_11;
+  std::string __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
+  __Pyx_TraceCall("simulate", __pyx_f[0], 225, 0, __PYX_ERR(0, 225, __pyx_L1_error));
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_heuristic = __pyx_optional_args->heuristic;
+    }
+  }
 
-  /* "multimcts/mcts.pyx":223
+  /* "multimcts/mcts.pyx":233
  *             heuristic (callable): A function that takes a state and returns a move.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
- *         if node._is_terminal:
+ *         terminal_team = None
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_1 = __pyx_v_node->state;
+  __Pyx_INCREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":225
+  /* "multimcts/mcts.pyx":235
  *         state = node.state
  * 
- *         if node._is_terminal:             # <<<<<<<<<<<<<<
- *             terminal_team = node.parent.state.get_current_team()
+ *         terminal_team = None             # <<<<<<<<<<<<<<
+ *         if node.is_terminal:
+ *             terminal_team = node.parent.team
+ */
+  __Pyx_INCREF(Py_None);
+  __pyx_v_terminal_team = Py_None;
+
+  /* "multimcts/mcts.pyx":236
+ * 
+ *         terminal_team = None
+ *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *             terminal_team = node.parent.team
  *         else:
  */
-  __pyx_t_2 = (__pyx_v_node->_is_terminal != 0);
+  __pyx_t_2 = (__pyx_v_node->is_terminal != 0);
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":226
- * 
- *         if node._is_terminal:
- *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":237
+ *         terminal_team = None
+ *         if node.is_terminal:
+ *             terminal_team = node.parent.team             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_terminal_team = __pyx_t_1;
+    __pyx_t_1 = __pyx_v_node->parent->team;
+    __Pyx_INCREF(__pyx_t_1);
+    __Pyx_DECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":225
- *         state = node.state
+    /* "multimcts/mcts.pyx":236
  * 
- *         if node._is_terminal:             # <<<<<<<<<<<<<<
- *             terminal_team = node.parent.state.get_current_team()
+ *         terminal_team = None
+ *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *             terminal_team = node.parent.team
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":228
- *             terminal_team = node.parent.state.get_current_team()
+  /* "multimcts/mcts.pyx":239
+ *             terminal_team = node.parent.team
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":229
+      /* "multimcts/mcts.pyx":240
  *         else:
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 if heuristic is not None:
  *                     move = heuristic(state)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
+      __Pyx_DECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":230
+      /* "multimcts/mcts.pyx":241
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
       __pyx_t_5 = (__pyx_v_heuristic != Py_None);
       __pyx_t_2 = (__pyx_t_5 != 0);
       if (__pyx_t_2) {
 
-        /* "multimcts/mcts.pyx":231
+        /* "multimcts/mcts.pyx":242
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  *                     move = heuristic(state)             # <<<<<<<<<<<<<<
  *                 else:
  *                     move = choice(state.get_legal_moves())
  */
         __Pyx_INCREF(__pyx_v_heuristic);
@@ -5193,55 +5116,55 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_state);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "multimcts/mcts.pyx":230
+        /* "multimcts/mcts.pyx":241
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
         goto __pyx_L6;
       }
 
-      /* "multimcts/mcts.pyx":233
+      /* "multimcts/mcts.pyx":244
  *                     move = heuristic(state)
  *                 else:
  *                     move = choice(state.get_legal_moves())             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
           }
         }
         __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5249,910 +5172,597 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
       }
       __pyx_L6:;
 
-      /* "multimcts/mcts.pyx":234
+      /* "multimcts/mcts.pyx":245
  *                 else:
  *                     move = choice(state.get_legal_moves())
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":236
+  /* "multimcts/mcts.pyx":247
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":237
+  /* "multimcts/mcts.pyx":248
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":238
+    /* "multimcts/mcts.pyx":249
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
- *         return reward
+ *         cdef map[string,double] crewards = map[string,double]()
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 238, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":237
+    /* "multimcts/mcts.pyx":248
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":240
+  /* "multimcts/mcts.pyx":251
  *             reward = {terminal_team: reward}
  * 
- *         return reward             # <<<<<<<<<<<<<<
+ *         cdef map[string,double] crewards = map[string,double]()             # <<<<<<<<<<<<<<
+ *         for team in reward:
+ *             if reward[team] == 0:
+ */
+  try {
+    __pyx_t_8 = std::map<std::string,double> ();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 251, __pyx_L1_error)
+  }
+  __pyx_v_crewards = __pyx_t_8;
+
+  /* "multimcts/mcts.pyx":252
  * 
- *     @staticmethod
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:             # <<<<<<<<<<<<<<
+ *             if reward[team] == 0:
+ *                 continue
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_reward);
-  __pyx_r = __pyx_v_reward;
+  if (likely(PyList_CheckExact(__pyx_v_reward)) || PyTuple_CheckExact(__pyx_v_reward)) {
+    __pyx_t_1 = __pyx_v_reward; __Pyx_INCREF(__pyx_t_1); __pyx_t_9 = 0;
+    __pyx_t_10 = NULL;
+  } else {
+    __pyx_t_9 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 252, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_10)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      } else {
+        if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
+    } else {
+      __pyx_t_3 = __pyx_t_10(__pyx_t_1);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 252, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_team, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "multimcts/mcts.pyx":253
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:
+ *             if reward[team] == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_reward, __pyx_v_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_3, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (__pyx_t_5) {
+
+      /* "multimcts/mcts.pyx":254
+ *         for team in reward:
+ *             if reward[team] == 0:
+ *                 continue             # <<<<<<<<<<<<<<
+ *             crewards[str(team).encode()] = float(reward[team])
+ * 
+ */
+      goto __pyx_L8_continue;
+
+      /* "multimcts/mcts.pyx":253
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:
+ *             if reward[team] == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])
+ */
+    }
+
+    /* "multimcts/mcts.pyx":255
+ *             if reward[team] == 0:
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])             # <<<<<<<<<<<<<<
+ * 
+ *         return crewards
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_reward, __pyx_v_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_11 = __Pyx_PyObject_AsDouble(__pyx_t_4); if (unlikely(__pyx_t_11 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_4), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    (__pyx_v_crewards[__pyx_t_12]) = __pyx_t_11;
+
+    /* "multimcts/mcts.pyx":252
+ * 
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:             # <<<<<<<<<<<<<<
+ *             if reward[team] == 0:
+ *                 continue
+ */
+    __pyx_L8_continue:;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "multimcts/mcts.pyx":257
+ *             crewards[str(team).encode()] = float(reward[team])
+ * 
+ *         return crewards             # <<<<<<<<<<<<<<
+ * 
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):
+ */
+  __pyx_r = __pyx_v_crewards;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":214
+  /* "multimcts/mcts.pyx":225
  *         return child
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_WriteUnraisable("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v_terminal_team);
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
-  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_XDECREF(__pyx_v_team);
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":243
+/* "multimcts/mcts.pyx":259
+ *         return crewards
  * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate[] = "Step 4: Backpropagation\n        Update all ancestors with the reward from this terminal node.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate = {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  PyObject *__pyx_v_reward = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("backpropagate (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_reward,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 243, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 243, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_reward = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 243, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 243, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_v_node, __pyx_v_reward);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward) {
-  double __pyx_v_val;
-  std::string __pyx_v_ckey;
-  std::map<std::string,float>  __pyx_v_creward;
-  PyObject *__pyx_v_key = NULL;
-  std::pair<std::string,float>  __pyx_v_item;
+static PyObject *__pyx_f_9multimcts_4mcts_4MCTS_backpropagate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, std::map<std::string,double>  __pyx_v_crewards) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  std::map<std::string,float>  __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  double __pyx_t_9;
-  int __pyx_t_10;
-  std::string __pyx_t_11;
-  int __pyx_t_12;
-  std::map<std::string,float> ::iterator __pyx_t_13;
-  std::pair<std::string,float>  __pyx_t_14;
+  int __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
+  __Pyx_TraceCall("backpropagate", __pyx_f[0], 259, 0, __PYX_ERR(0, 259, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":249
- *         cdef double val
- *         cdef string ckey
- *         cdef map[string,float] creward = map[string,float]()             # <<<<<<<<<<<<<<
- *         for key,val in reward.items():
- *             if val == 0:
- */
-  try {
-    __pyx_t_1 = std::map<std::string,float> ();
-  } catch(...) {
-    __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 249, __pyx_L1_error)
-  }
-  __pyx_v_creward = __pyx_t_1;
-
-  /* "multimcts/mcts.pyx":250
- *         cdef string ckey
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():             # <<<<<<<<<<<<<<
- *             if val == 0:
- *                 continue
- */
-  __pyx_t_3 = 0;
-  if (unlikely(__pyx_v_reward == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 250, __pyx_L1_error)
-  }
-  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_reward, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_2);
-  __pyx_t_2 = __pyx_t_6;
-  __pyx_t_6 = 0;
-  while (1) {
-    __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
-    if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 250, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_v_val = __pyx_t_9;
-
-    /* "multimcts/mcts.pyx":251
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():
- *             if val == 0:             # <<<<<<<<<<<<<<
- *                 continue
- *             ckey = str(key).encode()
- */
-    __pyx_t_10 = ((__pyx_v_val == 0.0) != 0);
-    if (__pyx_t_10) {
-
-      /* "multimcts/mcts.pyx":252
- *         for key,val in reward.items():
- *             if val == 0:
- *                 continue             # <<<<<<<<<<<<<<
- *             ckey = str(key).encode()
- *             creward[ckey] = val
- */
-      goto __pyx_L3_continue;
-
-      /* "multimcts/mcts.pyx":251
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():
- *             if val == 0:             # <<<<<<<<<<<<<<
- *                 continue
- *             ckey = str(key).encode()
- */
-    }
-
-    /* "multimcts/mcts.pyx":253
- *             if val == 0:
- *                 continue
- *             ckey = str(key).encode()             # <<<<<<<<<<<<<<
- *             creward[ckey] = val
- * 
- */
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_7), NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_11 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_ckey = __pyx_t_11;
-
-    /* "multimcts/mcts.pyx":254
- *                 continue
- *             ckey = str(key).encode()
- *             creward[ckey] = val             # <<<<<<<<<<<<<<
- * 
- *         cdef pair[string,float] item
- */
-    (__pyx_v_creward[__pyx_v_ckey]) = __pyx_v_val;
-    __pyx_L3_continue:;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "multimcts/mcts.pyx":257
- * 
- *         cdef pair[string,float] item
+  /* "multimcts/mcts.pyx":263
+ *         Update all ancestors with the reward from this terminal node.
+ *         """
  *         while node is not None:             # <<<<<<<<<<<<<<
- *             for item in creward:
- *                 ckey = item.first
- */
-  while (1) {
-    __pyx_t_10 = (((PyObject *)__pyx_v_node) != Py_None);
-    __pyx_t_12 = (__pyx_t_10 != 0);
-    if (!__pyx_t_12) break;
-
-    /* "multimcts/mcts.pyx":258
- *         cdef pair[string,float] item
- *         while node is not None:
- *             for item in creward:             # <<<<<<<<<<<<<<
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- */
-    __pyx_t_13 = __pyx_v_creward.begin();
-    for (;;) {
-      if (!(__pyx_t_13 != __pyx_v_creward.end())) break;
-      __pyx_t_14 = *__pyx_t_13;
-      ++__pyx_t_13;
-      __pyx_v_item = __pyx_t_14;
-
-      /* "multimcts/mcts.pyx":259
- *         while node is not None:
- *             for item in creward:
- *                 ckey = item.first             # <<<<<<<<<<<<<<
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0
- */
-      __pyx_t_11 = __pyx_v_item.first;
-      __pyx_v_ckey = __pyx_t_11;
-
-      /* "multimcts/mcts.pyx":260
- *             for item in creward:
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- */
-      __pyx_t_12 = ((__pyx_v_node->_total_reward.count(__pyx_v_ckey) == 0) != 0);
-      if (__pyx_t_12) {
-
-        /* "multimcts/mcts.pyx":261
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0             # <<<<<<<<<<<<<<
- *                 node._total_reward[ckey] += item.second
- *             node.visit()
- */
-        (__pyx_v_node->_total_reward[__pyx_v_ckey]) = 0.0;
-
-        /* "multimcts/mcts.pyx":260
- *             for item in creward:
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- */
-      }
-
-      /* "multimcts/mcts.pyx":262
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second             # <<<<<<<<<<<<<<
- *             node.visit()
+ *             node.apply_rewards(crewards)
  *             node = node.parent
  */
-      __pyx_t_11 = __pyx_v_ckey;
-      (__pyx_v_node->_total_reward[__pyx_t_11]) = ((__pyx_v_node->_total_reward[__pyx_t_11]) + __pyx_v_item.second);
+  while (1) {
+    __pyx_t_1 = (((PyObject *)__pyx_v_node) != Py_None);
+    __pyx_t_2 = (__pyx_t_1 != 0);
+    if (!__pyx_t_2) break;
 
-      /* "multimcts/mcts.pyx":258
- *         cdef pair[string,float] item
+    /* "multimcts/mcts.pyx":264
+ *         """
  *         while node is not None:
- *             for item in creward:             # <<<<<<<<<<<<<<
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- */
-    }
-
-    /* "multimcts/mcts.pyx":263
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- *             node.visit()             # <<<<<<<<<<<<<<
+ *             node.apply_rewards(crewards)             # <<<<<<<<<<<<<<
  *             node = node.parent
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_visit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = ((struct __pyx_vtabstruct_9multimcts_4mcts_Node *)__pyx_v_node->__pyx_vtab)->apply_rewards(__pyx_v_node, __pyx_v_crewards); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":264
- *                 node._total_reward[ckey] += item.second
- *             node.visit()
+    /* "multimcts/mcts.pyx":265
+ *         while node is not None:
+ *             node.apply_rewards(crewards)
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
- *     @cython.cdivision(True)
+ *     cdef Node get_best_child(self, Node node):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
-    __pyx_t_2 = 0;
+    __pyx_t_3 = ((PyObject *)__pyx_v_node->parent);
+    __Pyx_INCREF(__pyx_t_3);
+    __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_3));
+    __pyx_t_3 = 0;
   }
 
-  /* "multimcts/mcts.pyx":243
+  /* "multimcts/mcts.pyx":259
+ *         return crewards
  * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":269
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
+/* "multimcts/mcts.pyx":267
+ *             node = node.parent
+ * 
+ *     cdef Node get_best_child(self, Node node):             # <<<<<<<<<<<<<<
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child[] = "Find the child with the highest Upper Confidence Bound (UCB) score.\n        ucb = (x / n) + C * sqrt(ln(N) / n)\n        x=reward for this node\n        n=number of simulations for this node\n        N=number of simulations for parent node\n        C=exploration bias\n        ";
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  double __pyx_v_exploration_bias;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_best_child (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 269, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 269, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 269, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 269, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
-  int __pyx_v_visits;
-  double __pyx_v_reward;
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_get_best_child(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
+  double __pyx_v_parent_sqrtlog_visits;
+  double __pyx_v_best_score;
   double __pyx_v_ucb;
-  double __pyx_v_C;
-  double __pyx_v_ln_parent_visits;
-  std::string __pyx_v_cur_team;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best_child = 0;
-  std::pair<std::string,float>  __pyx_v_item;
-  double __pyx_v_best_score;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
-  std::string __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  int __pyx_t_7;
-  int __pyx_t_8;
-  std::map<std::string,float> ::iterator __pyx_t_9;
-  std::map<std::string,float>  *__pyx_t_10;
-  std::pair<std::string,float>  __pyx_t_11;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  PyObject *(*__pyx_t_4)(PyObject *);
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
+  __Pyx_TraceCall("get_best_child", __pyx_f[0], 267, 0, __PYX_ERR(0, 267, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":280
- *         cdef int visits
- *         cdef double reward, ucb
- *         cdef double C = exploration_bias             # <<<<<<<<<<<<<<
- *         cdef double ln_parent_visits = node.log_visits
- * 
- */
-  __pyx_v_C = __pyx_v_exploration_bias;
-
-  /* "multimcts/mcts.pyx":281
- *         cdef double reward, ucb
- *         cdef double C = exploration_bias
- *         cdef double ln_parent_visits = node.log_visits             # <<<<<<<<<<<<<<
- * 
- *         cdef string cur_team = node._team
- */
-  __pyx_t_1 = __pyx_v_node->log_visits;
-  __pyx_v_ln_parent_visits = __pyx_t_1;
-
-  /* "multimcts/mcts.pyx":283
- *         cdef double ln_parent_visits = node.log_visits
- * 
- *         cdef string cur_team = node._team             # <<<<<<<<<<<<<<
- * 
- *         cdef Node child, best_child
+  /* "multimcts/mcts.pyx":269
+ *     cdef Node get_best_child(self, Node node):
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits             # <<<<<<<<<<<<<<
+ *         cdef double best_score = -INFINITY
+ *         cdef double ucb
  */
-  __pyx_t_2 = __pyx_v_node->_team;
-  __pyx_v_cur_team = __pyx_t_2;
+  __pyx_t_1 = __pyx_v_node->sqrtlog_visits;
+  __pyx_v_parent_sqrtlog_visits = __pyx_t_1;
 
-  /* "multimcts/mcts.pyx":288
- *         cdef pair[string,float] item
- * 
+  /* "multimcts/mcts.pyx":270
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  *         cdef double best_score = -INFINITY             # <<<<<<<<<<<<<<
- * 
- *         for child in node.children:
+ *         cdef double ucb
+ *         cdef Node child, best_child = node.children[0]
  */
   __pyx_v_best_score = (-INFINITY);
 
-  /* "multimcts/mcts.pyx":290
+  /* "multimcts/mcts.pyx":272
  *         cdef double best_score = -INFINITY
+ *         cdef double ucb
+ *         cdef Node child, best_child = node.children[0]             # <<<<<<<<<<<<<<
+ *         cdef pair[string,double] item
+ * 
+ */
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_node->children, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_v_best_child = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "multimcts/mcts.pyx":275
+ *         cdef pair[string,double] item
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
+ *             if ucb > best_score:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-    __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
+  if (likely(PyList_CheckExact(__pyx_v_node->children)) || PyTuple_CheckExact(__pyx_v_node->children)) {
+    __pyx_t_2 = __pyx_v_node->children; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_4 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_node->children); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
-    if (likely(!__pyx_t_6)) {
-      if (likely(PyList_CheckExact(__pyx_t_4))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
+    if (likely(!__pyx_t_4)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
-      __pyx_t_3 = __pyx_t_6(__pyx_t_4);
-      if (unlikely(!__pyx_t_3)) {
+      __pyx_t_5 = __pyx_t_4(__pyx_t_2);
+      if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 290, __pyx_L1_error)
+          else __PYX_ERR(0, 275, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_GOTREF(__pyx_t_5);
     }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 290, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "multimcts/mcts.pyx":291
- * 
- *         for child in node.children:
- *             visits = child._num_visits             # <<<<<<<<<<<<<<
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
- *                 continue
- */
-    __pyx_t_7 = __pyx_v_child->_num_visits;
-    __pyx_v_visits = __pyx_t_7;
-
-    /* "multimcts/mcts.pyx":292
- *         for child in node.children:
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
- *                 continue
- * 
- */
-    __pyx_t_8 = ((__pyx_v_visits == 0) != 0);
-    if (__pyx_t_8) {
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_5));
+    __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":293
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
- *                 continue             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":276
  * 
- *             # Relative reward is this child's reward minus its siblings' rewards.
- */
-      goto __pyx_L3_continue;
-
-      /* "multimcts/mcts.pyx":292
  *         for child in node.children:
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
- *                 continue
- * 
- */
-    }
-
-    /* "multimcts/mcts.pyx":296
- * 
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]             # <<<<<<<<<<<<<<
- *             for item in child._total_reward:
- *                 reward -= item.second
- */
-    __pyx_v_reward = (2.0 * (__pyx_v_child->_total_reward[__pyx_v_cur_team]));
-
-    /* "multimcts/mcts.pyx":297
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:             # <<<<<<<<<<<<<<
- *                 reward -= item.second
- * 
- */
-    __pyx_t_10 = &__pyx_v_child->_total_reward;
-    __pyx_t_9 = __pyx_t_10->begin();
-    for (;;) {
-      if (!(__pyx_t_9 != __pyx_t_10->end())) break;
-      __pyx_t_11 = *__pyx_t_9;
-      ++__pyx_t_9;
-      __pyx_v_item = __pyx_t_11;
-
-      /* "multimcts/mcts.pyx":298
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:
- *                 reward -= item.second             # <<<<<<<<<<<<<<
- * 
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- */
-      __pyx_v_reward = (__pyx_v_reward - __pyx_v_item.second);
-
-      /* "multimcts/mcts.pyx":297
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:             # <<<<<<<<<<<<<<
- *                 reward -= item.second
- * 
- */
-    }
-
-    /* "multimcts/mcts.pyx":300
- *                 reward -= item.second
- * 
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
- * 
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)             # <<<<<<<<<<<<<<
  *             if ucb > best_score:
+ *                 best_score = ucb
  */
-    __pyx_v_ucb = ((__pyx_v_reward / ((double)__pyx_v_visits)) + (__pyx_v_C * sqrt((__pyx_v_ln_parent_visits / ((double)__pyx_v_visits)))));
+    __pyx_v_ucb = ((struct __pyx_vtabstruct_9multimcts_4mcts_Node *)__pyx_v_child->__pyx_vtab)->ucb(__pyx_v_child, __pyx_v_self->exploration_bias, __pyx_v_parent_sqrtlog_visits);
 
-    /* "multimcts/mcts.pyx":302
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- * 
+    /* "multimcts/mcts.pyx":277
+ *         for child in node.children:
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
-    __pyx_t_8 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
-    if (__pyx_t_8) {
+    __pyx_t_6 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
+    if (__pyx_t_6) {
 
-      /* "multimcts/mcts.pyx":303
- * 
+      /* "multimcts/mcts.pyx":278
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:
  *                 best_score = ucb             # <<<<<<<<<<<<<<
  *                 best_child = child
  * 
  */
       __pyx_v_best_score = __pyx_v_ucb;
 
-      /* "multimcts/mcts.pyx":304
+      /* "multimcts/mcts.pyx":279
  *             if ucb > best_score:
  *                 best_score = ucb
  *                 best_child = child             # <<<<<<<<<<<<<<
  * 
  *         return best_child
  */
       __Pyx_INCREF(((PyObject *)__pyx_v_child));
-      __Pyx_XDECREF_SET(__pyx_v_best_child, __pyx_v_child);
+      __Pyx_DECREF_SET(__pyx_v_best_child, __pyx_v_child);
 
-      /* "multimcts/mcts.pyx":302
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- * 
+      /* "multimcts/mcts.pyx":277
+ *         for child in node.children:
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
     }
 
-    /* "multimcts/mcts.pyx":290
- *         cdef double best_score = -INFINITY
+    /* "multimcts/mcts.pyx":275
+ *         cdef pair[string,double] item
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
+ *             if ucb > best_score:
  */
-    __pyx_L3_continue:;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":306
+  /* "multimcts/mcts.pyx":281
  *                 best_child = child
  * 
  *         return best_child             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  if (unlikely(!__pyx_v_best_child)) { __Pyx_RaiseUnboundLocalError("best_child"); __PYX_ERR(0, 306, __pyx_L1_error) }
   __Pyx_INCREF(((PyObject *)__pyx_v_best_child));
   __pyx_r = __pyx_v_best_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":269
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
+  /* "multimcts/mcts.pyx":267
+ *             node = node.parent
+ * 
+ *     cdef Node get_best_child(self, Node node):             # <<<<<<<<<<<<<<
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XDECREF((PyObject *)__pyx_v_best_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.exploration_bias,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -6342,46 +5952,49 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -6401,14 +6014,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -6491,45 +6105,48 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__12)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node", 0);
+  __Pyx_TraceCall("__pyx_unpickle_Node", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__13, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  */
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
@@ -6540,17 +6157,17 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
@@ -6575,23 +6192,23 @@
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
@@ -6609,15 +6226,15 @@
   if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
@@ -6632,28 +6249,28 @@
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
   /* "(tree fragment)":10
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result             # <<<<<<<<<<<<<<
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v___pyx_result);
   __pyx_r = __pyx_v___pyx_result;
   goto __pyx_L0;
 
   /* "(tree fragment)":1
@@ -6670,202 +6287,234 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
-  std::string __pyx_t_4;
-  std::map<std::string,float>  __pyx_t_5;
-  double __pyx_t_6;
+  double __pyx_t_2;
+  std::string __pyx_t_3;
+  int __pyx_t_4;
+  std::map<std::string,double>  __pyx_t_5;
+  int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node__set_state", 0);
+  __Pyx_TraceCall("__pyx_unpickle_Node__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]             # <<<<<<<<<<<<<<
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_children);
-  __Pyx_DECREF(__pyx_v___pyx_result->_children);
-  __pyx_v___pyx_result->_children = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->avg_reward = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_is_fully_expanded = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->children);
+  __Pyx_DECREF(__pyx_v___pyx_result->children);
+  __pyx_v___pyx_result->children = __pyx_t_1;
+  __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_is_terminal = __pyx_t_2;
+  __pyx_v___pyx_result->cteam = __pyx_t_3;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_move);
-  __Pyx_DECREF(__pyx_v___pyx_result->_move);
-  __pyx_v___pyx_result->_move = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->invsqrt_visits = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_num_visits = __pyx_t_3;
+  __pyx_v___pyx_result->is_fully_expanded = __pyx_t_4;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_parent);
-  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->_parent));
-  __pyx_v___pyx_result->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->is_terminal = __pyx_t_4;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 6, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_remaining_moves);
-  __Pyx_DECREF(__pyx_v___pyx_result->_remaining_moves);
-  __pyx_v___pyx_result->_remaining_moves = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v___pyx_result->move);
+  __Pyx_DECREF(__pyx_v___pyx_result->move);
+  __pyx_v___pyx_result->move = __pyx_t_1;
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 7, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_state);
-  __Pyx_DECREF(__pyx_v___pyx_result->_state);
-  __pyx_v___pyx_result->_state = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v___pyx_result->parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->parent));
+  __pyx_v___pyx_result->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 8, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_team = __pyx_t_4;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->remaining_moves);
+  __Pyx_DECREF(__pyx_v___pyx_result->remaining_moves);
+  __pyx_v___pyx_result->remaining_moves = __pyx_t_1;
+  __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 9, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __pyx_convert_map_from_py_std_3a__3a_string__and_float(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_5 = __pyx_convert_map_from_py_std_3a__3a_string__and_double(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_total_reward = __pyx_t_5;
+  __pyx_v___pyx_result->rewards = __pyx_t_5;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 10, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->log_visits = __pyx_t_6;
+  __pyx_v___pyx_result->sqrtlog_visits = __pyx_t_2;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 11, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->state);
+  __Pyx_DECREF(__pyx_v___pyx_result->state);
+  __pyx_v___pyx_result->state = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 12, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->team);
+  __Pyx_DECREF(__pyx_v___pyx_result->team);
+  __pyx_v___pyx_result->team = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 13, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->visits = __pyx_t_6;
 
   /* "(tree fragment)":13
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
   __pyx_t_7 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_8 = ((__pyx_t_7 > 11) != 0);
+  __pyx_t_8 = ((__pyx_t_7 > 14) != 0);
   if (__pyx_t_8) {
   } else {
-    __pyx_t_2 = __pyx_t_8;
+    __pyx_t_4 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_8 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
   __pyx_t_9 = (__pyx_t_8 != 0);
-  __pyx_t_2 = __pyx_t_9;
+  __pyx_t_4 = __pyx_t_9;
   __pyx_L4_bool_binop_done:;
-  if (__pyx_t_2) {
+  if (__pyx_t_4) {
 
     /* "(tree fragment)":14
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[11])             # <<<<<<<<<<<<<<
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[14])             # <<<<<<<<<<<<<<
  */
     __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_update); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
-    __pyx_t_10 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 11, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 14, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_12);
@@ -6879,40 +6528,41 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   }
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_MCTS(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -6995,36 +6645,39 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__14)
   __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS", 0);
+  __Pyx_TraceCall("__pyx_unpickle_MCTS", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__15, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):
@@ -7174,42 +6827,45 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
  *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.exploration_bias = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   double __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS__set_state", 0);
+  __Pyx_TraceCall("__pyx_unpickle_MCTS__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
  *     __pyx_result.exploration_bias = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -7305,34 +6961,37 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":31
  * 
  * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_f[1], 31, 0, __PYX_ERR(1, 31, __pyx_L1_error));
 
   /* "string.to_py":32
  * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
@@ -7355,34 +7014,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":37
  * 
  * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_f[1], 37, 0, __PYX_ERR(1, 37, __pyx_L1_error));
 
   /* "string.to_py":38
  * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
@@ -7405,34 +7067,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":43
  * 
  * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_f[1], 43, 0, __PYX_ERR(1, 43, __pyx_L1_error));
 
   /* "string.to_py":44
  * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
@@ -7455,34 +7120,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":49
  * 
  * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_f[1], 49, 0, __PYX_ERR(1, 49, __pyx_L1_error));
 
   /* "string.to_py":50
  * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
@@ -7505,34 +7173,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":55
  * 
  * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_f[1], 55, 0, __PYX_ERR(1, 55, __pyx_L1_error));
 
   /* "string.to_py":56
  * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * 
  */
@@ -7554,14 +7225,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
@@ -7570,20 +7242,22 @@
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  */
 
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
   Py_ssize_t __pyx_v_length;
   char const *__pyx_v_data;
   std::string __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   char const *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_string_from_py_std__in_string", __pyx_f[1], 13, 0, __PYX_ERR(1, 13, __pyx_L1_error));
 
   /* "string.from_py":14
  * @cname("__pyx_convert_string_from_py_std__in_string")
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
  *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  *     return string(data, length)
@@ -7619,43 +7293,46 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.to_py":201
  * 
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):             # <<<<<<<<<<<<<<
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
  */
 
-static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &__pyx_v_s) {
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____double(std::map<std::string,double>  const &__pyx_v_s) {
   PyObject *__pyx_v_o = NULL;
-  std::map<std::string,float> ::value_type const *__pyx_v_key_value;
-  std::map<std::string,float> ::const_iterator __pyx_v_iter;
+  std::map<std::string,double> ::value_type const *__pyx_v_key_value;
+  std::map<std::string,double> ::const_iterator __pyx_v_iter;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____float", 0);
+  __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____double", 0);
+  __Pyx_TraceCall("__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_f[1], 201, 0, __PYX_ERR(1, 201, __pyx_L1_error));
 
   /* "map.to_py":202
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
@@ -7725,65 +7402,68 @@
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_o);
   __pyx_r = __pyx_v_o;
   goto __pyx_L0;
 
   /* "map.to_py":201
  * 
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):             # <<<<<<<<<<<<<<
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_o);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
 
-static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *__pyx_v_o) {
+static std::map<std::string,double>  __pyx_convert_map_from_py_std_3a__3a_string__and_double(PyObject *__pyx_v_o) {
   PyObject *__pyx_v_d = 0;
-  std::map<std::string,float>  __pyx_v_m;
+  std::map<std::string,double>  __pyx_v_m;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_value = NULL;
-  std::map<std::string,float>  __pyx_r;
+  std::map<std::string,double>  __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   std::string __pyx_t_8;
-  float __pyx_t_9;
+  double __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_float", 0);
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_double", 0);
+  __Pyx_TraceCall("__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_f[1], 174, 0, __PYX_ERR(1, 174, __pyx_L1_error));
 
   /* "map.from_py":175
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:
  *     cdef dict d = o             # <<<<<<<<<<<<<<
  *     cdef map[X,Y] m
  *     for key, value in d.iteritems():
  */
   if (!(likely(PyDict_CheckExact(__pyx_v_o))||((__pyx_v_o) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_o)->tp_name), 0))) __PYX_ERR(1, 175, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_o;
   __Pyx_INCREF(__pyx_t_1);
@@ -7822,16 +7502,16 @@
  *     cdef map[X,Y] m
  *     for key, value in d.iteritems():
  *         m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
  *     return m
  * 
  */
     __pyx_t_8 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
-    __pyx_t_9 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_9 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
-    __pyx_v_m.insert(std::pair<std::string,float> (((std::string)__pyx_t_8), ((float)__pyx_t_9)));
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+    __pyx_v_m.insert(std::pair<std::string,double> (((std::string)__pyx_t_8), ((double)__pyx_t_9)));
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "map.from_py":179
  *     for key, value in d.iteritems():
  *         m.insert(pair[X,Y](<X>key, <Y>value))
  *     return m             # <<<<<<<<<<<<<<
@@ -7839,148 +7519,143 @@
  * 
  */
   __pyx_r = __pyx_v_m;
   goto __pyx_L0;
 
   /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_d);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static struct __pyx_vtabstruct_9multimcts_4mcts_Node __pyx_vtable_9multimcts_4mcts_Node;
 
 static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9multimcts_4mcts_Node *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_9multimcts_4mcts_Node *)o);
-  new((void*)&(p->_team)) std::string();
-  new((void*)&(p->_total_reward)) std::map<std::string,float> ();
-  p->_state = Py_None; Py_INCREF(Py_None);
-  p->_move = Py_None; Py_INCREF(Py_None);
-  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
-  p->_children = Py_None; Py_INCREF(Py_None);
-  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  p->__pyx_vtab = __pyx_vtabptr_9multimcts_4mcts_Node;
+  new((void*)&(p->cteam)) std::string();
+  new((void*)&(p->rewards)) std::map<std::string,double> ();
+  p->state = Py_None; Py_INCREF(Py_None);
+  p->move = Py_None; Py_INCREF(Py_None);
+  p->team = Py_None; Py_INCREF(Py_None);
+  p->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  p->children = Py_None; Py_INCREF(Py_None);
+  p->remaining_moves = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_9multimcts_4mcts_Node(PyObject *o) {
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
-  __Pyx_call_destructor(p->_team);
-  __Pyx_call_destructor(p->_total_reward);
-  Py_CLEAR(p->_state);
-  Py_CLEAR(p->_move);
-  Py_CLEAR(p->_parent);
-  Py_CLEAR(p->_children);
-  Py_CLEAR(p->_remaining_moves);
+  __Pyx_call_destructor(p->cteam);
+  __Pyx_call_destructor(p->rewards);
+  Py_CLEAR(p->state);
+  Py_CLEAR(p->move);
+  Py_CLEAR(p->team);
+  Py_CLEAR(p->parent);
+  Py_CLEAR(p->children);
+  Py_CLEAR(p->remaining_moves);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_9multimcts_4mcts_Node(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
-  if (p->_state) {
-    e = (*v)(p->_state, a); if (e) return e;
+  if (p->state) {
+    e = (*v)(p->state, a); if (e) return e;
+  }
+  if (p->move) {
+    e = (*v)(p->move, a); if (e) return e;
   }
-  if (p->_move) {
-    e = (*v)(p->_move, a); if (e) return e;
+  if (p->team) {
+    e = (*v)(p->team, a); if (e) return e;
   }
-  if (p->_parent) {
-    e = (*v)(((PyObject *)p->_parent), a); if (e) return e;
+  if (p->parent) {
+    e = (*v)(((PyObject *)p->parent), a); if (e) return e;
   }
-  if (p->_children) {
-    e = (*v)(p->_children, a); if (e) return e;
+  if (p->children) {
+    e = (*v)(p->children, a); if (e) return e;
   }
-  if (p->_remaining_moves) {
-    e = (*v)(p->_remaining_moves, a); if (e) return e;
+  if (p->remaining_moves) {
+    e = (*v)(p->remaining_moves, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_9multimcts_4mcts_Node(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
-  tmp = ((PyObject*)p->_state);
-  p->_state = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->state);
+  p->state = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_move);
-  p->_move = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->move);
+  p->move = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_parent);
-  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->team);
+  p->team = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_children);
-  p->_children = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->parent);
+  p->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_remaining_moves);
-  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->children);
+  p->children = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->remaining_moves);
+  p->remaining_moves = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_state(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_parent(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_move(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_children(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_remaining_moves(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(o);
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_rewards(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_9multimcts_4mcts_Node[] = {
-  {"visit", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_3visit, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_Node[] = {
   {(char *)"state", __pyx_getprop_9multimcts_4mcts_4Node_state, 0, (char *)0, 0},
-  {(char *)"parent", __pyx_getprop_9multimcts_4mcts_4Node_parent, 0, (char *)0, 0},
-  {(char *)"move", __pyx_getprop_9multimcts_4mcts_4Node_move, 0, (char *)0, 0},
-  {(char *)"children", __pyx_getprop_9multimcts_4mcts_4Node_children, 0, (char *)0, 0},
-  {(char *)"remaining_moves", __pyx_getprop_9multimcts_4mcts_4Node_remaining_moves, 0, (char *)0, 0},
+  {(char *)"rewards", __pyx_getprop_9multimcts_4mcts_4Node_rewards, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_9multimcts_4mcts_Node = {
   PyVarObject_HEAD_INIT(0, 0)
   "multimcts.mcts.Node", /*tp_name*/
   sizeof(struct __pyx_obj_9multimcts_4mcts_Node), /*tp_basicsize*/
@@ -8007,15 +7682,15 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n\n    Attributes:\n        children (list): The child nodes of the current node. These represent legal moves that have been visited.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ", /*tp_doc*/
+  "Represents a game state node in the MCTS search tree.\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n    Attributes:\n        children (List[Node]): The child nodes of the current node. These represent legal moves that have been visited.\n        visits (int): The number of times the node has been visited.\n        rewards (dict): All teams' rewards obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ", /*tp_doc*/
   __pyx_tp_traverse_9multimcts_4mcts_Node, /*tp_traverse*/
   __pyx_tp_clear_9multimcts_4mcts_Node, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_9multimcts_4mcts_Node, /*tp_methods*/
@@ -8047,23 +7722,27 @@
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
+static struct __pyx_vtabstruct_9multimcts_4mcts_MCTS __pyx_vtable_9multimcts_4mcts_MCTS;
 
 static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_9multimcts_4mcts_MCTS *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  p = ((struct __pyx_obj_9multimcts_4mcts_MCTS *)o);
+  p->__pyx_vtab = __pyx_vtabptr_9multimcts_4mcts_MCTS;
   return o;
 }
 
 static void __pyx_tp_dealloc_9multimcts_4mcts_MCTS(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
@@ -8074,21 +7753,16 @@
 
 static PyObject *__pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_9multimcts_4mcts_MCTS[] = {
   {"search", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_3search, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_2search},
-  {"select", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_5select, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_4select},
-  {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand},
-  {"simulate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_9simulate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_8simulate},
-  {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate},
-  {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_MCTS[] = {
   {(char *)"exploration_bias", __pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -8223,112 +7897,91 @@
   {&__pyx_kp_u_GameState_must_implement_get_cur, __pyx_k_GameState_must_implement_get_cur, sizeof(__pyx_k_GameState_must_implement_get_cur), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_get_leg, __pyx_k_GameState_must_implement_get_leg, sizeof(__pyx_k_GameState_must_implement_get_leg), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_get_rew, __pyx_k_GameState_must_implement_get_rew, sizeof(__pyx_k_GameState_must_implement_get_rew), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_is_term, __pyx_k_GameState_must_implement_is_term, sizeof(__pyx_k_GameState_must_implement_is_term), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 1, 0, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
-  {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_u_Invalid_return_type, __pyx_k_Invalid_return_type, sizeof(__pyx_k_Invalid_return_type), 0, 1, 0, 0},
   {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS, __pyx_k_MCTS, sizeof(__pyx_k_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_Move, __pyx_k_Move, sizeof(__pyx_k_Move), 0, 0, 1, 1},
   {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
   {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_kp_u_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 1, 0, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Rewards, __pyx_k_Rewards, sizeof(__pyx_k_Rewards), 0, 0, 1, 1},
   {&__pyx_n_s_Team, __pyx_k_Team, sizeof(__pyx_k_Team), 0, 0, 1, 1},
-  {&__pyx_kp_u_Tried_to_expand_a_node_with_no_r, __pyx_k_Tried_to_expand_a_node_with_no_r, sizeof(__pyx_k_Tried_to_expand_a_node_with_no_r), 0, 1, 0, 0},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
-  {&__pyx_n_s_backpropagate, __pyx_k_backpropagate, sizeof(__pyx_k_backpropagate), 0, 0, 1, 1},
-  {&__pyx_n_s_child, __pyx_k_child, sizeof(__pyx_k_child), 0, 0, 1, 1},
-  {&__pyx_n_s_children, __pyx_k_children, sizeof(__pyx_k_children), 0, 0, 1, 1},
   {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
-  {&__pyx_n_s_ckey, __pyx_k_ckey, sizeof(__pyx_k_ckey), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_creward, __pyx_k_creward, sizeof(__pyx_k_creward), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_expand, __pyx_k_expand, sizeof(__pyx_k_expand), 0, 0, 1, 1},
   {&__pyx_n_s_exploration_bias, __pyx_k_exploration_bias, sizeof(__pyx_k_exploration_bias), 0, 0, 1, 1},
-  {&__pyx_n_s_get_best_child, __pyx_k_get_best_child, sizeof(__pyx_k_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_get_current_team, __pyx_k_get_current_team, sizeof(__pyx_k_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_get_legal_moves, __pyx_k_get_legal_moves, sizeof(__pyx_k_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_get_reward, __pyx_k_get_reward, sizeof(__pyx_k_get_reward), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_heuristic, __pyx_k_heuristic, sizeof(__pyx_k_heuristic), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_is_terminal, __pyx_k_is_terminal, sizeof(__pyx_k_is_terminal), 0, 0, 1, 1},
-  {&__pyx_n_s_item, __pyx_k_item, sizeof(__pyx_k_item), 0, 0, 1, 1},
-  {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_iteritems, __pyx_k_iteritems, sizeof(__pyx_k_iteritems), 0, 0, 1, 1},
-  {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_make_move, __pyx_k_make_move, sizeof(__pyx_k_make_move), 0, 0, 1, 1},
   {&__pyx_n_s_max_iterations, __pyx_k_max_iterations, sizeof(__pyx_k_max_iterations), 0, 0, 1, 1},
   {&__pyx_n_s_max_time, __pyx_k_max_time, sizeof(__pyx_k_max_time), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 0, 1, 1},
   {&__pyx_n_u_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 1, 0, 1},
   {&__pyx_n_s_multimcts_mcts, __pyx_k_multimcts_mcts, sizeof(__pyx_k_multimcts_mcts), 0, 0, 1, 1},
   {&__pyx_kp_s_multimcts_mcts_pyx, __pyx_k_multimcts_mcts_pyx, sizeof(__pyx_k_multimcts_mcts_pyx), 0, 0, 1, 0},
   {&__pyx_kp_u_must_be_one_of, __pyx_k_must_be_one_of, sizeof(__pyx_k_must_be_one_of), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
-  {&__pyx_n_s_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 0, 1, 1},
   {&__pyx_n_u_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 1, 0, 1},
   {&__pyx_n_s_parent, __pyx_k_parent, sizeof(__pyx_k_parent), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_MCTS, __pyx_k_pyx_unpickle_MCTS, sizeof(__pyx_k_pyx_unpickle_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Node, __pyx_k_pyx_unpickle_Node, sizeof(__pyx_k_pyx_unpickle_Node), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_remaining_moves, __pyx_k_remaining_moves, sizeof(__pyx_k_remaining_moves), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_return_type, __pyx_k_return_type, sizeof(__pyx_k_return_type), 0, 0, 1, 1},
-  {&__pyx_n_s_reward, __pyx_k_reward, sizeof(__pyx_k_reward), 0, 0, 1, 1},
-  {&__pyx_n_s_select, __pyx_k_select, sizeof(__pyx_k_select), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
-  {&__pyx_n_s_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
   {&__pyx_n_u_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 1, 0, 1},
-  {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-  {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
-  {&__pyx_n_s_visit, __pyx_k_visit, sizeof(__pyx_k_visit), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 162, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -8337,210 +7990,176 @@
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "multimcts/mcts.pyx":204
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
- * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
- */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
-  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_24284988, __pyx_int_53904430, __pyx_int_227935910); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_56097295, __pyx_int_99932858, __pyx_int_59888949); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 22, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 26, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 30, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 36, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 40, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":197
- * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 2: Expansion
- *         Add a new child to this node.
- */
-  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 197, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":243
- * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
- *         """Step 4: Backpropagation
- *         Update all ancestors with the reward from this terminal node.
- */
-  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_val, __pyx_n_s_ckey, __pyx_n_s_creward, __pyx_n_s_key, __pyx_n_s_item); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 243, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 40, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyList_Type_pop.type = (PyObject*)&PyList_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_24284988 = PyInt_FromLong(24284988L); if (unlikely(!__pyx_int_24284988)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_53904430 = PyInt_FromLong(53904430L); if (unlikely(!__pyx_int_53904430)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_56097295 = PyInt_FromLong(56097295L); if (unlikely(!__pyx_int_56097295)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_59888949 = PyInt_FromLong(59888949L); if (unlikely(!__pyx_int_59888949)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_82662024 = PyInt_FromLong(82662024L); if (unlikely(!__pyx_int_82662024)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_99932858 = PyInt_FromLong(99932858L); if (unlikely(!__pyx_int_99932858)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_203704333 = PyInt_FromLong(203704333L); if (unlikely(!__pyx_int_203704333)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_227935910 = PyInt_FromLong(227935910L); if (unlikely(!__pyx_int_227935910)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_231097371 = PyInt_FromLong(231097371L); if (unlikely(!__pyx_int_231097371)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -8578,43 +8197,54 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
+  __pyx_vtabptr_9multimcts_4mcts_Node = &__pyx_vtable_9multimcts_4mcts_Node;
+  __pyx_vtable_9multimcts_4mcts_Node.apply_rewards = (PyObject *(*)(struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> ))__pyx_f_9multimcts_4mcts_4Node_apply_rewards;
+  __pyx_vtable_9multimcts_4mcts_Node.ucb = (double (*)(struct __pyx_obj_9multimcts_4mcts_Node *, double, double))__pyx_f_9multimcts_4mcts_4Node_ucb;
   if (PyType_Ready(&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts_Node.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_Node.tp_dictoffset && __pyx_type_9multimcts_4mcts_Node.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts_Node.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
+  if (__Pyx_SetVtable(__pyx_type_9multimcts_4mcts_Node.tp_dict, __pyx_vtabptr_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Node, (PyObject *)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __pyx_ptype_9multimcts_4mcts_Node = &__pyx_type_9multimcts_4mcts_Node;
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_vtabptr_9multimcts_4mcts_MCTS = &__pyx_vtable_9multimcts_4mcts_MCTS;
+  __pyx_vtable_9multimcts_4mcts_MCTS.select = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_select;
+  __pyx_vtable_9multimcts_4mcts_MCTS.expand = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_expand;
+  __pyx_vtable_9multimcts_4mcts_MCTS.simulate = (std::map<std::string,double>  (*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args))__pyx_f_9multimcts_4mcts_4MCTS_simulate;
+  __pyx_vtable_9multimcts_4mcts_MCTS.backpropagate = (PyObject *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> ))__pyx_f_9multimcts_4mcts_4MCTS_backpropagate;
+  __pyx_vtable_9multimcts_4mcts_MCTS.get_best_child = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_get_best_child;
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts_MCTS.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_MCTS.tp_dictoffset && __pyx_type_9multimcts_4mcts_MCTS.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts_MCTS.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_9multimcts_4mcts_MCTS, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 114, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_9multimcts_4mcts_MCTS, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 134, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__.doc = __pyx_doc_9multimcts_4mcts_4MCTS___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MCTS, (PyObject *)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_9multimcts_4mcts_MCTS.tp_dict, __pyx_vtabptr_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MCTS, (PyObject *)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __pyx_ptype_9multimcts_4mcts_MCTS = &__pyx_type_9multimcts_4mcts_MCTS;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -8733,14 +8363,15 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_mcts(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  __Pyx_TraceDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8842,17 +8473,18 @@
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
+  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_mcts(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":5
- * # cython: profile=False
+ * # cython: profile=True
  * 
  * from time import time             # <<<<<<<<<<<<<<
  * from random import shuffle, choice
  * from typing import Union, Dict, List, Any
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -9019,90 +8651,90 @@
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Move); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_u_GameState) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
@@ -9117,15 +8749,15 @@
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "multimcts/mcts.pyx":21
@@ -9137,111 +8769,54 @@
  */
   __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_4) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":197
- * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 2: Expansion
- *         Add a new child to this node.
- */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":196
- *         return node
- * 
- *     @staticmethod             # <<<<<<<<<<<<<<
- *     def expand(node:Node) -> Node:
- *         """Step 2: Expansion
- */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_expand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":243
- * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
- *         """Step 4: Backpropagation
- *         Update all ancestors with the reward from this terminal node.
- */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_4) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":242
- *         return reward
- * 
- *     @staticmethod             # <<<<<<<<<<<<<<
- *     def backpropagate(node:Node, reward:Rewards):
- *         """Step 4: Backpropagation
- */
-  __Pyx_GetNameInClass(__pyx_t_4, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
   /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_1__pyx_unpickle_Node, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Node, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_3__pyx_unpickle_MCTS, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MCTS, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3
- * # cython: profile=False
+ * # cython: profile=True
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
+  __Pyx_TraceReturn(Py_None, 0);
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -9309,34 +8884,14 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -9353,14 +8908,124 @@
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
+/* Profile */
+#if CYTHON_PROFILE
+static int __Pyx_TraceSetupAndCall(PyCodeObject** code,
+                                   PyFrameObject** frame,
+                                   PyThreadState* tstate,
+                                   const char *funcname,
+                                   const char *srcfile,
+                                   int firstlineno) {
+    PyObject *type, *value, *traceback;
+    int retval;
+    if (*frame == NULL || !CYTHON_PROFILE_REUSE_FRAME) {
+        if (*code == NULL) {
+            *code = __Pyx_createFrameCodeObject(funcname, srcfile, firstlineno);
+            if (*code == NULL) return 0;
+        }
+        *frame = PyFrame_New(
+            tstate,                          /*PyThreadState *tstate*/
+            *code,                           /*PyCodeObject *code*/
+            __pyx_d,                  /*PyObject *globals*/
+            0                                /*PyObject *locals*/
+        );
+        if (*frame == NULL) return 0;
+        if (CYTHON_TRACE && (*frame)->f_trace == NULL) {
+            Py_INCREF(Py_None);
+            (*frame)->f_trace = Py_None;
+        }
+#if PY_VERSION_HEX < 0x030400B1
+    } else {
+        (*frame)->f_tstate = tstate;
+#endif
+    }
+    __Pyx_PyFrame_SetLineNumber(*frame, firstlineno);
+    retval = 1;
+    __Pyx_EnterTracing(tstate);
+    __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+    #if CYTHON_TRACE
+    if (tstate->c_tracefunc)
+        retval = tstate->c_tracefunc(tstate->c_traceobj, *frame, PyTrace_CALL, NULL) == 0;
+    if (retval && tstate->c_profilefunc)
+    #endif
+        retval = tstate->c_profilefunc(tstate->c_profileobj, *frame, PyTrace_CALL, NULL) == 0;
+    __Pyx_LeaveTracing(tstate);
+    if (retval) {
+        __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+        return __Pyx_IsTracing(tstate, 0, 0) && retval;
+    } else {
+        Py_XDECREF(type);
+        Py_XDECREF(value);
+        Py_XDECREF(traceback);
+        return -1;
+    }
+}
+static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno) {
+    PyCodeObject *py_code = 0;
+#if PY_MAJOR_VERSION >= 3
+    py_code = PyCode_NewEmpty(srcfile, funcname, firstlineno);
+    if (likely(py_code)) {
+        py_code->co_flags |= CO_OPTIMIZED | CO_NEWLOCALS;
+    }
+#else
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
+    py_funcname = PyString_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    py_srcfile = PyString_FromString(srcfile);
+    if (unlikely(!py_srcfile)) goto bad;
+    py_code = PyCode_New(
+        0,
+        0,
+        0,
+        CO_OPTIMIZED | CO_NEWLOCALS,
+        __pyx_empty_bytes,     /*PyObject *code,*/
+        __pyx_empty_tuple,     /*PyObject *consts,*/
+        __pyx_empty_tuple,     /*PyObject *names,*/
+        __pyx_empty_tuple,     /*PyObject *varnames,*/
+        __pyx_empty_tuple,     /*PyObject *freevars,*/
+        __pyx_empty_tuple,     /*PyObject *cellvars,*/
+        py_srcfile,       /*PyObject *filename,*/
+        py_funcname,      /*PyObject *name,*/
+        firstlineno,
+        __pyx_empty_bytes      /*PyObject *lnotab*/
+    );
+bad:
+    Py_XDECREF(py_srcfile);
+    Py_XDECREF(py_funcname);
+#endif
+    return py_code;
+}
+#endif
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -9989,14 +9654,54 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* PyErrExceptionMatches */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
@@ -10314,27 +10019,14 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
@@ -10495,144 +10187,14 @@
         __Pyx_SET_SIZE(L, Py_SIZE(L) - 1);
         return PyList_GET_ITEM(L, PyList_GET_SIZE(L));
     }
     return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyList_Type_pop, L);
 }
 #endif
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* PyObjectCallMethod1 */
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
 }
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
@@ -10656,17 +10218,345 @@
         if (unlikely(!retval))
             return -1;
         Py_DECREF(retval);
     }
     return 0;
 }
 
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
+/* PyIntCompare */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+    if (op1 == op2) {
+        Py_RETURN_TRUE;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = Py_SIZE(op1);
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        if (intval == 0) {
+            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+        } else if (intval < 0) {
+            if (size >= 0)
+                Py_RETURN_FALSE;
+            intval = -intval;
+            size = -size;
+        } else {
+            if (size <= 0)
+                Py_RETURN_FALSE;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    return (
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr = NULL;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
+/* pyobject_as_double */
+static double __Pyx__PyObject_AsDouble(PyObject* obj) {
+    PyObject* float_value;
+#if !CYTHON_USE_TYPE_SLOTS
+    float_value = PyNumber_Float(obj);  if ((0)) goto bad;
+#else
+    PyNumberMethods *nb = Py_TYPE(obj)->tp_as_number;
+    if (likely(nb) && likely(nb->nb_float)) {
+        float_value = nb->nb_float(obj);
+        if (likely(float_value) && unlikely(!PyFloat_Check(float_value))) {
+            PyErr_Format(PyExc_TypeError,
+                "__float__ returned non-float (type %.200s)",
+                Py_TYPE(float_value)->tp_name);
+            Py_DECREF(float_value);
+            goto bad;
+        }
+    } else if (PyUnicode_CheckExact(obj) || PyBytes_CheckExact(obj)) {
+#if PY_MAJOR_VERSION >= 3
+        float_value = PyFloat_FromString(obj);
+#else
+        float_value = PyFloat_FromString(obj, 0);
+#endif
+    } else {
+        PyObject* args = PyTuple_New(1);
+        if (unlikely(!args)) goto bad;
+        PyTuple_SET_ITEM(args, 0, obj);
+        float_value = PyObject_Call((PyObject*)&PyFloat_Type, args, 0);
+        PyTuple_SET_ITEM(args, 0, 0);
+        Py_DECREF(args);
+    }
+#endif
+    if (likely(float_value)) {
+        double value = PyFloat_AS_DOUBLE(float_value);
+        Py_DECREF(float_value);
+        return value;
+    }
+bad:
+    return (double)-1;
+}
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
+    PyObject *module = 0;
+    PyObject *global_dict = 0;
+    PyObject *empty_dict = 0;
+    PyObject *list;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (!py_import)
+        goto bad;
+    #endif
+    if (from_list)
+        list = from_list;
+    else {
+        empty_list = PyList_New(0);
+        if (!empty_list)
+            goto bad;
+        list = empty_list;
+    }
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
+    empty_dict = PyDict_New();
+    if (!empty_dict)
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                module = PyImport_ImportModuleLevelObject(
+                    name, global_dict, empty_dict, list, 1);
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (!py_level)
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, global_dict, empty_dict, list, level);
+            #endif
+        }
+    }
+bad:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
+    return module;
+}
+
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
+    }
+    return value;
+}
+
+/* HasAttr */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (unlikely(!r)) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
@@ -10900,198 +10790,14 @@
         *pkey = next_item;
     } else {
         *pvalue = next_item;
     }
     return 1;
 }
 
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
-    PyObject *module = 0;
-    PyObject *global_dict = 0;
-    PyObject *empty_dict = 0;
-    PyObject *list;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
-        goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
-        empty_list = PyList_New(0);
-        if (!empty_list)
-            goto bad;
-        list = empty_list;
-    }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
-    empty_dict = PyDict_New();
-    if (!empty_dict)
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
-            #endif
-        }
-    }
-bad:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
-/* HasAttr */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
-    PyObject *r;
-    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "hasattr(): attribute name must be string");
-        return -1;
-    }
-    r = __Pyx_GetAttr(o, n);
-    if (unlikely(!r)) {
-        PyErr_Clear();
-        return 0;
-    } else {
-        Py_DECREF(r);
-        return 1;
-    }
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -11134,14 +10840,32 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
+/* SetVTable */
+static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+#if PY_VERSION_HEX >= 0x02070000
+    PyObject *ob = PyCapsule_New(vtable, 0, 0);
+#else
+    PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
+#endif
+    if (!ob)
+        goto bad;
+    if (PyDict_SetItem(dict, __pyx_n_s_pyx_vtable, ob) < 0)
+        goto bad;
+    Py_DECREF(ob);
+    return 0;
+bad:
+    Py_XDECREF(ob);
+    return -1;
+}
+
 /* PyObjectGetAttrStrNoError */
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
@@ -11260,43 +10984,14 @@
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -12066,34 +11761,14 @@
         result = PyObject_Call(metaclass, margs, mkw);
         Py_DECREF(margs);
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
-/* GetNameInClass */
-static PyObject *__Pyx_GetGlobalNameAfterAttributeLookup(PyObject *name) {
-    PyObject *result;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        return NULL;
-    __Pyx_PyErr_Clear();
-    __Pyx_GetModuleGlobalNameUncached(result, name);
-    return result;
-}
-static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name) {
-    PyObject *result;
-    result = __Pyx_PyObject_GetAttrStr(nmspace, name);
-    if (!result) {
-        result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
-    }
-    return result;
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
```

### Comparing `multimcts-0.4/multimcts/mcts.cpp` & `multimcts-0.4.1/multimcts/mcts.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1008,51 +1008,102 @@
   "multimcts/mcts.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9multimcts_4mcts_Node;
 struct __pyx_obj_9multimcts_4mcts_MCTS;
+struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate;
+
+/* "multimcts/mcts.pyx":225
+ *         return child
+ * 
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
+ *         """Step 3: Simulation (aka playout/rollout)
+ *         Play out a game, from the given node to termination, and return the final reward.
+ */
+struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate {
+  int __pyx_n;
+  PyObject *heuristic;
+};
 
 /* "multimcts/mcts.pyx":49
  * 
  * 
  * cdef class Node:             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
- * 
+ *     Args:
  */
 struct __pyx_obj_9multimcts_4mcts_Node {
   PyObject_HEAD
-  PyObject *_state;
-  PyObject *_move;
-  std::string _team;
-  struct __pyx_obj_9multimcts_4mcts_Node *_parent;
-  PyObject *_children;
-  PyObject *_remaining_moves;
-  std::map<std::string,float>  _total_reward;
-  int _num_visits;
-  double log_visits;
-  int _is_terminal;
-  int _is_fully_expanded;
+  struct __pyx_vtabstruct_9multimcts_4mcts_Node *__pyx_vtab;
+  PyObject *state;
+  PyObject *move;
+  PyObject *team;
+  std::string cteam;
+  struct __pyx_obj_9multimcts_4mcts_Node *parent;
+  PyObject *children;
+  PyObject *remaining_moves;
+  std::map<std::string,double>  rewards;
+  int visits;
+  int is_terminal;
+  int is_fully_expanded;
+  double avg_reward;
+  double sqrtlog_visits;
+  double invsqrt_visits;
 };
 
 
-/* "multimcts/mcts.pyx":114
+/* "multimcts/mcts.pyx":134
  * 
  * 
  * cdef class MCTS:             # <<<<<<<<<<<<<<
  *     cdef double exploration_bias
  * 
  */
 struct __pyx_obj_9multimcts_4mcts_MCTS {
   PyObject_HEAD
+  struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *__pyx_vtab;
   double exploration_bias;
 };
 
 
+
+/* "multimcts/mcts.pyx":49
+ * 
+ * 
+ * cdef class Node:             # <<<<<<<<<<<<<<
+ *     """Represents a game state node in the MCTS search tree.
+ *     Args:
+ */
+
+struct __pyx_vtabstruct_9multimcts_4mcts_Node {
+  PyObject *(*apply_rewards)(struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> );
+  double (*ucb)(struct __pyx_obj_9multimcts_4mcts_Node *, double, double);
+};
+static struct __pyx_vtabstruct_9multimcts_4mcts_Node *__pyx_vtabptr_9multimcts_4mcts_Node;
+
+
+/* "multimcts/mcts.pyx":134
+ * 
+ * 
+ * cdef class MCTS:             # <<<<<<<<<<<<<<
+ *     cdef double exploration_bias
+ * 
+ */
+
+struct __pyx_vtabstruct_9multimcts_4mcts_MCTS {
+  struct __pyx_obj_9multimcts_4mcts_Node *(*select)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+  struct __pyx_obj_9multimcts_4mcts_Node *(*expand)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+  std::map<std::string,double>  (*simulate)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args);
+  PyObject *(*backpropagate)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> );
+  struct __pyx_obj_9multimcts_4mcts_Node *(*get_best_child)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *);
+};
+static struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *__pyx_vtabptr_9multimcts_4mcts_MCTS;
+
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
@@ -1119,21 +1170,14 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1162,14 +1206,253 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
+/* Profile.proto */
+#ifndef CYTHON_PROFILE
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
+  #define CYTHON_PROFILE 0
+#else
+  #define CYTHON_PROFILE 1
+#endif
+#endif
+#ifndef CYTHON_TRACE_NOGIL
+  #define CYTHON_TRACE_NOGIL 0
+#else
+  #if CYTHON_TRACE_NOGIL && !defined(CYTHON_TRACE)
+    #define CYTHON_TRACE 1
+  #endif
+#endif
+#ifndef CYTHON_TRACE
+  #define CYTHON_TRACE 0
+#endif
+#if CYTHON_TRACE
+  #undef CYTHON_PROFILE_REUSE_FRAME
+#endif
+#ifndef CYTHON_PROFILE_REUSE_FRAME
+  #define CYTHON_PROFILE_REUSE_FRAME 0
+#endif
+#if CYTHON_PROFILE || CYTHON_TRACE
+  #include "compile.h"
+  #include "frameobject.h"
+  #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #if CYTHON_PROFILE_REUSE_FRAME
+    #define CYTHON_FRAME_MODIFIER static
+    #define CYTHON_FRAME_DEL(frame)
+  #else
+    #define CYTHON_FRAME_MODIFIER
+    #define CYTHON_FRAME_DEL(frame) Py_CLEAR(frame)
+  #endif
+  #define __Pyx_TraceDeclarations\
+      static PyCodeObject *__pyx_frame_code = NULL;\
+      CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
+      int __Pyx_use_tracing = 0;
+  #define __Pyx_TraceFrameInit(codeobj)\
+      if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
+#if PY_VERSION_HEX >= 0x030b00a2
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+#elif PY_VERSION_HEX >= 0x030a00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->cframe->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->cframe->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                 || tstate->c_profilefunc != NULL);\
+      } while (0)
+#else
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     (unlikely((tstate)->use_tracing) &&\
+         (!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #define __Pyx_EnterTracing(tstate)\
+      do { tstate->tracing++; tstate->use_tracing = 0; } while (0)
+  #define __Pyx_LeaveTracing(tstate)\
+      do {\
+          tstate->tracing--;\
+          tstate->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
+                                         || tstate->c_profilefunc != NULL);\
+      } while (0)
+#endif
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  if (nogil) {\
+      if (CYTHON_TRACE_NOGIL) {\
+          PyThreadState *tstate;\
+          PyGILState_STATE state = PyGILState_Ensure();\
+          tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 1, 1)) {\
+              __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          }\
+          PyGILState_Release(state);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  } else {\
+      PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #else
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
+  {   PyThreadState* tstate = PyThreadState_GET();\
+      if (__Pyx_IsTracing(tstate, 1, 1)) {\
+          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
+          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
+      }\
+  }
+  #endif
+  #define __Pyx_TraceException()\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 1)) {\
+          __Pyx_EnterTracing(tstate);\
+          PyObject *exc_info = __Pyx_GetExceptionTuple(tstate);\
+          if (exc_info) {\
+              if (CYTHON_TRACE && tstate->c_tracefunc)\
+                  tstate->c_tracefunc(\
+                      tstate->c_traceobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              tstate->c_profilefunc(\
+                  tstate->c_profileobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
+              Py_DECREF(exc_info);\
+          }\
+          __Pyx_LeaveTracing(tstate);\
+      }\
+  }
+  static void __Pyx_call_return_trace_func(PyThreadState *tstate, PyFrameObject *frame, PyObject *result) {
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_EnterTracing(tstate);
+      if (CYTHON_TRACE && tstate->c_tracefunc)
+          tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_RETURN, result);
+      if (tstate->c_profilefunc)
+          tstate->c_profilefunc(tstate->c_profileobj, frame, PyTrace_RETURN, result);
+      CYTHON_FRAME_DEL(frame);
+      __Pyx_LeaveTracing(tstate);
+      __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0)) {\
+                  __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+              }\
+              PyGILState_Release(state);\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0)) {\
+              __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceReturn(result, nogil)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0)) {\
+          __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
+      }\
+  }
+  #endif
+  static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno);
+  static int __Pyx_TraceSetupAndCall(PyCodeObject** code, PyFrameObject** frame, PyThreadState* tstate, const char *funcname, const char *srcfile, int firstlineno);
+#else
+  #define __Pyx_TraceDeclarations
+  #define __Pyx_TraceFrameInit(codeobj)
+  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)   if ((1)); else goto_error;
+  #define __Pyx_TraceException()
+  #define __Pyx_TraceReturn(result, nogil)
+#endif
+#if CYTHON_TRACE
+  static int __Pyx_call_line_trace_func(PyThreadState *tstate, PyFrameObject *frame, int lineno) {
+      int ret;
+      PyObject *type, *value, *traceback;
+      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+      __Pyx_PyFrame_SetLineNumber(frame, lineno);
+      __Pyx_EnterTracing(tstate);
+      ret = tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_LINE, NULL);
+      __Pyx_LeaveTracing(tstate);
+      if (likely(!ret)) {
+          __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+      } else {
+          Py_XDECREF(type);
+          Py_XDECREF(value);
+          Py_XDECREF(traceback);
+      }
+      return ret;
+  }
+  #ifdef WITH_THREAD
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      if (nogil) {\
+          if (CYTHON_TRACE_NOGIL) {\
+              int ret = 0;\
+              PyThreadState *tstate;\
+              PyGILState_STATE state = PyGILState_Ensure();\
+              tstate = __Pyx_PyThreadState_Current;\
+              if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+                  ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              }\
+              PyGILState_Release(state);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      } else {\
+          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+          if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+              int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+              if (unlikely(ret)) goto_error;\
+          }\
+      }\
+  }
+  #else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
+  if (likely(!__Pyx_use_tracing)); else {\
+      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
+      if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
+          int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
+          if (unlikely(ret)) goto_error;\
+      }\
+  }
+  #endif
+#else
+  #define __Pyx_TraceLine(lineno, nogil, goto_error)   if ((1)); else goto_error;
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
@@ -1286,14 +1569,19 @@
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1344,17 +1632,14 @@
 
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* ExtTypeTest.proto */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
-
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* pop.proto */
@@ -1393,38 +1678,14 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -1440,16 +1701,76 @@
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* append.proto */
 static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
 
-/* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
+/* PyIntCompare.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
+/* pyobject_as_double.proto */
+static double __Pyx__PyObject_AsDouble(PyObject* obj);
+#if CYTHON_COMPILING_IN_PYPY
+#define __Pyx_PyObject_AsDouble(obj)\
+(likely(PyFloat_CheckExact(obj)) ? PyFloat_AS_DOUBLE(obj) :\
+ likely(PyInt_CheckExact(obj)) ?\
+ PyFloat_AsDouble(obj) : __Pyx__PyObject_AsDouble(obj))
+#else
+#define __Pyx_PyObject_AsDouble(obj)\
+((likely(PyFloat_CheckExact(obj))) ?\
+ PyFloat_AS_DOUBLE(obj) : __Pyx__PyObject_AsDouble(obj))
+#endif
+
+/* ExtTypeTest.proto */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
+
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
@@ -1479,78 +1800,37 @@
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
-
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
-/* HasAttr.proto */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
-
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
+/* SetVTable.proto */
+static int __Pyx_SetVtable(PyObject *dict, void *vtable);
+
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
-/* ObjectGetItem.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
-#else
-#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
-#endif
-
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1626,18 +1906,14 @@
 
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
-/* GetNameInClass.proto */
-#define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
-static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1737,14 +2013,21 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+static PyObject *__pyx_f_9multimcts_4mcts_4Node_apply_rewards(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, std::map<std::string,double>  __pyx_v_crewards); /* proto*/
+static double __pyx_f_9multimcts_4mcts_4Node_ucb(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, double __pyx_v_exploration_bias, double __pyx_v_parent_sqrtlog_visits); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_expand(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
+static std::map<std::string,double>  __pyx_f_9multimcts_4mcts_4MCTS_simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args); /* proto*/
+static PyObject *__pyx_f_9multimcts_4mcts_4MCTS_backpropagate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, std::map<std::string,double>  __pyx_v_crewards); /* proto*/
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_get_best_child(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto*/
 
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'libcpp.utility' */
 
 /* Module declarations from 'libcpp.map' */
 
@@ -1763,105 +2046,86 @@
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *, PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
-static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &); /*proto*/
-static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *); /*proto*/
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____double(std::map<std::string,double>  const &); /*proto*/
+static std::map<std::string,double>  __pyx_convert_map_from_py_std_3a__3a_string__and_double(PyObject *); /*proto*/
 #define __Pyx_MODULE_NAME "multimcts.mcts"
 extern int __pyx_module_is_main_multimcts__mcts;
 int __pyx_module_is_main_multimcts__mcts = 0;
 
 /* Implementation of 'multimcts.mcts' */
-static PyObject *__pyx_builtin_staticmethod;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_ValueError;
-static PyObject *__pyx_builtin_IndexError;
 static const char __pyx_k_Any[] = "Any";
 static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_pop[] = "pop";
-static const char __pyx_k_val[] = "val";
 static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_List[] = "List";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Move[] = "Move";
 static const char __pyx_k_Node[] = "Node";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_Team[] = "Team";
-static const char __pyx_k_ckey[] = "ckey";
 static const char __pyx_k_dict[] = "__dict__";
-static const char __pyx_k_item[] = "item";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_move[] = "move";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Union[] = "Union";
-static const char __pyx_k_child[] = "child";
-static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_state[] = "state";
-static const char __pyx_k_visit[] = "visit";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_choice[] = "choice";
-static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_parent[] = "parent";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
-static const char __pyx_k_reward[] = "reward";
-static const char __pyx_k_select[] = "select";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Rewards[] = "Rewards";
-static const char __pyx_k_creward[] = "creward";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_shuffle[] = "shuffle";
-static const char __pyx_k_children[] = "children";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_max_time[] = "max_time";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_GameState[] = "GameState";
 static const char __pyx_k_heuristic[] = "heuristic";
 static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_make_move[] = "make_move";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
-static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_get_reward[] = "get_reward";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_is_terminal[] = "is_terminal";
 static const char __pyx_k_return_type[] = "return_type";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
-static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_stringsource[] = "stringsource";
-static const char __pyx_k_backpropagate[] = "backpropagate";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
-static const char __pyx_k_get_best_child[] = "get_best_child";
 static const char __pyx_k_max_iterations[] = "max_iterations";
 static const char __pyx_k_multimcts_mcts[] = "multimcts.mcts";
 static const char __pyx_k_must_be_one_of[] = ", must be one of ";
 static const char __pyx_k_get_legal_moves[] = "get_legal_moves";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
-static const char __pyx_k_remaining_moves[] = "remaining_moves";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_exploration_bias[] = "exploration_bias";
 static const char __pyx_k_get_current_team[] = "get_current_team";
 static const char __pyx_k_pyx_unpickle_MCTS[] = "__pyx_unpickle_MCTS";
 static const char __pyx_k_pyx_unpickle_Node[] = "__pyx_unpickle_Node";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_multimcts_mcts_pyx[] = "multimcts/mcts.pyx";
@@ -1873,17 +2137,16 @@
 static const char __pyx_k_GameState_get_legal_moves[] = "GameState.get_legal_moves";
 static const char __pyx_k_GameState_get_current_team[] = "GameState.get_current_team";
 static const char __pyx_k_GameState_must_implement_get_cur[] = "GameState must implement get_current_team.";
 static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
 static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
 static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
 static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
-static const char __pyx_k_Tried_to_expand_a_node_with_no_r[] = "Tried to expand a node with no remaining moves.";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))";
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_GameState;
 static PyObject *__pyx_n_u_GameState;
 static PyObject *__pyx_n_s_GameState_get_current_team;
 static PyObject *__pyx_n_s_GameState_get_legal_moves;
@@ -1893,167 +2156,135 @@
 static PyObject *__pyx_kp_u_GameState_must_implement_get_cur;
 static PyObject *__pyx_kp_u_GameState_must_implement_get_leg;
 static PyObject *__pyx_kp_u_GameState_must_implement_get_rew;
 static PyObject *__pyx_kp_u_GameState_must_implement_is_term;
 static PyObject *__pyx_kp_u_GameState_must_implement_make_mo;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
-static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_u_Invalid_return_type;
 static PyObject *__pyx_n_s_List;
 static PyObject *__pyx_n_s_MCTS;
 static PyObject *__pyx_n_s_Move;
 static PyObject *__pyx_n_s_Node;
 static PyObject *__pyx_kp_u_None;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_kp_u_One_or_more_of_max_time_max_iter;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_Rewards;
 static PyObject *__pyx_n_s_Team;
-static PyObject *__pyx_kp_u_Tried_to_expand_a_node_with_no_r;
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_append;
-static PyObject *__pyx_n_s_backpropagate;
-static PyObject *__pyx_n_s_child;
-static PyObject *__pyx_n_s_children;
 static PyObject *__pyx_n_s_choice;
-static PyObject *__pyx_n_s_ckey;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_creward;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_expand;
 static PyObject *__pyx_n_s_exploration_bias;
-static PyObject *__pyx_n_s_get_best_child;
 static PyObject *__pyx_n_s_get_current_team;
 static PyObject *__pyx_n_s_get_legal_moves;
 static PyObject *__pyx_n_s_get_reward;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_heuristic;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_is_terminal;
-static PyObject *__pyx_n_s_item;
-static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_iteritems;
-static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_lower;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_make_move;
 static PyObject *__pyx_n_s_max_iterations;
 static PyObject *__pyx_n_s_max_time;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_move;
 static PyObject *__pyx_n_u_move;
 static PyObject *__pyx_n_s_multimcts_mcts;
 static PyObject *__pyx_kp_s_multimcts_mcts_pyx;
 static PyObject *__pyx_kp_u_must_be_one_of;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
-static PyObject *__pyx_n_s_node;
 static PyObject *__pyx_n_u_node;
 static PyObject *__pyx_n_s_parent;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pop;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_MCTS;
 static PyObject *__pyx_n_s_pyx_unpickle_Node;
+static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_random;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_remaining_moves;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_return_type;
-static PyObject *__pyx_n_s_reward;
-static PyObject *__pyx_n_s_select;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shuffle;
-static PyObject *__pyx_n_s_simulate;
 static PyObject *__pyx_n_s_state;
 static PyObject *__pyx_n_u_state;
-static PyObject *__pyx_n_s_staticmethod;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_s_update;
-static PyObject *__pyx_n_s_val;
-static PyObject *__pyx_n_s_visit;
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyList_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
-static PyObject *__pyx_int_24284988;
-static PyObject *__pyx_int_53904430;
+static PyObject *__pyx_int_0;
+static PyObject *__pyx_int_56097295;
+static PyObject *__pyx_int_59888949;
 static PyObject *__pyx_int_82662024;
+static PyObject *__pyx_int_99932858;
 static PyObject *__pyx_int_203704333;
-static PyObject *__pyx_int_227935910;
 static PyObject *__pyx_int_231097371;
-static PyObject *__pyx_tuple_;
+static PyObject *__pyx_codeobj_;
 static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
+static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
+static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__3;
+static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
 /* Late includes */
 
 /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
@@ -2073,29 +2304,32 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj_)
   __Pyx_RefNannySetupContext("get_current_team", 0);
+  __Pyx_TraceCall("get_current_team", __pyx_f[0], 22, 0, __PYX_ERR(0, 22, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 24, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":22
  * 
@@ -2107,92 +2341,97 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves[] = "Returns a list of all legal moves from this state.";
+static char __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves[] = "List of all legal moves from this state.";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves = {"get_legal_moves", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_legal_moves (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__3)
   __Pyx_RefNannySetupContext("get_legal_moves", 0);
+  __Pyx_TraceCall("get_legal_moves", __pyx_f[0], 26, 0, __PYX_ERR(0, 26, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 28, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_4make_move[] = "Returns a new GameState, which is the result of applying the given move to this state.\n        Note: The current state (self) should NOT be modified. Rather, modify a copy of it.\n        ";
+static char __pyx_doc_9multimcts_4mcts_9GameState_4make_move[] = "A new GameState--the result of applying the given move to this state.\n        Note: The current state (self) should NOT be modified. Rather, modify a copy of it.\n        ";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_5make_move = {"make_move", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_9GameState_5make_move, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_9GameState_4make_move};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
   CYTHON_UNUSED PyObject *__pyx_v_move = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -2250,184 +2489,196 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__5)
   __Pyx_RefNannySetupContext("make_move", 0);
+  __Pyx_TraceCall("make_move", __pyx_f[0], 30, 0, __PYX_ERR(0, 30, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 34, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal[] = "Checks if the game is over.";
+static char __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal[] = "Is the game over?";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal = {"is_terminal", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_6is_terminal};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_terminal (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__7)
   __Pyx_RefNannySetupContext("is_terminal", 0);
+  __Pyx_TraceCall("is_terminal", __pyx_f[0], 36, 0, __PYX_ERR(0, 36, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_9GameState_8get_reward[] = "Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}\n        Note: This method is only called on terminal states.\n        ";
+static char __pyx_doc_9multimcts_4mcts_9GameState_8get_reward[] = "The reward earned by the team that played the game-ending move (the \"terminal team\", or the team from the previous state).\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}\n        Note: This method is only called on terminal states.\n        ";
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_9get_reward = {"get_reward", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_9get_reward, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_8get_reward};
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_reward (wrapper)", 0);
   __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_8get_reward(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__9)
   __Pyx_RefNannySetupContext("get_reward", 0);
+  __Pyx_TraceCall("get_reward", __pyx_f[0], 40, 0, __PYX_ERR(0, 40, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":75
- *     cdef bint _is_fully_expanded
+/* "multimcts/mcts.pyx":72
+ *     cdef double avg_reward, sqrtlog_visits, invsqrt_visits
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self._state = state
- *         self._parent = parent
+ *         self.state = state
+ *         self.parent = parent
  */
 
 /* Python wrapper */
 static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_9multimcts_4mcts_4Node_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent = 0;
@@ -2471,15 +2722,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -2490,335 +2741,390 @@
     }
     __pyx_v_state = values[0];
     __pyx_v_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[1]);
     __pyx_v_move = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 72, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parent), __pyx_ptype_9multimcts_4mcts_Node, 1, "parent", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_parent), __pyx_ptype_9multimcts_4mcts_Node, 1, "parent", 0))) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), __pyx_v_state, __pyx_v_parent, __pyx_v_move);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  std::map<std::string,double>  __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  std::string __pyx_t_4;
-  std::map<std::string,float>  __pyx_t_5;
-  int __pyx_t_6;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  std::string __pyx_t_6;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_TraceCall("__init__", __pyx_f[0], 72, 0, __PYX_ERR(0, 72, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":76
+  /* "multimcts/mcts.pyx":73
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self._state = state             # <<<<<<<<<<<<<<
- *         self._parent = parent
- *         self._move = move
+ *         self.state = state             # <<<<<<<<<<<<<<
+ *         self.parent = parent
+ *         self.move = move
  */
   __Pyx_INCREF(__pyx_v_state);
   __Pyx_GIVEREF(__pyx_v_state);
-  __Pyx_GOTREF(__pyx_v_self->_state);
-  __Pyx_DECREF(__pyx_v_self->_state);
-  __pyx_v_self->_state = __pyx_v_state;
+  __Pyx_GOTREF(__pyx_v_self->state);
+  __Pyx_DECREF(__pyx_v_self->state);
+  __pyx_v_self->state = __pyx_v_state;
 
-  /* "multimcts/mcts.pyx":77
+  /* "multimcts/mcts.pyx":74
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
- *         self._state = state
- *         self._parent = parent             # <<<<<<<<<<<<<<
- *         self._move = move
- *         self._team = str(self._state.get_current_team()).encode()
+ *         self.state = state
+ *         self.parent = parent             # <<<<<<<<<<<<<<
+ *         self.move = move
+ * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_parent));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_parent));
-  __Pyx_GOTREF(__pyx_v_self->_parent);
-  __Pyx_DECREF(((PyObject *)__pyx_v_self->_parent));
-  __pyx_v_self->_parent = __pyx_v_parent;
+  __Pyx_GOTREF(__pyx_v_self->parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v_self->parent));
+  __pyx_v_self->parent = __pyx_v_parent;
 
-  /* "multimcts/mcts.pyx":78
- *         self._state = state
- *         self._parent = parent
- *         self._move = move             # <<<<<<<<<<<<<<
- *         self._team = str(self._state.get_current_team()).encode()
+  /* "multimcts/mcts.pyx":75
+ *         self.state = state
+ *         self.parent = parent
+ *         self.move = move             # <<<<<<<<<<<<<<
  * 
+ *         self.children:List['Node'] = []
  */
   __Pyx_INCREF(__pyx_v_move);
   __Pyx_GIVEREF(__pyx_v_move);
-  __Pyx_GOTREF(__pyx_v_self->_move);
-  __Pyx_DECREF(__pyx_v_self->_move);
-  __pyx_v_self->_move = __pyx_v_move;
-
-  /* "multimcts/mcts.pyx":79
- *         self._parent = parent
- *         self._move = move
- *         self._team = str(self._state.get_current_team()).encode()             # <<<<<<<<<<<<<<
- * 
- *         self._children:List['Node'] = []
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_2), NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_self->_team = __pyx_t_4;
+  __Pyx_GOTREF(__pyx_v_self->move);
+  __Pyx_DECREF(__pyx_v_self->move);
+  __pyx_v_self->move = __pyx_v_move;
 
-  /* "multimcts/mcts.pyx":81
- *         self._team = str(self._state.get_current_team()).encode()
+  /* "multimcts/mcts.pyx":77
+ *         self.move = move
  * 
- *         self._children:List['Node'] = []             # <<<<<<<<<<<<<<
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY
+ *         self.children:List['Node'] = []             # <<<<<<<<<<<<<<
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v_self->_children);
-  __Pyx_DECREF(__pyx_v_self->_children);
-  __pyx_v_self->_children = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v_self->children);
+  __Pyx_DECREF(__pyx_v_self->children);
+  __pyx_v_self->children = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":82
- * 
- *         self._children:List['Node'] = []
- *         self._num_visits = 0             # <<<<<<<<<<<<<<
- *         self.log_visits = -INFINITY
- *         self._total_reward = map[string,float]()
- */
-  __pyx_v_self->_num_visits = 0;
-
-  /* "multimcts/mcts.pyx":83
- *         self._children:List['Node'] = []
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY             # <<<<<<<<<<<<<<
- *         self._total_reward = map[string,float]()
+  /* "multimcts/mcts.pyx":78
  * 
+ *         self.children:List['Node'] = []
+ *         self.visits = 0             # <<<<<<<<<<<<<<
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()
  */
-  __pyx_v_self->log_visits = (-INFINITY);
+  __pyx_v_self->visits = 0;
 
-  /* "multimcts/mcts.pyx":84
- *         self._num_visits = 0
- *         self.log_visits = -INFINITY
- *         self._total_reward = map[string,float]()             # <<<<<<<<<<<<<<
- * 
- *         self._is_terminal = self._state.is_terminal()
+  /* "multimcts/mcts.pyx":79
+ *         self.children:List['Node'] = []
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()             # <<<<<<<<<<<<<<
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
  */
   try {
-    __pyx_t_5 = std::map<std::string,float> ();
+    __pyx_t_2 = std::map<std::string,double> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 84, __pyx_L1_error)
+    __PYX_ERR(0, 79, __pyx_L1_error)
   }
-  __pyx_v_self->_total_reward = __pyx_t_5;
+  __pyx_v_self->rewards = __pyx_t_2;
 
-  /* "multimcts/mcts.pyx":86
- *         self._total_reward = map[string,float]()
- * 
- *         self._is_terminal = self._state.is_terminal()             # <<<<<<<<<<<<<<
- *         if self._is_terminal:
- *             self._is_fully_expanded = True
+  /* "multimcts/mcts.pyx":80
+ *         self.visits = 0
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()             # <<<<<<<<<<<<<<
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_self->_is_terminal = __pyx_t_6;
+  __pyx_v_self->is_terminal = __pyx_t_5;
 
-  /* "multimcts/mcts.pyx":87
- * 
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:             # <<<<<<<<<<<<<<
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []
- */
-  __pyx_t_6 = (__pyx_v_self->_is_terminal != 0);
-  if (__pyx_t_6) {
-
-    /* "multimcts/mcts.pyx":88
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:
- *             self._is_fully_expanded = True             # <<<<<<<<<<<<<<
- *             self._remaining_moves = []
+  /* "multimcts/mcts.pyx":81
+ *         self.rewards = map[string,double]()
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal             # <<<<<<<<<<<<<<
+ *         if self.is_fully_expanded:
+ *             self.remaining_moves = []
+ */
+  __pyx_t_5 = __pyx_v_self->is_terminal;
+  __pyx_v_self->is_fully_expanded = __pyx_t_5;
+
+  /* "multimcts/mcts.pyx":82
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *             self.remaining_moves = []
  *         else:
  */
-    __pyx_v_self->_is_fully_expanded = 1;
+  __pyx_t_5 = (__pyx_v_self->is_fully_expanded != 0);
+  if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":89
- *         if self._is_terminal:
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":83
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:
+ *             self.remaining_moves = []             # <<<<<<<<<<<<<<
  *         else:
- *             self._is_fully_expanded = False
+ *             self.remaining_moves = self.state.get_legal_moves()
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
-    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
-    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
-    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __Pyx_GOTREF(__pyx_v_self->remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->remaining_moves);
+    __pyx_v_self->remaining_moves = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":87
- * 
- *         self._is_terminal = self._state.is_terminal()
- *         if self._is_terminal:             # <<<<<<<<<<<<<<
- *             self._is_fully_expanded = True
- *             self._remaining_moves = []
+    /* "multimcts/mcts.pyx":82
+ *         self.is_terminal = self.state.is_terminal()
+ *         self.is_fully_expanded = self.is_terminal
+ *         if self.is_fully_expanded:             # <<<<<<<<<<<<<<
+ *             self.remaining_moves = []
+ *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":91
- *             self._remaining_moves = []
- *         else:
- *             self._is_fully_expanded = False             # <<<<<<<<<<<<<<
- *             self._remaining_moves = self._state.get_legal_moves()
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
- */
-  /*else*/ {
-    __pyx_v_self->_is_fully_expanded = 0;
-
-    /* "multimcts/mcts.pyx":92
+  /* "multimcts/mcts.pyx":85
+ *             self.remaining_moves = []
  *         else:
- *             self._is_fully_expanded = False
- *             self._remaining_moves = self._state.get_legal_moves()             # <<<<<<<<<<<<<<
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
+ *             self.remaining_moves = self.state.get_legal_moves()             # <<<<<<<<<<<<<<
+ *             shuffle(self.remaining_moves)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
+  /*else*/ {
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_1);
-    __Pyx_GOTREF(__pyx_v_self->_remaining_moves);
-    __Pyx_DECREF(__pyx_v_self->_remaining_moves);
-    __pyx_v_self->_remaining_moves = __pyx_t_1;
+    __Pyx_GOTREF(__pyx_v_self->remaining_moves);
+    __Pyx_DECREF(__pyx_v_self->remaining_moves);
+    __pyx_v_self->remaining_moves = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":93
- *             self._is_fully_expanded = False
- *             self._remaining_moves = self._state.get_legal_moves()
- *             shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":86
+ *         else:
+ *             self.remaining_moves = self.state.get_legal_moves()
+ *             shuffle(self.remaining_moves)             # <<<<<<<<<<<<<<
  * 
- *     @property
+ *         # The following are cached for performance.
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_self->_remaining_moves) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->_remaining_moves);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_self->remaining_moves) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_self->remaining_moves);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":75
- *     cdef bint _is_fully_expanded
+  /* "multimcts/mcts.pyx":89
+ * 
+ *         # The following are cached for performance.
+ *         self.team = self.state.get_current_team()             # <<<<<<<<<<<<<<
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->team);
+  __Pyx_DECREF(__pyx_v_self->team);
+  __pyx_v_self->team = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "multimcts/mcts.pyx":90
+ *         # The following are cached for performance.
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()             # <<<<<<<<<<<<<<
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0
+ */
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_self->team); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_1), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_self->cteam = __pyx_t_6;
+
+  /* "multimcts/mcts.pyx":91
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ */
+  __pyx_t_5 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+  __pyx_t_7 = (__pyx_t_5 != 0);
+  if (__pyx_t_7) {
+
+    /* "multimcts/mcts.pyx":92
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0             # <<<<<<<<<<<<<<
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0
+ */
+    (__pyx_v_self->rewards[__pyx_v_self->parent->cteam]) = 0.0;
+
+    /* "multimcts/mcts.pyx":91
+ *         self.team = self.state.get_current_team()
+ *         self.cteam = str(self.team).encode()
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ */
+  }
+
+  /* "multimcts/mcts.pyx":93
+ *         if self.parent is not None:
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0             # <<<<<<<<<<<<<<
+ *         self.invsqrt_visits = 0
+ *         self.avg_reward = 0
+ */
+  __pyx_v_self->sqrtlog_visits = 0.0;
+
+  /* "multimcts/mcts.pyx":94
+ *             self.rewards[self.parent.cteam] = 0
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0             # <<<<<<<<<<<<<<
+ *         self.avg_reward = 0
+ * 
+ */
+  __pyx_v_self->invsqrt_visits = 0.0;
+
+  /* "multimcts/mcts.pyx":95
+ *         self.sqrtlog_visits = 0
+ *         self.invsqrt_visits = 0
+ *         self.avg_reward = 0             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  __pyx_v_self->avg_reward = 0.0;
+
+  /* "multimcts/mcts.pyx":72
+ *     cdef double avg_reward, sqrtlog_visits, invsqrt_visits
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):             # <<<<<<<<<<<<<<
- *         self._state = state
- *         self._parent = parent
+ *         self.state = state
+ *         self.parent = parent
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":96
+/* "multimcts/mcts.pyx":98
  * 
  *     @property
- *     def state(self) -> GameState: return self._state             # <<<<<<<<<<<<<<
+ *     def state(self) -> GameState: return self.state             # <<<<<<<<<<<<<<
  *     @property
- *     def parent(self) -> 'Node': return self._parent
+ *     def rewards(self): return self.rewards
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2828,523 +3134,626 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_TraceCall("__get__", __pyx_f[0], 98, 0, __PYX_ERR(0, 98, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_state);
-  __pyx_r = __pyx_v_self->_state;
+  __Pyx_INCREF(__pyx_v_self->state);
+  __pyx_r = __pyx_v_self->state;
   goto __pyx_L0;
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.Node.state.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":98
- *     def state(self) -> GameState: return self._state
- *     @property
- *     def parent(self) -> 'Node': return self._parent             # <<<<<<<<<<<<<<
+/* "multimcts/mcts.pyx":100
+ *     def state(self) -> GameState: return self.state
  *     @property
- *     def move(self) -> Move: return self._move
+ *     def rewards(self): return self.rewards             # <<<<<<<<<<<<<<
+ * 
+ *     @cython.cdivision(True)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6parent___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6parent___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_TraceCall("__get__", __pyx_f[0], 100, 0, __PYX_ERR(0, 100, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
-  __pyx_r = ((PyObject *)__pyx_v_self->_parent);
+  __pyx_t_1 = __pyx_convert_map_to_py_std_3a__3a_string____double(__pyx_v_self->rewards); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.Node.rewards.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":100
- *     def parent(self) -> 'Node': return self._parent
- *     @property
- *     def move(self) -> Move: return self._move             # <<<<<<<<<<<<<<
- *     @property
- *     def children(self) -> List['Node']: return self._children
+/* "multimcts/mcts.pyx":103
+ * 
+ *     @cython.cdivision(True)
+ *     cdef apply_rewards(self, map[string,double] crewards):             # <<<<<<<<<<<<<<
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4move___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4move___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_f_9multimcts_4mcts_4Node_apply_rewards(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, std::map<std::string,double>  __pyx_v_crewards) {
+  std::pair<std::string,double>  __pyx_v_item;
+  double __pyx_v_total_rewards;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_move);
-  __pyx_r = __pyx_v_self->_move;
-  goto __pyx_L0;
+  std::map<std::string,double> ::iterator __pyx_t_1;
+  std::pair<std::string,double>  __pyx_t_2;
+  int __pyx_t_3;
+  std::string __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("apply_rewards", 0);
+  __Pyx_TraceCall("apply_rewards", __pyx_f[0], 103, 0, __PYX_ERR(0, 103, __pyx_L1_error));
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+  /* "multimcts/mcts.pyx":105
+ *     cdef apply_rewards(self, map[string,double] crewards):
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1             # <<<<<<<<<<<<<<
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))
+ */
+  __pyx_v_self->visits = (__pyx_v_self->visits + 1);
 
-/* "multimcts/mcts.pyx":102
- *     def move(self) -> Move: return self._move
- *     @property
- *     def children(self) -> List['Node']: return self._children             # <<<<<<<<<<<<<<
- *     @property
- *     def remaining_moves(self) -> List[Move]: return self._remaining_moves
+  /* "multimcts/mcts.pyx":107
+ *         self.visits += 1
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))             # <<<<<<<<<<<<<<
+ *         self.invsqrt_visits = 1 / sqrt(self.visits)
+ * 
  */
+  __pyx_v_self->sqrtlog_visits = sqrt(log(__pyx_v_self->visits));
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_8children___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  /* "multimcts/mcts.pyx":108
+ * 
+ *         self.sqrtlog_visits = sqrt(log(self.visits))
+ *         self.invsqrt_visits = 1 / sqrt(self.visits)             # <<<<<<<<<<<<<<
+ * 
+ *         cdef pair[string,double] item
+ */
+  __pyx_v_self->invsqrt_visits = (1.0 / sqrt(__pyx_v_self->visits));
 
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+  /* "multimcts/mcts.pyx":111
+ * 
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0             # <<<<<<<<<<<<<<
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:
+ */
+  __pyx_v_total_rewards = 0.0;
+
+  /* "multimcts/mcts.pyx":112
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0
+ *         for item in crewards:             # <<<<<<<<<<<<<<
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ */
+  __pyx_t_1 = __pyx_v_crewards.begin();
+  for (;;) {
+    if (!(__pyx_t_1 != __pyx_v_crewards.end())) break;
+    __pyx_t_2 = *__pyx_t_1;
+    ++__pyx_t_1;
+    __pyx_v_item = __pyx_t_2;
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_8children___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_children);
-  __pyx_r = __pyx_v_self->_children;
-  goto __pyx_L0;
+    /* "multimcts/mcts.pyx":113
+ *         cdef double total_rewards = 0
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:             # <<<<<<<<<<<<<<
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ */
+    __pyx_t_3 = ((__pyx_v_self->rewards.count(__pyx_v_item.first) == 0) != 0);
+    if (__pyx_t_3) {
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+      /* "multimcts/mcts.pyx":114
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0             # <<<<<<<<<<<<<<
+ *             self.rewards[item.first] += item.second
+ *             total_rewards += self.rewards[item.first]
+ */
+      (__pyx_v_self->rewards[__pyx_v_item.first]) = 0.0;
 
-/* "multimcts/mcts.pyx":104
- *     def children(self) -> List['Node']: return self._children
- *     @property
- *     def remaining_moves(self) -> List[Move]: return self._remaining_moves             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":113
+ *         cdef double total_rewards = 0
+ *         for item in crewards:
+ *             if self.rewards.count(item.first) == 0:             # <<<<<<<<<<<<<<
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ */
+    }
+
+    /* "multimcts/mcts.pyx":115
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second             # <<<<<<<<<<<<<<
+ *             total_rewards += self.rewards[item.first]
  * 
- *     @cython.cdivision(True)
  */
+    __pyx_t_4 = __pyx_v_item.first;
+    (__pyx_v_self->rewards[__pyx_t_4]) = ((__pyx_v_self->rewards[__pyx_t_4]) + __pyx_v_item.second);
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+    /* "multimcts/mcts.pyx":116
+ *                 self.rewards[item.first] = 0
+ *             self.rewards[item.first] += item.second
+ *             total_rewards += self.rewards[item.first]             # <<<<<<<<<<<<<<
+ * 
+ *         if self.parent is not None:
+ */
+    __pyx_v_total_rewards = (__pyx_v_total_rewards + (__pyx_v_self->rewards[__pyx_v_item.first]));
 
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+    /* "multimcts/mcts.pyx":112
+ *         cdef pair[string,double] item
+ *         cdef double total_rewards = 0
+ *         for item in crewards:             # <<<<<<<<<<<<<<
+ *             if self.rewards.count(item.first) == 0:
+ *                 self.rewards[item.first] = 0
+ */
+  }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_15remaining_moves___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
-  __pyx_r = __pyx_v_self->_remaining_moves;
-  goto __pyx_L0;
+  /* "multimcts/mcts.pyx":118
+ *             total_rewards += self.rewards[item.first]
+ * 
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
+ */
+  __pyx_t_3 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+  __pyx_t_5 = (__pyx_t_3 != 0);
+  if (__pyx_t_5) {
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+    /* "multimcts/mcts.pyx":120
+ *         if self.parent is not None:
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits             # <<<<<<<<<<<<<<
+ * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):
+ */
+    __pyx_v_self->avg_reward = (((2.0 * (__pyx_v_self->rewards[__pyx_v_self->parent->cteam])) - __pyx_v_total_rewards) / ((double)__pyx_v_self->visits));
 
-/* "multimcts/mcts.pyx":109
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def visit(self):             # <<<<<<<<<<<<<<
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)
+    /* "multimcts/mcts.pyx":118
+ *             total_rewards += self.rewards[item.first]
+ * 
+ *         if self.parent is not None:             # <<<<<<<<<<<<<<
+ *             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
  */
+  }
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3visit(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("visit (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_2visit(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  /* "multimcts/mcts.pyx":103
+ * 
+ *     @cython.cdivision(True)
+ *     cdef apply_rewards(self, map[string,double] crewards):             # <<<<<<<<<<<<<<
+ *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+ *         self.visits += 1
+ */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.Node.apply_rewards", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2visit(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("visit", 0);
-
-  /* "multimcts/mcts.pyx":110
- *     @cython.wraparound(False)
- *     def visit(self):
- *         self._num_visits += 1             # <<<<<<<<<<<<<<
- *         self.log_visits = log(self._num_visits)
+/* "multimcts/mcts.pyx":122
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
  * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
+ *         """Upper Confidence Bound
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
-  __pyx_v_self->_num_visits = (__pyx_v_self->_num_visits + 1);
 
-  /* "multimcts/mcts.pyx":111
- *     def visit(self):
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)             # <<<<<<<<<<<<<<
+static double __pyx_f_9multimcts_4mcts_4Node_ucb(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, double __pyx_v_exploration_bias, double __pyx_v_parent_sqrtlog_visits) {
+  double __pyx_r;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("ucb", 0);
+  __Pyx_TraceCall("ucb", __pyx_f[0], 122, 0, __PYX_ERR(0, 122, __pyx_L1_error));
+
+  /* "multimcts/mcts.pyx":131
+ *         """
+ *         # ucb = avgR + C * sqrt(ln(N)) * (1/sqrt(n))
+ *         return self.avg_reward + exploration_bias * parent_sqrtlog_visits * self.invsqrt_visits             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_v_self->log_visits = log(__pyx_v_self->_num_visits);
+  __pyx_r = (__pyx_v_self->avg_reward + ((__pyx_v_exploration_bias * __pyx_v_parent_sqrtlog_visits) * __pyx_v_self->invsqrt_visits));
+  goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":109
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def visit(self):             # <<<<<<<<<<<<<<
- *         self._num_visits += 1
- *         self.log_visits = log(self._num_visits)
+  /* "multimcts/mcts.pyx":122
+ *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
+ * 
+ *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
+ *         """Upper Confidence Bound
+ *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("multimcts.mcts.Node.ucb", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  int __pyx_t_9;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
+  int __pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)             # <<<<<<<<<<<<<<
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->avg_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->_is_terminal); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_self->cteam); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->invsqrt_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_self->_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_self->is_fully_expanded); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __pyx_convert_map_to_py_std_3a__3a_string____float(__pyx_v_self->_total_reward); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_self->is_terminal); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_self->log_visits); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_map_to_py_std_3a__3a_string____double(__pyx_v_self->rewards); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyTuple_New(11); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble(__pyx_v_self->sqrtlog_visits); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_INCREF(__pyx_v_self->_children);
-  __Pyx_GIVEREF(__pyx_v_self->_children);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_self->_children);
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->visits); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_9 = PyTuple_New(14); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self->children);
+  __Pyx_GIVEREF(__pyx_v_self->children);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_self->children);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2);
-  __Pyx_INCREF(__pyx_v_self->_move);
-  __Pyx_GIVEREF(__pyx_v_self->_move);
-  PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_v_self->_move);
+  PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_t_3);
-  __Pyx_INCREF(((PyObject *)__pyx_v_self->_parent));
-  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->_parent));
-  PyTuple_SET_ITEM(__pyx_t_7, 5, ((PyObject *)__pyx_v_self->_parent));
-  __Pyx_INCREF(__pyx_v_self->_remaining_moves);
-  __Pyx_GIVEREF(__pyx_v_self->_remaining_moves);
-  PyTuple_SET_ITEM(__pyx_t_7, 6, __pyx_v_self->_remaining_moves);
-  __Pyx_INCREF(__pyx_v_self->_state);
-  __Pyx_GIVEREF(__pyx_v_self->_state);
-  PyTuple_SET_ITEM(__pyx_t_7, 7, __pyx_v_self->_state);
+  PyTuple_SET_ITEM(__pyx_t_9, 3, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_7, 8, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_9, 4, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_7, 9, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_9, 5, __pyx_t_5);
+  __Pyx_INCREF(__pyx_v_self->move);
+  __Pyx_GIVEREF(__pyx_v_self->move);
+  PyTuple_SET_ITEM(__pyx_t_9, 6, __pyx_v_self->move);
+  __Pyx_INCREF(((PyObject *)__pyx_v_self->parent));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_self->parent));
+  PyTuple_SET_ITEM(__pyx_t_9, 7, ((PyObject *)__pyx_v_self->parent));
+  __Pyx_INCREF(__pyx_v_self->remaining_moves);
+  __Pyx_GIVEREF(__pyx_v_self->remaining_moves);
+  PyTuple_SET_ITEM(__pyx_t_9, 8, __pyx_v_self->remaining_moves);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_7, 10, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_9, 9, __pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_9, 10, __pyx_t_7);
+  __Pyx_INCREF(__pyx_v_self->state);
+  __Pyx_GIVEREF(__pyx_v_self->state);
+  PyTuple_SET_ITEM(__pyx_t_9, 11, __pyx_v_self->state);
+  __Pyx_INCREF(__pyx_v_self->team);
+  __Pyx_GIVEREF(__pyx_v_self->team);
+  PyTuple_SET_ITEM(__pyx_t_9, 12, __pyx_v_self->team);
+  __Pyx_GIVEREF(__pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_9, 13, __pyx_t_8);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
-  __pyx_v_state = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
+  __pyx_t_8 = 0;
+  __pyx_v_state = ((PyObject*)__pyx_t_9);
+  __pyx_t_9 = 0;
 
   /* "(tree fragment)":6
  *     cdef bint use_setstate
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_7 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_v__dict = __pyx_t_7;
-  __pyx_t_7 = 0;
+  __pyx_t_9 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_v__dict = __pyx_t_9;
+  __pyx_t_9 = 0;
 
   /* "(tree fragment)":7
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
-  __pyx_t_8 = (__pyx_v__dict != Py_None);
-  __pyx_t_9 = (__pyx_t_8 != 0);
-  if (__pyx_t_9) {
+  __pyx_t_10 = (__pyx_v__dict != Py_None);
+  __pyx_t_11 = (__pyx_t_10 != 0);
+  if (__pyx_t_11) {
 
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v__dict);
-    __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_6));
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v__dict);
+    __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_8));
+    __pyx_t_8 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
  *         state += (_dict,)
  *         use_setstate = True             # <<<<<<<<<<<<<<
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  */
     __pyx_v_use_setstate = 1;
 
     /* "(tree fragment)":7
- *     state = (self._children, self._is_fully_expanded, self._is_terminal, self._move, self._num_visits, self._parent, self._remaining_moves, self._state, self._team, self._total_reward, self.log_visits)
+ *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
     goto __pyx_L3;
   }
 
   /* "(tree fragment)":11
  *         use_setstate = True
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None             # <<<<<<<<<<<<<<
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None             # <<<<<<<<<<<<<<
  *     if use_setstate:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  */
   /*else*/ {
-    __pyx_t_8 = (__pyx_v_self->_children != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
+    __pyx_t_10 = (__pyx_v_self->children != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
+    } else {
+      __pyx_t_11 = __pyx_t_12;
+      goto __pyx_L4_bool_binop_done;
+    }
+    __pyx_t_12 = (__pyx_v_self->move != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
     if (!__pyx_t_10) {
     } else {
-      __pyx_t_9 = __pyx_t_10;
+      __pyx_t_11 = __pyx_t_10;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_10 = (__pyx_v_self->_move != Py_None);
-    __pyx_t_8 = (__pyx_t_10 != 0);
-    if (!__pyx_t_8) {
+    __pyx_t_10 = (((PyObject *)__pyx_v_self->parent) != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
     } else {
-      __pyx_t_9 = __pyx_t_8;
+      __pyx_t_11 = __pyx_t_12;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_8 = (((PyObject *)__pyx_v_self->_parent) != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
+    __pyx_t_12 = (__pyx_v_self->remaining_moves != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
     if (!__pyx_t_10) {
     } else {
-      __pyx_t_9 = __pyx_t_10;
+      __pyx_t_11 = __pyx_t_10;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_10 = (__pyx_v_self->_remaining_moves != Py_None);
-    __pyx_t_8 = (__pyx_t_10 != 0);
-    if (!__pyx_t_8) {
+    __pyx_t_10 = (__pyx_v_self->state != Py_None);
+    __pyx_t_12 = (__pyx_t_10 != 0);
+    if (!__pyx_t_12) {
     } else {
-      __pyx_t_9 = __pyx_t_8;
+      __pyx_t_11 = __pyx_t_12;
       goto __pyx_L4_bool_binop_done;
     }
-    __pyx_t_8 = (__pyx_v_self->_state != Py_None);
-    __pyx_t_10 = (__pyx_t_8 != 0);
-    __pyx_t_9 = __pyx_t_10;
+    __pyx_t_12 = (__pyx_v_self->team != Py_None);
+    __pyx_t_10 = (__pyx_t_12 != 0);
+    __pyx_t_11 = __pyx_t_10;
     __pyx_L4_bool_binop_done:;
-    __pyx_v_use_setstate = __pyx_t_9;
+    __pyx_v_use_setstate = __pyx_t_11;
   }
   __pyx_L3:;
 
   /* "(tree fragment)":12
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
  */
-  __pyx_t_9 = (__pyx_v_use_setstate != 0);
-  if (__pyx_t_9) {
+  __pyx_t_11 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_11) {
 
     /* "(tree fragment)":13
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state             # <<<<<<<<<<<<<<
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_24284988);
-    __Pyx_GIVEREF(__pyx_int_24284988);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_56097295);
+    __Pyx_GIVEREF(__pyx_int_56097295);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_int_56097295);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_7, 2, Py_None);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_9, 2, Py_None);
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_9);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_state);
+    __pyx_t_8 = 0;
+    __pyx_t_9 = 0;
+    __pyx_r = __pyx_t_7;
     __pyx_t_7 = 0;
-    __pyx_r = __pyx_t_5;
-    __pyx_t_5 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
  *     else:
- *         use_setstate = self._children is not None or self._move is not None or self._parent is not None or self._remaining_moves is not None or self._state is not None
+ *         use_setstate = self.children is not None or self.move is not None or self.parent is not None or self.remaining_moves is not None or self.state is not None or self.team is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
  */
   }
 
   /* "(tree fragment)":15
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, None), state
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, None), state
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_pyx_unpickle_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_24284988);
-    __Pyx_GIVEREF(__pyx_int_24284988);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_int_24284988);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_56097295);
+    __Pyx_GIVEREF(__pyx_int_56097295);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_int_56097295);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_state);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_v_state);
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
-    __pyx_t_5 = 0;
+    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_9);
     __pyx_t_7 = 0;
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_9 = 0;
+    __pyx_r = __pyx_t_8;
+    __pyx_t_8 = 0;
     goto __pyx_L0;
   }
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
@@ -3355,94 +3764,100 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.Node.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4Node_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_Node, (type(self), 0x1728f3c, state)
+ *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.Node.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":117
+/* "multimcts/mcts.pyx":137
  *     cdef double exploration_bias
  * 
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
- * 
+ *         Args:
  */
 
 /* Python wrapper */
 static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n\n        Args:\n            exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.\n                It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).\n                The default \342\210\2322 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.\n        ";
+static char __pyx_doc_9multimcts_4mcts_4MCTS___init__[] = "Initializes an MCTS agent.\n        Args:\n            exploration_bias (float): The exploration bias, which balances exploration (favoring untested moves) and exploitation (favoring good moves).\n                The default \342\210\2322 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.\n        ";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
 #endif
 static int __pyx_pw_9multimcts_4mcts_4MCTS_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_exploration_bias;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -3467,79 +3882,90 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 137, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 137, __pyx_L3_error)
     } else {
       __pyx_v_exploration_bias = ((double)1.414);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 137, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_exploration_bias);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias) {
   int __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_TraceCall("__init__", __pyx_f[0], 137, 0, __PYX_ERR(0, 137, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":125
+  /* "multimcts/mcts.pyx":143
  *                 The default 2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
  *         """
  *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->exploration_bias = __pyx_v_exploration_bias;
 
-  /* "multimcts/mcts.pyx":117
+  /* "multimcts/mcts.pyx":137
  *     cdef double exploration_bias
  * 
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
- * 
+ *         Args:
  */
 
   /* function exit code */
   __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":128
+/* "multimcts/mcts.pyx":146
  * 
  *     @property
- *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
- *         return self.exploration_bias
+ *     def exploration_bias(self) -> float: return self.exploration_bias             # <<<<<<<<<<<<<<
  * 
+ *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3549,65 +3975,52 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "multimcts/mcts.pyx":129
- *     @property
- *     def exploration_bias(self) -> float:
- *         return self.exploration_bias             # <<<<<<<<<<<<<<
- * 
- *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
- */
+  __Pyx_TraceCall("__get__", __pyx_f[0], 146, 0, __PYX_ERR(0, 146, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":128
- * 
- *     @property
- *     def exploration_bias(self) -> float:             # <<<<<<<<<<<<<<
- *         return self.exploration_bias
- * 
- */
-
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.exploration_bias.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":131
- *         return self.exploration_bias
+/* "multimcts/mcts.pyx":148
+ *     def exploration_bias(self) -> float: return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
- * 
+ *         Args:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_2search[] = "Searches for this state's best move until some limit has been reached.\n\n        Args:\n            state (GameState): The game state for which to find the best move.\n            max_time (int|float): The maximum time to search, in seconds.\n            max_iterations (int): The maximum number of selections/simulations to perform.\n            heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.\n            return_type (str): One of \"state\", \"move\", or \"node\".\n        Returns:\n            GameState: A new game state which is the result of applying the best move to the given state.\n        ";
+static char __pyx_doc_9multimcts_4mcts_4MCTS_2search[] = "Searches for this state's best move until some limit has been reached.\n        Args:\n            state (GameState): The game state for which to find the best move.\n            max_time (int|float): The maximum time to search, in seconds.\n            max_iterations (int): The maximum number of selections/simulations to perform.\n            heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.\n            return_type (str): One of \"state\", \"move\", or \"node\".\n        Returns:\n            GameState: A new game state which is the result of applying the best move to the given state.\n        ";
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_3search(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v_max_time = 0;
   PyObject *__pyx_v_max_iterations = 0;
   PyObject *__pyx_v_heuristic = 0;
   PyObject *__pyx_v_return_type = 0;
   int __pyx_lineno = 0;
@@ -3642,183 +4055,183 @@
         Py_ssize_t index;
         for (index = 1; index < 5 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 131, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 148, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_state = values[0];
     __pyx_v_max_time = values[1];
     __pyx_v_max_iterations = values[2];
     __pyx_v_heuristic = values[3];
     __pyx_v_return_type = ((PyObject*)values[4]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 131, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 148, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyUnicode_Type), 1, "return_type", 1))) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_return_type), (&PyUnicode_Type), 1, "return_type", 1))) __PYX_ERR(0, 148, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_state, __pyx_v_max_time, __pyx_v_max_iterations, __pyx_v_heuristic, __pyx_v_return_type);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_return_type) {
   PyObject *__pyx_v_VALID_RETURN_TYPES = NULL;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = NULL;
-  double __pyx_v_exploration_bias;
   double __pyx_v_end_time;
   int __pyx_v_i;
-  PyObject *__pyx_v_child = NULL;
-  PyObject *__pyx_v_reward = NULL;
-  PyObject *__pyx_v_best = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
+  std::map<std::string,double>  __pyx_v_rewards;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   int __pyx_t_8;
   double __pyx_t_9;
-  int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
+  std::map<std::string,double>  __pyx_t_10;
+  struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
+  __Pyx_TraceCall("search", __pyx_f[0], 148, 0, __PYX_ERR(0, 148, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_return_type);
 
-  /* "multimcts/mcts.pyx":143
+  /* "multimcts/mcts.pyx":159
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         return_type = return_type.lower()             # <<<<<<<<<<<<<<
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_return_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_return_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_return_type, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":144
+  /* "multimcts/mcts.pyx":160
  *         """
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}             # <<<<<<<<<<<<<<
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_state) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_move) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-  if (PySet_Add(__pyx_t_1, __pyx_n_u_node) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_state) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_move) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_1, __pyx_n_u_node) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __pyx_v_VALID_RETURN_TYPES = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":145
+  /* "multimcts/mcts.pyx":161
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
-  __pyx_t_4 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PySet_ContainsTF(__pyx_v_return_type, __pyx_v_VALID_RETURN_TYPES, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 161, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":146
+    /* "multimcts/mcts.pyx":162
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')             # <<<<<<<<<<<<<<
  * 
  *         if max_time is None and max_iterations is None:
  */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_return_type);
     __pyx_t_6 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_return_type);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_return_type);
-    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_return_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_return_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_must_be_one_of);
     __pyx_t_6 += 17;
     __Pyx_GIVEREF(__pyx_kp_u_must_be_one_of);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_must_be_one_of);
-    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_VALID_RETURN_TYPES, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 146, __pyx_L1_error)
+    __PYX_ERR(0, 162, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":145
+    /* "multimcts/mcts.pyx":161
  *         return_type = return_type.lower()
  *         VALID_RETURN_TYPES = {"state","move","node"}
  *         if return_type not in VALID_RETURN_TYPES:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":148
+  /* "multimcts/mcts.pyx":164
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   __pyx_t_4 = (__pyx_v_max_time == Py_None);
@@ -3830,1386 +4243,896 @@
   }
   __pyx_t_8 = (__pyx_v_max_iterations == Py_None);
   __pyx_t_4 = (__pyx_t_8 != 0);
   __pyx_t_5 = __pyx_t_4;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_5)) {
 
-    /* "multimcts/mcts.pyx":149
+    /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 149, __pyx_L1_error)
+    __PYX_ERR(0, 165, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":148
+    /* "multimcts/mcts.pyx":164
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
  * 
  *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":151
+  /* "multimcts/mcts.pyx":167
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
- *         cdef double exploration_bias = self.exploration_bias
+ *         cdef double end_time
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_v_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_v_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":153
- *         node = Node(state)
- * 
- *         cdef double exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":170
  * 
  *         cdef double end_time
+ *         cdef int i = 0             # <<<<<<<<<<<<<<
+ *         if max_time is not None:
+ *             end_time = time() + max_time
  */
-  __pyx_t_9 = __pyx_v_self->exploration_bias;
-  __pyx_v_exploration_bias = __pyx_t_9;
+  __pyx_v_i = 0;
 
-  /* "multimcts/mcts.pyx":157
+  /* "multimcts/mcts.pyx":171
  *         cdef double end_time
- *         cdef int i
+ *         cdef int i = 0
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
- *         if max_iterations is not None:
+ * 
  */
   __pyx_t_5 = (__pyx_v_max_time != Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":158
- *         cdef int i
+    /* "multimcts/mcts.pyx":172
+ *         cdef int i = 0
  *         if max_time is not None:
  *             end_time = time() + max_time             # <<<<<<<<<<<<<<
- *         if max_iterations is not None:
- *             i = max_iterations
+ * 
+ *         while True:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_end_time = __pyx_t_9;
 
-    /* "multimcts/mcts.pyx":157
+    /* "multimcts/mcts.pyx":171
  *         cdef double end_time
- *         cdef int i
+ *         cdef int i = 0
  *         if max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time() + max_time
- *         if max_iterations is not None:
+ * 
  */
   }
 
-  /* "multimcts/mcts.pyx":159
- *         if max_time is not None:
+  /* "multimcts/mcts.pyx":174
  *             end_time = time() + max_time
- *         if max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = max_iterations
  * 
+ *         while True:             # <<<<<<<<<<<<<<
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)
  */
-  __pyx_t_4 = (__pyx_v_max_iterations != Py_None);
-  __pyx_t_5 = (__pyx_t_4 != 0);
-  if (__pyx_t_5) {
+  while (1) {
 
-    /* "multimcts/mcts.pyx":160
- *             end_time = time() + max_time
- *         if max_iterations is not None:
- *             i = max_iterations             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":175
  * 
  *         while True:
+ *             child = self.select(node)             # <<<<<<<<<<<<<<
+ *             rewards = self.simulate(child, heuristic=heuristic)
+ *             self.backpropagate(child, rewards)
  */
-    __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_max_iterations); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
-    __pyx_v_i = __pyx_t_10;
+    __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->select(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
+    __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":159
- *         if max_time is not None:
- *             end_time = time() + max_time
- *         if max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = max_iterations
+    /* "multimcts/mcts.pyx":176
+ *         while True:
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
+ *             self.backpropagate(child, rewards)
  * 
  */
-  }
+    __pyx_t_11.__pyx_n = 1;
+    __pyx_t_11.heuristic = __pyx_v_heuristic;
+    __pyx_t_10 = ((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->simulate(__pyx_v_self, __pyx_v_child, &__pyx_t_11); 
+    __pyx_v_rewards = __pyx_t_10;
 
-  /* "multimcts/mcts.pyx":162
- *             i = max_iterations
+    /* "multimcts/mcts.pyx":177
+ *             child = self.select(node)
+ *             rewards = self.simulate(child, heuristic=heuristic)
+ *             self.backpropagate(child, rewards)             # <<<<<<<<<<<<<<
  * 
- *         while True:             # <<<<<<<<<<<<<<
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)
+ *             # If there is only one legal move, we don't need to search.
  */
-  while (1) {
+    __pyx_t_2 = ((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->backpropagate(__pyx_v_self, __pyx_v_child, __pyx_v_rewards); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":163
+    /* "multimcts/mcts.pyx":180
+ * 
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:             # <<<<<<<<<<<<<<
+ *                 break
  * 
- *         while True:
- *             child = self.select(node, exploration_bias)             # <<<<<<<<<<<<<<
- *             reward = self.simulate(child, heuristic=heuristic)
- *             self.backpropagate(child, reward)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_select); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_11 = NULL;
-    __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_11)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_11);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_10 = 1;
-      }
+    __pyx_t_5 = (__pyx_v_node->is_fully_expanded != 0);
+    if (__pyx_t_5) {
+    } else {
+      __pyx_t_4 = __pyx_t_5;
+      goto __pyx_L11_bool_binop_done;
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_v_node), __pyx_t_3};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_12 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      if (__pyx_t_11) {
-        __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
-      }
-      __Pyx_INCREF(((PyObject *)__pyx_v_node));
-      __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
-      __Pyx_GIVEREF(__pyx_t_3);
-      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_10, __pyx_t_3);
-      __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_2 = __pyx_v_node->children;
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_5 = ((__pyx_t_6 == 1) != 0);
+    __pyx_t_4 = __pyx_t_5;
+    __pyx_L11_bool_binop_done:;
+    if (__pyx_t_4) {
+
+      /* "multimcts/mcts.pyx":181
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *             if max_time is not None:
+ */
+      goto __pyx_L9_break;
+
+      /* "multimcts/mcts.pyx":180
+ * 
+ *             # If there is only one legal move, we don't need to search.
+ *             if node.is_fully_expanded and len(node.children) == 1:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
     }
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_2);
-    __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":164
- *         while True:
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)             # <<<<<<<<<<<<<<
- *             self.backpropagate(child, reward)
+    /* "multimcts/mcts.pyx":183
+ *                 break
  * 
+ *             if max_time is not None:             # <<<<<<<<<<<<<<
+ *                 if time() >= end_time:
+ *                     break
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_simulate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_v_child);
-    __Pyx_GIVEREF(__pyx_v_child);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_child);
-    __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_4 = (__pyx_v_max_time != Py_None);
+    __pyx_t_5 = (__pyx_t_4 != 0);
+    if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":165
- *             child = self.select(node, exploration_bias)
- *             reward = self.simulate(child, heuristic=heuristic)
- *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
- * 
- *             if max_time is not None and time() >= end_time:
- */
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 165, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_1 = NULL;
-    __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
-        __pyx_t_10 = 1;
+      /* "multimcts/mcts.pyx":184
+ * 
+ *             if max_time is not None:
+ *                 if time() >= end_time:             # <<<<<<<<<<<<<<
+ *                     break
+ *             if max_iterations is not None:
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+        }
       }
-    }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_12)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_3);
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_3);
-    } else
-    #endif
-    {
-      __pyx_t_2 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+      __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (__pyx_t_1) {
-        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1); __pyx_t_1 = NULL;
-      }
-      __Pyx_INCREF(__pyx_v_child);
-      __Pyx_GIVEREF(__pyx_v_child);
-      PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_10, __pyx_v_child);
-      __Pyx_INCREF(__pyx_v_reward);
-      __Pyx_GIVEREF(__pyx_v_reward);
-      PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_10, __pyx_v_reward);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_GE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":167
- *             self.backpropagate(child, reward)
- * 
- *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
- *                 break
+        /* "multimcts/mcts.pyx":185
+ *             if max_time is not None:
+ *                 if time() >= end_time:
+ *                     break             # <<<<<<<<<<<<<<
  *             if max_iterations is not None:
+ *                 i += 1
  */
-    __pyx_t_4 = (__pyx_v_max_time != Py_None);
-    __pyx_t_8 = (__pyx_t_4 != 0);
-    if (__pyx_t_8) {
-    } else {
-      __pyx_t_5 = __pyx_t_8;
-      goto __pyx_L12_bool_binop_done;
-    }
-    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_12);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
-      }
-    }
-    __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_t_12, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = __pyx_t_8;
-    __pyx_L12_bool_binop_done:;
-    if (__pyx_t_5) {
+        goto __pyx_L9_break;
 
-      /* "multimcts/mcts.pyx":168
+        /* "multimcts/mcts.pyx":184
  * 
- *             if max_time is not None and time() >= end_time:
- *                 break             # <<<<<<<<<<<<<<
+ *             if max_time is not None:
+ *                 if time() >= end_time:             # <<<<<<<<<<<<<<
+ *                     break
  *             if max_iterations is not None:
- *                 i -= 1
  */
-      goto __pyx_L10_break;
+      }
 
-      /* "multimcts/mcts.pyx":167
- *             self.backpropagate(child, reward)
- * 
- *             if max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
+      /* "multimcts/mcts.pyx":183
  *                 break
- *             if max_iterations is not None:
+ * 
+ *             if max_time is not None:             # <<<<<<<<<<<<<<
+ *                 if time() >= end_time:
+ *                     break
  */
     }
 
-    /* "multimcts/mcts.pyx":169
- *             if max_time is not None and time() >= end_time:
- *                 break
+    /* "multimcts/mcts.pyx":186
+ *                 if time() >= end_time:
+ *                     break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i -= 1
- *                 if i <= 0:
+ *                 i += 1
+ *                 if i >= max_iterations:
  */
     __pyx_t_5 = (__pyx_v_max_iterations != Py_None);
-    __pyx_t_8 = (__pyx_t_5 != 0);
-    if (__pyx_t_8) {
+    __pyx_t_4 = (__pyx_t_5 != 0);
+    if (__pyx_t_4) {
 
-      /* "multimcts/mcts.pyx":170
- *                 break
+      /* "multimcts/mcts.pyx":187
+ *                     break
  *             if max_iterations is not None:
- *                 i -= 1             # <<<<<<<<<<<<<<
- *                 if i <= 0:
+ *                 i += 1             # <<<<<<<<<<<<<<
+ *                 if i >= max_iterations:
  *                     break
  */
-      __pyx_v_i = (__pyx_v_i - 1);
+      __pyx_v_i = (__pyx_v_i + 1);
 
-      /* "multimcts/mcts.pyx":171
+      /* "multimcts/mcts.pyx":188
  *             if max_iterations is not None:
- *                 i -= 1
- *                 if i <= 0:             # <<<<<<<<<<<<<<
+ *                 i += 1
+ *                 if i >= max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
-      __pyx_t_8 = ((__pyx_v_i <= 0) != 0);
-      if (__pyx_t_8) {
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_v_max_iterations, Py_GE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (__pyx_t_4) {
 
-        /* "multimcts/mcts.pyx":172
- *                 i -= 1
- *                 if i <= 0:
+        /* "multimcts/mcts.pyx":189
+ *                 i += 1
+ *                 if i >= max_iterations:
  *                     break             # <<<<<<<<<<<<<<
  * 
- *         best = self.get_best_child(node, exploration_bias)
+ *         cdef Node best = self.get_best_child(node)
  */
-        goto __pyx_L10_break;
+        goto __pyx_L9_break;
 
-        /* "multimcts/mcts.pyx":171
+        /* "multimcts/mcts.pyx":188
  *             if max_iterations is not None:
- *                 i -= 1
- *                 if i <= 0:             # <<<<<<<<<<<<<<
+ *                 i += 1
+ *                 if i >= max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":169
- *             if max_time is not None and time() >= end_time:
- *                 break
+      /* "multimcts/mcts.pyx":186
+ *                 if time() >= end_time:
+ *                     break
  *             if max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i -= 1
- *                 if i <= 0:
+ *                 i += 1
+ *                 if i >= max_iterations:
  */
     }
   }
-  __pyx_L10_break:;
+  __pyx_L9_break:;
 
-  /* "multimcts/mcts.pyx":174
+  /* "multimcts/mcts.pyx":191
  *                     break
  * 
- *         best = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
+ *         cdef Node best = self.get_best_child(node)             # <<<<<<<<<<<<<<
  * 
  *         if return_type == "state":
  */
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 174, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = NULL;
-  __pyx_t_10 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_12);
-    if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-      __Pyx_INCREF(__pyx_t_1);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_12, function);
-      __pyx_t_10 = 1;
-    }
-  }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_12)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, ((PyObject *)__pyx_v_node), __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    if (__pyx_t_1) {
-      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_1); __pyx_t_1 = NULL;
-    }
-    __Pyx_INCREF(((PyObject *)__pyx_v_node));
-    __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-    PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, ((PyObject *)__pyx_v_node));
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_v_best = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->get_best_child(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_best = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":176
- *         best = self.get_best_child(node, exploration_bias)
+  /* "multimcts/mcts.pyx":193
+ *         cdef Node best = self.get_best_child(node)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_state, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_5 = (__pyx_t_8 != 0);
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_state, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":177
+    /* "multimcts/mcts.pyx":194
  * 
  *         if return_type == "state":
  *             return best.state             # <<<<<<<<<<<<<<
  *         elif return_type == "move":
  *             return best.move
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v_best->state);
+    __pyx_r = __pyx_v_best->state;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":176
- *         best = self.get_best_child(node, exploration_bias)
+    /* "multimcts/mcts.pyx":193
+ *         cdef Node best = self.get_best_child(node)
  * 
  *         if return_type == "state":             # <<<<<<<<<<<<<<
  *             return best.state
  *         elif return_type == "move":
  */
   }
 
-  /* "multimcts/mcts.pyx":178
+  /* "multimcts/mcts.pyx":195
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_move, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __pyx_t_8 = (__pyx_t_5 != 0);
-  if (__pyx_t_8) {
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_move, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_5 != 0);
+  if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":179
+    /* "multimcts/mcts.pyx":196
  *             return best.state
  *         elif return_type == "move":
  *             return best.move             # <<<<<<<<<<<<<<
  *         elif return_type == "node":
  *             return best
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_best, __pyx_n_s_move); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v_best->move);
+    __pyx_r = __pyx_v_best->move;
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":178
+    /* "multimcts/mcts.pyx":195
  *         if return_type == "state":
  *             return best.state
  *         elif return_type == "move":             # <<<<<<<<<<<<<<
  *             return best.move
  *         elif return_type == "node":
  */
   }
 
-  /* "multimcts/mcts.pyx":180
+  /* "multimcts/mcts.pyx":197
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
-  __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_node, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __pyx_t_5 = (__pyx_t_8 != 0);
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_v_return_type, __pyx_n_u_node, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":181
+    /* "multimcts/mcts.pyx":198
  *             return best.move
  *         elif return_type == "node":
  *             return best             # <<<<<<<<<<<<<<
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:
+ *     cdef Node select(self, Node node):
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_v_best);
-    __pyx_r = __pyx_v_best;
+    __Pyx_INCREF(((PyObject *)__pyx_v_best));
+    __pyx_r = ((PyObject *)__pyx_v_best);
     goto __pyx_L0;
 
-    /* "multimcts/mcts.pyx":180
+    /* "multimcts/mcts.pyx":197
  *         elif return_type == "move":
  *             return best.move
  *         elif return_type == "node":             # <<<<<<<<<<<<<<
  *             return best
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":131
- *         return self.exploration_bias
+  /* "multimcts/mcts.pyx":148
+ *     def exploration_bias(self) -> float: return self.exploration_bias
  * 
  *     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
- * 
+ *         Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_VALID_RETURN_TYPES);
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
-  __Pyx_XDECREF(__pyx_v_child);
-  __Pyx_XDECREF(__pyx_v_reward);
-  __Pyx_XDECREF(__pyx_v_best);
+  __Pyx_XDECREF((PyObject *)__pyx_v_child);
+  __Pyx_XDECREF((PyObject *)__pyx_v_best);
   __Pyx_XDECREF(__pyx_v_return_type);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":183
+/* "multimcts/mcts.pyx":200
  *             return best
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node select(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_4select[] = "Step 1: Selection\n        Traverse the tree for the node we most want to simulate.\n        Looks for an unexplored child of this node's best child's best child's...best child.\n        ";
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_5select(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  double __pyx_v_exploration_bias;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("select (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 183, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_4select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
+  __Pyx_TraceCall("select", __pyx_f[0], 200, 0, __PYX_ERR(0, 200, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":188
+  /* "multimcts/mcts.pyx":205
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
- *         while not node._is_terminal:             # <<<<<<<<<<<<<<
- *             if not node._is_fully_expanded:
+ *         while not node.is_terminal:             # <<<<<<<<<<<<<<
+ *             if not node.is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = ((!(__pyx_v_node->_is_terminal != 0)) != 0);
+    __pyx_t_1 = ((!(__pyx_v_node->is_terminal != 0)) != 0);
     if (!__pyx_t_1) break;
 
-    /* "multimcts/mcts.pyx":189
+    /* "multimcts/mcts.pyx":206
  *         """
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = ((!(__pyx_v_node->_is_fully_expanded != 0)) != 0);
+    __pyx_t_1 = ((!(__pyx_v_node->is_fully_expanded != 0)) != 0);
     if (__pyx_t_1) {
 
-      /* "multimcts/mcts.pyx":190
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:
+      /* "multimcts/mcts.pyx":207
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
- *                 node = self.get_best_child(node, exploration_bias)
+ *                 node = self.get_best_child(node)
  */
       __Pyx_XDECREF(((PyObject *)__pyx_r));
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_expand); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_4);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
-        }
-      }
-      __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, ((PyObject *)__pyx_v_node)) : __Pyx_PyObject_CallOneArg(__pyx_t_3, ((PyObject *)__pyx_v_node));
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->expand(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 190, __pyx_L1_error)
       __pyx_r = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2);
       __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":189
+      /* "multimcts/mcts.pyx":206
  *         """
- *         while not node._is_terminal:
- *             if not node._is_fully_expanded:             # <<<<<<<<<<<<<<
+ *         while not node.is_terminal:
+ *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":192
+    /* "multimcts/mcts.pyx":209
  *                 return self.expand(node)
  *             else:
- *                 node = self.get_best_child(node, exploration_bias)             # <<<<<<<<<<<<<<
- * 
+ *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
  *         return node
+ * 
  */
     /*else*/ {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 192, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = NULL;
-      __pyx_t_6 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_5);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
-          __pyx_t_6 = 1;
-        }
-      }
-      #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      } else
-      #endif
-      #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_5, ((PyObject *)__pyx_v_node), __pyx_t_4};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      } else
-      #endif
-      {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        if (__pyx_t_5) {
-          __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-        }
-        __Pyx_INCREF(((PyObject *)__pyx_v_node));
-        __Pyx_GIVEREF(((PyObject *)__pyx_v_node));
-        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, ((PyObject *)__pyx_v_node));
-        __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-        __pyx_t_4 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 192, __pyx_L1_error)
+      __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_9multimcts_4mcts_MCTS *)__pyx_v_self->__pyx_vtab)->get_best_child(__pyx_v_self, __pyx_v_node)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
       __pyx_t_2 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":194
- *                 node = self.get_best_child(node, exploration_bias)
- * 
+  /* "multimcts/mcts.pyx":210
+ *             else:
+ *                 node = self.get_best_child(node)
  *         return node             # <<<<<<<<<<<<<<
  * 
- *     @staticmethod
+ *     cdef Node expand(self, Node node):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_node));
   __pyx_r = __pyx_v_node;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":183
+  /* "multimcts/mcts.pyx":200
  *             return best
  * 
- *     def select(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node select(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":197
+/* "multimcts/mcts.pyx":212
+ *         return node
  * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node expand(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_6expand[] = "Step 2: Expansion\n        Add a new child to this node.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_7expand = {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand};
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_7expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("expand (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,0};
-    PyObject* values[1] = {0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expand") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expand", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 197, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6expand(__pyx_v_node);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_expand(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   PyObject *__pyx_v_move = NULL;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
+  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  int __pyx_t_11;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
+  __Pyx_TraceCall("expand", __pyx_f[0], 212, 0, __PYX_ERR(0, 212, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":201
+  /* "multimcts/mcts.pyx":216
  *         Add a new child to this node.
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
+ *         move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
+ *         if len(node.remaining_moves) == 0:
+ *             node.is_fully_expanded = True
  */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "multimcts/mcts.pyx":202
- *         """
- *         try:
- *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")
- */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 202, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_v_move = __pyx_t_5;
-      __pyx_t_5 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Pop(__pyx_v_node->remaining_moves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_move = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":201
- *         Add a new child to this node.
+  /* "multimcts/mcts.pyx":217
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
+ *             node.is_fully_expanded = True
+ * 
  */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_1 = __pyx_v_node->remaining_moves;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 217, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = ((__pyx_t_2 == 0) != 0);
+  if (__pyx_t_3) {
 
-    /* "multimcts/mcts.pyx":203
- *         try:
- *             move = node.remaining_moves.pop()
- *         except IndexError:             # <<<<<<<<<<<<<<
- *             raise IndexError("Tried to expand a node with no remaining moves.")
+    /* "multimcts/mcts.pyx":218
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:
+ *             node.is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)
  */
-    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
-    if (__pyx_t_6) {
-      __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 203, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GOTREF(__pyx_t_7);
+    __pyx_v_node->is_fully_expanded = 1;
 
-      /* "multimcts/mcts.pyx":204
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
- * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 204, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 204, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "multimcts/mcts.pyx":201
- *         Add a new child to this node.
+    /* "multimcts/mcts.pyx":217
  *         """
- *         try:             # <<<<<<<<<<<<<<
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
+ *         move = node.remaining_moves.pop()
+ *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
+ *             node.is_fully_expanded = True
+ * 
+ */
   }
 
-  /* "multimcts/mcts.pyx":206
- *             raise IndexError("Tried to expand a node with no remaining moves.")
+  /* "multimcts/mcts.pyx":220
+ *             node.is_fully_expanded = True
  * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)             # <<<<<<<<<<<<<<
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)             # <<<<<<<<<<<<<<
  *         node.children.append(child)
  * 
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node->state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_5, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_move);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_move);
+  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_state, __pyx_t_4) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_parent, ((PyObject *)__pyx_v_node)) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_parent, ((PyObject *)__pyx_v_node)) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_move, __pyx_v_move) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_child = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":207
+  /* "multimcts/mcts.pyx":221
  * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
+ *         cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)
  *         node.children.append(child)             # <<<<<<<<<<<<<<
  * 
- *         if len(node.remaining_moves) == 0:
- */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_Append(__pyx_t_4, ((PyObject *)__pyx_v_child)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "multimcts/mcts.pyx":209
- *         node.children.append(child)
- * 
- *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node._is_fully_expanded = True
- * 
- */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 209, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_11 = ((__pyx_t_10 == 0) != 0);
-  if (__pyx_t_11) {
-
-    /* "multimcts/mcts.pyx":210
- * 
- *         if len(node.remaining_moves) == 0:
- *             node._is_fully_expanded = True             # <<<<<<<<<<<<<<
- * 
  *         return child
  */
-    __pyx_v_node->_is_fully_expanded = 1;
+  __pyx_t_7 = __Pyx_PyObject_Append(__pyx_v_node->children, ((PyObject *)__pyx_v_child)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 221, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":209
+  /* "multimcts/mcts.pyx":223
  *         node.children.append(child)
  * 
- *         if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
- *             node._is_fully_expanded = True
- * 
- */
-  }
-
-  /* "multimcts/mcts.pyx":212
- *             node._is_fully_expanded = True
- * 
  *         return child             # <<<<<<<<<<<<<<
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_child));
   __pyx_r = __pyx_v_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":197
+  /* "multimcts/mcts.pyx":212
+ *         return node
  * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
+ *     cdef Node expand(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":214
+/* "multimcts/mcts.pyx":225
  *         return child
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_8simulate[] = "Step 3: Simulation (aka playout/rollout)\n        Play out a game, from the given node to termination, and return the final reward.\n        A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.\n\n        Args:\n            node (Node): The node from which to begin the simulation.\n            heuristic (callable): A function that takes a state and returns a move.\n        ";
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_9simulate(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  PyObject *__pyx_v_heuristic = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("simulate (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_heuristic,0};
-    PyObject* values[2] = {0,0};
-    values[1] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (kw_args == 1) {
-        const Py_ssize_t index = 1;
-        PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
-        if (value) { values[index] = value; kw_args--; }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_heuristic = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 214, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 214, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_heuristic);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_heuristic) {
+static std::map<std::string,double>  __pyx_f_9multimcts_4mcts_4MCTS_simulate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args) {
+  PyObject *__pyx_v_heuristic = ((PyObject *)Py_None);
   PyObject *__pyx_v_state = NULL;
   PyObject *__pyx_v_terminal_team = NULL;
   PyObject *__pyx_v_move = NULL;
   PyObject *__pyx_v_reward = NULL;
-  PyObject *__pyx_r = NULL;
+  std::map<std::string,double>  __pyx_v_crewards;
+  PyObject *__pyx_v_team = NULL;
+  std::map<std::string,double>  __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
+  std::map<std::string,double>  __pyx_t_8;
+  Py_ssize_t __pyx_t_9;
+  PyObject *(*__pyx_t_10)(PyObject *);
+  double __pyx_t_11;
+  std::string __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
+  __Pyx_TraceCall("simulate", __pyx_f[0], 225, 0, __PYX_ERR(0, 225, __pyx_L1_error));
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_heuristic = __pyx_optional_args->heuristic;
+    }
+  }
 
-  /* "multimcts/mcts.pyx":223
+  /* "multimcts/mcts.pyx":233
  *             heuristic (callable): A function that takes a state and returns a move.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
- *         if node._is_terminal:
+ *         terminal_team = None
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_1 = __pyx_v_node->state;
+  __Pyx_INCREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":225
+  /* "multimcts/mcts.pyx":235
  *         state = node.state
  * 
- *         if node._is_terminal:             # <<<<<<<<<<<<<<
- *             terminal_team = node.parent.state.get_current_team()
+ *         terminal_team = None             # <<<<<<<<<<<<<<
+ *         if node.is_terminal:
+ *             terminal_team = node.parent.team
+ */
+  __Pyx_INCREF(Py_None);
+  __pyx_v_terminal_team = Py_None;
+
+  /* "multimcts/mcts.pyx":236
+ * 
+ *         terminal_team = None
+ *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *             terminal_team = node.parent.team
  *         else:
  */
-  __pyx_t_2 = (__pyx_v_node->_is_terminal != 0);
+  __pyx_t_2 = (__pyx_v_node->is_terminal != 0);
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":226
- * 
- *         if node._is_terminal:
- *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":237
+ *         terminal_team = None
+ *         if node.is_terminal:
+ *             terminal_team = node.parent.team             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-      }
-    }
-    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_terminal_team = __pyx_t_1;
+    __pyx_t_1 = __pyx_v_node->parent->team;
+    __Pyx_INCREF(__pyx_t_1);
+    __Pyx_DECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":225
- *         state = node.state
+    /* "multimcts/mcts.pyx":236
  * 
- *         if node._is_terminal:             # <<<<<<<<<<<<<<
- *             terminal_team = node.parent.state.get_current_team()
+ *         terminal_team = None
+ *         if node.is_terminal:             # <<<<<<<<<<<<<<
+ *             terminal_team = node.parent.team
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":228
- *             terminal_team = node.parent.state.get_current_team()
+  /* "multimcts/mcts.pyx":239
+ *             terminal_team = node.parent.team
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":229
+      /* "multimcts/mcts.pyx":240
  *         else:
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 if heuristic is not None:
  *                     move = heuristic(state)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
+      __Pyx_DECREF_SET(__pyx_v_terminal_team, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":230
+      /* "multimcts/mcts.pyx":241
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
       __pyx_t_5 = (__pyx_v_heuristic != Py_None);
       __pyx_t_2 = (__pyx_t_5 != 0);
       if (__pyx_t_2) {
 
-        /* "multimcts/mcts.pyx":231
+        /* "multimcts/mcts.pyx":242
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:
  *                     move = heuristic(state)             # <<<<<<<<<<<<<<
  *                 else:
  *                     move = choice(state.get_legal_moves())
  */
         __Pyx_INCREF(__pyx_v_heuristic);
@@ -5221,55 +5144,55 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_state);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "multimcts/mcts.pyx":230
+        /* "multimcts/mcts.pyx":241
  *             while not state.is_terminal():
  *                 terminal_team = state.get_current_team()
  *                 if heuristic is not None:             # <<<<<<<<<<<<<<
  *                     move = heuristic(state)
  *                 else:
  */
         goto __pyx_L6;
       }
 
-      /* "multimcts/mcts.pyx":233
+      /* "multimcts/mcts.pyx":244
  *                     move = heuristic(state)
  *                 else:
  *                     move = choice(state.get_legal_moves())             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
       /*else*/ {
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_6, function);
           }
         }
         __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5277,910 +5200,597 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
         __pyx_t_1 = 0;
       }
       __pyx_L6:;
 
-      /* "multimcts/mcts.pyx":234
+      /* "multimcts/mcts.pyx":245
  *                 else:
  *                     move = choice(state.get_legal_moves())
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":236
+  /* "multimcts/mcts.pyx":247
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":237
+  /* "multimcts/mcts.pyx":248
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":238
+    /* "multimcts/mcts.pyx":249
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
- *         return reward
+ *         cdef map[string,double] crewards = map[string,double]()
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 238, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":237
+    /* "multimcts/mcts.pyx":248
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":240
+  /* "multimcts/mcts.pyx":251
  *             reward = {terminal_team: reward}
  * 
- *         return reward             # <<<<<<<<<<<<<<
+ *         cdef map[string,double] crewards = map[string,double]()             # <<<<<<<<<<<<<<
+ *         for team in reward:
+ *             if reward[team] == 0:
+ */
+  try {
+    __pyx_t_8 = std::map<std::string,double> ();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 251, __pyx_L1_error)
+  }
+  __pyx_v_crewards = __pyx_t_8;
+
+  /* "multimcts/mcts.pyx":252
  * 
- *     @staticmethod
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:             # <<<<<<<<<<<<<<
+ *             if reward[team] == 0:
+ *                 continue
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_reward);
-  __pyx_r = __pyx_v_reward;
+  if (likely(PyList_CheckExact(__pyx_v_reward)) || PyTuple_CheckExact(__pyx_v_reward)) {
+    __pyx_t_1 = __pyx_v_reward; __Pyx_INCREF(__pyx_t_1); __pyx_t_9 = 0;
+    __pyx_t_10 = NULL;
+  } else {
+    __pyx_t_9 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 252, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_10)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      } else {
+        if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 252, __pyx_L1_error)
+        #else
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 252, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        #endif
+      }
+    } else {
+      __pyx_t_3 = __pyx_t_10(__pyx_t_1);
+      if (unlikely(!__pyx_t_3)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 252, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_3);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_team, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "multimcts/mcts.pyx":253
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:
+ *             if reward[team] == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])
+ */
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_reward, __pyx_v_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_3, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (__pyx_t_5) {
+
+      /* "multimcts/mcts.pyx":254
+ *         for team in reward:
+ *             if reward[team] == 0:
+ *                 continue             # <<<<<<<<<<<<<<
+ *             crewards[str(team).encode()] = float(reward[team])
+ * 
+ */
+      goto __pyx_L8_continue;
+
+      /* "multimcts/mcts.pyx":253
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:
+ *             if reward[team] == 0:             # <<<<<<<<<<<<<<
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])
+ */
+    }
+
+    /* "multimcts/mcts.pyx":255
+ *             if reward[team] == 0:
+ *                 continue
+ *             crewards[str(team).encode()] = float(reward[team])             # <<<<<<<<<<<<<<
+ * 
+ *         return crewards
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_reward, __pyx_v_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_11 = __Pyx_PyObject_AsDouble(__pyx_t_4); if (unlikely(__pyx_t_11 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_team); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_4), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    (__pyx_v_crewards[__pyx_t_12]) = __pyx_t_11;
+
+    /* "multimcts/mcts.pyx":252
+ * 
+ *         cdef map[string,double] crewards = map[string,double]()
+ *         for team in reward:             # <<<<<<<<<<<<<<
+ *             if reward[team] == 0:
+ *                 continue
+ */
+    __pyx_L8_continue:;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "multimcts/mcts.pyx":257
+ *             crewards[str(team).encode()] = float(reward[team])
+ * 
+ *         return crewards             # <<<<<<<<<<<<<<
+ * 
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):
+ */
+  __pyx_r = __pyx_v_crewards;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":214
+  /* "multimcts/mcts.pyx":225
  *         return child
  * 
- *     def simulate(self, node:Node, *, heuristic=None) -> Rewards:             # <<<<<<<<<<<<<<
+ *     cdef map[string,double] simulate(self, Node node, heuristic=None):             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout/rollout)
  *         Play out a game, from the given node to termination, and return the final reward.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_WriteUnraisable("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v_terminal_team);
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
-  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_XDECREF(__pyx_v_team);
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":243
+/* "multimcts/mcts.pyx":259
+ *         return crewards
  * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate[] = "Step 4: Backpropagation\n        Update all ancestors with the reward from this terminal node.\n        ";
-static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate = {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate};
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  PyObject *__pyx_v_reward = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("backpropagate (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_reward,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 243, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 243, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_reward = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 243, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 243, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_v_node, __pyx_v_reward);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, PyObject *__pyx_v_reward) {
-  double __pyx_v_val;
-  std::string __pyx_v_ckey;
-  std::map<std::string,float>  __pyx_v_creward;
-  PyObject *__pyx_v_key = NULL;
-  std::pair<std::string,float>  __pyx_v_item;
+static PyObject *__pyx_f_9multimcts_4mcts_4MCTS_backpropagate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, std::map<std::string,double>  __pyx_v_crewards) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  std::map<std::string,float>  __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
-  double __pyx_t_9;
-  int __pyx_t_10;
-  std::string __pyx_t_11;
-  int __pyx_t_12;
-  std::map<std::string,float> ::iterator __pyx_t_13;
-  std::pair<std::string,float>  __pyx_t_14;
+  int __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
+  __Pyx_TraceCall("backpropagate", __pyx_f[0], 259, 0, __PYX_ERR(0, 259, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":249
- *         cdef double val
- *         cdef string ckey
- *         cdef map[string,float] creward = map[string,float]()             # <<<<<<<<<<<<<<
- *         for key,val in reward.items():
- *             if val == 0:
- */
-  try {
-    __pyx_t_1 = std::map<std::string,float> ();
-  } catch(...) {
-    __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 249, __pyx_L1_error)
-  }
-  __pyx_v_creward = __pyx_t_1;
-
-  /* "multimcts/mcts.pyx":250
- *         cdef string ckey
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():             # <<<<<<<<<<<<<<
- *             if val == 0:
- *                 continue
- */
-  __pyx_t_3 = 0;
-  if (unlikely(__pyx_v_reward == Py_None)) {
-    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 250, __pyx_L1_error)
-  }
-  __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_reward, 0, __pyx_n_s_items, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_2);
-  __pyx_t_2 = __pyx_t_6;
-  __pyx_t_6 = 0;
-  while (1) {
-    __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
-    if (unlikely(__pyx_t_8 == 0)) break;
-    if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 250, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_v_val = __pyx_t_9;
-
-    /* "multimcts/mcts.pyx":251
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():
- *             if val == 0:             # <<<<<<<<<<<<<<
- *                 continue
- *             ckey = str(key).encode()
- */
-    __pyx_t_10 = ((__pyx_v_val == 0.0) != 0);
-    if (__pyx_t_10) {
-
-      /* "multimcts/mcts.pyx":252
- *         for key,val in reward.items():
- *             if val == 0:
- *                 continue             # <<<<<<<<<<<<<<
- *             ckey = str(key).encode()
- *             creward[ckey] = val
- */
-      goto __pyx_L3_continue;
-
-      /* "multimcts/mcts.pyx":251
- *         cdef map[string,float] creward = map[string,float]()
- *         for key,val in reward.items():
- *             if val == 0:             # <<<<<<<<<<<<<<
- *                 continue
- *             ckey = str(key).encode()
- */
-    }
-
-    /* "multimcts/mcts.pyx":253
- *             if val == 0:
- *                 continue
- *             ckey = str(key).encode()             # <<<<<<<<<<<<<<
- *             creward[ckey] = val
- * 
- */
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_key); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_7), NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_11 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_v_ckey = __pyx_t_11;
-
-    /* "multimcts/mcts.pyx":254
- *                 continue
- *             ckey = str(key).encode()
- *             creward[ckey] = val             # <<<<<<<<<<<<<<
- * 
- *         cdef pair[string,float] item
- */
-    (__pyx_v_creward[__pyx_v_ckey]) = __pyx_v_val;
-    __pyx_L3_continue:;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "multimcts/mcts.pyx":257
- * 
- *         cdef pair[string,float] item
+  /* "multimcts/mcts.pyx":263
+ *         Update all ancestors with the reward from this terminal node.
+ *         """
  *         while node is not None:             # <<<<<<<<<<<<<<
- *             for item in creward:
- *                 ckey = item.first
- */
-  while (1) {
-    __pyx_t_10 = (((PyObject *)__pyx_v_node) != Py_None);
-    __pyx_t_12 = (__pyx_t_10 != 0);
-    if (!__pyx_t_12) break;
-
-    /* "multimcts/mcts.pyx":258
- *         cdef pair[string,float] item
- *         while node is not None:
- *             for item in creward:             # <<<<<<<<<<<<<<
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- */
-    __pyx_t_13 = __pyx_v_creward.begin();
-    for (;;) {
-      if (!(__pyx_t_13 != __pyx_v_creward.end())) break;
-      __pyx_t_14 = *__pyx_t_13;
-      ++__pyx_t_13;
-      __pyx_v_item = __pyx_t_14;
-
-      /* "multimcts/mcts.pyx":259
- *         while node is not None:
- *             for item in creward:
- *                 ckey = item.first             # <<<<<<<<<<<<<<
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0
- */
-      __pyx_t_11 = __pyx_v_item.first;
-      __pyx_v_ckey = __pyx_t_11;
-
-      /* "multimcts/mcts.pyx":260
- *             for item in creward:
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- */
-      __pyx_t_12 = ((__pyx_v_node->_total_reward.count(__pyx_v_ckey) == 0) != 0);
-      if (__pyx_t_12) {
-
-        /* "multimcts/mcts.pyx":261
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0             # <<<<<<<<<<<<<<
- *                 node._total_reward[ckey] += item.second
- *             node.visit()
- */
-        (__pyx_v_node->_total_reward[__pyx_v_ckey]) = 0.0;
-
-        /* "multimcts/mcts.pyx":260
- *             for item in creward:
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:             # <<<<<<<<<<<<<<
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- */
-      }
-
-      /* "multimcts/mcts.pyx":262
- *                 if node._total_reward.count(ckey) == 0:
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second             # <<<<<<<<<<<<<<
- *             node.visit()
+ *             node.apply_rewards(crewards)
  *             node = node.parent
  */
-      __pyx_t_11 = __pyx_v_ckey;
-      (__pyx_v_node->_total_reward[__pyx_t_11]) = ((__pyx_v_node->_total_reward[__pyx_t_11]) + __pyx_v_item.second);
+  while (1) {
+    __pyx_t_1 = (((PyObject *)__pyx_v_node) != Py_None);
+    __pyx_t_2 = (__pyx_t_1 != 0);
+    if (!__pyx_t_2) break;
 
-      /* "multimcts/mcts.pyx":258
- *         cdef pair[string,float] item
+    /* "multimcts/mcts.pyx":264
+ *         """
  *         while node is not None:
- *             for item in creward:             # <<<<<<<<<<<<<<
- *                 ckey = item.first
- *                 if node._total_reward.count(ckey) == 0:
- */
-    }
-
-    /* "multimcts/mcts.pyx":263
- *                     node._total_reward[ckey] = 0
- *                 node._total_reward[ckey] += item.second
- *             node.visit()             # <<<<<<<<<<<<<<
+ *             node.apply_rewards(crewards)             # <<<<<<<<<<<<<<
  *             node = node.parent
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_visit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 263, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = ((struct __pyx_vtabstruct_9multimcts_4mcts_Node *)__pyx_v_node->__pyx_vtab)->apply_rewards(__pyx_v_node, __pyx_v_crewards); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":264
- *                 node._total_reward[ckey] += item.second
- *             node.visit()
+    /* "multimcts/mcts.pyx":265
+ *         while node is not None:
+ *             node.apply_rewards(crewards)
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
- *     @cython.cdivision(True)
+ *     cdef Node get_best_child(self, Node node):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_parent); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2));
-    __pyx_t_2 = 0;
+    __pyx_t_3 = ((PyObject *)__pyx_v_node->parent);
+    __Pyx_INCREF(__pyx_t_3);
+    __Pyx_DECREF_SET(__pyx_v_node, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_3));
+    __pyx_t_3 = 0;
   }
 
-  /* "multimcts/mcts.pyx":243
+  /* "multimcts/mcts.pyx":259
+ *         return crewards
  * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
+ *     cdef backpropagate(self, Node node, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":269
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
+/* "multimcts/mcts.pyx":267
+ *             node = node.parent
+ * 
+ *     cdef Node get_best_child(self, Node node):             # <<<<<<<<<<<<<<
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  */
 
-/* Python wrapper */
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child[] = "Find the child with the highest Upper Confidence Bound (UCB) score.\n        ucb = (x / n) + C * sqrt(ln(N) / n)\n        x=reward for this node\n        n=number of simulations for this node\n        N=number of simulations for parent node\n        C=exploration bias\n        ";
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = 0;
-  double __pyx_v_exploration_bias;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_best_child (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node,&__pyx_n_s_exploration_bias,0};
-    PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exploration_bias)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 269, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 269, __pyx_L3_error)
-      }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-    }
-    __pyx_v_node = ((struct __pyx_obj_9multimcts_4mcts_Node *)values[0]);
-    __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 269, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node), __pyx_ptype_9multimcts_4mcts_Node, 1, "node", 0))) __PYX_ERR(0, 269, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), __pyx_v_node, __pyx_v_exploration_bias);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, double __pyx_v_exploration_bias) {
-  int __pyx_v_visits;
-  double __pyx_v_reward;
+static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_get_best_child(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
+  double __pyx_v_parent_sqrtlog_visits;
+  double __pyx_v_best_score;
   double __pyx_v_ucb;
-  double __pyx_v_C;
-  double __pyx_v_ln_parent_visits;
-  std::string __pyx_v_cur_team;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best_child = 0;
-  std::pair<std::string,float>  __pyx_v_item;
-  double __pyx_v_best_score;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
-  std::string __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  int __pyx_t_7;
-  int __pyx_t_8;
-  std::map<std::string,float> ::iterator __pyx_t_9;
-  std::map<std::string,float>  *__pyx_t_10;
-  std::pair<std::string,float>  __pyx_t_11;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  PyObject *(*__pyx_t_4)(PyObject *);
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
+  __Pyx_TraceCall("get_best_child", __pyx_f[0], 267, 0, __PYX_ERR(0, 267, __pyx_L1_error));
 
-  /* "multimcts/mcts.pyx":280
- *         cdef int visits
- *         cdef double reward, ucb
- *         cdef double C = exploration_bias             # <<<<<<<<<<<<<<
- *         cdef double ln_parent_visits = node.log_visits
- * 
- */
-  __pyx_v_C = __pyx_v_exploration_bias;
-
-  /* "multimcts/mcts.pyx":281
- *         cdef double reward, ucb
- *         cdef double C = exploration_bias
- *         cdef double ln_parent_visits = node.log_visits             # <<<<<<<<<<<<<<
- * 
- *         cdef string cur_team = node._team
- */
-  __pyx_t_1 = __pyx_v_node->log_visits;
-  __pyx_v_ln_parent_visits = __pyx_t_1;
-
-  /* "multimcts/mcts.pyx":283
- *         cdef double ln_parent_visits = node.log_visits
- * 
- *         cdef string cur_team = node._team             # <<<<<<<<<<<<<<
- * 
- *         cdef Node child, best_child
+  /* "multimcts/mcts.pyx":269
+ *     cdef Node get_best_child(self, Node node):
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits             # <<<<<<<<<<<<<<
+ *         cdef double best_score = -INFINITY
+ *         cdef double ucb
  */
-  __pyx_t_2 = __pyx_v_node->_team;
-  __pyx_v_cur_team = __pyx_t_2;
+  __pyx_t_1 = __pyx_v_node->sqrtlog_visits;
+  __pyx_v_parent_sqrtlog_visits = __pyx_t_1;
 
-  /* "multimcts/mcts.pyx":288
- *         cdef pair[string,float] item
- * 
+  /* "multimcts/mcts.pyx":270
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  *         cdef double best_score = -INFINITY             # <<<<<<<<<<<<<<
- * 
- *         for child in node.children:
+ *         cdef double ucb
+ *         cdef Node child, best_child = node.children[0]
  */
   __pyx_v_best_score = (-INFINITY);
 
-  /* "multimcts/mcts.pyx":290
+  /* "multimcts/mcts.pyx":272
  *         cdef double best_score = -INFINITY
+ *         cdef double ucb
+ *         cdef Node child, best_child = node.children[0]             # <<<<<<<<<<<<<<
+ *         cdef pair[string,double] item
+ * 
+ */
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_node->children, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_v_best_child = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "multimcts/mcts.pyx":275
+ *         cdef pair[string,double] item
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
+ *             if ucb > best_score:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_node), __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-    __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
+  if (likely(PyList_CheckExact(__pyx_v_node->children)) || PyTuple_CheckExact(__pyx_v_node->children)) {
+    __pyx_t_2 = __pyx_v_node->children; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_4 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_node->children); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
-    if (likely(!__pyx_t_6)) {
-      if (likely(PyList_CheckExact(__pyx_t_4))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
+    if (likely(!__pyx_t_4)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
-      __pyx_t_3 = __pyx_t_6(__pyx_t_4);
-      if (unlikely(!__pyx_t_3)) {
+      __pyx_t_5 = __pyx_t_4(__pyx_t_2);
+      if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 290, __pyx_L1_error)
+          else __PYX_ERR(0, 275, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_GOTREF(__pyx_t_5);
     }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 290, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    /* "multimcts/mcts.pyx":291
- * 
- *         for child in node.children:
- *             visits = child._num_visits             # <<<<<<<<<<<<<<
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
- *                 continue
- */
-    __pyx_t_7 = __pyx_v_child->_num_visits;
-    __pyx_v_visits = __pyx_t_7;
-
-    /* "multimcts/mcts.pyx":292
- *         for child in node.children:
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
- *                 continue
- * 
- */
-    __pyx_t_8 = ((__pyx_v_visits == 0) != 0);
-    if (__pyx_t_8) {
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_child, ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_5));
+    __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":293
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
- *                 continue             # <<<<<<<<<<<<<<
+    /* "multimcts/mcts.pyx":276
  * 
- *             # Relative reward is this child's reward minus its siblings' rewards.
- */
-      goto __pyx_L3_continue;
-
-      /* "multimcts/mcts.pyx":292
  *         for child in node.children:
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...             # <<<<<<<<<<<<<<
- *                 continue
- * 
- */
-    }
-
-    /* "multimcts/mcts.pyx":296
- * 
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]             # <<<<<<<<<<<<<<
- *             for item in child._total_reward:
- *                 reward -= item.second
- */
-    __pyx_v_reward = (2.0 * (__pyx_v_child->_total_reward[__pyx_v_cur_team]));
-
-    /* "multimcts/mcts.pyx":297
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:             # <<<<<<<<<<<<<<
- *                 reward -= item.second
- * 
- */
-    __pyx_t_10 = &__pyx_v_child->_total_reward;
-    __pyx_t_9 = __pyx_t_10->begin();
-    for (;;) {
-      if (!(__pyx_t_9 != __pyx_t_10->end())) break;
-      __pyx_t_11 = *__pyx_t_9;
-      ++__pyx_t_9;
-      __pyx_v_item = __pyx_t_11;
-
-      /* "multimcts/mcts.pyx":298
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:
- *                 reward -= item.second             # <<<<<<<<<<<<<<
- * 
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- */
-      __pyx_v_reward = (__pyx_v_reward - __pyx_v_item.second);
-
-      /* "multimcts/mcts.pyx":297
- *             # Relative reward is this child's reward minus its siblings' rewards.
- *             reward = 2 * child._total_reward[cur_team]
- *             for item in child._total_reward:             # <<<<<<<<<<<<<<
- *                 reward -= item.second
- * 
- */
-    }
-
-    /* "multimcts/mcts.pyx":300
- *                 reward -= item.second
- * 
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
- * 
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)             # <<<<<<<<<<<<<<
  *             if ucb > best_score:
+ *                 best_score = ucb
  */
-    __pyx_v_ucb = ((__pyx_v_reward / ((double)__pyx_v_visits)) + (__pyx_v_C * sqrt((__pyx_v_ln_parent_visits / ((double)__pyx_v_visits)))));
+    __pyx_v_ucb = ((struct __pyx_vtabstruct_9multimcts_4mcts_Node *)__pyx_v_child->__pyx_vtab)->ucb(__pyx_v_child, __pyx_v_self->exploration_bias, __pyx_v_parent_sqrtlog_visits);
 
-    /* "multimcts/mcts.pyx":302
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- * 
+    /* "multimcts/mcts.pyx":277
+ *         for child in node.children:
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
-    __pyx_t_8 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
-    if (__pyx_t_8) {
+    __pyx_t_6 = ((__pyx_v_ucb > __pyx_v_best_score) != 0);
+    if (__pyx_t_6) {
 
-      /* "multimcts/mcts.pyx":303
- * 
+      /* "multimcts/mcts.pyx":278
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:
  *                 best_score = ucb             # <<<<<<<<<<<<<<
  *                 best_child = child
  * 
  */
       __pyx_v_best_score = __pyx_v_ucb;
 
-      /* "multimcts/mcts.pyx":304
+      /* "multimcts/mcts.pyx":279
  *             if ucb > best_score:
  *                 best_score = ucb
  *                 best_child = child             # <<<<<<<<<<<<<<
  * 
  *         return best_child
  */
       __Pyx_INCREF(((PyObject *)__pyx_v_child));
-      __Pyx_XDECREF_SET(__pyx_v_best_child, __pyx_v_child);
+      __Pyx_DECREF_SET(__pyx_v_best_child, __pyx_v_child);
 
-      /* "multimcts/mcts.pyx":302
- *             ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
- * 
+      /* "multimcts/mcts.pyx":277
+ *         for child in node.children:
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
  *             if ucb > best_score:             # <<<<<<<<<<<<<<
  *                 best_score = ucb
  *                 best_child = child
  */
     }
 
-    /* "multimcts/mcts.pyx":290
- *         cdef double best_score = -INFINITY
+    /* "multimcts/mcts.pyx":275
+ *         cdef pair[string,double] item
  * 
  *         for child in node.children:             # <<<<<<<<<<<<<<
- *             visits = child._num_visits
- *             if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
+ *             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
+ *             if ucb > best_score:
  */
-    __pyx_L3_continue:;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":306
+  /* "multimcts/mcts.pyx":281
  *                 best_child = child
  * 
  *         return best_child             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  if (unlikely(!__pyx_v_best_child)) { __Pyx_RaiseUnboundLocalError("best_child"); __PYX_ERR(0, 306, __pyx_L1_error) }
   __Pyx_INCREF(((PyObject *)__pyx_v_best_child));
   __pyx_r = __pyx_v_best_child;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":269
- *     @cython.boundscheck(False)
- *     @cython.wraparound(False)
- *     def get_best_child(self, node:Node, exploration_bias:float) -> Node:             # <<<<<<<<<<<<<<
- *         """Find the child with the highest Upper Confidence Bound (UCB) score.
- *         ucb = (x / n) + C * sqrt(ln(N) / n)
+  /* "multimcts/mcts.pyx":267
+ *             node = node.parent
+ * 
+ *     cdef Node get_best_child(self, Node node):             # <<<<<<<<<<<<<<
+ *         """Find the child with the highest Upper Confidence Bound (UCB)."""
+ *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XDECREF((PyObject *)__pyx_v_best_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_14__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.exploration_bias,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -6370,46 +5980,49 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(((struct __pyx_obj_9multimcts_4mcts_MCTS *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -6429,14 +6042,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -6519,45 +6133,48 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__12)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node", 0);
+  __Pyx_TraceCall("__pyx_unpickle_Node", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__13, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  */
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
@@ -6568,17 +6185,17 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
@@ -6603,23 +6220,23 @@
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_9multimcts_4mcts_Node), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
@@ -6637,15 +6254,15 @@
   if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
@@ -6660,28 +6277,28 @@
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  *     __pyx_result = Node.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
   /* "(tree fragment)":10
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result             # <<<<<<<<<<<<<<
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v___pyx_result);
   __pyx_r = __pyx_v___pyx_result;
   goto __pyx_L0;
 
   /* "(tree fragment)":1
@@ -6698,202 +6315,234 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
-  std::string __pyx_t_4;
-  std::map<std::string,float>  __pyx_t_5;
-  double __pyx_t_6;
+  double __pyx_t_2;
+  std::string __pyx_t_3;
+  int __pyx_t_4;
+  std::map<std::string,double>  __pyx_t_5;
+  int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node__set_state", 0);
+  __Pyx_TraceCall("__pyx_unpickle_Node__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]             # <<<<<<<<<<<<<<
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_children);
-  __Pyx_DECREF(__pyx_v___pyx_result->_children);
-  __pyx_v___pyx_result->_children = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->avg_reward = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_is_fully_expanded = __pyx_t_2;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->children);
+  __Pyx_DECREF(__pyx_v___pyx_result->children);
+  __pyx_v___pyx_result->children = __pyx_t_1;
+  __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_is_terminal = __pyx_t_2;
+  __pyx_v___pyx_result->cteam = __pyx_t_3;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_move);
-  __Pyx_DECREF(__pyx_v___pyx_result->_move);
-  __pyx_v___pyx_result->_move = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->invsqrt_visits = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_num_visits = __pyx_t_3;
+  __pyx_v___pyx_result->is_fully_expanded = __pyx_t_4;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_parent);
-  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->_parent));
-  __pyx_v___pyx_result->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->is_terminal = __pyx_t_4;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 6, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_remaining_moves);
-  __Pyx_DECREF(__pyx_v___pyx_result->_remaining_moves);
-  __pyx_v___pyx_result->_remaining_moves = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v___pyx_result->move);
+  __Pyx_DECREF(__pyx_v___pyx_result->move);
+  __pyx_v___pyx_result->move = __pyx_t_1;
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 7, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_9multimcts_4mcts_Node))))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
-  __Pyx_GOTREF(__pyx_v___pyx_result->_state);
-  __Pyx_DECREF(__pyx_v___pyx_result->_state);
-  __pyx_v___pyx_result->_state = __pyx_t_1;
+  __Pyx_GOTREF(__pyx_v___pyx_result->parent);
+  __Pyx_DECREF(((PyObject *)__pyx_v___pyx_result->parent));
+  __pyx_v___pyx_result->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 8, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_team = __pyx_t_4;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->remaining_moves);
+  __Pyx_DECREF(__pyx_v___pyx_result->remaining_moves);
+  __pyx_v___pyx_result->remaining_moves = __pyx_t_1;
+  __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 9, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __pyx_convert_map_from_py_std_3a__3a_string__and_float(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_5 = __pyx_convert_map_from_py_std_3a__3a_string__and_double(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->_total_reward = __pyx_t_5;
+  __pyx_v___pyx_result->rewards = __pyx_t_5;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 10, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result->log_visits = __pyx_t_6;
+  __pyx_v___pyx_result->sqrtlog_visits = __pyx_t_2;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 11, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->state);
+  __Pyx_DECREF(__pyx_v___pyx_result->state);
+  __pyx_v___pyx_result->state = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 12, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->team);
+  __Pyx_DECREF(__pyx_v___pyx_result->team);
+  __pyx_v___pyx_result->team = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 13, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result->visits = __pyx_t_6;
 
   /* "(tree fragment)":13
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
   __pyx_t_7 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_8 = ((__pyx_t_7 > 11) != 0);
+  __pyx_t_8 = ((__pyx_t_7 > 14) != 0);
   if (__pyx_t_8) {
   } else {
-    __pyx_t_2 = __pyx_t_8;
+    __pyx_t_4 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_8 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
   __pyx_t_9 = (__pyx_t_8 != 0);
-  __pyx_t_2 = __pyx_t_9;
+  __pyx_t_4 = __pyx_t_9;
   __pyx_L4_bool_binop_done:;
-  if (__pyx_t_2) {
+  if (__pyx_t_4) {
 
     /* "(tree fragment)":14
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[11])             # <<<<<<<<<<<<<<
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[14])             # <<<<<<<<<<<<<<
  */
     __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_update); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
-    __pyx_t_10 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 11, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 14, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_12);
@@ -6907,40 +6556,41 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[11])
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[14])
  */
   }
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_MCTS(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -7023,36 +6673,39 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__14)
   __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS", 0);
+  __Pyx_TraceCall("__pyx_unpickle_MCTS", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__15, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):
@@ -7202,42 +6855,45 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
  *         __pyx_unpickle_MCTS__set_state(<MCTS> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.exploration_bias = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_MCTS__set_state(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   double __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS__set_state", 0);
+  __Pyx_TraceCall("__pyx_unpickle_MCTS__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
  *     __pyx_result.exploration_bias = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -7333,34 +6989,37 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":31
  * 
  * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_f[1], 31, 0, __PYX_ERR(1, 31, __pyx_L1_error));
 
   /* "string.to_py":32
  * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
@@ -7383,34 +7042,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":37
  * 
  * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_f[1], 37, 0, __PYX_ERR(1, 37, __pyx_L1_error));
 
   /* "string.to_py":38
  * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
@@ -7433,34 +7095,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":43
  * 
  * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_f[1], 43, 0, __PYX_ERR(1, 43, __pyx_L1_error));
 
   /* "string.to_py":44
  * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
@@ -7483,34 +7148,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":49
  * 
  * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
  * cdef extern from *:
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_f[1], 49, 0, __PYX_ERR(1, 49, __pyx_L1_error));
 
   /* "string.to_py":50
  * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
@@ -7533,34 +7201,37 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":55
  * 
  * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_f[1], 55, 0, __PYX_ERR(1, 55, __pyx_L1_error));
 
   /* "string.to_py":56
  * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * 
  */
@@ -7582,14 +7253,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
@@ -7598,20 +7270,22 @@
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  */
 
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
   Py_ssize_t __pyx_v_length;
   char const *__pyx_v_data;
   std::string __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   char const *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
+  __Pyx_TraceCall("__pyx_convert_string_from_py_std__in_string", __pyx_f[1], 13, 0, __PYX_ERR(1, 13, __pyx_L1_error));
 
   /* "string.from_py":14
  * @cname("__pyx_convert_string_from_py_std__in_string")
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
  *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  *     return string(data, length)
@@ -7647,43 +7321,46 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.to_py":201
  * 
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):             # <<<<<<<<<<<<<<
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
  */
 
-static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____float(std::map<std::string,float>  const &__pyx_v_s) {
+static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____double(std::map<std::string,double>  const &__pyx_v_s) {
   PyObject *__pyx_v_o = NULL;
-  std::map<std::string,float> ::value_type const *__pyx_v_key_value;
-  std::map<std::string,float> ::const_iterator __pyx_v_iter;
+  std::map<std::string,double> ::value_type const *__pyx_v_key_value;
+  std::map<std::string,double> ::const_iterator __pyx_v_iter;
   PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____float", 0);
+  __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____double", 0);
+  __Pyx_TraceCall("__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_f[1], 201, 0, __PYX_ERR(1, 201, __pyx_L1_error));
 
   /* "map.to_py":202
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_o = ((PyObject*)__pyx_t_1);
@@ -7753,65 +7430,68 @@
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_o);
   __pyx_r = __pyx_v_o;
   goto __pyx_L0;
 
   /* "map.to_py":201
  * 
- * @cname("__pyx_convert_map_to_py_std_3a__3a_string____float")
- * cdef object __pyx_convert_map_to_py_std_3a__3a_string____float(const map[X,Y]& s):             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
+ * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):             # <<<<<<<<<<<<<<
  *     o = {}
  *     cdef const map[X,Y].value_type *key_value
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_o);
   __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
 
-static std::map<std::string,float>  __pyx_convert_map_from_py_std_3a__3a_string__and_float(PyObject *__pyx_v_o) {
+static std::map<std::string,double>  __pyx_convert_map_from_py_std_3a__3a_string__and_double(PyObject *__pyx_v_o) {
   PyObject *__pyx_v_d = 0;
-  std::map<std::string,float>  __pyx_v_m;
+  std::map<std::string,double>  __pyx_v_m;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_value = NULL;
-  std::map<std::string,float>  __pyx_r;
+  std::map<std::string,double>  __pyx_r;
+  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   std::string __pyx_t_8;
-  float __pyx_t_9;
+  double __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_float", 0);
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_double", 0);
+  __Pyx_TraceCall("__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_f[1], 174, 0, __PYX_ERR(1, 174, __pyx_L1_error));
 
   /* "map.from_py":175
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:
  *     cdef dict d = o             # <<<<<<<<<<<<<<
  *     cdef map[X,Y] m
  *     for key, value in d.iteritems():
  */
   if (!(likely(PyDict_CheckExact(__pyx_v_o))||((__pyx_v_o) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_o)->tp_name), 0))) __PYX_ERR(1, 175, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_o;
   __Pyx_INCREF(__pyx_t_1);
@@ -7850,16 +7530,16 @@
  *     cdef map[X,Y] m
  *     for key, value in d.iteritems():
  *         m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
  *     return m
  * 
  */
     __pyx_t_8 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
-    __pyx_t_9 = __pyx_PyFloat_AsFloat(__pyx_v_value); if (unlikely((__pyx_t_9 == (float)-1) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
-    __pyx_v_m.insert(std::pair<std::string,float> (((std::string)__pyx_t_8), ((float)__pyx_t_9)));
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_9 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
+    __pyx_v_m.insert(std::pair<std::string,double> (((std::string)__pyx_t_8), ((double)__pyx_t_9)));
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "map.from_py":179
  *     for key, value in d.iteritems():
  *         m.insert(pair[X,Y](<X>key, <Y>value))
  *     return m             # <<<<<<<<<<<<<<
@@ -7867,148 +7547,143 @@
  * 
  */
   __pyx_r = __pyx_v_m;
   goto __pyx_L0;
 
   /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_d);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static struct __pyx_vtabstruct_9multimcts_4mcts_Node __pyx_vtable_9multimcts_4mcts_Node;
 
 static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9multimcts_4mcts_Node *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_9multimcts_4mcts_Node *)o);
-  new((void*)&(p->_team)) std::string();
-  new((void*)&(p->_total_reward)) std::map<std::string,float> ();
-  p->_state = Py_None; Py_INCREF(Py_None);
-  p->_move = Py_None; Py_INCREF(Py_None);
-  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
-  p->_children = Py_None; Py_INCREF(Py_None);
-  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  p->__pyx_vtab = __pyx_vtabptr_9multimcts_4mcts_Node;
+  new((void*)&(p->cteam)) std::string();
+  new((void*)&(p->rewards)) std::map<std::string,double> ();
+  p->state = Py_None; Py_INCREF(Py_None);
+  p->move = Py_None; Py_INCREF(Py_None);
+  p->team = Py_None; Py_INCREF(Py_None);
+  p->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  p->children = Py_None; Py_INCREF(Py_None);
+  p->remaining_moves = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_9multimcts_4mcts_Node(PyObject *o) {
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
-  __Pyx_call_destructor(p->_team);
-  __Pyx_call_destructor(p->_total_reward);
-  Py_CLEAR(p->_state);
-  Py_CLEAR(p->_move);
-  Py_CLEAR(p->_parent);
-  Py_CLEAR(p->_children);
-  Py_CLEAR(p->_remaining_moves);
+  __Pyx_call_destructor(p->cteam);
+  __Pyx_call_destructor(p->rewards);
+  Py_CLEAR(p->state);
+  Py_CLEAR(p->move);
+  Py_CLEAR(p->team);
+  Py_CLEAR(p->parent);
+  Py_CLEAR(p->children);
+  Py_CLEAR(p->remaining_moves);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_9multimcts_4mcts_Node(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
-  if (p->_state) {
-    e = (*v)(p->_state, a); if (e) return e;
+  if (p->state) {
+    e = (*v)(p->state, a); if (e) return e;
+  }
+  if (p->move) {
+    e = (*v)(p->move, a); if (e) return e;
   }
-  if (p->_move) {
-    e = (*v)(p->_move, a); if (e) return e;
+  if (p->team) {
+    e = (*v)(p->team, a); if (e) return e;
   }
-  if (p->_parent) {
-    e = (*v)(((PyObject *)p->_parent), a); if (e) return e;
+  if (p->parent) {
+    e = (*v)(((PyObject *)p->parent), a); if (e) return e;
   }
-  if (p->_children) {
-    e = (*v)(p->_children, a); if (e) return e;
+  if (p->children) {
+    e = (*v)(p->children, a); if (e) return e;
   }
-  if (p->_remaining_moves) {
-    e = (*v)(p->_remaining_moves, a); if (e) return e;
+  if (p->remaining_moves) {
+    e = (*v)(p->remaining_moves, a); if (e) return e;
   }
   return 0;
 }
 
 static int __pyx_tp_clear_9multimcts_4mcts_Node(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_9multimcts_4mcts_Node *p = (struct __pyx_obj_9multimcts_4mcts_Node *)o;
-  tmp = ((PyObject*)p->_state);
-  p->_state = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->state);
+  p->state = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_move);
-  p->_move = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->move);
+  p->move = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_parent);
-  p->_parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->team);
+  p->team = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_children);
-  p->_children = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->parent);
+  p->parent = ((struct __pyx_obj_9multimcts_4mcts_Node *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
-  tmp = ((PyObject*)p->_remaining_moves);
-  p->_remaining_moves = Py_None; Py_INCREF(Py_None);
+  tmp = ((PyObject*)p->children);
+  p->children = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->remaining_moves);
+  p->remaining_moves = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_state(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_9multimcts_4mcts_4Node_5state_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_parent(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_6parent_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_move(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_4move_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_children(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_8children_1__get__(o);
-}
-
-static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_remaining_moves(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_9multimcts_4mcts_4Node_15remaining_moves_1__get__(o);
+static PyObject *__pyx_getprop_9multimcts_4mcts_4Node_rewards(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_9multimcts_4mcts_4Node_7rewards_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_9multimcts_4mcts_Node[] = {
-  {"visit", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_3visit, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_5__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_7__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4Node_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_Node[] = {
   {(char *)"state", __pyx_getprop_9multimcts_4mcts_4Node_state, 0, (char *)0, 0},
-  {(char *)"parent", __pyx_getprop_9multimcts_4mcts_4Node_parent, 0, (char *)0, 0},
-  {(char *)"move", __pyx_getprop_9multimcts_4mcts_4Node_move, 0, (char *)0, 0},
-  {(char *)"children", __pyx_getprop_9multimcts_4mcts_4Node_children, 0, (char *)0, 0},
-  {(char *)"remaining_moves", __pyx_getprop_9multimcts_4mcts_4Node_remaining_moves, 0, (char *)0, 0},
+  {(char *)"rewards", __pyx_getprop_9multimcts_4mcts_4Node_rewards, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_9multimcts_4mcts_Node = {
   PyVarObject_HEAD_INIT(0, 0)
   "multimcts.mcts.Node", /*tp_name*/
   sizeof(struct __pyx_obj_9multimcts_4mcts_Node), /*tp_basicsize*/
@@ -8035,15 +7710,15 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n\n    Attributes:\n        children (list): The child nodes of the current node. These represent legal moves that have been visited.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ", /*tp_doc*/
+  "Represents a game state node in the MCTS search tree.\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n        move (Move): The move that was played from the parent node to get to this node.\n    Attributes:\n        children (List[Node]): The child nodes of the current node. These represent legal moves that have been visited.\n        visits (int): The number of times the node has been visited.\n        rewards (dict): All teams' rewards obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ", /*tp_doc*/
   __pyx_tp_traverse_9multimcts_4mcts_Node, /*tp_traverse*/
   __pyx_tp_clear_9multimcts_4mcts_Node, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_9multimcts_4mcts_Node, /*tp_methods*/
@@ -8075,23 +7750,27 @@
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
+static struct __pyx_vtabstruct_9multimcts_4mcts_MCTS __pyx_vtable_9multimcts_4mcts_MCTS;
 
 static PyObject *__pyx_tp_new_9multimcts_4mcts_MCTS(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_9multimcts_4mcts_MCTS *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  p = ((struct __pyx_obj_9multimcts_4mcts_MCTS *)o);
+  p->__pyx_vtab = __pyx_vtabptr_9multimcts_4mcts_MCTS;
   return o;
 }
 
 static void __pyx_tp_dealloc_9multimcts_4mcts_MCTS(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
@@ -8102,21 +7781,16 @@
 
 static PyObject *__pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_9multimcts_4mcts_4MCTS_16exploration_bias_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_9multimcts_4mcts_MCTS[] = {
   {"search", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_3search, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_2search},
-  {"select", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_5select, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_4select},
-  {"expand", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_7expand, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_6expand},
-  {"simulate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_9simulate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_8simulate},
-  {"backpropagate", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_11backpropagate, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_10backpropagate},
-  {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_4MCTS_12get_best_child},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_15__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_17__setstate_cython__, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_5__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_9multimcts_4mcts_4MCTS_7__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_9multimcts_4mcts_MCTS[] = {
   {(char *)"exploration_bias", __pyx_getprop_9multimcts_4mcts_4MCTS_exploration_bias, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -8251,112 +7925,91 @@
   {&__pyx_kp_u_GameState_must_implement_get_cur, __pyx_k_GameState_must_implement_get_cur, sizeof(__pyx_k_GameState_must_implement_get_cur), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_get_leg, __pyx_k_GameState_must_implement_get_leg, sizeof(__pyx_k_GameState_must_implement_get_leg), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_get_rew, __pyx_k_GameState_must_implement_get_rew, sizeof(__pyx_k_GameState_must_implement_get_rew), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_is_term, __pyx_k_GameState_must_implement_is_term, sizeof(__pyx_k_GameState_must_implement_is_term), 0, 1, 0, 0},
   {&__pyx_kp_u_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 1, 0, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
-  {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_u_Invalid_return_type, __pyx_k_Invalid_return_type, sizeof(__pyx_k_Invalid_return_type), 0, 1, 0, 0},
   {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS, __pyx_k_MCTS, sizeof(__pyx_k_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_Move, __pyx_k_Move, sizeof(__pyx_k_Move), 0, 0, 1, 1},
   {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
   {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_kp_u_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 1, 0, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_Rewards, __pyx_k_Rewards, sizeof(__pyx_k_Rewards), 0, 0, 1, 1},
   {&__pyx_n_s_Team, __pyx_k_Team, sizeof(__pyx_k_Team), 0, 0, 1, 1},
-  {&__pyx_kp_u_Tried_to_expand_a_node_with_no_r, __pyx_k_Tried_to_expand_a_node_with_no_r, sizeof(__pyx_k_Tried_to_expand_a_node_with_no_r), 0, 1, 0, 0},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
-  {&__pyx_n_s_backpropagate, __pyx_k_backpropagate, sizeof(__pyx_k_backpropagate), 0, 0, 1, 1},
-  {&__pyx_n_s_child, __pyx_k_child, sizeof(__pyx_k_child), 0, 0, 1, 1},
-  {&__pyx_n_s_children, __pyx_k_children, sizeof(__pyx_k_children), 0, 0, 1, 1},
   {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
-  {&__pyx_n_s_ckey, __pyx_k_ckey, sizeof(__pyx_k_ckey), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_creward, __pyx_k_creward, sizeof(__pyx_k_creward), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_expand, __pyx_k_expand, sizeof(__pyx_k_expand), 0, 0, 1, 1},
   {&__pyx_n_s_exploration_bias, __pyx_k_exploration_bias, sizeof(__pyx_k_exploration_bias), 0, 0, 1, 1},
-  {&__pyx_n_s_get_best_child, __pyx_k_get_best_child, sizeof(__pyx_k_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_get_current_team, __pyx_k_get_current_team, sizeof(__pyx_k_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_get_legal_moves, __pyx_k_get_legal_moves, sizeof(__pyx_k_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_get_reward, __pyx_k_get_reward, sizeof(__pyx_k_get_reward), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_heuristic, __pyx_k_heuristic, sizeof(__pyx_k_heuristic), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_is_terminal, __pyx_k_is_terminal, sizeof(__pyx_k_is_terminal), 0, 0, 1, 1},
-  {&__pyx_n_s_item, __pyx_k_item, sizeof(__pyx_k_item), 0, 0, 1, 1},
-  {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_iteritems, __pyx_k_iteritems, sizeof(__pyx_k_iteritems), 0, 0, 1, 1},
-  {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_lower, __pyx_k_lower, sizeof(__pyx_k_lower), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_make_move, __pyx_k_make_move, sizeof(__pyx_k_make_move), 0, 0, 1, 1},
   {&__pyx_n_s_max_iterations, __pyx_k_max_iterations, sizeof(__pyx_k_max_iterations), 0, 0, 1, 1},
   {&__pyx_n_s_max_time, __pyx_k_max_time, sizeof(__pyx_k_max_time), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 0, 1, 1},
   {&__pyx_n_u_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 1, 0, 1},
   {&__pyx_n_s_multimcts_mcts, __pyx_k_multimcts_mcts, sizeof(__pyx_k_multimcts_mcts), 0, 0, 1, 1},
   {&__pyx_kp_s_multimcts_mcts_pyx, __pyx_k_multimcts_mcts_pyx, sizeof(__pyx_k_multimcts_mcts_pyx), 0, 0, 1, 0},
   {&__pyx_kp_u_must_be_one_of, __pyx_k_must_be_one_of, sizeof(__pyx_k_must_be_one_of), 0, 1, 0, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
-  {&__pyx_n_s_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 0, 1, 1},
   {&__pyx_n_u_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 1, 0, 1},
   {&__pyx_n_s_parent, __pyx_k_parent, sizeof(__pyx_k_parent), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_MCTS, __pyx_k_pyx_unpickle_MCTS, sizeof(__pyx_k_pyx_unpickle_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Node, __pyx_k_pyx_unpickle_Node, sizeof(__pyx_k_pyx_unpickle_Node), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_remaining_moves, __pyx_k_remaining_moves, sizeof(__pyx_k_remaining_moves), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_return_type, __pyx_k_return_type, sizeof(__pyx_k_return_type), 0, 0, 1, 1},
-  {&__pyx_n_s_reward, __pyx_k_reward, sizeof(__pyx_k_reward), 0, 0, 1, 1},
-  {&__pyx_n_s_select, __pyx_k_select, sizeof(__pyx_k_select), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
-  {&__pyx_n_s_simulate, __pyx_k_simulate, sizeof(__pyx_k_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
   {&__pyx_n_u_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 1, 0, 1},
-  {&__pyx_n_s_staticmethod, __pyx_k_staticmethod, sizeof(__pyx_k_staticmethod), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-  {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
-  {&__pyx_n_s_visit, __pyx_k_visit, sizeof(__pyx_k_visit), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 162, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -8365,210 +8018,176 @@
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "multimcts/mcts.pyx":204
- *             move = node.remaining_moves.pop()
- *         except IndexError:
- *             raise IndexError("Tried to expand a node with no remaining moves.")             # <<<<<<<<<<<<<<
- * 
- *         child = Node(state=node.state.make_move(move), parent=node, move=move)
- */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Tried_to_expand_a_node_with_no_r); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x1728f3c, 0x336842e, 0xd9606a6):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1728f3c, 0x336842e, 0xd9606a6) = (_children, _is_fully_expanded, _is_terminal, _move, _num_visits, _parent, _remaining_moves, _state, _team, _total_reward, log_visits))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
-  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_24284988, __pyx_int_53904430, __pyx_int_227935910); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_56097295, __pyx_int_99932858, __pyx_int_59888949); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 22, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 26, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 30, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 36, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 40, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":197
- * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 2: Expansion
- *         Add a new child to this node.
- */
-  __pyx_tuple__20 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 197, __pyx_L1_error)
-
-  /* "multimcts/mcts.pyx":243
- * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
- *         """Step 4: Backpropagation
- *         Update all ancestors with the reward from this terminal node.
- */
-  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_val, __pyx_n_s_ckey, __pyx_n_s_creward, __pyx_n_s_key, __pyx_n_s_item); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 243, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 40, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyList_Type_pop.type = (PyObject*)&PyList_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_24284988 = PyInt_FromLong(24284988L); if (unlikely(!__pyx_int_24284988)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_53904430 = PyInt_FromLong(53904430L); if (unlikely(!__pyx_int_53904430)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_56097295 = PyInt_FromLong(56097295L); if (unlikely(!__pyx_int_56097295)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_59888949 = PyInt_FromLong(59888949L); if (unlikely(!__pyx_int_59888949)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_82662024 = PyInt_FromLong(82662024L); if (unlikely(!__pyx_int_82662024)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_99932858 = PyInt_FromLong(99932858L); if (unlikely(!__pyx_int_99932858)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_203704333 = PyInt_FromLong(203704333L); if (unlikely(!__pyx_int_203704333)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_227935910 = PyInt_FromLong(227935910L); if (unlikely(!__pyx_int_227935910)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_231097371 = PyInt_FromLong(231097371L); if (unlikely(!__pyx_int_231097371)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -8606,43 +8225,54 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
+  __pyx_vtabptr_9multimcts_4mcts_Node = &__pyx_vtable_9multimcts_4mcts_Node;
+  __pyx_vtable_9multimcts_4mcts_Node.apply_rewards = (PyObject *(*)(struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> ))__pyx_f_9multimcts_4mcts_4Node_apply_rewards;
+  __pyx_vtable_9multimcts_4mcts_Node.ucb = (double (*)(struct __pyx_obj_9multimcts_4mcts_Node *, double, double))__pyx_f_9multimcts_4mcts_4Node_ucb;
   if (PyType_Ready(&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts_Node.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_Node.tp_dictoffset && __pyx_type_9multimcts_4mcts_Node.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts_Node.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
+  if (__Pyx_SetVtable(__pyx_type_9multimcts_4mcts_Node.tp_dict, __pyx_vtabptr_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Node, (PyObject *)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_Node) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __pyx_ptype_9multimcts_4mcts_Node = &__pyx_type_9multimcts_4mcts_Node;
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_vtabptr_9multimcts_4mcts_MCTS = &__pyx_vtable_9multimcts_4mcts_MCTS;
+  __pyx_vtable_9multimcts_4mcts_MCTS.select = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_select;
+  __pyx_vtable_9multimcts_4mcts_MCTS.expand = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_expand;
+  __pyx_vtable_9multimcts_4mcts_MCTS.simulate = (std::map<std::string,double>  (*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate *__pyx_optional_args))__pyx_f_9multimcts_4mcts_4MCTS_simulate;
+  __pyx_vtable_9multimcts_4mcts_MCTS.backpropagate = (PyObject *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *, std::map<std::string,double> ))__pyx_f_9multimcts_4mcts_4MCTS_backpropagate;
+  __pyx_vtable_9multimcts_4mcts_MCTS.get_best_child = (struct __pyx_obj_9multimcts_4mcts_Node *(*)(struct __pyx_obj_9multimcts_4mcts_MCTS *, struct __pyx_obj_9multimcts_4mcts_Node *))__pyx_f_9multimcts_4mcts_4MCTS_get_best_child;
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts_MCTS.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts_MCTS.tp_dictoffset && __pyx_type_9multimcts_4mcts_MCTS.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts_MCTS.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_9multimcts_4mcts_MCTS, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 114, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_9multimcts_4mcts_MCTS, "__init__"); if (unlikely(!wrapper)) __PYX_ERR(0, 134, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
       __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__ = *((PyWrapperDescrObject *)wrapper)->d_base;
       __pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__.doc = __pyx_doc_9multimcts_4mcts_4MCTS___init__;
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_9multimcts_4mcts_4MCTS___init__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MCTS, (PyObject *)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_9multimcts_4mcts_MCTS.tp_dict, __pyx_vtabptr_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MCTS, (PyObject *)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_9multimcts_4mcts_MCTS) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __pyx_ptype_9multimcts_4mcts_MCTS = &__pyx_type_9multimcts_4mcts_MCTS;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -8761,14 +8391,15 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_mcts(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  __Pyx_TraceDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8870,17 +8501,18 @@
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
+  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_mcts(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":5
- * # cython: profile=False
+ * # cython: profile=True
  * 
  * from time import time             # <<<<<<<<<<<<<<
  * from random import shuffle, choice
  * from typing import Union, Dict, List, Any
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -9047,90 +8679,90 @@
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
- *         """Returns a list of all legal moves from this state."""
+ *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Move); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
- *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_u_GameState) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
- *         """Checks if the game is over."""
+ *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
- *         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+ *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rewards); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
@@ -9145,15 +8777,15 @@
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "multimcts/mcts.pyx":21
@@ -9165,111 +8797,54 @@
  */
   __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_4) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":197
- * 
- *     @staticmethod
- *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
- *         """Step 2: Expansion
- *         Add a new child to this node.
- */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":196
- *         return node
- * 
- *     @staticmethod             # <<<<<<<<<<<<<<
- *     def expand(node:Node) -> Node:
- *         """Step 2: Expansion
- */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_expand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":243
- * 
- *     @staticmethod
- *     def backpropagate(node:Node, reward:Rewards):             # <<<<<<<<<<<<<<
- *         """Step 4: Backpropagation
- *         Update all ancestors with the reward from this terminal node.
- */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_4) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
-  /* "multimcts/mcts.pyx":242
- *         return reward
- * 
- *     @staticmethod             # <<<<<<<<<<<<<<
- *     def backpropagate(node:Node, reward:Rewards):
- *         """Step 4: Backpropagation
- */
-  __Pyx_GetNameInClass(__pyx_t_4, (PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_9multimcts_4mcts_MCTS->tp_dict, __pyx_n_s_backpropagate, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  PyType_Modified(__pyx_ptype_9multimcts_4mcts_MCTS);
-
   /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_1__pyx_unpickle_Node, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Node, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result._children = __pyx_state[0]; __pyx_result._is_fully_expanded = __pyx_state[1]; __pyx_result._is_terminal = __pyx_state[2]; __pyx_result._move = __pyx_state[3]; __pyx_result._num_visits = __pyx_state[4]; __pyx_result._parent = __pyx_state[5]; __pyx_result._remaining_moves = __pyx_state[6]; __pyx_result._state = __pyx_state[7]; __pyx_result._team = __pyx_state[8]; __pyx_result._total_reward = __pyx_state[9]; __pyx_result.log_visits = __pyx_state[10]
- *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
+ *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_9multimcts_4mcts_3__pyx_unpickle_MCTS, NULL, __pyx_n_s_multimcts_mcts); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MCTS, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3
- * # cython: profile=False
+ * # cython: profile=True
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "map.from_py":174
  * 
- * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_float")
- * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_float(object o) except *:             # <<<<<<<<<<<<<<
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
+  __Pyx_TraceReturn(Py_None, 0);
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -9337,34 +8912,14 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -9381,14 +8936,124 @@
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
+/* Profile */
+#if CYTHON_PROFILE
+static int __Pyx_TraceSetupAndCall(PyCodeObject** code,
+                                   PyFrameObject** frame,
+                                   PyThreadState* tstate,
+                                   const char *funcname,
+                                   const char *srcfile,
+                                   int firstlineno) {
+    PyObject *type, *value, *traceback;
+    int retval;
+    if (*frame == NULL || !CYTHON_PROFILE_REUSE_FRAME) {
+        if (*code == NULL) {
+            *code = __Pyx_createFrameCodeObject(funcname, srcfile, firstlineno);
+            if (*code == NULL) return 0;
+        }
+        *frame = PyFrame_New(
+            tstate,                          /*PyThreadState *tstate*/
+            *code,                           /*PyCodeObject *code*/
+            __pyx_d,                  /*PyObject *globals*/
+            0                                /*PyObject *locals*/
+        );
+        if (*frame == NULL) return 0;
+        if (CYTHON_TRACE && (*frame)->f_trace == NULL) {
+            Py_INCREF(Py_None);
+            (*frame)->f_trace = Py_None;
+        }
+#if PY_VERSION_HEX < 0x030400B1
+    } else {
+        (*frame)->f_tstate = tstate;
+#endif
+    }
+    __Pyx_PyFrame_SetLineNumber(*frame, firstlineno);
+    retval = 1;
+    __Pyx_EnterTracing(tstate);
+    __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
+    #if CYTHON_TRACE
+    if (tstate->c_tracefunc)
+        retval = tstate->c_tracefunc(tstate->c_traceobj, *frame, PyTrace_CALL, NULL) == 0;
+    if (retval && tstate->c_profilefunc)
+    #endif
+        retval = tstate->c_profilefunc(tstate->c_profileobj, *frame, PyTrace_CALL, NULL) == 0;
+    __Pyx_LeaveTracing(tstate);
+    if (retval) {
+        __Pyx_ErrRestoreInState(tstate, type, value, traceback);
+        return __Pyx_IsTracing(tstate, 0, 0) && retval;
+    } else {
+        Py_XDECREF(type);
+        Py_XDECREF(value);
+        Py_XDECREF(traceback);
+        return -1;
+    }
+}
+static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno) {
+    PyCodeObject *py_code = 0;
+#if PY_MAJOR_VERSION >= 3
+    py_code = PyCode_NewEmpty(srcfile, funcname, firstlineno);
+    if (likely(py_code)) {
+        py_code->co_flags |= CO_OPTIMIZED | CO_NEWLOCALS;
+    }
+#else
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
+    py_funcname = PyString_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    py_srcfile = PyString_FromString(srcfile);
+    if (unlikely(!py_srcfile)) goto bad;
+    py_code = PyCode_New(
+        0,
+        0,
+        0,
+        CO_OPTIMIZED | CO_NEWLOCALS,
+        __pyx_empty_bytes,     /*PyObject *code,*/
+        __pyx_empty_tuple,     /*PyObject *consts,*/
+        __pyx_empty_tuple,     /*PyObject *names,*/
+        __pyx_empty_tuple,     /*PyObject *varnames,*/
+        __pyx_empty_tuple,     /*PyObject *freevars,*/
+        __pyx_empty_tuple,     /*PyObject *cellvars,*/
+        py_srcfile,       /*PyObject *filename,*/
+        py_funcname,      /*PyObject *name,*/
+        firstlineno,
+        __pyx_empty_bytes      /*PyObject *lnotab*/
+    );
+bad:
+    Py_XDECREF(py_srcfile);
+    Py_XDECREF(py_funcname);
+#endif
+    return py_code;
+}
+#endif
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -10017,14 +9682,54 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* PyErrExceptionMatches */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
@@ -10342,27 +10047,14 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
-/* ExtTypeTest */
-static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    if (likely(__Pyx_TypeCheck(obj, type)))
-        return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
-    return 0;
-}
-
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
@@ -10523,144 +10215,14 @@
         __Pyx_SET_SIZE(L, Py_SIZE(L) - 1);
         return PyList_GET_ITEM(L, PyList_GET_SIZE(L));
     }
     return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyList_Type_pop, L);
 }
 #endif
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* PyObjectCallMethod1 */
 static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
     PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
     Py_DECREF(method);
     return result;
 }
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
@@ -10684,17 +10246,345 @@
         if (unlikely(!retval))
             return -1;
         Py_DECREF(retval);
     }
     return 0;
 }
 
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
+/* PyIntCompare */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+    if (op1 == op2) {
+        Py_RETURN_TRUE;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = Py_SIZE(op1);
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        if (intval == 0) {
+            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+        } else if (intval < 0) {
+            if (size >= 0)
+                Py_RETURN_FALSE;
+            intval = -intval;
+            size = -size;
+        } else {
+            if (size <= 0)
+                Py_RETURN_FALSE;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    return (
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr = NULL;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
+/* pyobject_as_double */
+static double __Pyx__PyObject_AsDouble(PyObject* obj) {
+    PyObject* float_value;
+#if !CYTHON_USE_TYPE_SLOTS
+    float_value = PyNumber_Float(obj);  if ((0)) goto bad;
+#else
+    PyNumberMethods *nb = Py_TYPE(obj)->tp_as_number;
+    if (likely(nb) && likely(nb->nb_float)) {
+        float_value = nb->nb_float(obj);
+        if (likely(float_value) && unlikely(!PyFloat_Check(float_value))) {
+            PyErr_Format(PyExc_TypeError,
+                "__float__ returned non-float (type %.200s)",
+                Py_TYPE(float_value)->tp_name);
+            Py_DECREF(float_value);
+            goto bad;
+        }
+    } else if (PyUnicode_CheckExact(obj) || PyBytes_CheckExact(obj)) {
+#if PY_MAJOR_VERSION >= 3
+        float_value = PyFloat_FromString(obj);
+#else
+        float_value = PyFloat_FromString(obj, 0);
+#endif
+    } else {
+        PyObject* args = PyTuple_New(1);
+        if (unlikely(!args)) goto bad;
+        PyTuple_SET_ITEM(args, 0, obj);
+        float_value = PyObject_Call((PyObject*)&PyFloat_Type, args, 0);
+        PyTuple_SET_ITEM(args, 0, 0);
+        Py_DECREF(args);
+    }
+#endif
+    if (likely(float_value)) {
+        double value = PyFloat_AS_DOUBLE(float_value);
+        Py_DECREF(float_value);
+        return value;
+    }
+bad:
+    return (double)-1;
+}
+
+/* ExtTypeTest */
+static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    if (likely(__Pyx_TypeCheck(obj, type)))
+        return 1;
+    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
+                 Py_TYPE(obj)->tp_name, type->tp_name);
+    return 0;
+}
+
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
+    PyObject *module = 0;
+    PyObject *global_dict = 0;
+    PyObject *empty_dict = 0;
+    PyObject *list;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (!py_import)
+        goto bad;
+    #endif
+    if (from_list)
+        list = from_list;
+    else {
+        empty_list = PyList_New(0);
+        if (!empty_list)
+            goto bad;
+        list = empty_list;
+    }
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
+    empty_dict = PyDict_New();
+    if (!empty_dict)
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                module = PyImport_ImportModuleLevelObject(
+                    name, global_dict, empty_dict, list, 1);
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (!py_level)
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, global_dict, empty_dict, list, level);
+            #endif
+        }
+    }
+bad:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
+    return module;
+}
+
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
+    }
+    return value;
+}
+
+/* HasAttr */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (unlikely(!r)) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
@@ -10928,198 +10818,14 @@
         *pkey = next_item;
     } else {
         *pvalue = next_item;
     }
     return 1;
 }
 
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
-    PyObject *module = 0;
-    PyObject *global_dict = 0;
-    PyObject *empty_dict = 0;
-    PyObject *list;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
-        goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
-        empty_list = PyList_New(0);
-        if (!empty_list)
-            goto bad;
-        list = empty_list;
-    }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
-    empty_dict = PyDict_New();
-    if (!empty_dict)
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
-            #endif
-        }
-    }
-bad:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
-/* HasAttr */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
-    PyObject *r;
-    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "hasattr(): attribute name must be string");
-        return -1;
-    }
-    r = __Pyx_GetAttr(o, n);
-    if (unlikely(!r)) {
-        PyErr_Clear();
-        return 0;
-    } else {
-        Py_DECREF(r);
-        return 1;
-    }
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -11162,14 +10868,32 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
+/* SetVTable */
+static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+#if PY_VERSION_HEX >= 0x02070000
+    PyObject *ob = PyCapsule_New(vtable, 0, 0);
+#else
+    PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
+#endif
+    if (!ob)
+        goto bad;
+    if (PyDict_SetItem(dict, __pyx_n_s_pyx_vtable, ob) < 0)
+        goto bad;
+    Py_DECREF(ob);
+    return 0;
+bad:
+    Py_XDECREF(ob);
+    return -1;
+}
+
 /* PyObjectGetAttrStrNoError */
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
@@ -11288,43 +11012,14 @@
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -12094,34 +11789,14 @@
         result = PyObject_Call(metaclass, margs, mkw);
         Py_DECREF(margs);
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
-/* GetNameInClass */
-static PyObject *__Pyx_GetGlobalNameAfterAttributeLookup(PyObject *name) {
-    PyObject *result;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        return NULL;
-    __Pyx_PyErr_Clear();
-    __Pyx_GetModuleGlobalNameUncached(result, name);
-    return result;
-}
-static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name) {
-    PyObject *result;
-    result = __Pyx_PyObject_GetAttrStr(nmspace, name);
-    if (!result) {
-        result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
-    }
-    return result;
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
```

### Comparing `multimcts-0.4/multimcts/mcts.pyx` & `multimcts-0.4.1/multimcts/mcts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,125 @@
-# distutils: language=c++
-# cython: language_level=3
-# cython: profile=False
-
+from math import sqrt, log
 from time import time
 from random import shuffle, choice
 from typing import Union, Dict, List, Any
 
-from libc.math cimport log, sqrt, INFINITY
-from libcpp.map cimport map
-from libcpp.string cimport string
-from libcpp.pair cimport pair
-cimport cython
-
 
 Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
 Team = Union[int,str]
 Rewards = Dict[Team,float]
 
 
 class GameState:
     def get_current_team(self) -> Team:
         """The identifier of the current player's team."""
         raise NotImplementedError("GameState must implement get_current_team.")
 
     def get_legal_moves(self) -> List[Move]:
-        """Returns a list of all legal moves from this state."""
+        """List of all legal moves from this state."""
         raise NotImplementedError("GameState must implement get_legal_moves.")
 
     def make_move(self, move:Move) -> 'GameState':
-        """Returns a new GameState, which is the result of applying the given move to this state.
+        """A new GameState--the result of applying the given move to this state.
         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
         """
         raise NotImplementedError("GameState must implement make_move.")
 
     def is_terminal(self) -> bool:
-        """Checks if the game is over."""
+        """Is the game over?"""
         raise NotImplementedError("GameState must implement is_terminal.")
 
     def get_reward(self) -> Union[float,Rewards]:
-        """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
+        """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}
         Note: This method is only called on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
 
-cdef class Node:
+class Node:
     """Represents a game state node in the MCTS search tree.
-
     Args:
         state (GameState): The game state at the current node.
         parent (Node): The parent of the current node in the search tree.
         move (Move): The move that was played from the parent node to get to this node.
-
     Attributes:
-        children (list): The child nodes of the current node. These represent legal moves that have been visited.
-        num_visits (int): The number of times the node has been visited.
-        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.
+        children (List[Node]): The child nodes of the current node. These represent legal moves that have been visited.
+        visits (int): The number of times the node has been visited.
+        rewards (dict): All teams' rewards obtained from simulations through the node. Keys are teams; values are rewards.
         is_terminal (bool): Whether the node represents a terminal state.
         is_fully_expanded (bool): Whether all children of the node have been visited.
         remaining_moves (list): A list of moves that have not yet been tried.
     """
-    cdef _state, _move
-    cdef string _team
-    cdef Node _parent
-    cdef _children, _remaining_moves
-    cdef map[string,float] _total_reward
-    cdef int _num_visits
-    cdef double log_visits
-    cdef bint _is_terminal
-    cdef bint _is_fully_expanded
-
     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
-        self._state = state
-        self._parent = parent
-        self._move = move
-        self._team = str(self._state.get_current_team()).encode()
-
-        self._children:List['Node'] = []
-        self._num_visits = 0
-        self.log_visits = -INFINITY
-        self._total_reward = map[string,float]()
-
-        self._is_terminal = self._state.is_terminal()
-        if self._is_terminal:
-            self._is_fully_expanded = True
-            self._remaining_moves = []
+        self.state = state
+        self.parent = parent
+        self.move = move
+
+        self.children:List['Node'] = []
+        self.visits = 0
+        self.rewards = {}
+        self.is_terminal = self.state.is_terminal()
+        self.is_fully_expanded = self.is_terminal
+        if self.is_fully_expanded:
+            self.remaining_moves = []
         else:
-            self._is_fully_expanded = False
-            self._remaining_moves = self._state.get_legal_moves()
-            shuffle(self._remaining_moves)#.do a c-shuffle? need memoryview?
-
-    @property
-    def state(self) -> GameState: return self._state
-    @property
-    def parent(self) -> 'Node': return self._parent
-    @property
-    def move(self) -> Move: return self._move
-    @property
-    def children(self) -> List['Node']: return self._children
-    @property
-    def remaining_moves(self) -> List[Move]: return self._remaining_moves
-
-    @cython.cdivision(True)
-    @cython.boundscheck(False)
-    @cython.wraparound(False)
-    def visit(self):
-        self._num_visits += 1
-        self.log_visits = log(self._num_visits)
+            self.remaining_moves = self.state.get_legal_moves()
+            shuffle(self.remaining_moves)
 
+        # The following are cached for performance.
+        self.team = self.state.get_current_team()
+        if self.parent is not None:
+            self.rewards[self.parent.team] = 0
+        self.sqrtlog_visits = 0
+        self.invsqrt_visits = 0
+        self.avg_reward = 0
+
+    def apply_rewards(self, rewards:Rewards):
+        """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
+        self.visits += 1
+
+        self.sqrtlog_visits = sqrt(log(self.visits))
+        self.invsqrt_visits = 1 / sqrt(self.visits)
+
+        total_rewards = 0
+        for k,v in rewards.items():
+            if k not in self.rewards:
+                self.rewards[k] = 0
+            self.rewards[k] += v
+            total_rewards += self.rewards[k]
+
+        if self.parent is not None:
+            # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
+            self.avg_reward = ((2 * self.rewards[self.parent.team]) - total_rewards) / self.visits
+
+    def ucb(self, exploration_bias:float, parent_sqrtlog_visits:float):
+        """Upper Confidence Bound
+        ucb = (x / n) + C * sqrt(ln(N) / n)
+        x=reward for this node
+        n=number of simulations for this node
+        N=number of simulations for parent node
+        C=exploration bias
+        """
+        # ucb = avgR + C * sqrt(ln(N)) * (1/sqrt(n))
+        return self.avg_reward + exploration_bias * parent_sqrtlog_visits * self.invsqrt_visits
 
-cdef class MCTS:
-    cdef double exploration_bias
 
+class MCTS:
     def __init__(self, exploration_bias:float=1.414):
         """Initializes an MCTS agent.
-
         Args:
-            exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.
-                It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).
+            exploration_bias (float): The exploration bias, which balances exploration (favoring untested moves) and exploitation (favoring good moves).
                 The default √2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
         """
         self.exploration_bias = exploration_bias
 
-    @property
-    def exploration_bias(self) -> float:
-        return self.exploration_bias
-
     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
         """Searches for this state's best move until some limit has been reached.
-
         Args:
             state (GameState): The game state for which to find the best move.
             max_time (int|float): The maximum time to search, in seconds.
             max_iterations (int): The maximum number of selections/simulations to perform.
             heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.
             return_type (str): One of "state", "move", or "node".
         Returns:
@@ -146,161 +131,131 @@
             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
 
         if max_time is None and max_iterations is None:
             raise ValueError("One or more of max_time/max_iterations is required.")
 
         node = Node(state)
 
-        cdef double exploration_bias = self.exploration_bias
-
-        cdef double end_time
-        cdef int i
         if max_time is not None:
             end_time = time() + max_time
         if max_iterations is not None:
-            i = max_iterations
+            i = 0
 
         while True:
-            child = self.select(node, exploration_bias)
-            reward = self.simulate(child, heuristic=heuristic)
-            self.backpropagate(child, reward)
+            child = self.select(node)
+            rewards = self.simulate(child, heuristic=heuristic)
+            self.backpropagate(child, rewards)
 
-            if max_time is not None and time() >= end_time:
+            # If there is only one legal move, we don't need to search.
+            if node.is_fully_expanded and len(node.children) == 1:
                 break
+
+            if max_time is not None:
+                if time() >= end_time:
+                    break
             if max_iterations is not None:
-                i -= 1
-                if i <= 0:
+                i += 1
+                if i >= max_iterations:
                     break
 
-        best = self.get_best_child(node, exploration_bias)
+        best = self.get_best_child(node)
 
         if return_type == "state":
             return best.state
         elif return_type == "move":
             return best.move
         elif return_type == "node":
             return best
 
-    def select(self, node:Node, exploration_bias:float) -> Node:
+    def select(self, node:Node) -> Node:
         """Step 1: Selection
         Traverse the tree for the node we most want to simulate.
         Looks for an unexplored child of this node's best child's best child's...best child.
         """
-        while not node._is_terminal:
-            if not node._is_fully_expanded:
+        while not node.is_terminal:
+            if not node.is_fully_expanded:
                 return self.expand(node)
             else:
-                node = self.get_best_child(node, exploration_bias)
-
+                node = self.get_best_child(node)
         return node
 
-    @staticmethod
-    def expand(node:Node) -> Node:
+    def expand(self, node:Node) -> Node:
         """Step 2: Expansion
         Add a new child to this node.
         """
-        try:
-            move = node.remaining_moves.pop()
-        except IndexError:
-            raise IndexError("Tried to expand a node with no remaining moves.")
+        move = node.remaining_moves.pop()
+        if len(node.remaining_moves) == 0:
+            node.is_fully_expanded = True
 
         child = Node(state=node.state.make_move(move), parent=node, move=move)
         node.children.append(child)
 
-        if len(node.remaining_moves) == 0:
-            node._is_fully_expanded = True
-
         return child
 
-    def simulate(self, node:Node, *, heuristic=None) -> Rewards:
+    def simulate(self, node:Node, heuristic=None) -> Rewards:
         """Step 3: Simulation (aka playout/rollout)
         Play out a game, from the given node to termination, and return the final reward.
         A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.
-
         Args:
             node (Node): The node from which to begin the simulation.
             heuristic (callable): A function that takes a state and returns a move.
         """
         state = node.state
 
-        if node._is_terminal:
-            terminal_team = node.parent.state.get_current_team()
+        terminal_team = None
+        if node.is_terminal:
+            terminal_team = node.parent.team
         else:
             while not state.is_terminal():
                 terminal_team = state.get_current_team()
                 if heuristic is not None:
                     move = heuristic(state)
                 else:
                     move = choice(state.get_legal_moves())
                 state = state.make_move(move)
 
         reward = state.get_reward()
         if not isinstance(reward, dict):
             reward = {terminal_team: reward}
 
-        return reward
+        return {k:v for k,v in reward.items() if v!=0}
 
-    @staticmethod
-    def backpropagate(node:Node, reward:Rewards):
+    def backpropagate(self, node:Node, rewards:Rewards):
         """Step 4: Backpropagation
         Update all ancestors with the reward from this terminal node.
         """
-        cdef double val
-        cdef string ckey
-        cdef map[string,float] creward = map[string,float]()
-        for key,val in reward.items():
-            if val == 0:
-                continue
-            ckey = str(key).encode()
-            creward[ckey] = val
-
-        cdef pair[string,float] item
         while node is not None:
-            for item in creward:
-                ckey = item.first
-                if node._total_reward.count(ckey) == 0:
-                    node._total_reward[ckey] = 0
-                node._total_reward[ckey] += item.second
-            node.visit()
+            node.apply_rewards(rewards)
             node = node.parent
 
-    @cython.cdivision(True)
-    @cython.boundscheck(False)
-    @cython.wraparound(False)
-    def get_best_child(self, node:Node, exploration_bias:float) -> Node:
-        """Find the child with the highest Upper Confidence Bound (UCB) score.
-        ucb = (x / n) + C * sqrt(ln(N) / n)
-        x=reward for this node
-        n=number of simulations for this node
-        N=number of simulations for parent node
-        C=exploration bias
-        """
-        # Initialize UCB variables.
-        cdef int visits
-        cdef double reward, ucb
-        cdef double C = exploration_bias
-        cdef double ln_parent_visits = node.log_visits
-
-        cdef string cur_team = node._team
-
-        cdef Node child, best_child
-        cdef pair[string,float] item
-
-        cdef double best_score = -INFINITY
+    def get_best_child(self, node:Node) -> Node:
+        """Find the child with the highest Upper Confidence Bound (UCB)."""
+        parent_sqrtlog_visits = node.sqrtlog_visits
+        best_score = float('-inf')
 
         for child in node.children:
-            visits = child._num_visits
-            if visits == 0: # This should never happen but we're skipping div by 0 checks so just to be safe...
-                continue
-
-            # Relative reward is this child's reward minus its siblings' rewards.
-            reward = 2 * child._total_reward[cur_team]
-            for item in child._total_reward:
-                reward -= item.second
-
-            ucb = (reward / visits) + C * sqrt(ln_parent_visits / visits)
-
+            ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
             if ucb > best_score:
                 best_score = ucb
                 best_child = child
 
         return best_child
+
+
+if __name__ == "__main__":
+    class Score10(GameState):
+        def __init__(self, player=1, score=-4):
+            self.player = player
+            self.score = score
+        def get_current_team(self): return self.player
+        def get_legal_moves(self): return list(range(-9,10))
+        def make_move(self, move): return Score10(-1*self.player, self.score+move)
+        def is_terminal(self): return abs(self.score) >= 10
+        def get_reward(self): return -1 * self.player * self.score
+        def __repr__(self): return f'{str(self.score).rjust(3)} : {"pos" if self.player==1 else "neg"} to play'
+    mcts = MCTS()
+    state = Score10()
+    while not state.is_terminal():
+        move = mcts.search(state, max_iterations=100, return_type="move")
+        print(state, f'(chose {move})')
+        state = state.make_move(move)
+    print(state)
```

### Comparing `multimcts-0.4/multimcts.egg-info/PKG-INFO` & `multimcts-0.4.1/multimcts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.4
+Version: 0.4.1
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,53 +13,44 @@
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
 
 
 ## Features
 
-- Efficient MCTS implementation
+- Efficient (largely C-compiled) MCTS implementation
 - Support for any number of players/teams
 - Easily create AI for any board game
 
 
-## Game Implementation
+## Usage
 
 ### For your game, you will need to:
-- Represent the game state in code
+- Represent a game state in code
 - Identify all legal moves
 - Determine if the game is over and who won
 
 ### You do NOT need to:
 - Understand strategy
 - Have domain knowledge
 - Evaluate the favorability of a game state
 
-
-## Installation
-
+You can install with pip.
 ```bash
 pip install multimcts
 ```
 
-
-## Usage
-
-To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
+To use MultiMCTS, you must first define your game by subclassing `GameState` and implementing the required methods (see the [Tic-Tac-Toe](https://github.com/taylorvance/multimcts/blob/main/examples/tictactoe.py) example):
 - `get_current_team` -- Returns the current team.
 - `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
 - `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
 - `is_terminal` -- Returns whether the game is over.
 - `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
-Then you can use MCTS to search for the best move. It will search until some limit is reached.
-```python
-state = mcts.search(MyGameState(), max_time=5, max_iterations=10000)
-```
-
+Then you can use MCTS to search for the best move. It will search until your defined limit is reached. The following shows how to simulate a game using MCTS:
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
     pass
```

### Comparing `multimcts-0.4/setup.py` & `multimcts-0.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
 setup(
     name='multimcts',
-    version='0.4',
+    version='0.4.1',
     description='Monte Carlo Tree Search for multiple teams',
     author='Taylor Vance',
     author_email='mirrors.cities0w@icloud.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/taylorvance/multimcts',
```

