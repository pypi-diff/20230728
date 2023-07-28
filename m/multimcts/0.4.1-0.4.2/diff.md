# Comparing `tmp/multimcts-0.4.1.tar.gz` & `tmp/multimcts-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.4.1.tar", last modified: Fri Jul 28 21:07:22 2023, max compression
+gzip compressed data, was "multimcts-0.4.2.tar", last modified: Fri Jul 28 21:14:39 2023, max compression
```

## Comparing `multimcts-0.4.1.tar` & `multimcts-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.694677 multimcts-0.4.1/
--rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.4.1/LICENSE
--rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:07:22.694542 multimcts-0.4.1/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     2673 2023-07-28 21:05:02.000000 multimcts-0.4.1/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.693800 multimcts-0.4.1/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.4.1/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   529256 2023-07-27 19:57:49.000000 multimcts-0.4.1/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)   529951 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts/mcts.cpp
--rw-r--r--   0 taylorvance   (501) staff       (20)    10793 2023-07-28 14:44:52.000000 multimcts-0.4.1/multimcts/mcts.py
--rw-r--r--   0 taylorvance   (501) staff       (20)    11224 2023-07-28 13:26:02.000000 multimcts-0.4.1/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:07:22.694335 multimcts-0.4.1/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      268 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-28 21:07:22.000000 multimcts-0.4.1/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.4.1/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-28 21:07:22.694740 multimcts-0.4.1/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      619 2023-07-27 02:14:35.000000 multimcts-0.4.1/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:14:39.109374 multimcts-0.4.2/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.4.2/LICENSE
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:14:39.109233 multimcts-0.4.2/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2673 2023-07-28 21:05:02.000000 multimcts-0.4.2/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:14:39.108433 multimcts-0.4.2/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.4.2/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   529256 2023-07-28 21:12:45.000000 multimcts-0.4.2/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)   510542 2023-07-28 21:14:39.000000 multimcts-0.4.2/multimcts/mcts.cpp
+-rw-r--r--   0 taylorvance   (501) staff       (20)    11225 2023-07-28 21:14:31.000000 multimcts-0.4.2/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-28 21:14:39.109021 multimcts-0.4.2/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2989 2023-07-28 21:14:39.000000 multimcts-0.4.2/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      250 2023-07-28 21:14:39.000000 multimcts-0.4.2/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-28 21:14:39.000000 multimcts-0.4.2/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-28 21:14:39.000000 multimcts-0.4.2/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.4.2/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-28 21:14:39.109420 multimcts-0.4.2/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      619 2023-07-28 21:12:40.000000 multimcts-0.4.2/setup.py
```

### Comparing `multimcts-0.4.1/LICENSE` & `multimcts-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multimcts-0.4.1/PKG-INFO` & `multimcts-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.4.1
+Version: 0.4.2
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `multimcts-0.4.1/README.md` & `multimcts-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `multimcts-0.4.1/multimcts/mcts.c` & `multimcts-0.4.2/multimcts/mcts.c`

 * *Files identical despite different names*

### Comparing `multimcts-0.4.1/multimcts/mcts.cpp` & `multimcts-0.4.2/multimcts/mcts.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1170,14 +1170,21 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1206,253 +1213,14 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
-/* Profile.proto */
-#ifndef CYTHON_PROFILE
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
-  #define CYTHON_PROFILE 0
-#else
-  #define CYTHON_PROFILE 1
-#endif
-#endif
-#ifndef CYTHON_TRACE_NOGIL
-  #define CYTHON_TRACE_NOGIL 0
-#else
-  #if CYTHON_TRACE_NOGIL && !defined(CYTHON_TRACE)
-    #define CYTHON_TRACE 1
-  #endif
-#endif
-#ifndef CYTHON_TRACE
-  #define CYTHON_TRACE 0
-#endif
-#if CYTHON_TRACE
-  #undef CYTHON_PROFILE_REUSE_FRAME
-#endif
-#ifndef CYTHON_PROFILE_REUSE_FRAME
-  #define CYTHON_PROFILE_REUSE_FRAME 0
-#endif
-#if CYTHON_PROFILE || CYTHON_TRACE
-  #include "compile.h"
-  #include "frameobject.h"
-  #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #if CYTHON_PROFILE_REUSE_FRAME
-    #define CYTHON_FRAME_MODIFIER static
-    #define CYTHON_FRAME_DEL(frame)
-  #else
-    #define CYTHON_FRAME_MODIFIER
-    #define CYTHON_FRAME_DEL(frame) Py_CLEAR(frame)
-  #endif
-  #define __Pyx_TraceDeclarations\
-      static PyCodeObject *__pyx_frame_code = NULL;\
-      CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
-      int __Pyx_use_tracing = 0;
-  #define __Pyx_TraceFrameInit(codeobj)\
-      if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
-#if PY_VERSION_HEX >= 0x030b00a2
-  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
-     (unlikely((tstate)->cframe->use_tracing) &&\
-         (!(check_tracing) || !(tstate)->tracing) &&\
-         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
-#elif PY_VERSION_HEX >= 0x030a00b1
-  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
-     (unlikely((tstate)->cframe->use_tracing) &&\
-         (!(check_tracing) || !(tstate)->tracing) &&\
-         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate)\
-      do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
-  #define __Pyx_LeaveTracing(tstate)\
-      do {\
-          tstate->tracing--;\
-          tstate->cframe->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
-                                 || tstate->c_profilefunc != NULL);\
-      } while (0)
-#else
-  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
-     (unlikely((tstate)->use_tracing) &&\
-         (!(check_tracing) || !(tstate)->tracing) &&\
-         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate)\
-      do { tstate->tracing++; tstate->use_tracing = 0; } while (0)
-  #define __Pyx_LeaveTracing(tstate)\
-      do {\
-          tstate->tracing--;\
-          tstate->use_tracing = ((CYTHON_TRACE && tstate->c_tracefunc != NULL)\
-                                         || tstate->c_profilefunc != NULL);\
-      } while (0)
-#endif
-  #ifdef WITH_THREAD
-  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
-  if (nogil) {\
-      if (CYTHON_TRACE_NOGIL) {\
-          PyThreadState *tstate;\
-          PyGILState_STATE state = PyGILState_Ensure();\
-          tstate = __Pyx_PyThreadState_Current;\
-          if (__Pyx_IsTracing(tstate, 1, 1)) {\
-              __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
-          }\
-          PyGILState_Release(state);\
-          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
-      }\
-  } else {\
-      PyThreadState* tstate = PyThreadState_GET();\
-      if (__Pyx_IsTracing(tstate, 1, 1)) {\
-          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
-          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
-      }\
-  }
-  #else
-  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)\
-  {   PyThreadState* tstate = PyThreadState_GET();\
-      if (__Pyx_IsTracing(tstate, 1, 1)) {\
-          __Pyx_use_tracing = __Pyx_TraceSetupAndCall(&__pyx_frame_code, &__pyx_frame, tstate, funcname, srcfile, firstlineno);\
-          if (unlikely(__Pyx_use_tracing < 0)) goto_error;\
-      }\
-  }
-  #endif
-  #define __Pyx_TraceException()\
-  if (likely(!__Pyx_use_tracing)); else {\
-      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
-      if (__Pyx_IsTracing(tstate, 0, 1)) {\
-          __Pyx_EnterTracing(tstate);\
-          PyObject *exc_info = __Pyx_GetExceptionTuple(tstate);\
-          if (exc_info) {\
-              if (CYTHON_TRACE && tstate->c_tracefunc)\
-                  tstate->c_tracefunc(\
-                      tstate->c_traceobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
-              tstate->c_profilefunc(\
-                  tstate->c_profileobj, __pyx_frame, PyTrace_EXCEPTION, exc_info);\
-              Py_DECREF(exc_info);\
-          }\
-          __Pyx_LeaveTracing(tstate);\
-      }\
-  }
-  static void __Pyx_call_return_trace_func(PyThreadState *tstate, PyFrameObject *frame, PyObject *result) {
-      PyObject *type, *value, *traceback;
-      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
-      __Pyx_EnterTracing(tstate);
-      if (CYTHON_TRACE && tstate->c_tracefunc)
-          tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_RETURN, result);
-      if (tstate->c_profilefunc)
-          tstate->c_profilefunc(tstate->c_profileobj, frame, PyTrace_RETURN, result);
-      CYTHON_FRAME_DEL(frame);
-      __Pyx_LeaveTracing(tstate);
-      __Pyx_ErrRestoreInState(tstate, type, value, traceback);
-  }
-  #ifdef WITH_THREAD
-  #define __Pyx_TraceReturn(result, nogil)\
-  if (likely(!__Pyx_use_tracing)); else {\
-      if (nogil) {\
-          if (CYTHON_TRACE_NOGIL) {\
-              PyThreadState *tstate;\
-              PyGILState_STATE state = PyGILState_Ensure();\
-              tstate = __Pyx_PyThreadState_Current;\
-              if (__Pyx_IsTracing(tstate, 0, 0)) {\
-                  __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
-              }\
-              PyGILState_Release(state);\
-          }\
-      } else {\
-          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
-          if (__Pyx_IsTracing(tstate, 0, 0)) {\
-              __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
-          }\
-      }\
-  }
-  #else
-  #define __Pyx_TraceReturn(result, nogil)\
-  if (likely(!__Pyx_use_tracing)); else {\
-      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
-      if (__Pyx_IsTracing(tstate, 0, 0)) {\
-          __Pyx_call_return_trace_func(tstate, __pyx_frame, (PyObject*)result);\
-      }\
-  }
-  #endif
-  static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno);
-  static int __Pyx_TraceSetupAndCall(PyCodeObject** code, PyFrameObject** frame, PyThreadState* tstate, const char *funcname, const char *srcfile, int firstlineno);
-#else
-  #define __Pyx_TraceDeclarations
-  #define __Pyx_TraceFrameInit(codeobj)
-  #define __Pyx_TraceCall(funcname, srcfile, firstlineno, nogil, goto_error)   if ((1)); else goto_error;
-  #define __Pyx_TraceException()
-  #define __Pyx_TraceReturn(result, nogil)
-#endif
-#if CYTHON_TRACE
-  static int __Pyx_call_line_trace_func(PyThreadState *tstate, PyFrameObject *frame, int lineno) {
-      int ret;
-      PyObject *type, *value, *traceback;
-      __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
-      __Pyx_PyFrame_SetLineNumber(frame, lineno);
-      __Pyx_EnterTracing(tstate);
-      ret = tstate->c_tracefunc(tstate->c_traceobj, frame, PyTrace_LINE, NULL);
-      __Pyx_LeaveTracing(tstate);
-      if (likely(!ret)) {
-          __Pyx_ErrRestoreInState(tstate, type, value, traceback);
-      } else {
-          Py_XDECREF(type);
-          Py_XDECREF(value);
-          Py_XDECREF(traceback);
-      }
-      return ret;
-  }
-  #ifdef WITH_THREAD
-  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
-  if (likely(!__Pyx_use_tracing)); else {\
-      if (nogil) {\
-          if (CYTHON_TRACE_NOGIL) {\
-              int ret = 0;\
-              PyThreadState *tstate;\
-              PyGILState_STATE state = PyGILState_Ensure();\
-              tstate = __Pyx_PyThreadState_Current;\
-              if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
-                  ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
-              }\
-              PyGILState_Release(state);\
-              if (unlikely(ret)) goto_error;\
-          }\
-      } else {\
-          PyThreadState* tstate = __Pyx_PyThreadState_Current;\
-          if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
-              int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
-              if (unlikely(ret)) goto_error;\
-          }\
-      }\
-  }
-  #else
-  #define __Pyx_TraceLine(lineno, nogil, goto_error)\
-  if (likely(!__Pyx_use_tracing)); else {\
-      PyThreadState* tstate = __Pyx_PyThreadState_Current;\
-      if (__Pyx_IsTracing(tstate, 0, 0) && tstate->c_tracefunc && __pyx_frame->f_trace) {\
-          int ret = __Pyx_call_line_trace_func(tstate, __pyx_frame, lineno);\
-          if (unlikely(ret)) goto_error;\
-      }\
-  }
-  #endif
-#else
-  #define __Pyx_TraceLine(lineno, nogil, goto_error)   if ((1)); else goto_error;
-#endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
@@ -1569,19 +1337,14 @@
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
-
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1746,14 +1509,19 @@
  PyFloat_AsDouble(obj) : __Pyx__PyObject_AsDouble(obj))
 #else
 #define __Pyx_PyObject_AsDouble(obj)\
 ((likely(PyFloat_CheckExact(obj))) ?\
  PyFloat_AS_DOUBLE(obj) : __Pyx__PyObject_AsDouble(obj))
 #endif
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
@@ -2255,36 +2023,36 @@
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_56097295;
 static PyObject *__pyx_int_59888949;
 static PyObject *__pyx_int_82662024;
 static PyObject *__pyx_int_99932858;
 static PyObject *__pyx_int_203704333;
 static PyObject *__pyx_int_231097371;
-static PyObject *__pyx_codeobj_;
+static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
-static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
-static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
 /* Late includes */
 
 /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
@@ -2304,32 +2072,29 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj_)
   __Pyx_RefNannySetupContext("get_current_team", 0);
-  __Pyx_TraceCall("get_current_team", __pyx_f[0], 22, 0, __PYX_ERR(0, 22, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 24, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":22
  * 
@@ -2341,15 +2106,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
@@ -2371,32 +2135,29 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__3)
   __Pyx_RefNannySetupContext("get_legal_moves", 0);
-  __Pyx_TraceCall("get_legal_moves", __pyx_f[0], 26, 0, __PYX_ERR(0, 26, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
  *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 28, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
@@ -2408,15 +2169,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
@@ -2489,32 +2249,29 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__5)
   __Pyx_RefNannySetupContext("make_move", 0);
-  __Pyx_TraceCall("make_move", __pyx_f[0], 30, 0, __PYX_ERR(0, 30, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 34, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
@@ -2526,15 +2283,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
@@ -2556,32 +2312,29 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__7)
   __Pyx_RefNannySetupContext("is_terminal", 0);
-  __Pyx_TraceCall("is_terminal", __pyx_f[0], 36, 0, __PYX_ERR(0, 36, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
  *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
@@ -2593,15 +2346,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
@@ -2623,32 +2375,29 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__9)
   __Pyx_RefNannySetupContext("get_reward", 0);
-  __Pyx_TraceCall("get_reward", __pyx_f[0], 40, 0, __PYX_ERR(0, 40, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 46, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
@@ -2660,15 +2409,14 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":72
  *     cdef double avg_reward, sqrtlog_visits, invsqrt_visits
  * 
@@ -2761,28 +2509,26 @@
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4Node___init__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v_state, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_parent, PyObject *__pyx_v_move) {
   int __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::map<std::string,double>  __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   std::string __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 72, 0, __PYX_ERR(0, 72, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":73
  * 
  *     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
  *         self.state = state             # <<<<<<<<<<<<<<
  *         self.parent = parent
  *         self.move = move
@@ -3106,15 +2852,14 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":98
  * 
  *     @property
@@ -3134,33 +2879,24 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_5state___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 98, 0, __PYX_ERR(0, 98, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->state);
   __pyx_r = __pyx_v_self->state;
   goto __pyx_L0;
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("multimcts.mcts.Node.state.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":100
  *     def state(self) -> GameState: return self.state
  *     @property
@@ -3180,37 +2916,34 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_7rewards___get__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 100, 0, __PYX_ERR(0, 100, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_convert_map_to_py_std_3a__3a_string____double(__pyx_v_self->rewards); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.Node.rewards.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":103
  * 
  *     @cython.cdivision(True)
@@ -3219,26 +2952,21 @@
  *         self.visits += 1
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts_4Node_apply_rewards(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, std::map<std::string,double>  __pyx_v_crewards) {
   std::pair<std::string,double>  __pyx_v_item;
   double __pyx_v_total_rewards;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   std::map<std::string,double> ::iterator __pyx_t_1;
   std::pair<std::string,double>  __pyx_t_2;
   int __pyx_t_3;
   std::string __pyx_t_4;
   int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_rewards", 0);
-  __Pyx_TraceCall("apply_rewards", __pyx_f[0], 103, 0, __PYX_ERR(0, 103, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":105
  *     cdef apply_rewards(self, map[string,double] crewards):
  *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
  *         self.visits += 1             # <<<<<<<<<<<<<<
  * 
  *         self.sqrtlog_visits = sqrt(log(self.visits))
@@ -3377,42 +3105,31 @@
  *     cdef apply_rewards(self, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
  *         self.visits += 1
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("multimcts.mcts.Node.apply_rewards", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":122
  *             self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
  * 
  *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
  *         """Upper Confidence Bound
  *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
 static double __pyx_f_9multimcts_4mcts_4Node_ucb(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, double __pyx_v_exploration_bias, double __pyx_v_parent_sqrtlog_visits) {
   double __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ucb", 0);
-  __Pyx_TraceCall("ucb", __pyx_f[0], 122, 0, __PYX_ERR(0, 122, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":131
  *         """
  *         # ucb = avgR + C * sqrt(ln(N)) * (1/sqrt(n))
  *         return self.avg_reward + exploration_bias * parent_sqrtlog_visits * self.invsqrt_visits             # <<<<<<<<<<<<<<
  * 
  * 
@@ -3425,19 +3142,15 @@
  * 
  *     cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):             # <<<<<<<<<<<<<<
  *         """Upper Confidence Bound
  *         ucb = (x / n) + C * sqrt(ln(N) / n)
  */
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_WriteUnraisable("multimcts.mcts.Node.ucb", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
@@ -3458,15 +3171,14 @@
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_2__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
@@ -3476,15 +3188,14 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
-  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.avg_reward, self.children, self.cteam, self.invsqrt_visits, self.is_fully_expanded, self.is_terminal, self.move, self.parent, self.remaining_moves, self.rewards, self.sqrtlog_visits, self.state, self.team, self.visits)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -3772,15 +3483,14 @@
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.Node.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
@@ -3799,22 +3509,20 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node_4__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
-  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Node, (type(self), 0x357fa0f, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Node__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -3834,15 +3542,14 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.Node.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":137
  *     cdef double exploration_bias
  * 
@@ -3915,21 +3622,16 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_9multimcts_4mcts_4MCTS___init__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, double __pyx_v_exploration_bias) {
   int __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
-  __Pyx_TraceCall("__init__", __pyx_f[0], 137, 0, __PYX_ERR(0, 137, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":143
  *                 The default 2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
  *         """
  *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -3942,20 +3644,14 @@
  *     def __init__(self, exploration_bias:float=1.414):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  *         Args:
  */
 
   /* function exit code */
   __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":146
  * 
  *     @property
@@ -3975,37 +3671,34 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_16exploration_bias___get__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
-  __Pyx_TraceCall("__get__", __pyx_f[0], 146, 0, __PYX_ERR(0, 146, __pyx_L1_error));
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.exploration_bias.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":148
  *     def exploration_bias(self) -> float: return self.exploration_bias
  * 
@@ -4097,15 +3790,14 @@
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node = NULL;
   double __pyx_v_end_time;
   int __pyx_v_i;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = NULL;
   std::map<std::string,double>  __pyx_v_rewards;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best = 0;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
@@ -4114,15 +3806,14 @@
   double __pyx_t_9;
   std::map<std::string,double>  __pyx_t_10;
   struct __pyx_opt_args_9multimcts_4mcts_4MCTS_simulate __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
-  __Pyx_TraceCall("search", __pyx_f[0], 148, 0, __PYX_ERR(0, 148, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_return_type);
 
   /* "multimcts/mcts.pyx":159
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         return_type = return_type.lower()             # <<<<<<<<<<<<<<
  *         VALID_RETURN_TYPES = {"state","move","node"}
@@ -4250,15 +3941,15 @@
     /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 165, __pyx_L1_error)
 
     /* "multimcts/mcts.pyx":164
  *             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
@@ -4688,38 +4379,35 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_VALID_RETURN_TYPES);
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XDECREF((PyObject *)__pyx_v_best);
   __Pyx_XDECREF(__pyx_v_return_type);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":200
  *             return best
  * 
  *     cdef Node select(self, Node node):             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
 static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_select(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
-  __Pyx_TraceCall("select", __pyx_f[0], 200, 0, __PYX_ERR(0, 200, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
   /* "multimcts/mcts.pyx":205
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
  *         while not node.is_terminal:             # <<<<<<<<<<<<<<
  *             if not node.is_fully_expanded:
@@ -4801,15 +4489,14 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":212
  *         return node
  * 
@@ -4818,28 +4505,26 @@
  *         Add a new child to this node.
  */
 
 static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_expand(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   PyObject *__pyx_v_move = NULL;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
-  __Pyx_TraceCall("expand", __pyx_f[0], 212, 0, __PYX_ERR(0, 212, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":216
  *         Add a new child to this node.
  *         """
  *         move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
  *         if len(node.remaining_moves) == 0:
  *             node.is_fully_expanded = True
@@ -4954,15 +4639,14 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":225
  *         return child
  * 
@@ -4976,15 +4660,14 @@
   PyObject *__pyx_v_state = NULL;
   PyObject *__pyx_v_terminal_team = NULL;
   PyObject *__pyx_v_move = NULL;
   PyObject *__pyx_v_reward = NULL;
   std::map<std::string,double>  __pyx_v_crewards;
   PyObject *__pyx_v_team = NULL;
   std::map<std::string,double>  __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
@@ -4994,15 +4677,14 @@
   PyObject *(*__pyx_t_10)(PyObject *);
   double __pyx_t_11;
   std::string __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
-  __Pyx_TraceCall("simulate", __pyx_f[0], 225, 0, __PYX_ERR(0, 225, __pyx_L1_error));
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_heuristic = __pyx_optional_args->heuristic;
     }
   }
 
   /* "multimcts/mcts.pyx":233
@@ -5460,39 +5142,36 @@
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v_terminal_team);
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XDECREF(__pyx_v_team);
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":259
  *         return crewards
  * 
  *     cdef backpropagate(self, Node node, map[string,double] crewards):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts_4MCTS_backpropagate(CYTHON_UNUSED struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node, std::map<std::string,double>  __pyx_v_crewards) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
-  __Pyx_TraceCall("backpropagate", __pyx_f[0], 259, 0, __PYX_ERR(0, 259, __pyx_L1_error));
   __Pyx_INCREF((PyObject *)__pyx_v_node);
 
   /* "multimcts/mcts.pyx":263
  *         Update all ancestors with the reward from this terminal node.
  *         """
  *         while node is not None:             # <<<<<<<<<<<<<<
  *             node.apply_rewards(crewards)
@@ -5541,15 +5220,14 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":267
  *             node = node.parent
  * 
@@ -5561,27 +5239,25 @@
 static struct __pyx_obj_9multimcts_4mcts_Node *__pyx_f_9multimcts_4mcts_4MCTS_get_best_child(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_node) {
   double __pyx_v_parent_sqrtlog_visits;
   double __pyx_v_best_score;
   double __pyx_v_ucb;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v_best_child = 0;
   struct __pyx_obj_9multimcts_4mcts_Node *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
-  __Pyx_TraceCall("get_best_child", __pyx_f[0], 267, 0, __PYX_ERR(0, 267, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":269
  *     cdef Node get_best_child(self, Node node):
  *         """Find the child with the highest Upper Confidence Bound (UCB)."""
  *         cdef double parent_sqrtlog_visits = node.sqrtlog_visits             # <<<<<<<<<<<<<<
  *         cdef double best_score = -INFINITY
  *         cdef double ucb
@@ -5742,15 +5418,14 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_child);
   __Pyx_XDECREF((PyObject *)__pyx_v_best_child);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
@@ -5771,26 +5446,24 @@
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4__reduce_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
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
-  __Pyx_TraceCall("__reduce_cython__", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.exploration_bias,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -5980,15 +5653,14 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
@@ -6007,22 +5679,20 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6__setstate_cython__(struct __pyx_obj_9multimcts_4mcts_MCTS *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
-  __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_MCTS, (type(self), 0xc24480d, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_MCTS__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -6042,15 +5712,14 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -6133,39 +5802,36 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts___pyx_unpickle_Node(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
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
-  __Pyx_TraceFrameInit(__pyx_codeobj__12)
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node", 0);
-  __Pyx_TraceCall("__pyx_unpickle_Node", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__13, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):
@@ -6315,30 +5981,28 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
  *         __pyx_unpickle_Node__set_state(<Node> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]
  *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_9multimcts_4mcts___pyx_unpickle_Node__set_state(struct __pyx_obj_9multimcts_4mcts_Node *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   double __pyx_t_2;
   std::string __pyx_t_3;
   int __pyx_t_4;
   std::map<std::string,double>  __pyx_t_5;
   int __pyx_t_6;
@@ -6348,15 +6012,14 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Node__set_state", 0);
-  __Pyx_TraceCall("__pyx_unpickle_Node__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Node__set_state(Node __pyx_result, tuple __pyx_state):
  *     __pyx_result.avg_reward = __pyx_state[0]; __pyx_result.children = __pyx_state[1]; __pyx_result.cteam = __pyx_state[2]; __pyx_result.invsqrt_visits = __pyx_state[3]; __pyx_result.is_fully_expanded = __pyx_state[4]; __pyx_result.is_terminal = __pyx_state[5]; __pyx_result.move = __pyx_state[6]; __pyx_result.parent = __pyx_state[7]; __pyx_result.remaining_moves = __pyx_state[8]; __pyx_result.rewards = __pyx_state[9]; __pyx_result.sqrtlog_visits = __pyx_state[10]; __pyx_result.state = __pyx_state[11]; __pyx_result.team = __pyx_state[12]; __pyx_result.visits = __pyx_state[13]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[14])
@@ -6582,15 +6245,14 @@
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_Node__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_MCTS(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
@@ -6673,39 +6335,36 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_2__pyx_unpickle_MCTS(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
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
-  __Pyx_TraceFrameInit(__pyx_codeobj__14)
   __Pyx_RefNannySetupContext("__pyx_unpickle_MCTS", 0);
-  __Pyx_TraceCall("__pyx_unpickle_MCTS", __pyx_f[1], 1, 0, __PYX_ERR(1, 1, __pyx_L1_error));
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xc24480d, 0xdc6441b, 0x4ed5288) = (exploration_bias))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__15, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc24480d, 0xdc6441b, 0x4ed5288):
@@ -6855,45 +6514,42 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
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
-  __Pyx_TraceCall("__pyx_unpickle_MCTS__set_state", __pyx_f[1], 11, 0, __PYX_ERR(1, 11, __pyx_L1_error));
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_MCTS__set_state(MCTS __pyx_result, tuple __pyx_state):
  *     __pyx_result.exploration_bias = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -6989,37 +6645,34 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("multimcts.mcts.__pyx_unpickle_MCTS__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_f[1], 31, 0, __PYX_ERR(1, 31, __pyx_L1_error));
 
   /* "string.to_py":32
  * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
@@ -7042,37 +6695,34 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_f[1], 37, 0, __PYX_ERR(1, 37, __pyx_L1_error));
 
   /* "string.to_py":38
  * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
@@ -7095,37 +6745,34 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_f[1], 43, 0, __PYX_ERR(1, 43, __pyx_L1_error));
 
   /* "string.to_py":44
  * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
@@ -7148,37 +6795,34 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_f[1], 49, 0, __PYX_ERR(1, 49, __pyx_L1_error));
 
   /* "string.to_py":50
  * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * cdef extern from *:
  *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
@@ -7201,37 +6845,34 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
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
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_f[1], 55, 0, __PYX_ERR(1, 55, __pyx_L1_error));
 
   /* "string.to_py":56
  * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
  * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
  *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
  * 
  */
@@ -7253,15 +6894,14 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
@@ -7270,22 +6910,20 @@
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  */
 
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
   Py_ssize_t __pyx_v_length;
   char const *__pyx_v_data;
   std::string __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   char const *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
-  __Pyx_TraceCall("__pyx_convert_string_from_py_std__in_string", __pyx_f[1], 13, 0, __PYX_ERR(1, 13, __pyx_L1_error));
 
   /* "string.from_py":14
  * @cname("__pyx_convert_string_from_py_std__in_string")
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
  *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
  *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
  *     return string(data, length)
@@ -7321,15 +6959,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.to_py":201
  * 
  * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
@@ -7339,24 +6976,22 @@
  */
 
 static PyObject *__pyx_convert_map_to_py_std_3a__3a_string____double(std::map<std::string,double>  const &__pyx_v_s) {
   PyObject *__pyx_v_o = NULL;
   std::map<std::string,double> ::value_type const *__pyx_v_key_value;
   std::map<std::string,double> ::const_iterator __pyx_v_iter;
   PyObject *__pyx_r = NULL;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_map_to_py_std_3a__3a_string____double", 0);
-  __Pyx_TraceCall("__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_f[1], 201, 0, __PYX_ERR(1, 201, __pyx_L1_error));
 
   /* "map.to_py":202
  * @cname("__pyx_convert_map_to_py_std_3a__3a_string____double")
  * cdef object __pyx_convert_map_to_py_std_3a__3a_string____double(const map[X,Y]& s):
  *     o = {}             # <<<<<<<<<<<<<<
  *     cdef const map[X,Y].value_type *key_value
  *     cdef map[X,Y].const_iterator iter = s.begin()
@@ -7445,15 +7080,14 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("map.to_py.__pyx_convert_map_to_py_std_3a__3a_string____double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_o);
   __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "map.from_py":174
  * 
  * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
@@ -7464,30 +7098,28 @@
 
 static std::map<std::string,double>  __pyx_convert_map_from_py_std_3a__3a_string__and_double(PyObject *__pyx_v_o) {
   PyObject *__pyx_v_d = 0;
   std::map<std::string,double>  __pyx_v_m;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_value = NULL;
   std::map<std::string,double>  __pyx_r;
-  __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   std::string __pyx_t_8;
   double __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and_double", 0);
-  __Pyx_TraceCall("__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_f[1], 174, 0, __PYX_ERR(1, 174, __pyx_L1_error));
 
   /* "map.from_py":175
  * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
  * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:
  *     cdef dict d = o             # <<<<<<<<<<<<<<
  *     cdef map[X,Y] m
  *     for key, value in d.iteritems():
@@ -7564,15 +7196,14 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_d);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_value);
-  __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static struct __pyx_vtabstruct_9multimcts_4mcts_Node __pyx_vtable_9multimcts_4mcts_Node;
 
 static PyObject *__pyx_tp_new_9multimcts_4mcts_Node(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_9multimcts_4mcts_Node *p;
@@ -8018,160 +7649,160 @@
   /* "multimcts/mcts.pyx":24
  *     def get_current_team(self) -> Team:
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
  * 
  *     def get_legal_moves(self) -> List[Move]:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "multimcts/mcts.pyx":28
  *     def get_legal_moves(self) -> List[Move]:
  *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
  * 
  *     def make_move(self, move:Move) -> 'GameState':
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "multimcts/mcts.pyx":34
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  *         """
  *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
  * 
  *     def is_terminal(self) -> bool:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "multimcts/mcts.pyx":38
  *     def is_terminal(self) -> bool:
  *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
  *     def get_reward(self) -> Union[float,Rewards]:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "multimcts/mcts.pyx":46
  *         Note: This method is only called on terminal states.
  *         """
  *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "multimcts/mcts.pyx":165
  * 
  *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         node = Node(state)
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 165, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x357fa0f, 0x5f4daba, 0x391d535):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x357fa0f, 0x5f4daba, 0x391d535) = (avg_reward, children, cteam, invsqrt_visits, is_fully_expanded, is_terminal, move, parent, remaining_moves, rewards, sqrtlog_visits, state, team, visits))" % __pyx_checksum)
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_56097295, __pyx_int_99932858, __pyx_int_59888949); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_56097295, __pyx_int_99932858, __pyx_int_59888949); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_203704333, __pyx_int_231097371, __pyx_int_82662024); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "multimcts/mcts.pyx":22
  * 
  * class GameState:
  *     def get_current_team(self) -> Team:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 22, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":26
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self) -> List[Move]:             # <<<<<<<<<<<<<<
  *         """List of all legal moves from this state."""
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 26, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 26, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":30
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def make_move(self, move:Move) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """A new GameState--the result of applying the given move to this state.
  *         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
  */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 30, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 30, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":36
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 36, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":40
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
  *     def get_reward(self) -> Union[float,Rewards]:             # <<<<<<<<<<<<<<
  *         """The reward earned by the team that played the game-ending move (the "terminal team", or the team from the previous state).
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 40, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Node(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
+  __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Node, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MCTS, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -8391,15 +8022,14 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_mcts(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
-  __Pyx_TraceDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8501,18 +8131,17 @@
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  __Pyx_TraceCall("__Pyx_PyMODINIT_FUNC PyInit_mcts(void)", __pyx_f[0], 1, 0, __PYX_ERR(0, 1, __pyx_L1_error));
 
   /* "multimcts/mcts.pyx":5
- * # cython: profile=True
+ * # cython: profile=False
  * 
  * from time import time             # <<<<<<<<<<<<<<
  * from random import shuffle, choice
  * from typing import Union, Dict, List, Any
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -8679,15 +8308,15 @@
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_3) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":26
@@ -8705,15 +8334,15 @@
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_5) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":30
@@ -8726,15 +8355,15 @@
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_u_GameState) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_3) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":36
@@ -8743,15 +8372,15 @@
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Is the game over?"""
  *         raise NotImplementedError("GameState must implement is_terminal.")
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_5) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":40
@@ -8777,15 +8406,15 @@
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "multimcts/mcts.pyx":21
@@ -8822,29 +8451,28 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MCTS, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # cython: language_level=3
- * # cython: profile=True
+ * # cython: profile=False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "map.from_py":174
  * 
  * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and_double")
  * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and_double(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef dict d = o
  *     cdef map[X,Y] m
  */
-  __Pyx_TraceReturn(Py_None, 0);
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -8912,14 +8540,34 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
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
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -8936,124 +8584,14 @@
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
-/* Profile */
-#if CYTHON_PROFILE
-static int __Pyx_TraceSetupAndCall(PyCodeObject** code,
-                                   PyFrameObject** frame,
-                                   PyThreadState* tstate,
-                                   const char *funcname,
-                                   const char *srcfile,
-                                   int firstlineno) {
-    PyObject *type, *value, *traceback;
-    int retval;
-    if (*frame == NULL || !CYTHON_PROFILE_REUSE_FRAME) {
-        if (*code == NULL) {
-            *code = __Pyx_createFrameCodeObject(funcname, srcfile, firstlineno);
-            if (*code == NULL) return 0;
-        }
-        *frame = PyFrame_New(
-            tstate,                          /*PyThreadState *tstate*/
-            *code,                           /*PyCodeObject *code*/
-            __pyx_d,                  /*PyObject *globals*/
-            0                                /*PyObject *locals*/
-        );
-        if (*frame == NULL) return 0;
-        if (CYTHON_TRACE && (*frame)->f_trace == NULL) {
-            Py_INCREF(Py_None);
-            (*frame)->f_trace = Py_None;
-        }
-#if PY_VERSION_HEX < 0x030400B1
-    } else {
-        (*frame)->f_tstate = tstate;
-#endif
-    }
-    __Pyx_PyFrame_SetLineNumber(*frame, firstlineno);
-    retval = 1;
-    __Pyx_EnterTracing(tstate);
-    __Pyx_ErrFetchInState(tstate, &type, &value, &traceback);
-    #if CYTHON_TRACE
-    if (tstate->c_tracefunc)
-        retval = tstate->c_tracefunc(tstate->c_traceobj, *frame, PyTrace_CALL, NULL) == 0;
-    if (retval && tstate->c_profilefunc)
-    #endif
-        retval = tstate->c_profilefunc(tstate->c_profileobj, *frame, PyTrace_CALL, NULL) == 0;
-    __Pyx_LeaveTracing(tstate);
-    if (retval) {
-        __Pyx_ErrRestoreInState(tstate, type, value, traceback);
-        return __Pyx_IsTracing(tstate, 0, 0) && retval;
-    } else {
-        Py_XDECREF(type);
-        Py_XDECREF(value);
-        Py_XDECREF(traceback);
-        return -1;
-    }
-}
-static PyCodeObject *__Pyx_createFrameCodeObject(const char *funcname, const char *srcfile, int firstlineno) {
-    PyCodeObject *py_code = 0;
-#if PY_MAJOR_VERSION >= 3
-    py_code = PyCode_NewEmpty(srcfile, funcname, firstlineno);
-    if (likely(py_code)) {
-        py_code->co_flags |= CO_OPTIMIZED | CO_NEWLOCALS;
-    }
-#else
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
-    py_funcname = PyString_FromString(funcname);
-    if (unlikely(!py_funcname)) goto bad;
-    py_srcfile = PyString_FromString(srcfile);
-    if (unlikely(!py_srcfile)) goto bad;
-    py_code = PyCode_New(
-        0,
-        0,
-        0,
-        CO_OPTIMIZED | CO_NEWLOCALS,
-        __pyx_empty_bytes,     /*PyObject *code,*/
-        __pyx_empty_tuple,     /*PyObject *consts,*/
-        __pyx_empty_tuple,     /*PyObject *names,*/
-        __pyx_empty_tuple,     /*PyObject *varnames,*/
-        __pyx_empty_tuple,     /*PyObject *freevars,*/
-        __pyx_empty_tuple,     /*PyObject *cellvars,*/
-        py_srcfile,       /*PyObject *filename,*/
-        py_funcname,      /*PyObject *name,*/
-        firstlineno,
-        __pyx_empty_bytes      /*PyObject *lnotab*/
-    );
-bad:
-    Py_XDECREF(py_srcfile);
-    Py_XDECREF(py_funcname);
-#endif
-    return py_code;
-}
-#endif
-
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
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -9682,54 +9220,14 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-    else state = (PyGILState_STATE)0;
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
-    }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
-    }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
-#endif
-}
-
 /* PyErrExceptionMatches */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
@@ -10469,14 +9967,54 @@
         Py_DECREF(float_value);
         return value;
     }
 bad:
     return (double)-1;
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
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
```

### Comparing `multimcts-0.4.1/multimcts/mcts.py` & `multimcts-0.4.2/multimcts/mcts.pyx`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-from math import sqrt, log
+# distutils: language=c++
+# cython: language_level=3
+# cython: profile=False
+
 from time import time
 from random import shuffle, choice
 from typing import Union, Dict, List, Any
 
+from libc.math cimport log, sqrt, INFINITY
+from libcpp.map cimport map
+from libcpp.string cimport string
+from libcpp.pair cimport pair
+cimport cython
+
 
 Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
 Team = Union[int,str]
 Rewards = Dict[Team,float]
 
 
 class GameState:
@@ -33,91 +42,113 @@
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}
         Note: This method is only called on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
 
-class Node:
+cdef class Node:
     """Represents a game state node in the MCTS search tree.
     Args:
         state (GameState): The game state at the current node.
         parent (Node): The parent of the current node in the search tree.
         move (Move): The move that was played from the parent node to get to this node.
     Attributes:
         children (List[Node]): The child nodes of the current node. These represent legal moves that have been visited.
         visits (int): The number of times the node has been visited.
         rewards (dict): All teams' rewards obtained from simulations through the node. Keys are teams; values are rewards.
         is_terminal (bool): Whether the node represents a terminal state.
         is_fully_expanded (bool): Whether all children of the node have been visited.
         remaining_moves (list): A list of moves that have not yet been tried.
     """
+    cdef state, move, team
+    cdef string cteam
+    cdef Node parent
+    cdef children, remaining_moves
+    cdef map[string,double] rewards
+    cdef int visits
+    cdef bint is_terminal, is_fully_expanded
+    cdef double avg_reward, sqrtlog_visits, invsqrt_visits
+
     def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
         self.state = state
         self.parent = parent
         self.move = move
 
         self.children:List['Node'] = []
         self.visits = 0
-        self.rewards = {}
+        self.rewards = map[string,double]()
         self.is_terminal = self.state.is_terminal()
         self.is_fully_expanded = self.is_terminal
         if self.is_fully_expanded:
             self.remaining_moves = []
         else:
             self.remaining_moves = self.state.get_legal_moves()
             shuffle(self.remaining_moves)
 
         # The following are cached for performance.
         self.team = self.state.get_current_team()
+        self.cteam = str(self.team).encode()
         if self.parent is not None:
-            self.rewards[self.parent.team] = 0
+            self.rewards[self.parent.cteam] = 0
         self.sqrtlog_visits = 0
         self.invsqrt_visits = 0
         self.avg_reward = 0
 
-    def apply_rewards(self, rewards:Rewards):
+    @property
+    def state(self) -> GameState: return self.state
+    @property
+    def rewards(self): return self.rewards
+
+    @cython.cdivision(True)
+    cdef apply_rewards(self, map[string,double] crewards):
         """Update this node's visits and rewards, and cache some variables for more efficient UCB calculation."""
         self.visits += 1
 
         self.sqrtlog_visits = sqrt(log(self.visits))
         self.invsqrt_visits = 1 / sqrt(self.visits)
 
-        total_rewards = 0
-        for k,v in rewards.items():
-            if k not in self.rewards:
-                self.rewards[k] = 0
-            self.rewards[k] += v
-            total_rewards += self.rewards[k]
+        cdef pair[string,double] item
+        cdef double total_rewards = 0
+        for item in crewards:
+            if self.rewards.count(item.first) == 0:
+                self.rewards[item.first] = 0
+            self.rewards[item.first] += item.second
+            total_rewards += self.rewards[item.first]
 
         if self.parent is not None:
             # Average reward is (reward for my parent's team - rewards for all other teams) / num visits to this node.
-            self.avg_reward = ((2 * self.rewards[self.parent.team]) - total_rewards) / self.visits
+            self.avg_reward = ((2 * self.rewards[self.parent.cteam]) - total_rewards) / self.visits
 
-    def ucb(self, exploration_bias:float, parent_sqrtlog_visits:float):
+    cdef double ucb(self, double exploration_bias, double parent_sqrtlog_visits):
         """Upper Confidence Bound
         ucb = (x / n) + C * sqrt(ln(N) / n)
         x=reward for this node
         n=number of simulations for this node
         N=number of simulations for parent node
         C=exploration bias
         """
         # ucb = avgR + C * sqrt(ln(N)) * (1/sqrt(n))
         return self.avg_reward + exploration_bias * parent_sqrtlog_visits * self.invsqrt_visits
 
 
-class MCTS:
+cdef class MCTS:
+    cdef double exploration_bias
+
     def __init__(self, exploration_bias:float=1.414):
         """Initializes an MCTS agent.
         Args:
             exploration_bias (float): The exploration bias, which balances exploration (favoring untested moves) and exploitation (favoring good moves).
                 The default √2 is often used in practice. However, the optimal value depends on the game and is usually found by experimentation.
         """
         self.exploration_bias = exploration_bias
 
+    @property
+    def exploration_bias(self) -> float: return self.exploration_bias
+
     def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
         """Searches for this state's best move until some limit has been reached.
         Args:
             state (GameState): The game state for which to find the best move.
             max_time (int|float): The maximum time to search, in seconds.
             max_iterations (int): The maximum number of selections/simulations to perform.
             heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.
@@ -131,18 +162,18 @@
             raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
 
         if max_time is None and max_iterations is None:
             raise ValueError("One or more of max_time/max_iterations is required.")
 
         node = Node(state)
 
+        cdef double end_time
+        cdef int i = 0
         if max_time is not None:
             end_time = time() + max_time
-        if max_iterations is not None:
-            i = 0
 
         while True:
             child = self.select(node)
             rewards = self.simulate(child, heuristic=heuristic)
             self.backpropagate(child, rewards)
 
             # If there is only one legal move, we don't need to search.
@@ -153,49 +184,49 @@
                 if time() >= end_time:
                     break
             if max_iterations is not None:
                 i += 1
                 if i >= max_iterations:
                     break
 
-        best = self.get_best_child(node)
+        cdef Node best = self.get_best_child(node)
 
         if return_type == "state":
             return best.state
         elif return_type == "move":
             return best.move
         elif return_type == "node":
             return best
 
-    def select(self, node:Node) -> Node:
+    cdef Node select(self, Node node):
         """Step 1: Selection
         Traverse the tree for the node we most want to simulate.
         Looks for an unexplored child of this node's best child's best child's...best child.
         """
         while not node.is_terminal:
             if not node.is_fully_expanded:
                 return self.expand(node)
             else:
                 node = self.get_best_child(node)
         return node
 
-    def expand(self, node:Node) -> Node:
+    cdef Node expand(self, Node node):
         """Step 2: Expansion
         Add a new child to this node.
         """
         move = node.remaining_moves.pop()
         if len(node.remaining_moves) == 0:
             node.is_fully_expanded = True
 
-        child = Node(state=node.state.make_move(move), parent=node, move=move)
+        cdef Node child = Node(state=node.state.make_move(move), parent=node, move=move)
         node.children.append(child)
 
         return child
 
-    def simulate(self, node:Node, heuristic=None) -> Rewards:
+    cdef map[string,double] simulate(self, Node node, heuristic=None):
         """Step 3: Simulation (aka playout/rollout)
         Play out a game, from the given node to termination, and return the final reward.
         A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.
         Args:
             node (Node): The node from which to begin the simulation.
             heuristic (callable): A function that takes a state and returns a move.
         """
@@ -213,49 +244,38 @@
                     move = choice(state.get_legal_moves())
                 state = state.make_move(move)
 
         reward = state.get_reward()
         if not isinstance(reward, dict):
             reward = {terminal_team: reward}
 
-        return {k:v for k,v in reward.items() if v!=0}
+        cdef map[string,double] crewards = map[string,double]()
+        for team in reward:
+            if reward[team] == 0:
+                continue
+            crewards[str(team).encode()] = float(reward[team])
+
+        return crewards
 
-    def backpropagate(self, node:Node, rewards:Rewards):
+    cdef backpropagate(self, Node node, map[string,double] crewards):
         """Step 4: Backpropagation
         Update all ancestors with the reward from this terminal node.
         """
         while node is not None:
-            node.apply_rewards(rewards)
+            node.apply_rewards(crewards)
             node = node.parent
 
-    def get_best_child(self, node:Node) -> Node:
+    cdef Node get_best_child(self, Node node):
         """Find the child with the highest Upper Confidence Bound (UCB)."""
-        parent_sqrtlog_visits = node.sqrtlog_visits
-        best_score = float('-inf')
+        cdef double parent_sqrtlog_visits = node.sqrtlog_visits
+        cdef double best_score = -INFINITY
+        cdef double ucb
+        cdef Node child, best_child = node.children[0]
+        cdef pair[string,double] item
 
         for child in node.children:
             ucb = child.ucb(self.exploration_bias, parent_sqrtlog_visits)
             if ucb > best_score:
                 best_score = ucb
                 best_child = child
 
         return best_child
-
-
-if __name__ == "__main__":
-    class Score10(GameState):
-        def __init__(self, player=1, score=-4):
-            self.player = player
-            self.score = score
-        def get_current_team(self): return self.player
-        def get_legal_moves(self): return list(range(-9,10))
-        def make_move(self, move): return Score10(-1*self.player, self.score+move)
-        def is_terminal(self): return abs(self.score) >= 10
-        def get_reward(self): return -1 * self.player * self.score
-        def __repr__(self): return f'{str(self.score).rjust(3)} : {"pos" if self.player==1 else "neg"} to play'
-    mcts = MCTS()
-    state = Score10()
-    while not state.is_terminal():
-        move = mcts.search(state, max_iterations=100, return_type="move")
-        print(state, f'(chose {move})')
-        state = state.make_move(move)
-    print(state)
```

### Comparing `multimcts-0.4.1/multimcts.egg-info/PKG-INFO` & `multimcts-0.4.2/multimcts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.4.1
+Version: 0.4.2
 Summary: Monte Carlo Tree Search for multiple teams
 Home-page: https://github.com/taylorvance/multimcts
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `multimcts-0.4.1/setup.py` & `multimcts-0.4.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
 setup(
     name='multimcts',
-    version='0.4.1',
+    version='0.4.2',
     description='Monte Carlo Tree Search for multiple teams',
     author='Taylor Vance',
     author_email='mirrors.cities0w@icloud.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/taylorvance/multimcts',
```

