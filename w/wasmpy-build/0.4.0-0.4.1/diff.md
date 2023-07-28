# Comparing `tmp/wasmpy-build-0.4.0.tar.gz` & `tmp/wasmpy-build-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.4.0.tar", last modified: Thu Jul 27 17:30:23 2023, max compression
+gzip compressed data, was "wasmpy-build-0.4.1.tar", last modified: Fri Jul 28 12:09:45 2023, max compression
```

## Comparing `wasmpy-build-0.4.0.tar` & `wasmpy-build-0.4.1.tar`

### file list

```diff
@@ -1,681 +1,681 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:23.345973 wasmpy-build-0.4.0/
--rw-rw-rw-   0        0        0     1068 2023-07-13 12:38:30.000000 wasmpy-build-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1741 2023-07-27 17:30:23.345973 wasmpy-build-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-07-27 17:22:55.000000 wasmpy-build-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 17:30:23.346973 wasmpy-build-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1389 2023-07-27 17:25:08.000000 wasmpy-build-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.182128 wasmpy-build-0.4.0/wasmpy_build/
--rw-rw-rw-   0        0        0     3012 2023-07-27 17:19:32.000000 wasmpy-build-0.4.0/wasmpy_build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.178587 wasmpy-build-0.4.0/wasmpy_build/include/
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.318980 wasmpy-build-0.4.0/wasmpy_build/include/cp310/
--rw-rw-rw-   0        0        0    13936 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/LICENSE
--rw-rw-rw-   0        0        0     3224 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/Python.h
--rw-rw-rw-   0        0        0      344 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/README.rst
--rw-rw-rw-   0        0        0    31279 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/abstract.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/bltinmodule.h
--rw-rw-rw-   0        0        0     1222 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/boolobject.h
--rw-rw-rw-   0        0        0     1480 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/bytearrayobject.h
--rw-rw-rw-   0        0        0     2581 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/bytesobject.h
--rw-rw-rw-   0        0        0      716 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cellobject.h
--rw-rw-rw-   0        0        0     5665 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/ceval.h
--rw-rw-rw-   0        0        0     1647 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/classobject.h
--rw-rw-rw-   0        0        0      318 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/code.h
--rw-rw-rw-   0        0        0     7029 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/codecs.h
--rw-rw-rw-   0        0        0      520 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/compile.h
--rw-rw-rw-   0        0        0     1802 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/complexobject.h
--rw-rw-rw-   0        0        0     1950 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/context.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.361417 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/
--rw-rw-rw-   0        0        0    14054 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4119 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1468 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/ceval.h
--rw-rw-rw-   0        0        0     7570 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/compile.h
--rw-rw-rw-   0        0        0     3734 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/dictobject.h
--rw-rw-rw-   0        0        0      723 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4267 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3152 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1630 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/import.h
--rw-rw-rw-   0        0        0     7597 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/initconfig.h
--rw-rw-rw-   0        0        0      387 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1243 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19613 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/object.h
--rw-rw-rw-   0        0        0     3356 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     1387 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pydebug.h
--rw-rw-rw-   0        0        0     5476 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pyfpe.h
--rw-rw-rw-   0        0        0     2095 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pymem.h
--rw-rw-rw-   0        0        0    11914 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     9196 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pytime.h
--rw-rw-rw-   0        0        0      506 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      404 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/traceback.h
--rw-rw-rw-   0        0        0      975 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    44284 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9635 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/datetime.h
--rw-rw-rw-   0        0        0     2988 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/descrobject.h
--rw-rw-rw-   0        0        0     3835 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/errcode.h
--rw-rw-rw-   0        0        0      825 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/eval.h
--rw-rw-rw-   0        0        0     1098 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/exports.h
--rw-rw-rw-   0        0        0     1567 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/fileobject.h
--rw-rw-rw-   0        0        0      510 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/fileutils.h
--rw-rw-rw-   0        0        0     4354 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/frameobject.h
--rw-rw-rw-   0        0        0     4233 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/funcobject.h
--rw-rw-rw-   0        0        0      332 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/genericaliasobject.h
--rw-rw-rw-   0        0        0     3339 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/genobject.h
--rw-rw-rw-   0        0        0     2992 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/import.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.431056 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/
--rw-rw-rw-   0        0        0      479 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1122 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     2971 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    28828 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6457 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16979 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     5271 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0      864 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3484 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      696 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1040 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2809 2023-07-27 16:44:11.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      822 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_context.h
--rw-rw-rw-   0        0        0      648 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1703 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      480 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_format.h
--rw-rw-rw-   0        0        0     6859 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4185 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      346 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5613 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     9286 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      350 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_list.h
--rw-rw-rw-   0        0        0     2589 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1047 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0     5989 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_object.h
--rw-rw-rw-   0        0        0      626 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_parser.h
--rw-rw-rw-   0        0        0     1981 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2736 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2308 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     4939 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3211 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3925 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4902 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      386 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5569 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      548 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     2966 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      423 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0      898 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0      629 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      633 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-27 16:44:11.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/interpreteridobject.h
--rw-rw-rw-   0        0        0      775 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/intrcheck.h
--rw-rw-rw-   0        0        0      589 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/iterobject.h
--rw-rw-rw-   0        0        0     1773 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/listobject.h
--rw-rw-rw-   0        0        0     3791 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/longintrepr.h
--rw-rw-rw-   0        0        0     8575 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/longobject.h
--rw-rw-rw-   0        0        0      795 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/marshal.h
--rw-rw-rw-   0        0        0     2756 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/memoryobject.h
--rw-rw-rw-   0        0        0     4137 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/methodobject.h
--rw-rw-rw-   0        0        0    10303 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/modsupport.h
--rw-rw-rw-   0        0        0     2430 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/moduleobject.h
--rw-rw-rw-   0        0        0      347 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/namespaceobject.h
--rw-rw-rw-   0        0        0    28318 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/object.h
--rw-rw-rw-   0        0        0     8425 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/objimpl.h
--rw-rw-rw-   0        0        0     5509 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/osdefs.h
--rw-rw-rw-   0        0        0      289 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/osmodule.h
--rw-rw-rw-   0        0        0     1301 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/patchlevel.h
--rw-rw-rw-   0        0        0     2474 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/py_curses.h
--rw-rw-rw-   0        0        0     1725 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pycapsule.h
--rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyconfig.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pydtrace.h
--rw-rw-rw-   0        0        0    12360 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyexpat.h
--rw-rw-rw-   0        0        0      460 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyframe.h
--rw-rw-rw-   0        0        0     4216 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyhash.h
--rw-rw-rw-   0        0        0     2047 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymacro.h
--rw-rw-rw-   0        0        0     8313 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymath.h
--rw-rw-rw-   0        0        0     3897 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymem.h
--rw-rw-rw-   0        0        0    31798 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyport.h
--rw-rw-rw-   0        0        0     5176 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystrcmp.h
--rw-rw-rw-   0        0        0      845 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystrtod.h
--rw-rw-rw-   0        0        0     1108 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pythonrun.h
--rw-rw-rw-   0        0        0     5939 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/pythread.h
--rw-rw-rw-   0        0        0      628 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/rangeobject.h
--rw-rw-rw-   0        0        0     3375 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/setobject.h
--rw-rw-rw-   0        0        0     2512 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/sliceobject.h
--rw-rw-rw-   0        0        0     2072 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/structmember.h
--rw-rw-rw-   0        0        0     1382 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/structseq.h
--rw-rw-rw-   0        0        0     1238 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/token.h
--rw-rw-rw-   0        0        0      584 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/traceback.h
--rw-rw-rw-   0        0        0     1113 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/tracemalloc.h
--rw-rw-rw-   0        0        0     1606 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/tupleobject.h
--rw-rw-rw-   0        0        0     2460 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/typeslots.h
--rw-rw-rw-   0        0        0    36074 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/unicodeobject.h
--rw-rw-rw-   0        0        0     1775 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/warnings.h
--rw-rw-rw-   0        0        0     2857 2023-07-27 17:26:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp310/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.526593 wasmpy-build-0.4.0/wasmpy_build/include/cp311/
--rw-rw-rw-   0        0        0    13936 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/LICENSE
--rw-rw-rw-   0        0        0     2854 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/Python.h
--rw-rw-rw-   0        0        0      344 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/README.rst
--rw-rw-rw-   0        0        0    32615 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/abstract.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/bltinmodule.h
--rw-rw-rw-   0        0        0     1210 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/boolobject.h
--rw-rw-rw-   0        0        0     1458 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/bytearrayobject.h
--rw-rw-rw-   0        0        0     2605 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/bytesobject.h
--rw-rw-rw-   0        0        0     6213 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/ceval.h
--rw-rw-rw-   0        0        0     7029 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/codecs.h
--rw-rw-rw-   0        0        0      520 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/compile.h
--rw-rw-rw-   0        0        0      722 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/complexobject.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.586590 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/
--rw-rw-rw-   0        0        0     8229 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/abstract.h
--rw-rw-rw-   0        0        0     1305 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4568 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/bytesobject.h
--rw-rw-rw-   0        0        0      723 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/cellobject.h
--rw-rw-rw-   0        0        0     1239 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/ceval.h
--rw-rw-rw-   0        0        0     1656 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/classobject.h
--rw-rw-rw-   0        0        0    11484 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/compile.h
--rw-rw-rw-   0        0        0     1248 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/complexobject.h
--rw-rw-rw-   0        0        0     1959 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/context.h
--rw-rw-rw-   0        0        0     1642 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/descrobject.h
--rw-rw-rw-   0        0        0     3324 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/dictobject.h
--rw-rw-rw-   0        0        0      818 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/fileobject.h
--rw-rw-rw-   0        0        0      232 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/fileutils.h
--rw-rw-rw-   0        0        0      702 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/floatobject.h
--rw-rw-rw-   0        0        0     1108 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/frameobject.h
--rw-rw-rw-   0        0        0     4424 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/funcobject.h
--rw-rw-rw-   0        0        0     3279 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/genobject.h
--rw-rw-rw-   0        0        0     1526 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/import.h
--rw-rw-rw-   0        0        0     7817 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/initconfig.h
--rw-rw-rw-   0        0        0     1769 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/listobject.h
--rw-rw-rw-   0        0        0     3817 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/longintrepr.h
--rw-rw-rw-   0        0        0     4532 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/longobject.h
--rw-rw-rw-   0        0        0     2556 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/methodobject.h
--rw-rw-rw-   0        0        0     4234 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/modsupport.h
--rw-rw-rw-   0        0        0    18305 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/object.h
--rw-rw-rw-   0        0        0     2998 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     3505 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pthread_stubs.h
--rw-rw-rw-   0        0        0     1387 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1073 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pydebug.h
--rw-rw-rw-   0        0        0     4522 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyfpe.h
--rw-rw-rw-   0        0        0      582 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyframe.h
--rw-rw-rw-   0        0        0     2099 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pymem.h
--rw-rw-rw-   0        0        0    14351 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     1426 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pythread.h
--rw-rw-rw-   0        0        0    12158 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pytime.h
--rw-rw-rw-   0        0        0     1997 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/setobject.h
--rw-rw-rw-   0        0        0      489 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      444 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/traceback.h
--rw-rw-rw-   0        0        0     1513 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    41910 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0      560 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/warnings.h
--rw-rw-rw-   0        0        0     2103 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/weakrefobject.h
--rw-rw-rw-   0        0        0     9635 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/datetime.h
--rw-rw-rw-   0        0        0     1244 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/descrobject.h
--rw-rw-rw-   0        0        0     3834 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/errcode.h
--rw-rw-rw-   0        0        0     1098 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/exports.h
--rw-rw-rw-   0        0        0     1566 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/fileobject.h
--rw-rw-rw-   0        0        0      509 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/fileutils.h
--rw-rw-rw-   0        0        0     1527 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/floatobject.h
--rw-rw-rw-   0        0        0      336 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/frameobject.h
--rw-rw-rw-   0        0        0      332 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/genericaliasobject.h
--rw-rw-rw-   0        0        0     2991 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/import.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.686125 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/
--rw-rw-rw-   0        0        0      611 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1122 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     3031 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    29315 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6535 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16979 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     6062 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     1424 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
--rw-rw-rw-   0        0        0     3469 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_call.h
--rw-rw-rw-   0        0        0     4409 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0    15923 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1040 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2839 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0     1239 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_context.h
--rw-rw-rw-   0        0        0     5684 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_dict.h
--rw-rw-rw-   0        0        0      706 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0      562 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
--rw-rw-rw-   0        0        0      842 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_exceptions.h
--rw-rw-rw-   0        0        0     7320 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     1307 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_floatobject.h
--rw-rw-rw-   0        0        0      480 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_format.h
--rw-rw-rw-   0        0        0     7567 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_frame.h
--rw-rw-rw-   0        0        0      413 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_function.h
--rw-rw-rw-   0        0        0     6895 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_gc.h
--rw-rw-rw-   0        0        0     1164 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_genobject.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     1436 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_global_objects.h
--rw-rw-rw-   0        0        0    12980 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_global_strings.h
--rw-rw-rw-   0        0        0     3696 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4185 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      743 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5787 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     6660 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      546 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
--rw-rw-rw-   0        0        0     1352 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_list.h
--rw-rw-rw-   0        0        0     3519 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1040 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0      390 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_namespace.h
--rw-rw-rw-   0        0        0    10035 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_object.h
--rw-rw-rw-   0        0        0    18986 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_opcode.h
--rw-rw-rw-   0        0        0      626 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_parser.h
--rw-rw-rw-   0        0        0      606 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2736 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2483 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3505 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     9435 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pymath.h
--rw-rw-rw-   0        0        0     3708 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     4100 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     5988 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0    49092 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
--rw-rw-rw-   0        0        0      937 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_signal.h
--rw-rw-rw-   0        0        0      336 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
--rw-rw-rw-   0        0        0      933 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_strhex.h
--rw-rw-rw-   0        0        0      574 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5629 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      605 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3497 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0     2089 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0     1158 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_typeobject.h
--rw-rw-rw-   0        0        0      898 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0     1716 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
--rw-rw-rw-   0        0        0      678 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      739 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      775 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/intrcheck.h
--rw-rw-rw-   0        0        0      589 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/iterobject.h
--rw-rw-rw-   0        0        0     1772 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/listobject.h
--rw-rw-rw-   0        0        0     3254 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/longobject.h
--rw-rw-rw-   0        0        0      819 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/marshal.h
--rw-rw-rw-   0        0        0     2802 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/memoryobject.h
--rw-rw-rw-   0        0        0     5062 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/methodobject.h
--rw-rw-rw-   0        0        0     6438 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/modsupport.h
--rw-rw-rw-   0        0        0     2353 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/moduleobject.h
--rw-rw-rw-   0        0        0    29768 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/object.h
--rw-rw-rw-   0        0        0     8408 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/objimpl.h
--rw-rw-rw-   0        0        0    11187 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/osdefs.h
--rw-rw-rw-   0        0        0      289 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/osmodule.h
--rw-rw-rw-   0        0        0     1299 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/patchlevel.h
--rw-rw-rw-   0        0        0     2471 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/py_curses.h
--rw-rw-rw-   0        0        0     5117 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pybuffer.h
--rw-rw-rw-   0        0        0     1725 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pycapsule.h
--rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyconfig.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pydtrace.h
--rw-rw-rw-   0        0        0    12715 2023-07-27 17:26:17.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyexpat.h
--rw-rw-rw-   0        0        0      545 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyframe.h
--rw-rw-rw-   0        0        0     4147 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyhash.h
--rw-rw-rw-   0        0        0     2216 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymacconfig.h
--rw-rw-rw-   0        0        0     6064 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymacro.h
--rw-rw-rw-   0        0        0     1979 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymath.h
--rw-rw-rw-   0        0        0     3896 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymem.h
--rw-rw-rw-   0        0        0    24642 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyport.h
--rw-rw-rw-   0        0        0     4561 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pystrcmp.h
--rw-rw-rw-   0        0        0     1557 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pystrtod.h
--rw-rw-rw-   0        0        0     1187 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pythonrun.h
--rw-rw-rw-   0        0        0     4834 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pythread.h
--rw-rw-rw-   0        0        0      851 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/pytypedefs.h
--rw-rw-rw-   0        0        0      628 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/rangeobject.h
--rw-rw-rw-   0        0        0     1537 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/setobject.h
--rw-rw-rw-   0        0        0     2512 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/sliceobject.h
--rw-rw-rw-   0        0        0     2038 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/structmember.h
--rw-rw-rw-   0        0        0     1380 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/structseq.h
--rw-rw-rw-   0        0        0     1377 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-07-27 17:26:07.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/token.h
--rw-rw-rw-   0        0        0      583 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/traceback.h
--rw-rw-rw-   0        0        0     1113 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/tracemalloc.h
--rw-rw-rw-   0        0        0     1605 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/tupleobject.h
--rw-rw-rw-   0        0        0     2342 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/typeslots.h
--rw-rw-rw-   0        0        0    35958 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/unicodeobject.h
--rw-rw-rw-   0        0        0     1129 2023-07-27 17:26:13.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/warnings.h
--rw-rw-rw-   0        0        0     1220 2023-07-27 17:26:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp311/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.905180 wasmpy-build-0.4.0/wasmpy_build/include/cp38/
--rw-rw-rw-   0        0        0    13937 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/LICENSE
--rw-rw-rw-   0        0        0    26491 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/Python-ast.h
--rw-rw-rw-   0        0        0     3615 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/Python.h
--rw-rw-rw-   0        0        0    30164 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/abstract.h
--rw-rw-rw-   0        0        0     1229 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/asdl.h
--rw-rw-rw-   0        0        0      944 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/ast.h
--rw-rw-rw-   0        0        0      468 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/bitset.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/bltinmodule.h
--rw-rw-rw-   0        0        0      884 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/boolobject.h
--rw-rw-rw-   0        0        0     2110 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytearrayobject.h
--rw-rw-rw-   0        0        0     3301 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytes_methods.h
--rw-rw-rw-   0        0        0     8485 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytesobject.h
--rw-rw-rw-   0        0        0      709 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cellobject.h
--rw-rw-rw-   0        0        0     8320 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/ceval.h
--rw-rw-rw-   0        0        0     1700 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/classobject.h
--rw-rw-rw-   0        0        0     7158 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/code.h
--rw-rw-rw-   0        0        0     6751 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/codecs.h
--rw-rw-rw-   0        0        0     3543 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/compile.h
--rw-rw-rw-   0        0        0     1803 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/complexobject.h
--rw-rw-rw-   0        0        0     2002 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/context.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.932380 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/
--rw-rw-rw-   0        0        0    12294 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/abstract.h
--rw-rw-rw-   0        0        0     3845 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/fileobject.h
--rw-rw-rw-   0        0        0    16028 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0    15691 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/object.h
--rw-rw-rw-   0        0        0     3600 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/objimpl.h
--rw-rw-rw-   0        0        0     4717 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2263 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pymem.h
--rw-rw-rw-   0        0        0     9810 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pystate.h
--rw-rw-rw-   0        0        0      547 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46308 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9260 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/datetime.h
--rw-rw-rw-   0        0        0     3005 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/descrobject.h
--rw-rw-rw-   0        0        0     3700 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/dictobject.h
--rw-rw-rw-   0        0        0      460 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/dtoa.h
--rw-rw-rw-   0        0        0    22469 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/enumobject.h
--rw-rw-rw-   0        0        0     1695 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/errcode.h
--rw-rw-rw-   0        0        0     1201 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/eval.h
--rw-rw-rw-   0        0        0     1567 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/fileobject.h
--rw-rw-rw-   0        0        0     4363 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/fileutils.h
--rw-rw-rw-   0        0        0     4788 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/floatobject.h
--rw-rw-rw-   0        0        0     3304 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/frameobject.h
--rw-rw-rw-   0        0        0     4174 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/funcobject.h
--rw-rw-rw-   0        0        0     3710 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/grammar.h
--rw-rw-rw-   0        0        0     4882 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/import.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.977380 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/
--rw-rw-rw-   0        0        0     1122 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16944 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0      966 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      542 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      779 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_context.h
--rw-rw-rw-   0        0        0     1254 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1520 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3698 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     5207 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     1548 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_long.h
--rw-rw-rw-   0        0        0     2896 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_object.h
--rw-rw-rw-   0        0        0     2037 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     1327 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3814 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     8217 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     9578 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     3072 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      416 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      591 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/interpreteridobject.h
--rw-rw-rw-   0        0        0      864 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/intrcheck.h
--rw-rw-rw-   0        0        0      563 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/iterobject.h
--rw-rw-rw-   0        0        0     2917 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/listobject.h
--rw-rw-rw-   0        0        0     3791 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/longintrepr.h
--rw-rw-rw-   0        0        0     9483 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/longobject.h
--rw-rw-rw-   0        0        0      795 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/marshal.h
--rw-rw-rw-   0        0        0     2757 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/memoryobject.h
--rw-rw-rw-   0        0        0     4394 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/methodobject.h
--rw-rw-rw-   0        0        0     9564 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/modsupport.h
--rw-rw-rw-   0        0        0     2334 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/moduleobject.h
--rw-rw-rw-   0        0        0      347 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/namespaceobject.h
--rw-rw-rw-   0        0        0     1330 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/node.h
--rw-rw-rw-   0        0        0    29576 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/object.h
--rw-rw-rw-   0        0        0    10517 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/objimpl.h
--rw-rw-rw-   0        0        0     1298 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/odictobject.h
--rw-rw-rw-   0        0        0     5164 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/osdefs.h
--rw-rw-rw-   0        0        0      289 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/osmodule.h
--rw-rw-rw-   0        0        0     2976 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/parsetok.h
--rw-rw-rw-   0        0        0     1299 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/patchlevel.h
--rw-rw-rw-   0        0        0      836 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/picklebufobject.h
--rw-rw-rw-   0        0        0     2477 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/py_curses.h
--rw-rw-rw-   0        0        0     2745 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyarena.h
--rw-rw-rw-   0        0        0     1726 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pycapsule.h
--rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyconfig.h
--rw-rw-rw-   0        0        0     1387 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyctype.h
--rw-rw-rw-   0        0        0     1214 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydtrace.h
--rw-rw-rw-   0        0        0    12720 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyexpat.h
--rw-rw-rw-   0        0        0      341 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyfpe.h
--rw-rw-rw-   0        0        0     4133 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyhash.h
--rw-rw-rw-   0        0        0     2048 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymacconfig.h
--rw-rw-rw-   0        0        0     3778 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymacro.h
--rw-rw-rw-   0        0        0     8312 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymath.h
--rw-rw-rw-   0        0        0     5410 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymem.h
--rw-rw-rw-   0        0        0    30362 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyport.h
--rw-rw-rw-   0        0        0     4641 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystrcmp.h
--rw-rw-rw-   0        0        0      845 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystrtod.h
--rw-rw-rw-   0        0        0     7560 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pythonrun.h
--rw-rw-rw-   0        0        0     5661 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pythread.h
--rw-rw-rw-   0        0        0     8922 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/pytime.h
--rw-rw-rw-   0        0        0      629 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/rangeobject.h
--rw-rw-rw-   0        0        0     3356 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/setobject.h
--rw-rw-rw-   0        0        0     2513 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/sliceobject.h
--rw-rw-rw-   0        0        0     2028 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/structmember.h
--rw-rw-rw-   0        0        0     1369 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/structseq.h
--rw-rw-rw-   0        0        0     5281 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/symtable.h
--rw-rw-rw-   0        0        0     1238 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/sysmodule.h
--rw-rw-rw-   0        0        0     2429 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/token.h
--rw-rw-rw-   0        0        0      601 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/traceback.h
--rw-rw-rw-   0        0        0     1113 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/tracemalloc.h
--rw-rw-rw-   0        0        0     1653 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/tupleobject.h
--rw-rw-rw-   0        0        0     2253 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/ucnhash.h
--rw-rw-rw-   0        0        0    35664 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/unicodeobject.h
--rw-rw-rw-   0        0        0     1775 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/warnings.h
--rw-rw-rw-   0        0        0     2860 2023-07-27 17:26:25.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp38/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:23.213448 wasmpy-build-0.4.0/wasmpy_build/include/cp39/
--rw-rw-rw-   0        0        0    13937 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/LICENSE
--rw-rw-rw-   0        0        0    26193 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/Python-ast.h
--rw-rw-rw-   0        0        0     3532 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/Python.h
--rw-rw-rw-   0        0        0    30352 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/abstract.h
--rw-rw-rw-   0        0        0     1224 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/asdl.h
--rw-rw-rw-   0        0        0      943 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/ast.h
--rw-rw-rw-   0        0        0      468 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/bitset.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/bltinmodule.h
--rw-rw-rw-   0        0        0      883 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/boolobject.h
--rw-rw-rw-   0        0        0     1480 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/bytearrayobject.h
--rw-rw-rw-   0        0        0     3036 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/bytesobject.h
--rw-rw-rw-   0        0        0      708 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cellobject.h
--rw-rw-rw-   0        0        0     5916 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/ceval.h
--rw-rw-rw-   0        0        0     1647 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/classobject.h
--rw-rw-rw-   0        0        0      318 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/code.h
--rw-rw-rw-   0        0        0     6751 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/codecs.h
--rw-rw-rw-   0        0        0     3739 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/compile.h
--rw-rw-rw-   0        0        0     1802 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/complexobject.h
--rw-rw-rw-   0        0        0     1950 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/context.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:23.265430 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/
--rw-rw-rw-   0        0        0    14200 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4114 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1537 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/ceval.h
--rw-rw-rw-   0        0        0     6989 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/code.h
--rw-rw-rw-   0        0        0     3797 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4004 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3059 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1473 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/import.h
--rw-rw-rw-   0        0        0    16979 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1364 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19358 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/object.h
--rw-rw-rw-   0        0        0     4456 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/objimpl.h
--rw-rw-rw-   0        0        0     5101 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2096 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pymem.h
--rw-rw-rw-   0        0        0    10134 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pystate.h
--rw-rw-rw-   0        0        0      575 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46154 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9255 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/datetime.h
--rw-rw-rw-   0        0        0     3005 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/descrobject.h
--rw-rw-rw-   0        0        0     3699 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/dictobject.h
--rw-rw-rw-   0        0        0    22469 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/enumobject.h
--rw-rw-rw-   0        0        0     1624 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/errcode.h
--rw-rw-rw-   0        0        0     1201 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/eval.h
--rw-rw-rw-   0        0        0     1098 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/exports.h
--rw-rw-rw-   0        0        0     1567 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/fileobject.h
--rw-rw-rw-   0        0        0      602 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/fileutils.h
--rw-rw-rw-   0        0        0     4354 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/frameobject.h
--rw-rw-rw-   0        0        0     4033 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/funcobject.h
--rw-rw-rw-   0        0        0      332 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/genericaliasobject.h
--rw-rw-rw-   0        0        0     3515 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/grammar.h
--rw-rw-rw-   0        0        0     2992 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/import.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:23.342980 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/
--rw-rw-rw-   0        0        0      953 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pegen_interface.h
--rw-rw-rw-   0        0        0      479 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1122 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16977 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     3384 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     2620 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_byteswap.h
--rw-rw-rw-   0        0        0      864 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3403 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      541 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      800 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_context.h
--rw-rw-rw-   0        0        0      648 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1541 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     6647 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-27 17:26:26.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4185 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      471 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5222 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     5296 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_interp.h
--rw-rw-rw-   0        0        0     1548 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_long.h
--rw-rw-rw-   0        0        0     4157 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_object.h
--rw-rw-rw-   0        0        0     1936 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2026 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3740 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3363 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3576 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4452 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      548 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3052 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      440 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      633 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-27 17:26:19.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/interpreteridobject.h
--rw-rw-rw-   0        0        0      864 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/intrcheck.h
--rw-rw-rw-   0        0        0      517 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/iterobject.h
--rw-rw-rw-   0        0        0     1773 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/listobject.h
--rw-rw-rw-   0        0        0     3791 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/longintrepr.h
--rw-rw-rw-   0        0        0     9476 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/longobject.h
--rw-rw-rw-   0        0        0      795 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/marshal.h
--rw-rw-rw-   0        0        0     2756 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/memoryobject.h
--rw-rw-rw-   0        0        0     3767 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/methodobject.h
--rw-rw-rw-   0        0        0     9932 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/modsupport.h
--rw-rw-rw-   0        0        0     2333 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/moduleobject.h
--rw-rw-rw-   0        0        0      347 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/namespaceobject.h
--rw-rw-rw-   0        0        0     1283 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/node.h
--rw-rw-rw-   0        0        0    24604 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/object.h
--rw-rw-rw-   0        0        0     8403 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/objimpl.h
--rw-rw-rw-   0        0        0     1297 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/odictobject.h
--rw-rw-rw-   0        0        0     4900 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/osdefs.h
--rw-rw-rw-   0        0        0      289 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/osmodule.h
--rw-rw-rw-   0        0        0     2976 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/parsetok.h
--rw-rw-rw-   0        0        0     1299 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/patchlevel.h
--rw-rw-rw-   0        0        0      835 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/picklebufobject.h
--rw-rw-rw-   0        0        0     2474 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/py_curses.h
--rw-rw-rw-   0        0        0     2745 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyarena.h
--rw-rw-rw-   0        0        0     1725 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pycapsule.h
--rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyconfig.h
--rw-rw-rw-   0        0        0     1387 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydtrace.h
--rw-rw-rw-   0        0        0    12361 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyexpat.h
--rw-rw-rw-   0        0        0      444 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyfpe.h
--rw-rw-rw-   0        0        0      460 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyframe.h
--rw-rw-rw-   0        0        0     4256 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyhash.h
--rw-rw-rw-   0        0        0     2103 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymacro.h
--rw-rw-rw-   0        0        0     8580 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymath.h
--rw-rw-rw-   0        0        0     4410 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymem.h
--rw-rw-rw-   0        0        0    31387 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyport.h
--rw-rw-rw-   0        0        0     5176 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystrcmp.h
--rw-rw-rw-   0        0        0      845 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystrtod.h
--rw-rw-rw-   0        0        0     7588 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pythonrun.h
--rw-rw-rw-   0        0        0     5939 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pythread.h
--rw-rw-rw-   0        0        0     8924 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/pytime.h
--rw-rw-rw-   0        0        0      628 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/rangeobject.h
--rw-rw-rw-   0        0        0     3318 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/setobject.h
--rw-rw-rw-   0        0        0     2512 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/sliceobject.h
--rw-rw-rw-   0        0        0     2028 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/structmember.h
--rw-rw-rw-   0        0        0     1382 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/structseq.h
--rw-rw-rw-   0        0        0     5280 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/symtable.h
--rw-rw-rw-   0        0        0     1238 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/sysmodule.h
--rw-rw-rw-   0        0        0     2642 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/token.h
--rw-rw-rw-   0        0        0      584 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/traceback.h
--rw-rw-rw-   0        0        0     1113 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/tracemalloc.h
--rw-rw-rw-   0        0        0     1606 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/tupleobject.h
--rw-rw-rw-   0        0        0     2350 2023-07-27 17:26:27.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-07-27 17:26:20.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/ucnhash.h
--rw-rw-rw-   0        0        0    35358 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/unicodeobject.h
--rw-rw-rw-   0        0        0     1775 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/warnings.h
--rw-rw-rw-   0        0        0     2857 2023-07-27 17:26:30.000000 wasmpy-build-0.4.0/wasmpy_build/include/cp39/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-27 17:30:22.200728 wasmpy-build-0.4.0/wasmpy_build.egg-info/
--rw-rw-rw-   0        0        0     1741 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    28898 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-27 17:30:22.000000 wasmpy-build-0.4.0/wasmpy_build.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.443723 wasmpy-build-0.4.1/
+-rw-rw-rw-   0        0        0     1068 2023-07-13 12:38:30.000000 wasmpy-build-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1741 2023-07-28 12:09:45.442732 wasmpy-build-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-07-27 17:22:55.000000 wasmpy-build-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:09:45.443723 wasmpy-build-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2023-07-28 12:06:45.000000 wasmpy-build-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.287963 wasmpy-build-0.4.1/wasmpy_build/
+-rw-rw-rw-   0        0        0     3012 2023-07-27 17:19:32.000000 wasmpy-build-0.4.1/wasmpy_build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.282165 wasmpy-build-0.4.1/wasmpy_build/include/
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.672872 wasmpy-build-0.4.1/wasmpy_build/include/cp310/
+-rw-rw-rw-   0        0        0    13936 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/LICENSE
+-rw-rw-rw-   0        0        0     3224 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/README.rst
+-rw-rw-rw-   0        0        0    31279 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/bltinmodule.h
+-rw-rw-rw-   0        0        0     1222 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/boolobject.h
+-rw-rw-rw-   0        0        0     1480 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2581 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/bytesobject.h
+-rw-rw-rw-   0        0        0      716 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cellobject.h
+-rw-rw-rw-   0        0        0     5665 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/ceval.h
+-rw-rw-rw-   0        0        0     1647 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/code.h
+-rw-rw-rw-   0        0        0     7029 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/compile.h
+-rw-rw-rw-   0        0        0     1802 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/complexobject.h
+-rw-rw-rw-   0        0        0     1950 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/context.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.843706 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/
+-rw-rw-rw-   0        0        0    14054 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4119 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1468 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/ceval.h
+-rw-rw-rw-   0        0        0     7570 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/compile.h
+-rw-rw-rw-   0        0        0     3734 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4267 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3152 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1630 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/import.h
+-rw-rw-rw-   0        0        0     7597 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      387 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1243 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19613 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/object.h
+-rw-rw-rw-   0        0        0     3356 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     1387 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     5476 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0     2095 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pymem.h
+-rw-rw-rw-   0        0        0    11914 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     9196 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pytime.h
+-rw-rw-rw-   0        0        0      506 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      404 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/traceback.h
+-rw-rw-rw-   0        0        0      975 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    44284 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/datetime.h
+-rw-rw-rw-   0        0        0     2988 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/descrobject.h
+-rw-rw-rw-   0        0        0     3835 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/errcode.h
+-rw-rw-rw-   0        0        0      825 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/exports.h
+-rw-rw-rw-   0        0        0     1567 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/fileobject.h
+-rw-rw-rw-   0        0        0      510 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/fileutils.h
+-rw-rw-rw-   0        0        0     4354 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/frameobject.h
+-rw-rw-rw-   0        0        0     4233 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/funcobject.h
+-rw-rw-rw-   0        0        0      332 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3339 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/genobject.h
+-rw-rw-rw-   0        0        0     2992 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/import.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.939454 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/
+-rw-rw-rw-   0        0        0      479 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1122 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     2971 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    28828 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6457 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     5271 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0      864 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3484 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      696 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1040 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2809 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      822 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      648 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1703 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      480 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     6859 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4185 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      346 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5613 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     9286 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      350 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     2589 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1047 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0     5989 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_object.h
+-rw-rw-rw-   0        0        0      626 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0     1981 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2736 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2308 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     4939 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3211 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3925 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4902 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      386 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5569 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      548 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     2966 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      423 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0      898 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0      629 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/interpreteridobject.h
+-rw-rw-rw-   0        0        0      775 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/intrcheck.h
+-rw-rw-rw-   0        0        0      589 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/iterobject.h
+-rw-rw-rw-   0        0        0     1773 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/listobject.h
+-rw-rw-rw-   0        0        0     3791 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/longintrepr.h
+-rw-rw-rw-   0        0        0     8575 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/longobject.h
+-rw-rw-rw-   0        0        0      795 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/marshal.h
+-rw-rw-rw-   0        0        0     2756 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/memoryobject.h
+-rw-rw-rw-   0        0        0     4137 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/methodobject.h
+-rw-rw-rw-   0        0        0    10303 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/modsupport.h
+-rw-rw-rw-   0        0        0     2430 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/moduleobject.h
+-rw-rw-rw-   0        0        0      347 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/namespaceobject.h
+-rw-rw-rw-   0        0        0    28318 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/object.h
+-rw-rw-rw-   0        0        0     8425 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/objimpl.h
+-rw-rw-rw-   0        0        0     5509 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/osdefs.h
+-rw-rw-rw-   0        0        0      289 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/osmodule.h
+-rw-rw-rw-   0        0        0     1301 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/patchlevel.h
+-rw-rw-rw-   0        0        0     2474 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/py_curses.h
+-rw-rw-rw-   0        0        0     1725 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pydtrace.h
+-rw-rw-rw-   0        0        0    12360 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyexpat.h
+-rw-rw-rw-   0        0        0      460 2023-07-28 12:08:04.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyframe.h
+-rw-rw-rw-   0        0        0     4216 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyhash.h
+-rw-rw-rw-   0        0        0     2047 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymacro.h
+-rw-rw-rw-   0        0        0     8313 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymath.h
+-rw-rw-rw-   0        0        0     3897 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymem.h
+-rw-rw-rw-   0        0        0    31798 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyport.h
+-rw-rw-rw-   0        0        0     5176 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystrcmp.h
+-rw-rw-rw-   0        0        0      845 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystrtod.h
+-rw-rw-rw-   0        0        0     1108 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pythonrun.h
+-rw-rw-rw-   0        0        0     5939 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/pythread.h
+-rw-rw-rw-   0        0        0      628 2023-07-27 17:26:27.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/rangeobject.h
+-rw-rw-rw-   0        0        0     3375 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/setobject.h
+-rw-rw-rw-   0        0        0     2512 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/sliceobject.h
+-rw-rw-rw-   0        0        0     2072 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/structmember.h
+-rw-rw-rw-   0        0        0     1382 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/structseq.h
+-rw-rw-rw-   0        0        0     1238 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/traceback.h
+-rw-rw-rw-   0        0        0     1113 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/tracemalloc.h
+-rw-rw-rw-   0        0        0     1606 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/tupleobject.h
+-rw-rw-rw-   0        0        0     2460 2023-07-28 12:08:01.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/typeslots.h
+-rw-rw-rw-   0        0        0    36074 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/unicodeobject.h
+-rw-rw-rw-   0        0        0     1775 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/warnings.h
+-rw-rw-rw-   0        0        0     2857 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp310/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:44.148808 wasmpy-build-0.4.1/wasmpy_build/include/cp311/
+-rw-rw-rw-   0        0        0    13936 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/LICENSE
+-rw-rw-rw-   0        0        0     2854 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/README.rst
+-rw-rw-rw-   0        0        0    31278 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/bltinmodule.h
+-rw-rw-rw-   0        0        0     1210 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/boolobject.h
+-rw-rw-rw-   0        0        0     1458 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2605 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/bytesobject.h
+-rw-rw-rw-   0        0        0     6213 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/ceval.h
+-rw-rw-rw-   0        0        0     7029 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/compile.h
+-rw-rw-rw-   0        0        0      722 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/complexobject.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:44.222395 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/
+-rw-rw-rw-   0        0        0     8229 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/abstract.h
+-rw-rw-rw-   0        0        0     1305 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4568 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/cellobject.h
+-rw-rw-rw-   0        0        0     1239 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/ceval.h
+-rw-rw-rw-   0        0        0     1656 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/classobject.h
+-rw-rw-rw-   0        0        0    11484 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/compile.h
+-rw-rw-rw-   0        0        0     1248 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/complexobject.h
+-rw-rw-rw-   0        0        0     1959 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/context.h
+-rw-rw-rw-   0        0        0     1642 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/descrobject.h
+-rw-rw-rw-   0        0        0     3324 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      818 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/fileobject.h
+-rw-rw-rw-   0        0        0      232 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/fileutils.h
+-rw-rw-rw-   0        0        0      702 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/floatobject.h
+-rw-rw-rw-   0        0        0     1108 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     4424 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/funcobject.h
+-rw-rw-rw-   0        0        0     3279 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/genobject.h
+-rw-rw-rw-   0        0        0     1526 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/import.h
+-rw-rw-rw-   0        0        0     7817 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/initconfig.h
+-rw-rw-rw-   0        0        0     1769 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/listobject.h
+-rw-rw-rw-   0        0        0     3817 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/longintrepr.h
+-rw-rw-rw-   0        0        0     4532 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/longobject.h
+-rw-rw-rw-   0        0        0     2556 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/methodobject.h
+-rw-rw-rw-   0        0        0     4234 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/modsupport.h
+-rw-rw-rw-   0        0        0    18305 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/object.h
+-rw-rw-rw-   0        0        0     2998 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     3505 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h
+-rw-rw-rw-   0        0        0     1387 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1073 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     4522 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0      582 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyframe.h
+-rw-rw-rw-   0        0        0     2099 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pymem.h
+-rw-rw-rw-   0        0        0    14351 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     1426 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pythread.h
+-rw-rw-rw-   0        0        0    12158 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pytime.h
+-rw-rw-rw-   0        0        0     1997 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/setobject.h
+-rw-rw-rw-   0        0        0      489 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      444 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1513 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    41910 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0      560 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/warnings.h
+-rw-rw-rw-   0        0        0     2103 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/weakrefobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/datetime.h
+-rw-rw-rw-   0        0        0     1244 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/descrobject.h
+-rw-rw-rw-   0        0        0     3834 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/errcode.h
+-rw-rw-rw-   0        0        0     1098 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/exports.h
+-rw-rw-rw-   0        0        0     1566 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/fileobject.h
+-rw-rw-rw-   0        0        0      509 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/fileutils.h
+-rw-rw-rw-   0        0        0     1527 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/floatobject.h
+-rw-rw-rw-   0        0        0      336 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/frameobject.h
+-rw-rw-rw-   0        0        0      332 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/genericaliasobject.h
+-rw-rw-rw-   0        0        0     2991 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/import.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:44.366962 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/
+-rw-rw-rw-   0        0        0      611 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1122 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     3031 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    29315 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6535 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     6062 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     1424 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
+-rw-rw-rw-   0        0        0     3469 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     4409 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0    15923 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1040 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2839 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0     1239 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     5684 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_dict.h
+-rw-rw-rw-   0        0        0      706 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0      562 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
+-rw-rw-rw-   0        0        0      842 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h
+-rw-rw-rw-   0        0        0     7320 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     1307 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h
+-rw-rw-rw-   0        0        0      480 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     7567 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_frame.h
+-rw-rw-rw-   0        0        0      413 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_function.h
+-rw-rw-rw-   0        0        0     6895 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0     1164 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_genobject.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-27 17:26:26.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     1436 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h
+-rw-rw-rw-   0        0        0    12980 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h
+-rw-rw-rw-   0        0        0     3696 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4185 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      743 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5787 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     6660 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      546 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
+-rw-rw-rw-   0        0        0     1352 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     3519 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1040 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0      390 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_namespace.h
+-rw-rw-rw-   0        0        0    10035 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_object.h
+-rw-rw-rw-   0        0        0    18986 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_opcode.h
+-rw-rw-rw-   0        0        0      626 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0      606 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2736 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2483 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3505 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     9435 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pymath.h
+-rw-rw-rw-   0        0        0     3708 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     4100 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     5988 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0    49092 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
+-rw-rw-rw-   0        0        0      937 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_signal.h
+-rw-rw-rw-   0        0        0      336 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
+-rw-rw-rw-   0        0        0      933 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_strhex.h
+-rw-rw-rw-   0        0        0      574 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5629 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      605 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3497 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0     2089 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0     1158 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h
+-rw-rw-rw-   0        0        0      898 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0     1716 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
+-rw-rw-rw-   0        0        0      678 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      739 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      775 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/intrcheck.h
+-rw-rw-rw-   0        0        0      589 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/iterobject.h
+-rw-rw-rw-   0        0        0     1772 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/listobject.h
+-rw-rw-rw-   0        0        0     3254 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/longobject.h
+-rw-rw-rw-   0        0        0      819 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/marshal.h
+-rw-rw-rw-   0        0        0     2802 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/memoryobject.h
+-rw-rw-rw-   0        0        0     5062 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/methodobject.h
+-rw-rw-rw-   0        0        0     6438 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/modsupport.h
+-rw-rw-rw-   0        0        0     2353 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/moduleobject.h
+-rw-rw-rw-   0        0        0    29768 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/object.h
+-rw-rw-rw-   0        0        0     8408 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/objimpl.h
+-rw-rw-rw-   0        0        0    11187 2023-07-28 12:08:05.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/osdefs.h
+-rw-rw-rw-   0        0        0      289 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/osmodule.h
+-rw-rw-rw-   0        0        0     1299 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/patchlevel.h
+-rw-rw-rw-   0        0        0     2471 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/py_curses.h
+-rw-rw-rw-   0        0        0     5117 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pybuffer.h
+-rw-rw-rw-   0        0        0     1725 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pydtrace.h
+-rw-rw-rw-   0        0        0    12715 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyexpat.h
+-rw-rw-rw-   0        0        0      545 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyframe.h
+-rw-rw-rw-   0        0        0     4147 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyhash.h
+-rw-rw-rw-   0        0        0     2216 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymacconfig.h
+-rw-rw-rw-   0        0        0     6064 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymacro.h
+-rw-rw-rw-   0        0        0     1979 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymath.h
+-rw-rw-rw-   0        0        0     3896 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymem.h
+-rw-rw-rw-   0        0        0    24642 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyport.h
+-rw-rw-rw-   0        0        0     4561 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pystrcmp.h
+-rw-rw-rw-   0        0        0     1557 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pystrtod.h
+-rw-rw-rw-   0        0        0     1187 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pythonrun.h
+-rw-rw-rw-   0        0        0     4834 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pythread.h
+-rw-rw-rw-   0        0        0      851 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/pytypedefs.h
+-rw-rw-rw-   0        0        0      628 2023-07-27 17:26:27.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/rangeobject.h
+-rw-rw-rw-   0        0        0     1537 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/setobject.h
+-rw-rw-rw-   0        0        0     2512 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/sliceobject.h
+-rw-rw-rw-   0        0        0     2038 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/structmember.h
+-rw-rw-rw-   0        0        0     1380 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/structseq.h
+-rw-rw-rw-   0        0        0     1377 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-28 11:36:57.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/token.h
+-rw-rw-rw-   0        0        0      583 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/traceback.h
+-rw-rw-rw-   0        0        0     1113 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/tracemalloc.h
+-rw-rw-rw-   0        0        0     1605 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/tupleobject.h
+-rw-rw-rw-   0        0        0     2342 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/typeslots.h
+-rw-rw-rw-   0        0        0    36804 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/unicodeobject.h
+-rw-rw-rw-   0        0        0     1129 2023-07-28 12:08:06.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/warnings.h
+-rw-rw-rw-   0        0        0     1220 2023-07-28 12:08:09.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp311/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.035739 wasmpy-build-0.4.1/wasmpy_build/include/cp38/
+-rw-rw-rw-   0        0        0    13937 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/LICENSE
+-rw-rw-rw-   0        0        0    26491 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/Python-ast.h
+-rw-rw-rw-   0        0        0     3615 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/Python.h
+-rw-rw-rw-   0        0        0    30164 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/abstract.h
+-rw-rw-rw-   0        0        0     1229 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/asdl.h
+-rw-rw-rw-   0        0        0      944 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/bltinmodule.h
+-rw-rw-rw-   0        0        0      884 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/boolobject.h
+-rw-rw-rw-   0        0        0     2110 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3301 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytes_methods.h
+-rw-rw-rw-   0        0        0     8485 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytesobject.h
+-rw-rw-rw-   0        0        0      709 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cellobject.h
+-rw-rw-rw-   0        0        0     8320 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/ceval.h
+-rw-rw-rw-   0        0        0     1700 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/classobject.h
+-rw-rw-rw-   0        0        0     7158 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/code.h
+-rw-rw-rw-   0        0        0     6751 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/codecs.h
+-rw-rw-rw-   0        0        0     3543 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/compile.h
+-rw-rw-rw-   0        0        0     1803 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/complexobject.h
+-rw-rw-rw-   0        0        0     2002 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/context.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.069348 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/
+-rw-rw-rw-   0        0        0    12294 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/abstract.h
+-rw-rw-rw-   0        0        0     3845 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/fileobject.h
+-rw-rw-rw-   0        0        0    16028 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0    15691 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/object.h
+-rw-rw-rw-   0        0        0     3600 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     4717 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2263 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pymem.h
+-rw-rw-rw-   0        0        0     9810 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pystate.h
+-rw-rw-rw-   0        0        0      547 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46308 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9260 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/datetime.h
+-rw-rw-rw-   0        0        0     3005 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/descrobject.h
+-rw-rw-rw-   0        0        0     3700 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/dictobject.h
+-rw-rw-rw-   0        0        0      460 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/dtoa.h
+-rw-rw-rw-   0        0        0    22469 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/enumobject.h
+-rw-rw-rw-   0        0        0     1695 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/errcode.h
+-rw-rw-rw-   0        0        0     1201 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/eval.h
+-rw-rw-rw-   0        0        0     1567 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/fileobject.h
+-rw-rw-rw-   0        0        0     4363 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/fileutils.h
+-rw-rw-rw-   0        0        0     4788 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/floatobject.h
+-rw-rw-rw-   0        0        0     3304 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/frameobject.h
+-rw-rw-rw-   0        0        0     4174 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/funcobject.h
+-rw-rw-rw-   0        0        0     3710 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/grammar.h
+-rw-rw-rw-   0        0        0     4882 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/import.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.109219 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/
+-rw-rw-rw-   0        0        0     1122 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16944 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0      966 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      542 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      779 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     1254 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1520 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3698 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     5207 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     1548 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     2896 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     2037 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     1327 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3814 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     8217 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     9578 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     3072 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      416 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      591 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/interpreteridobject.h
+-rw-rw-rw-   0        0        0      864 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/intrcheck.h
+-rw-rw-rw-   0        0        0      563 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/iterobject.h
+-rw-rw-rw-   0        0        0     2917 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/listobject.h
+-rw-rw-rw-   0        0        0     3791 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/longintrepr.h
+-rw-rw-rw-   0        0        0     9483 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/longobject.h
+-rw-rw-rw-   0        0        0      795 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/marshal.h
+-rw-rw-rw-   0        0        0     2757 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/memoryobject.h
+-rw-rw-rw-   0        0        0     4394 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/methodobject.h
+-rw-rw-rw-   0        0        0     9564 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/modsupport.h
+-rw-rw-rw-   0        0        0     2334 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/moduleobject.h
+-rw-rw-rw-   0        0        0      347 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/namespaceobject.h
+-rw-rw-rw-   0        0        0     1330 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/node.h
+-rw-rw-rw-   0        0        0    29576 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/object.h
+-rw-rw-rw-   0        0        0    10517 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/objimpl.h
+-rw-rw-rw-   0        0        0     1298 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/odictobject.h
+-rw-rw-rw-   0        0        0     5164 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/osdefs.h
+-rw-rw-rw-   0        0        0      289 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/osmodule.h
+-rw-rw-rw-   0        0        0     2976 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/parsetok.h
+-rw-rw-rw-   0        0        0     1299 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/patchlevel.h
+-rw-rw-rw-   0        0        0      836 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/picklebufobject.h
+-rw-rw-rw-   0        0        0     2477 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/py_curses.h
+-rw-rw-rw-   0        0        0     2745 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyarena.h
+-rw-rw-rw-   0        0        0     1726 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyctype.h
+-rw-rw-rw-   0        0        0     1214 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydtrace.h
+-rw-rw-rw-   0        0        0    12720 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyexpat.h
+-rw-rw-rw-   0        0        0      341 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyfpe.h
+-rw-rw-rw-   0        0        0     4133 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyhash.h
+-rw-rw-rw-   0        0        0     2048 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymacconfig.h
+-rw-rw-rw-   0        0        0     3778 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymacro.h
+-rw-rw-rw-   0        0        0     8312 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymath.h
+-rw-rw-rw-   0        0        0     5410 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymem.h
+-rw-rw-rw-   0        0        0    30362 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyport.h
+-rw-rw-rw-   0        0        0     4641 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystrcmp.h
+-rw-rw-rw-   0        0        0      845 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystrtod.h
+-rw-rw-rw-   0        0        0     7560 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pythonrun.h
+-rw-rw-rw-   0        0        0     5661 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pythread.h
+-rw-rw-rw-   0        0        0     8922 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/pytime.h
+-rw-rw-rw-   0        0        0      629 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/rangeobject.h
+-rw-rw-rw-   0        0        0     3356 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/setobject.h
+-rw-rw-rw-   0        0        0     2513 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/sliceobject.h
+-rw-rw-rw-   0        0        0     2028 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/structmember.h
+-rw-rw-rw-   0        0        0     1369 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/structseq.h
+-rw-rw-rw-   0        0        0     5281 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/symtable.h
+-rw-rw-rw-   0        0        0     1238 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/sysmodule.h
+-rw-rw-rw-   0        0        0     2429 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/token.h
+-rw-rw-rw-   0        0        0      601 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/traceback.h
+-rw-rw-rw-   0        0        0     1113 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/tracemalloc.h
+-rw-rw-rw-   0        0        0     1653 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/tupleobject.h
+-rw-rw-rw-   0        0        0     2253 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/ucnhash.h
+-rw-rw-rw-   0        0        0    35664 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/unicodeobject.h
+-rw-rw-rw-   0        0        0     1775 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/warnings.h
+-rw-rw-rw-   0        0        0     2860 2023-07-28 12:08:15.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp38/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.345738 wasmpy-build-0.4.1/wasmpy_build/include/cp39/
+-rw-rw-rw-   0        0        0    13937 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/LICENSE
+-rw-rw-rw-   0        0        0    26193 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/Python-ast.h
+-rw-rw-rw-   0        0        0     3532 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/Python.h
+-rw-rw-rw-   0        0        0    30352 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/abstract.h
+-rw-rw-rw-   0        0        0     1224 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/asdl.h
+-rw-rw-rw-   0        0        0      943 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/bltinmodule.h
+-rw-rw-rw-   0        0        0      883 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/boolobject.h
+-rw-rw-rw-   0        0        0     1480 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3036 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/bytesobject.h
+-rw-rw-rw-   0        0        0      708 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cellobject.h
+-rw-rw-rw-   0        0        0     5916 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/ceval.h
+-rw-rw-rw-   0        0        0     1647 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/code.h
+-rw-rw-rw-   0        0        0     6751 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/codecs.h
+-rw-rw-rw-   0        0        0     3739 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/compile.h
+-rw-rw-rw-   0        0        0     1802 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/complexobject.h
+-rw-rw-rw-   0        0        0     1950 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/context.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.389245 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/
+-rw-rw-rw-   0        0        0    14200 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4114 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1537 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/ceval.h
+-rw-rw-rw-   0        0        0     6989 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/code.h
+-rw-rw-rw-   0        0        0     3797 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4004 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3059 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1473 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/import.h
+-rw-rw-rw-   0        0        0    16979 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1364 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19358 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/object.h
+-rw-rw-rw-   0        0        0     4456 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     5101 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2096 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pymem.h
+-rw-rw-rw-   0        0        0    10134 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pystate.h
+-rw-rw-rw-   0        0        0      575 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46154 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9255 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/datetime.h
+-rw-rw-rw-   0        0        0     3005 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/descrobject.h
+-rw-rw-rw-   0        0        0     3699 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/dictobject.h
+-rw-rw-rw-   0        0        0    22469 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/enumobject.h
+-rw-rw-rw-   0        0        0     1624 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/errcode.h
+-rw-rw-rw-   0        0        0     1201 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/exports.h
+-rw-rw-rw-   0        0        0     1567 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/fileobject.h
+-rw-rw-rw-   0        0        0      602 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/fileutils.h
+-rw-rw-rw-   0        0        0     4354 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/frameobject.h
+-rw-rw-rw-   0        0        0     4033 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/funcobject.h
+-rw-rw-rw-   0        0        0      332 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3515 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/grammar.h
+-rw-rw-rw-   0        0        0     2992 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/import.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:45.440725 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/
+-rw-rw-rw-   0        0        0      953 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pegen_interface.h
+-rw-rw-rw-   0        0        0      479 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1122 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16977 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     3384 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     2620 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h
+-rw-rw-rw-   0        0        0      864 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3403 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      541 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      800 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      648 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1541 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     6647 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4185 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      471 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5222 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     5296 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0     1548 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     4157 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     1936 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2026 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3740 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3363 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3576 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4452 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      548 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3052 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      440 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/interpreteridobject.h
+-rw-rw-rw-   0        0        0      864 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/intrcheck.h
+-rw-rw-rw-   0        0        0      517 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/iterobject.h
+-rw-rw-rw-   0        0        0     1773 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/listobject.h
+-rw-rw-rw-   0        0        0     3791 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/longintrepr.h
+-rw-rw-rw-   0        0        0     9476 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/longobject.h
+-rw-rw-rw-   0        0        0      795 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/marshal.h
+-rw-rw-rw-   0        0        0     2756 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/memoryobject.h
+-rw-rw-rw-   0        0        0     3767 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/methodobject.h
+-rw-rw-rw-   0        0        0     9932 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/modsupport.h
+-rw-rw-rw-   0        0        0     2333 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/moduleobject.h
+-rw-rw-rw-   0        0        0      347 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/namespaceobject.h
+-rw-rw-rw-   0        0        0     1283 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/node.h
+-rw-rw-rw-   0        0        0    24604 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/object.h
+-rw-rw-rw-   0        0        0     8403 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/objimpl.h
+-rw-rw-rw-   0        0        0     1297 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/odictobject.h
+-rw-rw-rw-   0        0        0     4900 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/osdefs.h
+-rw-rw-rw-   0        0        0      289 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/osmodule.h
+-rw-rw-rw-   0        0        0     2976 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/parsetok.h
+-rw-rw-rw-   0        0        0     1299 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/patchlevel.h
+-rw-rw-rw-   0        0        0      835 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/picklebufobject.h
+-rw-rw-rw-   0        0        0     2474 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/py_curses.h
+-rw-rw-rw-   0        0        0     2745 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyarena.h
+-rw-rw-rw-   0        0        0     1725 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydtrace.h
+-rw-rw-rw-   0        0        0    12361 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyexpat.h
+-rw-rw-rw-   0        0        0      444 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyfpe.h
+-rw-rw-rw-   0        0        0      460 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyframe.h
+-rw-rw-rw-   0        0        0     4256 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyhash.h
+-rw-rw-rw-   0        0        0     2103 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymacro.h
+-rw-rw-rw-   0        0        0     8580 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymath.h
+-rw-rw-rw-   0        0        0     4410 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymem.h
+-rw-rw-rw-   0        0        0    31387 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyport.h
+-rw-rw-rw-   0        0        0     5176 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystrcmp.h
+-rw-rw-rw-   0        0        0      845 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystrtod.h
+-rw-rw-rw-   0        0        0     7588 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pythonrun.h
+-rw-rw-rw-   0        0        0     5939 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pythread.h
+-rw-rw-rw-   0        0        0     8924 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/pytime.h
+-rw-rw-rw-   0        0        0      628 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/rangeobject.h
+-rw-rw-rw-   0        0        0     3318 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/setobject.h
+-rw-rw-rw-   0        0        0     2512 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/sliceobject.h
+-rw-rw-rw-   0        0        0     2028 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/structmember.h
+-rw-rw-rw-   0        0        0     1382 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/structseq.h
+-rw-rw-rw-   0        0        0     5280 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/symtable.h
+-rw-rw-rw-   0        0        0     1238 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/sysmodule.h
+-rw-rw-rw-   0        0        0     2642 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/traceback.h
+-rw-rw-rw-   0        0        0     1113 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/tracemalloc.h
+-rw-rw-rw-   0        0        0     1606 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/tupleobject.h
+-rw-rw-rw-   0        0        0     2350 2023-07-28 12:08:17.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-28 12:08:11.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/ucnhash.h
+-rw-rw-rw-   0        0        0    35358 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/unicodeobject.h
+-rw-rw-rw-   0        0        0     1775 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/warnings.h
+-rw-rw-rw-   0        0        0     2857 2023-07-28 12:08:20.000000 wasmpy-build-0.4.1/wasmpy_build/include/cp39/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-28 12:09:43.306067 wasmpy-build-0.4.1/wasmpy_build.egg-info/
+-rw-rw-rw-   0        0        0     1741 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28898 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 12:09:43.000000 wasmpy-build-0.4.1/wasmpy_build.egg-info/top_level.txt
```

### Comparing `wasmpy-build-0.4.0/LICENSE` & `wasmpy-build-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/PKG-INFO` & `wasmpy-build-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.4.0
+Version: 0.4.1
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wasmpy-build-0.4.0/README.md` & `wasmpy-build-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/setup.py` & `wasmpy-build-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
             paths.append(os.path.join("..", path, file))
 
     return paths
 
 
 setuptools.setup(
     name="wasmpy-build",
-    version="0.4.0",
+    version="0.4.1",
     author="Olivia Ryan",
     author_email="olivia.r.dev@gmail.com",
     description="WebAssembly build tool for CPython C extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/olivi-r/wasmpy-build",
     packages=["wasmpy_build"],
     package_data={"wasmpy_build": recurse_files("wasmpy_build/include")},
     entry_points={
         "console_scripts": [
             "wasmpy-build=wasmpy_build:buildc",
-            "wasmpy-build++=wasmpy_build:buidcpp",
+            "wasmpy-build++=wasmpy_build:buildcpp",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build/__init__.py` & `wasmpy-build-0.4.1/wasmpy_build/__init__.py`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/LICENSE` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/Python.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/boolobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cellobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/classobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/codecs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/complexobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/frameobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/odictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/picklebufobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pyctype.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pydebug.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/pytime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/cpython/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/datetime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/descrobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/dynamic_annotations.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/errcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/eval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/exports.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/funcobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/genobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_accu.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_asdl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ast_state.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_atomic.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_bitutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_call.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_condvar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_dtoa.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_gc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_gil.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_hamt.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_hashtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_interp.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_long.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_parser.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pathconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pyarena.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_runtime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_symtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_ucnhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_unionobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/internal/pycore_warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/intrcheck.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/iterobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/longintrepr.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/longobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/marshal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/memoryobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/modsupport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/opcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/osdefs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/patchlevel.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/py_curses.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pycapsule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pydtrace.d` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pydtrace.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyexpat.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymacconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymacro.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymath.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pyport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystrhex.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pystrtod.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/pythread.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/rangeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/setobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/sliceobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/structmember.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/structseq.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/token.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/tracemalloc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/typeslots.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp310/weakrefobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp310/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/LICENSE` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/Python.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/abstract.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 /* Abstract Object Interface (many thanks to Jim Fulton) */
 
 #ifndef Py_ABSTRACTOBJECT_H
 #define Py_ABSTRACTOBJECT_H
 #ifdef __cplusplus
-extern "C"
-{
+extern "C" {
 #endif
 
 /* === Object Protocol ================================================== */
 
 /* Implemented elsewhere:
 
    int PyObject_Print(PyObject *o, FILE *fp, int flags);
 
    Print an object 'o' on file 'fp'.  Returns -1 on error. The flags argument
    is used to enable certain printing options. The only option currently
    supported is Py_Print_RAW.
 
    (What should be said about Py_Print_RAW?). */
 
+
 /* Implemented elsewhere:
 
    int PyObject_HasAttrString(PyObject *o, const char *attr_name);
 
    Returns 1 if object 'o' has the attribute attr_name, and 0 otherwise.
 
    This is equivalent to the Python expression: hasattr(o,attr_name).
 
    This function always succeeds. */
 
+
 /* Implemented elsewhere:
 
    PyObject* PyObject_GetAttrString(PyObject *o, const char *attr_name);
 
    Retrieve an attributed named attr_name form object o.
    Returns the attribute value on success, or NULL on failure.
 
    This is the equivalent of the Python expression: o.attr_name. */
 
+
 /* Implemented elsewhere:
 
    int PyObject_HasAttr(PyObject *o, PyObject *attr_name);
 
    Returns 1 if o has the attribute attr_name, and 0 otherwise.
 
    This is equivalent to the Python expression: hasattr(o,attr_name).
@@ -53,24 +55,26 @@
    PyObject* PyObject_GetAttr(PyObject *o, PyObject *attr_name);
 
    Retrieve an attributed named 'attr_name' form object 'o'.
    Returns the attribute value on success, or NULL on failure.
 
    This is the equivalent of the Python expression: o.attr_name. */
 
+
 /* Implemented elsewhere:
 
    int PyObject_SetAttrString(PyObject *o, const char *attr_name, PyObject *v);
 
    Set the value of the attribute named attr_name, for object 'o',
    to the value 'v'. Raise an exception and return -1 on failure; return 0 on
    success.
 
    This is the equivalent of the Python statement o.attr_name=v. */
 
+
 /* Implemented elsewhere:
 
    int PyObject_SetAttr(PyObject *o, PyObject *attr_name, PyObject *v);
 
    Set the value of the attribute named attr_name, for object 'o', to the value
    'v'. an exception and return -1 on failure; return 0 on success.
 
@@ -80,764 +84,790 @@
 
    int PyObject_DelAttrString(PyObject *o, const char *attr_name);
 
    Delete attribute named attr_name, for object o. Returns
    -1 on failure.
 
    This is the equivalent of the Python statement: del o.attr_name. */
-#define PyObject_DelAttrString(O, A) PyObject_SetAttrString((O), (A), NULL)
+#define PyObject_DelAttrString(O,A) PyObject_SetAttrString((O),(A), NULL)
+
 
 /* Implemented as a macro:
 
    int PyObject_DelAttr(PyObject *o, PyObject *attr_name);
 
    Delete attribute named attr_name, for object o. Returns -1
    on failure.  This is the equivalent of the Python
    statement: del o.attr_name. */
-#define PyObject_DelAttr(O, A) PyObject_SetAttr((O), (A), NULL)
+#define  PyObject_DelAttr(O,A) PyObject_SetAttr((O),(A), NULL)
+
 
-   /* Implemented elsewhere:
+/* Implemented elsewhere:
+
+   PyObject *PyObject_Repr(PyObject *o);
 
-      PyObject *PyObject_Repr(PyObject *o);
+   Compute the string representation of object 'o'.  Returns the
+   string representation on success, NULL on failure.
 
-      Compute the string representation of object 'o'.  Returns the
-      string representation on success, NULL on failure.
+   This is the equivalent of the Python expression: repr(o).
 
-      This is the equivalent of the Python expression: repr(o).
+   Called by the repr() built-in function. */
 
-      Called by the repr() built-in function. */
 
-   /* Implemented elsewhere:
+/* Implemented elsewhere:
 
-      PyObject *PyObject_Str(PyObject *o);
+   PyObject *PyObject_Str(PyObject *o);
 
-      Compute the string representation of object, o.  Returns the
-      string representation on success, NULL on failure.
+   Compute the string representation of object, o.  Returns the
+   string representation on success, NULL on failure.
 
-      This is the equivalent of the Python expression: str(o).
+   This is the equivalent of the Python expression: str(o).
 
-      Called by the str() and print() built-in functions. */
+   Called by the str() and print() built-in functions. */
 
-   /* Declared elsewhere
 
-      PyAPI_FUNC(int) PyCallable_Check(PyObject *o);
+/* Declared elsewhere
 
-      Determine if the object, o, is callable.  Return 1 if the object is callable
-      and 0 otherwise.
+   PyAPI_FUNC(int) PyCallable_Check(PyObject *o);
+
+   Determine if the object, o, is callable.  Return 1 if the object is callable
+   and 0 otherwise.
+
+   This function always succeeds. */
 
-      This function always succeeds. */
 
 #ifdef PY_SSIZE_T_CLEAN
-#define PyObject_CallFunction _PyObject_CallFunction_SizeT
-#define PyObject_CallMethod _PyObject_CallMethod_SizeT
+#  define PyObject_CallFunction _PyObject_CallFunction_SizeT
+#  define PyObject_CallMethod _PyObject_CallMethod_SizeT
 #endif
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03090000
-   /* Call a callable Python object without any arguments */
-   PyAPI_FUNC(uint64_t) PyObject_CallNoArgs(PyObject *func);
+
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03090000
+/* Call a callable Python object without any arguments */
+PyAPI_FUNC(uint64_t) PyObject_CallNoArgs(PyObject *func);
 #endif
 
-   /* Call a callable Python object 'callable' with arguments given by the
-      tuple 'args' and keywords arguments given by the dictionary 'kwargs'.
 
-      'args' must not be NULL, use an empty tuple if no arguments are
-      needed. If no named arguments are needed, 'kwargs' can be NULL.
+/* Call a callable Python object 'callable' with arguments given by the
+   tuple 'args' and keywords arguments given by the dictionary 'kwargs'.
 
-      This is the equivalent of the Python expression:
-      callable(*args, **kwargs). */
-   PyAPI_FUNC(uint64_t) PyObject_Call(PyObject *callable,
-                                      PyObject *args, PyObject *kwargs);
+   'args' must not be NULL, use an empty tuple if no arguments are
+   needed. If no named arguments are needed, 'kwargs' can be NULL.
 
-   /* Call a callable Python object 'callable', with arguments given by the
-      tuple 'args'.  If no arguments are needed, then 'args' can be NULL.
+   This is the equivalent of the Python expression:
+   callable(*args, **kwargs). */
+PyAPI_FUNC(uint64_t) PyObject_Call(PyObject *callable,
+                                     PyObject *args, PyObject *kwargs);
 
-      Returns the result of the call on success, or NULL on failure.
 
-      This is the equivalent of the Python expression:
-      callable(*args). */
-   PyAPI_FUNC(uint64_t) PyObject_CallObject(PyObject *callable,
-                                            PyObject *args);
+/* Call a callable Python object 'callable', with arguments given by the
+   tuple 'args'.  If no arguments are needed, then 'args' can be NULL.
 
-   /* Call a callable Python object, callable, with a variable number of C
-      arguments. The C arguments are described using a mkvalue-style format
-      string.
+   Returns the result of the call on success, or NULL on failure.
 
-      The format may be NULL, indicating that no arguments are provided.
+   This is the equivalent of the Python expression:
+   callable(*args). */
+PyAPI_FUNC(uint64_t) PyObject_CallObject(PyObject *callable,
+                                           PyObject *args);
 
-      Returns the result of the call on success, or NULL on failure.
+/* Call a callable Python object, callable, with a variable number of C
+   arguments. The C arguments are described using a mkvalue-style format
+   string.
 
-      This is the equivalent of the Python expression:
-      callable(arg1, arg2, ...). */
-   PyAPI_FUNC(uint64_t) PyObject_CallFunction(PyObject *callable,
-                                              const char *format, ...);
+   The format may be NULL, indicating that no arguments are provided.
 
-   /* Call the method named 'name' of object 'obj' with a variable number of
-      C arguments.  The C arguments are described by a mkvalue format string.
+   Returns the result of the call on success, or NULL on failure.
 
-      The format can be NULL, indicating that no arguments are provided.
+   This is the equivalent of the Python expression:
+   callable(arg1, arg2, ...). */
+PyAPI_FUNC(uint64_t) PyObject_CallFunction(PyObject *callable,
+                                             const char *format, ...);
 
-      Returns the result of the call on success, or NULL on failure.
+/* Call the method named 'name' of object 'obj' with a variable number of
+   C arguments.  The C arguments are described by a mkvalue format string.
 
-      This is the equivalent of the Python expression:
-      obj.name(arg1, arg2, ...). */
-   PyAPI_FUNC(uint64_t) PyObject_CallMethod(PyObject *obj,
-                                            const char *name,
-                                            const char *format, ...);
+   The format can be NULL, indicating that no arguments are provided.
 
-   PyAPI_FUNC(uint64_t) _PyObject_CallFunction_SizeT(PyObject *callable,
-                                                     const char *format,
-                                                     ...);
+   Returns the result of the call on success, or NULL on failure.
 
-   PyAPI_FUNC(uint64_t) _PyObject_CallMethod_SizeT(PyObject *obj,
-                                                   const char *name,
-                                                   const char *format,
-                                                   ...);
+   This is the equivalent of the Python expression:
+   obj.name(arg1, arg2, ...). */
+PyAPI_FUNC(uint64_t) PyObject_CallMethod(PyObject *obj,
+                                           const char *name,
+                                           const char *format, ...);
 
-   /* Call a callable Python object 'callable' with a variable number of C
-      arguments. The C arguments are provided as PyObject* values, terminated
-      by a NULL.
+PyAPI_FUNC(uint64_t) _PyObject_CallFunction_SizeT(PyObject *callable,
+                                                    const char *format,
+                                                    ...);
 
-      Returns the result of the call on success, or NULL on failure.
+PyAPI_FUNC(uint64_t) _PyObject_CallMethod_SizeT(PyObject *obj,
+                                                  const char *name,
+                                                  const char *format,
+                                                  ...);
 
-      This is the equivalent of the Python expression:
-      callable(arg1, arg2, ...). */
-   PyAPI_FUNC(uint64_t) PyObject_CallFunctionObjArgs(PyObject *callable,
-                                                     ...);
+/* Call a callable Python object 'callable' with a variable number of C
+   arguments. The C arguments are provided as PyObject* values, terminated
+   by a NULL.
 
-   /* Call the method named 'name' of object 'obj' with a variable number of
-      C arguments.  The C arguments are provided as PyObject* values, terminated
-      by NULL.
+   Returns the result of the call on success, or NULL on failure.
 
-      Returns the result of the call on success, or NULL on failure.
+   This is the equivalent of the Python expression:
+   callable(arg1, arg2, ...). */
+PyAPI_FUNC(uint64_t) PyObject_CallFunctionObjArgs(PyObject *callable,
+                                                    ...);
 
-      This is the equivalent of the Python expression: obj.name(*args). */
+/* Call the method named 'name' of object 'obj' with a variable number of
+   C arguments.  The C arguments are provided as PyObject* values, terminated
+   by NULL.
 
-   PyAPI_FUNC(uint64_t) PyObject_CallMethodObjArgs(
-       PyObject *obj,
-       PyObject *name,
-       ...);
+   Returns the result of the call on success, or NULL on failure.
 
-   /* Implemented elsewhere:
+   This is the equivalent of the Python expression: obj.name(*args). */
 
-      Py_hash_t PyObject_Hash(PyObject *o);
+PyAPI_FUNC(uint64_t) PyObject_CallMethodObjArgs(
+    PyObject *obj,
+    PyObject *name,
+    ...);
 
-      Compute and return the hash, hash_value, of an object, o.  On
-      failure, return -1.
 
-      This is the equivalent of the Python expression: hash(o). */
+/* Implemented elsewhere:
+
+   Py_hash_t PyObject_Hash(PyObject *o);
+
+   Compute and return the hash, hash_value, of an object, o.  On
+   failure, return -1.
+
+   This is the equivalent of the Python expression: hash(o). */
+
+
+/* Implemented elsewhere:
 
-   /* Implemented elsewhere:
+   int PyObject_IsTrue(PyObject *o);
 
-      int PyObject_IsTrue(PyObject *o);
+   Returns 1 if the object, o, is considered to be true, 0 if o is
+   considered to be false and -1 on failure.
 
-      Returns 1 if the object, o, is considered to be true, 0 if o is
-      considered to be false and -1 on failure.
+   This is equivalent to the Python expression: not not o. */
 
-      This is equivalent to the Python expression: not not o. */
 
-   /* Implemented elsewhere:
+/* Implemented elsewhere:
+
+   int PyObject_Not(PyObject *o);
+
+   Returns 0 if the object, o, is considered to be true, 1 if o is
+   considered to be false and -1 on failure.
+
+   This is equivalent to the Python expression: not o. */
 
-      int PyObject_Not(PyObject *o);
 
-      Returns 0 if the object, o, is considered to be true, 1 if o is
-      considered to be false and -1 on failure.
+/* Get the type of an object.
 
-      This is equivalent to the Python expression: not o. */
+   On success, returns a type object corresponding to the object type of object
+   'o'. On failure, returns NULL.
 
-   /* Get the type of an object.
+   This is equivalent to the Python expression: type(o) */
+PyAPI_FUNC(uint64_t) PyObject_Type(PyObject *o);
 
-      On success, returns a type object corresponding to the object type of object
-      'o'. On failure, returns NULL.
 
-      This is equivalent to the Python expression: type(o) */
-   PyAPI_FUNC(uint64_t) PyObject_Type(PyObject *o);
+/* Return the size of object 'o'.  If the object 'o' provides both sequence and
+   mapping protocols, the sequence size is returned.
 
-   /* Return the size of object 'o'.  If the object 'o' provides both sequence and
-      mapping protocols, the sequence size is returned.
+   On error, -1 is returned.
 
-      On error, -1 is returned.
+   This is the equivalent to the Python expression: len(o) */
+PyAPI_FUNC(Py_ssize_t) PyObject_Size(PyObject *o);
 
-      This is the equivalent to the Python expression: len(o) */
-   PyAPI_FUNC(Py_ssize_t) PyObject_Size(PyObject *o);
 
 /* For DLL compatibility */
 #undef PyObject_Length
-   PyAPI_FUNC(Py_ssize_t) PyObject_Length(PyObject *o);
+PyAPI_FUNC(Py_ssize_t) PyObject_Length(PyObject *o);
 #define PyObject_Length PyObject_Size
 
-   /* Return element of 'o' corresponding to the object 'key'. Return NULL
-     on failure.
+/* Return element of 'o' corresponding to the object 'key'. Return NULL
+  on failure.
 
-     This is the equivalent of the Python expression: o[key] */
-   PyAPI_FUNC(uint64_t) PyObject_GetItem(PyObject *o, PyObject *key);
+  This is the equivalent of the Python expression: o[key] */
+PyAPI_FUNC(uint64_t) PyObject_GetItem(PyObject *o, PyObject *key);
 
-   /* Map the object 'key' to the value 'v' into 'o'.
 
-      Raise an exception and return -1 on failure; return 0 on success.
+/* Map the object 'key' to the value 'v' into 'o'.
 
-      This is the equivalent of the Python statement: o[key]=v. */
-   PyAPI_FUNC(int) PyObject_SetItem(PyObject *o, PyObject *key, PyObject *v);
+   Raise an exception and return -1 on failure; return 0 on success.
 
-   /* Remove the mapping for the string 'key' from the object 'o'.
-      Returns -1 on failure.
+   This is the equivalent of the Python statement: o[key]=v. */
+PyAPI_FUNC(int) PyObject_SetItem(PyObject *o, PyObject *key, PyObject *v);
 
-      This is equivalent to the Python statement: del o[key]. */
-   PyAPI_FUNC(int) PyObject_DelItemString(PyObject *o, const char *key);
+/* Remove the mapping for the string 'key' from the object 'o'.
+   Returns -1 on failure.
 
-   /* Delete the mapping for the object 'key' from the object 'o'.
-      Returns -1 on failure.
+   This is equivalent to the Python statement: del o[key]. */
+PyAPI_FUNC(int) PyObject_DelItemString(PyObject *o, const char *key);
 
-      This is the equivalent of the Python statement: del o[key]. */
-   PyAPI_FUNC(int) PyObject_DelItem(PyObject *o, PyObject *key);
+/* Delete the mapping for the object 'key' from the object 'o'.
+   Returns -1 on failure.
 
-   /* === Old Buffer API ============================================ */
+   This is the equivalent of the Python statement: del o[key]. */
+PyAPI_FUNC(int) PyObject_DelItem(PyObject *o, PyObject *key);
 
-   /* FIXME:  usage of these should all be replaced in Python itself
-      but for backwards compatibility we will implement them.
-      Their usage without a corresponding "unlock" mechanism
-      may create issues (but they would already be there). */
 
-   /* Takes an arbitrary object which must support the (character, single segment)
-      buffer interface and returns a pointer to a read-only memory location
-      usable as character based input for subsequent processing.
+/* === Old Buffer API ============================================ */
 
-      Return 0 on success.  buffer and buffer_len are only set in case no error
-      occurs. Otherwise, -1 is returned and an exception set. */
-   Py_DEPRECATED(3.0)
-       PyAPI_FUNC(int) PyObject_AsCharBuffer(PyObject *obj,
-                                             const char **buffer,
-                                             Py_ssize_t *buffer_len);
+/* FIXME:  usage of these should all be replaced in Python itself
+   but for backwards compatibility we will implement them.
+   Their usage without a corresponding "unlock" mechanism
+   may create issues (but they would already be there). */
 
-   /* Checks whether an arbitrary object supports the (character, single segment)
-      buffer interface.
+/* Takes an arbitrary object which must support the (character, single segment)
+   buffer interface and returns a pointer to a read-only memory location
+   usable as character based input for subsequent processing.
 
-      Returns 1 on success, 0 on failure. */
-   Py_DEPRECATED(3.0) PyAPI_FUNC(int) PyObject_CheckReadBuffer(PyObject *obj);
+   Return 0 on success.  buffer and buffer_len are only set in case no error
+   occurs. Otherwise, -1 is returned and an exception set. */
+Py_DEPRECATED(3.0)
+PyAPI_FUNC(int) PyObject_AsCharBuffer(PyObject *obj,
+                                      const char **buffer,
+                                      Py_ssize_t *buffer_len);
 
-   /* Same as PyObject_AsCharBuffer() except that this API expects (readable,
-      single segment) buffer interface and returns a pointer to a read-only memory
-      location which can contain arbitrary data.
+/* Checks whether an arbitrary object supports the (character, single segment)
+   buffer interface.
 
-      0 is returned on success.  buffer and buffer_len are only set in case no
-      error occurs.  Otherwise, -1 is returned and an exception set. */
-   Py_DEPRECATED(3.0)
-       PyAPI_FUNC(int) PyObject_AsReadBuffer(PyObject *obj,
-                                             const void **buffer,
-                                             Py_ssize_t *buffer_len);
+   Returns 1 on success, 0 on failure. */
+Py_DEPRECATED(3.0) PyAPI_FUNC(int) PyObject_CheckReadBuffer(PyObject *obj);
 
-   /* Takes an arbitrary object which must support the (writable, single segment)
-      buffer interface and returns a pointer to a writable memory location in
-      buffer of size 'buffer_len'.
+/* Same as PyObject_AsCharBuffer() except that this API expects (readable,
+   single segment) buffer interface and returns a pointer to a read-only memory
+   location which can contain arbitrary data.
 
-      Return 0 on success.  buffer and buffer_len are only set in case no error
-      occurs. Otherwise, -1 is returned and an exception set. */
-   Py_DEPRECATED(3.0)
-       PyAPI_FUNC(int) PyObject_AsWriteBuffer(PyObject *obj,
-                                              void **buffer,
-                                              Py_ssize_t *buffer_len);
+   0 is returned on success.  buffer and buffer_len are only set in case no
+   error occurs.  Otherwise, -1 is returned and an exception set. */
+Py_DEPRECATED(3.0)
+PyAPI_FUNC(int) PyObject_AsReadBuffer(PyObject *obj,
+                                      const void **buffer,
+                                      Py_ssize_t *buffer_len);
 
-   /* === New Buffer API ============================================ */
+/* Takes an arbitrary object which must support the (writable, single segment)
+   buffer interface and returns a pointer to a writable memory location in
+   buffer of size 'buffer_len'.
 
-   /* Takes an arbitrary object and returns the result of calling
-      obj.__format__(format_spec). */
-   PyAPI_FUNC(uint64_t) PyObject_Format(PyObject *obj,
-                                        PyObject *format_spec);
+   Return 0 on success.  buffer and buffer_len are only set in case no error
+   occurs. Otherwise, -1 is returned and an exception set. */
+Py_DEPRECATED(3.0)
+PyAPI_FUNC(int) PyObject_AsWriteBuffer(PyObject *obj,
+                                       void **buffer,
+                                       Py_ssize_t *buffer_len);
 
-   /* ==== Iterators ================================================ */
 
-   /* Takes an object and returns an iterator for it.
-      This is typically a new iterator but if the argument is an iterator, this
-      returns itself. */
-   PyAPI_FUNC(uint64_t) PyObject_GetIter(PyObject *);
+/* === New Buffer API ============================================ */
 
-   /* Takes an AsyncIterable object and returns an AsyncIterator for it.
-      This is typically a new iterator but if the argument is an AsyncIterator,
-      this returns itself. */
-   PyAPI_FUNC(uint64_t) PyObject_GetAIter(PyObject *);
+/* Takes an arbitrary object and returns the result of calling
+   obj.__format__(format_spec). */
+PyAPI_FUNC(uint64_t) PyObject_Format(PyObject *obj,
+                                       PyObject *format_spec);
 
-   /* Returns non-zero if the object 'obj' provides iterator protocols, and 0 otherwise.
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyIter_Check(PyObject *);
+/* ==== Iterators ================================================ */
 
-   /* Returns non-zero if the object 'obj' provides AsyncIterator protocols, and 0 otherwise.
+/* Takes an object and returns an iterator for it.
+   This is typically a new iterator but if the argument is an iterator, this
+   returns itself. */
+PyAPI_FUNC(uint64_t) PyObject_GetIter(PyObject *);
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyAIter_Check(PyObject *);
+/* Takes an AsyncIterable object and returns an AsyncIterator for it.
+   This is typically a new iterator but if the argument is an AsyncIterator,
+   this returns itself. */
+PyAPI_FUNC(uint64_t) PyObject_GetAIter(PyObject *);
 
-   /* Takes an iterator object and calls its tp_iternext slot,
-      returning the next value.
+/* Returns non-zero if the object 'obj' provides iterator protocols, and 0 otherwise.
 
-      If the iterator is exhausted, this returns NULL without setting an
-      exception.
+   This function always succeeds. */
+PyAPI_FUNC(int) PyIter_Check(PyObject *);
+
+/* Returns non-zero if the object 'obj' provides AsyncIterator protocols, and 0 otherwise.
+
+   This function always succeeds. */
+PyAPI_FUNC(int) PyAIter_Check(PyObject *);
 
-      NULL with an exception means an error occurred. */
-   PyAPI_FUNC(uint64_t) PyIter_Next(PyObject *);
+/* Takes an iterator object and calls its tp_iternext slot,
+   returning the next value.
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x030A0000
+   If the iterator is exhausted, this returns NULL without setting an
+   exception.
 
-   /* Takes generator, coroutine or iterator object and sends the value into it.
-      Returns:
-      - PYGEN_RETURN (0) if generator has returned.
-        'result' parameter is filled with return value
-      - PYGEN_ERROR (-1) if exception was raised.
-        'result' parameter is NULL
-      - PYGEN_NEXT (1) if generator has yielded.
-        'result' parameter is filled with yielded value. */
-   PyAPI_FUNC(PySendResult) PyIter_Send(PyObject *, PyObject *, PyObject **);
+   NULL with an exception means an error occurred. */
+PyAPI_FUNC(uint64_t) PyIter_Next(PyObject *);
+
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x030A0000
+
+/* Takes generator, coroutine or iterator object and sends the value into it.
+   Returns:
+   - PYGEN_RETURN (0) if generator has returned.
+     'result' parameter is filled with return value
+   - PYGEN_ERROR (-1) if exception was raised.
+     'result' parameter is NULL
+   - PYGEN_NEXT (1) if generator has yielded.
+     'result' parameter is filled with yielded value. */
+PyAPI_FUNC(PySendResult) PyIter_Send(PyObject *, PyObject *, PyObject **);
 #endif
 
-   /* === Number Protocol ================================================== */
 
-   /* Returns 1 if the object 'o' provides numeric protocols, and 0 otherwise.
+/* === Number Protocol ================================================== */
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyNumber_Check(PyObject *o);
+/* Returns 1 if the object 'o' provides numeric protocols, and 0 otherwise.
 
-   /* Returns the result of adding o1 and o2, or NULL on failure.
+   This function always succeeds. */
+PyAPI_FUNC(int) PyNumber_Check(PyObject *o);
+
+/* Returns the result of adding o1 and o2, or NULL on failure.
 
-      This is the equivalent of the Python expression: o1 + o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Add(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 + o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Add(PyObject *o1, PyObject *o2);
 
-   /* Returns the result of subtracting o2 from o1, or NULL on failure.
+/* Returns the result of subtracting o2 from o1, or NULL on failure.
 
-      This is the equivalent of the Python expression: o1 - o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Subtract(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 - o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Subtract(PyObject *o1, PyObject *o2);
 
-   /* Returns the result of multiplying o1 and o2, or NULL on failure.
+/* Returns the result of multiplying o1 and o2, or NULL on failure.
 
-      This is the equivalent of the Python expression: o1 * o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Multiply(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 * o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Multiply(PyObject *o1, PyObject *o2);
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03050000
-   /* This is the equivalent of the Python expression: o1 @ o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_MatrixMultiply(PyObject *o1, PyObject *o2);
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03050000
+/* This is the equivalent of the Python expression: o1 @ o2. */
+PyAPI_FUNC(uint64_t) PyNumber_MatrixMultiply(PyObject *o1, PyObject *o2);
 #endif
 
-   /* Returns the result of dividing o1 by o2 giving an integral result,
-      or NULL on failure.
+/* Returns the result of dividing o1 by o2 giving an integral result,
+   or NULL on failure.
+
+   This is the equivalent of the Python expression: o1 // o2. */
+PyAPI_FUNC(uint64_t) PyNumber_FloorDivide(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 // o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_FloorDivide(PyObject *o1, PyObject *o2);
+/* Returns the result of dividing o1 by o2 giving a float result, or NULL on
+   failure.
 
-   /* Returns the result of dividing o1 by o2 giving a float result, or NULL on
-      failure.
+   This is the equivalent of the Python expression: o1 / o2. */
+PyAPI_FUNC(uint64_t) PyNumber_TrueDivide(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 / o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_TrueDivide(PyObject *o1, PyObject *o2);
+/* Returns the remainder of dividing o1 by o2, or NULL on failure.
 
-   /* Returns the remainder of dividing o1 by o2, or NULL on failure.
+   This is the equivalent of the Python expression: o1 % o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Remainder(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 % o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Remainder(PyObject *o1, PyObject *o2);
+/* See the built-in function divmod.
 
-   /* See the built-in function divmod.
+   Returns NULL on failure.
 
-      Returns NULL on failure.
+   This is the equivalent of the Python expression: divmod(o1, o2). */
+PyAPI_FUNC(uint64_t) PyNumber_Divmod(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: divmod(o1, o2). */
-   PyAPI_FUNC(uint64_t) PyNumber_Divmod(PyObject *o1, PyObject *o2);
+/* See the built-in function pow. Returns NULL on failure.
 
-   /* See the built-in function pow. Returns NULL on failure.
+   This is the equivalent of the Python expression: pow(o1, o2, o3),
+   where o3 is optional. */
+PyAPI_FUNC(uint64_t) PyNumber_Power(PyObject *o1, PyObject *o2,
+                                      PyObject *o3);
 
-      This is the equivalent of the Python expression: pow(o1, o2, o3),
-      where o3 is optional. */
-   PyAPI_FUNC(uint64_t) PyNumber_Power(PyObject *o1, PyObject *o2,
-                                       PyObject *o3);
+/* Returns the negation of o on success, or NULL on failure.
 
-   /* Returns the negation of o on success, or NULL on failure.
+ This is the equivalent of the Python expression: -o. */
+PyAPI_FUNC(uint64_t) PyNumber_Negative(PyObject *o);
 
-    This is the equivalent of the Python expression: -o. */
-   PyAPI_FUNC(uint64_t) PyNumber_Negative(PyObject *o);
+/* Returns the positive of o on success, or NULL on failure.
 
-   /* Returns the positive of o on success, or NULL on failure.
+   This is the equivalent of the Python expression: +o. */
+PyAPI_FUNC(uint64_t) PyNumber_Positive(PyObject *o);
 
-      This is the equivalent of the Python expression: +o. */
-   PyAPI_FUNC(uint64_t) PyNumber_Positive(PyObject *o);
+/* Returns the absolute value of 'o', or NULL on failure.
 
-   /* Returns the absolute value of 'o', or NULL on failure.
+   This is the equivalent of the Python expression: abs(o). */
+PyAPI_FUNC(uint64_t) PyNumber_Absolute(PyObject *o);
 
-      This is the equivalent of the Python expression: abs(o). */
-   PyAPI_FUNC(uint64_t) PyNumber_Absolute(PyObject *o);
+/* Returns the bitwise negation of 'o' on success, or NULL on failure.
 
-   /* Returns the bitwise negation of 'o' on success, or NULL on failure.
+   This is the equivalent of the Python expression: ~o. */
+PyAPI_FUNC(uint64_t) PyNumber_Invert(PyObject *o);
 
-      This is the equivalent of the Python expression: ~o. */
-   PyAPI_FUNC(uint64_t) PyNumber_Invert(PyObject *o);
+/* Returns the result of left shifting o1 by o2 on success, or NULL on failure.
 
-   /* Returns the result of left shifting o1 by o2 on success, or NULL on failure.
+   This is the equivalent of the Python expression: o1 << o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Lshift(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 << o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Lshift(PyObject *o1, PyObject *o2);
+/* Returns the result of right shifting o1 by o2 on success, or NULL on
+   failure.
 
-   /* Returns the result of right shifting o1 by o2 on success, or NULL on
-      failure.
+   This is the equivalent of the Python expression: o1 >> o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Rshift(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 >> o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Rshift(PyObject *o1, PyObject *o2);
+/* Returns the result of bitwise and of o1 and o2 on success, or NULL on
+   failure.
 
-   /* Returns the result of bitwise and of o1 and o2 on success, or NULL on
-      failure.
+   This is the equivalent of the Python expression: o1 & o2. */
+PyAPI_FUNC(uint64_t) PyNumber_And(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 & o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_And(PyObject *o1, PyObject *o2);
+/* Returns the bitwise exclusive or of o1 by o2 on success, or NULL on failure.
 
-   /* Returns the bitwise exclusive or of o1 by o2 on success, or NULL on failure.
+   This is the equivalent of the Python expression: o1 ^ o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Xor(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 ^ o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Xor(PyObject *o1, PyObject *o2);
+/* Returns the result of bitwise or on o1 and o2 on success, or NULL on
+   failure.
 
-   /* Returns the result of bitwise or on o1 and o2 on success, or NULL on
-      failure.
+   This is the equivalent of the Python expression: o1 | o2. */
+PyAPI_FUNC(uint64_t) PyNumber_Or(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 | o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_Or(PyObject *o1, PyObject *o2);
+/* Returns 1 if obj is an index integer (has the nb_index slot of the
+   tp_as_number structure filled in), and 0 otherwise. */
+PyAPI_FUNC(int) PyIndex_Check(PyObject *);
 
-   /* Returns 1 if obj is an index integer (has the nb_index slot of the
-      tp_as_number structure filled in), and 0 otherwise. */
-   PyAPI_FUNC(int) PyIndex_Check(PyObject *);
+/* Returns the object 'o' converted to a Python int, or NULL with an exception
+   raised on failure. */
+PyAPI_FUNC(uint64_t) PyNumber_Index(PyObject *o);
 
-   /* Returns the object 'o' converted to a Python int, or NULL with an exception
-      raised on failure. */
-   PyAPI_FUNC(uint64_t) PyNumber_Index(PyObject *o);
+/* Returns the object 'o' converted to Py_ssize_t by going through
+   PyNumber_Index() first.
 
-   /* Returns the object 'o' converted to Py_ssize_t by going through
-      PyNumber_Index() first.
+   If an overflow error occurs while converting the int to Py_ssize_t, then the
+   second argument 'exc' is the error-type to return.  If it is NULL, then the
+   overflow error is cleared and the value is clipped. */
+PyAPI_FUNC(Py_ssize_t) PyNumber_AsSsize_t(PyObject *o, PyObject *exc);
 
-      If an overflow error occurs while converting the int to Py_ssize_t, then the
-      second argument 'exc' is the error-type to return.  If it is NULL, then the
-      overflow error is cleared and the value is clipped. */
-   PyAPI_FUNC(Py_ssize_t) PyNumber_AsSsize_t(PyObject *o, PyObject *exc);
+/* Returns the object 'o' converted to an integer object on success, or NULL
+   on failure.
 
-   /* Returns the object 'o' converted to an integer object on success, or NULL
-      on failure.
+   This is the equivalent of the Python expression: int(o). */
+PyAPI_FUNC(uint64_t) PyNumber_Long(PyObject *o);
 
-      This is the equivalent of the Python expression: int(o). */
-   PyAPI_FUNC(uint64_t) PyNumber_Long(PyObject *o);
+/* Returns the object 'o' converted to a float object on success, or NULL
+  on failure.
 
-   /* Returns the object 'o' converted to a float object on success, or NULL
-     on failure.
+  This is the equivalent of the Python expression: float(o). */
+PyAPI_FUNC(uint64_t) PyNumber_Float(PyObject *o);
 
-     This is the equivalent of the Python expression: float(o). */
-   PyAPI_FUNC(uint64_t) PyNumber_Float(PyObject *o);
 
-   /* --- In-place variants of (some of) the above number protocol functions -- */
+/* --- In-place variants of (some of) the above number protocol functions -- */
 
-   /* Returns the result of adding o2 to o1, possibly in-place, or NULL
-      on failure.
+/* Returns the result of adding o2 to o1, possibly in-place, or NULL
+   on failure.
 
-      This is the equivalent of the Python expression: o1 += o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceAdd(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 += o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceAdd(PyObject *o1, PyObject *o2);
 
-   /* Returns the result of subtracting o2 from o1, possibly in-place or
-      NULL on failure.
+/* Returns the result of subtracting o2 from o1, possibly in-place or
+   NULL on failure.
 
-      This is the equivalent of the Python expression: o1 -= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceSubtract(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 -= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceSubtract(PyObject *o1, PyObject *o2);
 
-   /* Returns the result of multiplying o1 by o2, possibly in-place, or NULL on
-      failure.
+/* Returns the result of multiplying o1 by o2, possibly in-place, or NULL on
+   failure.
 
-      This is the equivalent of the Python expression: o1 *= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceMultiply(PyObject *o1, PyObject *o2);
+   This is the equivalent of the Python expression: o1 *= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceMultiply(PyObject *o1, PyObject *o2);
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03050000
-   /* This is the equivalent of the Python expression: o1 @= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceMatrixMultiply(PyObject *o1, PyObject *o2);
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03050000
+/* This is the equivalent of the Python expression: o1 @= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceMatrixMultiply(PyObject *o1, PyObject *o2);
 #endif
 
-   /* Returns the result of dividing o1 by o2 giving an integral result, possibly
-      in-place, or NULL on failure.
+/* Returns the result of dividing o1 by o2 giving an integral result, possibly
+   in-place, or NULL on failure.
 
-      This is the equivalent of the Python expression: o1 /= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceFloorDivide(PyObject *o1,
-                                                    PyObject *o2);
+   This is the equivalent of the Python expression: o1 /= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceFloorDivide(PyObject *o1,
+                                                   PyObject *o2);
 
-   /* Returns the result of dividing o1 by o2 giving a float result, possibly
-      in-place, or null on failure.
+/* Returns the result of dividing o1 by o2 giving a float result, possibly
+   in-place, or null on failure.
 
-      This is the equivalent of the Python expression: o1 /= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceTrueDivide(PyObject *o1,
-                                                   PyObject *o2);
+   This is the equivalent of the Python expression: o1 /= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceTrueDivide(PyObject *o1,
+                                                  PyObject *o2);
 
-   /* Returns the remainder of dividing o1 by o2, possibly in-place, or NULL on
-      failure.
+/* Returns the remainder of dividing o1 by o2, possibly in-place, or NULL on
+   failure.
+
+   This is the equivalent of the Python expression: o1 %= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceRemainder(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 %= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceRemainder(PyObject *o1, PyObject *o2);
+/* Returns the result of raising o1 to the power of o2, possibly in-place,
+   or NULL on failure.
 
-   /* Returns the result of raising o1 to the power of o2, possibly in-place,
-      or NULL on failure.
+   This is the equivalent of the Python expression: o1 **= o2,
+   or o1 = pow(o1, o2, o3) if o3 is present. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlacePower(PyObject *o1, PyObject *o2,
+                                             PyObject *o3);
 
-      This is the equivalent of the Python expression: o1 **= o2,
-      or o1 = pow(o1, o2, o3) if o3 is present. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlacePower(PyObject *o1, PyObject *o2,
-                                              PyObject *o3);
+/* Returns the result of left shifting o1 by o2, possibly in-place, or NULL
+   on failure.
 
-   /* Returns the result of left shifting o1 by o2, possibly in-place, or NULL
-      on failure.
+   This is the equivalent of the Python expression: o1 <<= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceLshift(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 <<= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceLshift(PyObject *o1, PyObject *o2);
+/* Returns the result of right shifting o1 by o2, possibly in-place or NULL
+   on failure.
 
-   /* Returns the result of right shifting o1 by o2, possibly in-place or NULL
-      on failure.
+   This is the equivalent of the Python expression: o1 >>= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceRshift(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 >>= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceRshift(PyObject *o1, PyObject *o2);
+/* Returns the result of bitwise and of o1 and o2, possibly in-place, or NULL
+   on failure.
 
-   /* Returns the result of bitwise and of o1 and o2, possibly in-place, or NULL
-      on failure.
+   This is the equivalent of the Python expression: o1 &= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceAnd(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 &= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceAnd(PyObject *o1, PyObject *o2);
+/* Returns the bitwise exclusive or of o1 by o2, possibly in-place, or NULL
+   on failure.
 
-   /* Returns the bitwise exclusive or of o1 by o2, possibly in-place, or NULL
-      on failure.
+   This is the equivalent of the Python expression: o1 ^= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceXor(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 ^= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceXor(PyObject *o1, PyObject *o2);
+/* Returns the result of bitwise or of o1 and o2, possibly in-place,
+   or NULL on failure.
 
-   /* Returns the result of bitwise or of o1 and o2, possibly in-place,
-      or NULL on failure.
+   This is the equivalent of the Python expression: o1 |= o2. */
+PyAPI_FUNC(uint64_t) PyNumber_InPlaceOr(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 |= o2. */
-   PyAPI_FUNC(uint64_t) PyNumber_InPlaceOr(PyObject *o1, PyObject *o2);
+/* Returns the integer n converted to a string with a base, with a base
+   marker of 0b, 0o or 0x prefixed if applicable.
 
-   /* Returns the integer n converted to a string with a base, with a base
-      marker of 0b, 0o or 0x prefixed if applicable.
+   If n is not an int object, it is converted with PyNumber_Index first. */
+PyAPI_FUNC(uint64_t) PyNumber_ToBase(PyObject *n, int base);
 
-      If n is not an int object, it is converted with PyNumber_Index first. */
-   PyAPI_FUNC(uint64_t) PyNumber_ToBase(PyObject *n, int base);
 
-   /* === Sequence protocol ================================================ */
+/* === Sequence protocol ================================================ */
 
-   /* Return 1 if the object provides sequence protocol, and zero
-      otherwise.
+/* Return 1 if the object provides sequence protocol, and zero
+   otherwise.
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PySequence_Check(PyObject *o);
+   This function always succeeds. */
+PyAPI_FUNC(int) PySequence_Check(PyObject *o);
 
-   /* Return the size of sequence object o, or -1 on failure. */
-   PyAPI_FUNC(Py_ssize_t) PySequence_Size(PyObject *o);
+/* Return the size of sequence object o, or -1 on failure. */
+PyAPI_FUNC(Py_ssize_t) PySequence_Size(PyObject *o);
 
 /* For DLL compatibility */
 #undef PySequence_Length
-   PyAPI_FUNC(Py_ssize_t) PySequence_Length(PyObject *o);
+PyAPI_FUNC(Py_ssize_t) PySequence_Length(PyObject *o);
 #define PySequence_Length PySequence_Size
 
-   /* Return the concatenation of o1 and o2 on success, and NULL on failure.
 
-      This is the equivalent of the Python expression: o1 + o2. */
-   PyAPI_FUNC(uint64_t) PySequence_Concat(PyObject *o1, PyObject *o2);
+/* Return the concatenation of o1 and o2 on success, and NULL on failure.
 
-   /* Return the result of repeating sequence object 'o' 'count' times,
-     or NULL on failure.
+   This is the equivalent of the Python expression: o1 + o2. */
+PyAPI_FUNC(uint64_t) PySequence_Concat(PyObject *o1, PyObject *o2);
 
-     This is the equivalent of the Python expression: o * count. */
-   PyAPI_FUNC(uint64_t) PySequence_Repeat(PyObject *o, Py_ssize_t count);
+/* Return the result of repeating sequence object 'o' 'count' times,
+  or NULL on failure.
 
-   /* Return the ith element of o, or NULL on failure.
+  This is the equivalent of the Python expression: o * count. */
+PyAPI_FUNC(uint64_t) PySequence_Repeat(PyObject *o, Py_ssize_t count);
 
-      This is the equivalent of the Python expression: o[i]. */
-   PyAPI_FUNC(uint64_t) PySequence_GetItem(PyObject *o, Py_ssize_t i);
+/* Return the ith element of o, or NULL on failure.
 
-   /* Return the slice of sequence object o between i1 and i2, or NULL on failure.
+   This is the equivalent of the Python expression: o[i]. */
+PyAPI_FUNC(uint64_t) PySequence_GetItem(PyObject *o, Py_ssize_t i);
 
-      This is the equivalent of the Python expression: o[i1:i2]. */
-   PyAPI_FUNC(uint64_t) PySequence_GetSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2);
+/* Return the slice of sequence object o between i1 and i2, or NULL on failure.
 
-   /* Assign object 'v' to the ith element of the sequence 'o'. Raise an exception
-      and return -1 on failure; return 0 on success.
+   This is the equivalent of the Python expression: o[i1:i2]. */
+PyAPI_FUNC(uint64_t) PySequence_GetSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2);
 
-      This is the equivalent of the Python statement o[i] = v. */
-   PyAPI_FUNC(int) PySequence_SetItem(PyObject *o, Py_ssize_t i, PyObject *v);
+/* Assign object 'v' to the ith element of the sequence 'o'. Raise an exception
+   and return -1 on failure; return 0 on success.
 
-   /* Delete the 'i'-th element of the sequence 'v'. Returns -1 on failure.
+   This is the equivalent of the Python statement o[i] = v. */
+PyAPI_FUNC(int) PySequence_SetItem(PyObject *o, Py_ssize_t i, PyObject *v);
 
-      This is the equivalent of the Python statement: del o[i]. */
-   PyAPI_FUNC(int) PySequence_DelItem(PyObject *o, Py_ssize_t i);
+/* Delete the 'i'-th element of the sequence 'v'. Returns -1 on failure.
 
-   /* Assign the sequence object 'v' to the slice in sequence object 'o',
-      from 'i1' to 'i2'. Returns -1 on failure.
+   This is the equivalent of the Python statement: del o[i]. */
+PyAPI_FUNC(int) PySequence_DelItem(PyObject *o, Py_ssize_t i);
 
-      This is the equivalent of the Python statement: o[i1:i2] = v. */
-   PyAPI_FUNC(int) PySequence_SetSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2,
-                                       PyObject *v);
+/* Assign the sequence object 'v' to the slice in sequence object 'o',
+   from 'i1' to 'i2'. Returns -1 on failure.
 
-   /* Delete the slice in sequence object 'o' from 'i1' to 'i2'.
-      Returns -1 on failure.
+   This is the equivalent of the Python statement: o[i1:i2] = v. */
+PyAPI_FUNC(int) PySequence_SetSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2,
+                                    PyObject *v);
 
-      This is the equivalent of the Python statement: del o[i1:i2]. */
-   PyAPI_FUNC(int) PySequence_DelSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2);
+/* Delete the slice in sequence object 'o' from 'i1' to 'i2'.
+   Returns -1 on failure.
 
-   /* Returns the sequence 'o' as a tuple on success, and NULL on failure.
+   This is the equivalent of the Python statement: del o[i1:i2]. */
+PyAPI_FUNC(int) PySequence_DelSlice(PyObject *o, Py_ssize_t i1, Py_ssize_t i2);
 
-      This is equivalent to the Python expression: tuple(o). */
-   PyAPI_FUNC(uint64_t) PySequence_Tuple(PyObject *o);
+/* Returns the sequence 'o' as a tuple on success, and NULL on failure.
 
-   /* Returns the sequence 'o' as a list on success, and NULL on failure.
-      This is equivalent to the Python expression: list(o) */
-   PyAPI_FUNC(uint64_t) PySequence_List(PyObject *o);
+   This is equivalent to the Python expression: tuple(o). */
+PyAPI_FUNC(uint64_t) PySequence_Tuple(PyObject *o);
 
-   /* Return the sequence 'o' as a list, unless it's already a tuple or list.
+/* Returns the sequence 'o' as a list on success, and NULL on failure.
+   This is equivalent to the Python expression: list(o) */
+PyAPI_FUNC(uint64_t) PySequence_List(PyObject *o);
 
-      Use PySequence_Fast_GET_ITEM to access the members of this list, and
-      PySequence_Fast_GET_SIZE to get its length.
+/* Return the sequence 'o' as a list, unless it's already a tuple or list.
 
-      Returns NULL on failure.  If the object does not support iteration, raises a
-      TypeError exception with 'm' as the message text. */
-   PyAPI_FUNC(uint64_t) PySequence_Fast(PyObject *o, const char *m);
+   Use PySequence_Fast_GET_ITEM to access the members of this list, and
+   PySequence_Fast_GET_SIZE to get its length.
+
+   Returns NULL on failure.  If the object does not support iteration, raises a
+   TypeError exception with 'm' as the message text. */
+PyAPI_FUNC(uint64_t) PySequence_Fast(PyObject *o, const char* m);
 
 /* Return the size of the sequence 'o', assuming that 'o' was returned by
    PySequence_Fast and is not NULL. */
 #define PySequence_Fast_GET_SIZE(o) \
-   (PyList_Check(o) ? PyList_GET_SIZE(o) : PyTuple_GET_SIZE(o))
+    (PyList_Check(o) ? PyList_GET_SIZE(o) : PyTuple_GET_SIZE(o))
 
 /* Return the 'i'-th element of the sequence 'o', assuming that o was returned
    by PySequence_Fast, and that i is within bounds. */
-#define PySequence_Fast_GET_ITEM(o, i) \
-   (PyList_Check(o) ? PyList_GET_ITEM(o, i) : PyTuple_GET_ITEM(o, i))
+#define PySequence_Fast_GET_ITEM(o, i)\
+     (PyList_Check(o) ? PyList_GET_ITEM(o, i) : PyTuple_GET_ITEM(o, i))
 
 /* Return a pointer to the underlying item array for
    an object returned by PySequence_Fast */
-#define PySequence_Fast_ITEMS(sf)                      \
-   (PyList_Check(sf) ? ((PyListObject *)(sf))->ob_item \
-                     : ((PyTupleObject *)(sf))->ob_item)
-
-   /* Return the number of occurrences on value on 'o', that is, return
-      the number of keys for which o[key] == value.
-
-      On failure, return -1.  This is equivalent to the Python expression:
-      o.count(value). */
-   PyAPI_FUNC(Py_ssize_t) PySequence_Count(PyObject *o, PyObject *value);
+#define PySequence_Fast_ITEMS(sf) \
+    (PyList_Check(sf) ? ((PyListObject *)(sf))->ob_item \
+                      : ((PyTupleObject *)(sf))->ob_item)
+
+/* Return the number of occurrences on value on 'o', that is, return
+   the number of keys for which o[key] == value.
+
+   On failure, return -1.  This is equivalent to the Python expression:
+   o.count(value). */
+PyAPI_FUNC(Py_ssize_t) PySequence_Count(PyObject *o, PyObject *value);
 
-   /* Return 1 if 'ob' is in the sequence 'seq'; 0 if 'ob' is not in the sequence
-      'seq'; -1 on error.
+/* Return 1 if 'ob' is in the sequence 'seq'; 0 if 'ob' is not in the sequence
+   'seq'; -1 on error.
 
-      Use __contains__ if possible, else _PySequence_IterSearch(). */
-   PyAPI_FUNC(int) PySequence_Contains(PyObject *seq, PyObject *ob);
+   Use __contains__ if possible, else _PySequence_IterSearch(). */
+PyAPI_FUNC(int) PySequence_Contains(PyObject *seq, PyObject *ob);
 
 /* For DLL-level backwards compatibility */
 #undef PySequence_In
-   /* Determine if the sequence 'o' contains 'value'. If an item in 'o' is equal
-      to 'value', return 1, otherwise return 0. On error, return -1.
+/* Determine if the sequence 'o' contains 'value'. If an item in 'o' is equal
+   to 'value', return 1, otherwise return 0. On error, return -1.
 
-      This is equivalent to the Python expression: value in o. */
-   PyAPI_FUNC(int) PySequence_In(PyObject *o, PyObject *value);
+   This is equivalent to the Python expression: value in o. */
+PyAPI_FUNC(int) PySequence_In(PyObject *o, PyObject *value);
 
 /* For source-level backwards compatibility */
 #define PySequence_In PySequence_Contains
 
-   /* Return the first index for which o[i] == value.
-      On error, return -1.
 
-      This is equivalent to the Python expression: o.index(value). */
-   PyAPI_FUNC(Py_ssize_t) PySequence_Index(PyObject *o, PyObject *value);
+/* Return the first index for which o[i] == value.
+   On error, return -1.
+
+   This is equivalent to the Python expression: o.index(value). */
+PyAPI_FUNC(Py_ssize_t) PySequence_Index(PyObject *o, PyObject *value);
 
-   /* --- In-place versions of some of the above Sequence functions --- */
 
-   /* Append sequence 'o2' to sequence 'o1', in-place when possible. Return the
-      resulting object, which could be 'o1', or NULL on failure.
+/* --- In-place versions of some of the above Sequence functions --- */
 
-     This is the equivalent of the Python expression: o1 += o2. */
-   PyAPI_FUNC(uint64_t) PySequence_InPlaceConcat(PyObject *o1, PyObject *o2);
+/* Append sequence 'o2' to sequence 'o1', in-place when possible. Return the
+   resulting object, which could be 'o1', or NULL on failure.
 
-   /* Repeat sequence 'o' by 'count', in-place when possible. Return the resulting
-      object, which could be 'o', or NULL on failure.
+  This is the equivalent of the Python expression: o1 += o2. */
+PyAPI_FUNC(uint64_t) PySequence_InPlaceConcat(PyObject *o1, PyObject *o2);
 
-      This is the equivalent of the Python expression: o1 *= count.  */
-   PyAPI_FUNC(uint64_t) PySequence_InPlaceRepeat(PyObject *o, Py_ssize_t count);
+/* Repeat sequence 'o' by 'count', in-place when possible. Return the resulting
+   object, which could be 'o', or NULL on failure.
 
-   /* === Mapping protocol ================================================= */
+   This is the equivalent of the Python expression: o1 *= count.  */
+PyAPI_FUNC(uint64_t) PySequence_InPlaceRepeat(PyObject *o, Py_ssize_t count);
 
-   /* Return 1 if the object provides mapping protocol, and 0 otherwise.
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyMapping_Check(PyObject *o);
+/* === Mapping protocol ================================================= */
 
-   /* Returns the number of keys in mapping object 'o' on success, and -1 on
-     failure. This is equivalent to the Python expression: len(o). */
-   PyAPI_FUNC(Py_ssize_t) PyMapping_Size(PyObject *o);
+/* Return 1 if the object provides mapping protocol, and 0 otherwise.
+
+   This function always succeeds. */
+PyAPI_FUNC(int) PyMapping_Check(PyObject *o);
+
+/* Returns the number of keys in mapping object 'o' on success, and -1 on
+  failure. This is equivalent to the Python expression: len(o). */
+PyAPI_FUNC(Py_ssize_t) PyMapping_Size(PyObject *o);
 
 /* For DLL compatibility */
 #undef PyMapping_Length
-   PyAPI_FUNC(Py_ssize_t) PyMapping_Length(PyObject *o);
+PyAPI_FUNC(Py_ssize_t) PyMapping_Length(PyObject *o);
 #define PyMapping_Length PyMapping_Size
 
+
 /* Implemented as a macro:
 
    int PyMapping_DelItemString(PyObject *o, const char *key);
 
    Remove the mapping for the string 'key' from the mapping 'o'. Returns -1 on
    failure.
 
    This is equivalent to the Python statement: del o[key]. */
-#define PyMapping_DelItemString(O, K) PyObject_DelItemString((O), (K))
+#define PyMapping_DelItemString(O,K) PyObject_DelItemString((O),(K))
 
 /* Implemented as a macro:
 
    int PyMapping_DelItem(PyObject *o, PyObject *key);
 
    Remove the mapping for the object 'key' from the mapping object 'o'.
    Returns -1 on failure.
 
    This is equivalent to the Python statement: del o[key]. */
-#define PyMapping_DelItem(O, K) PyObject_DelItem((O), (K))
+#define PyMapping_DelItem(O,K) PyObject_DelItem((O),(K))
 
-   /* On success, return 1 if the mapping object 'o' has the key 'key',
-      and 0 otherwise.
+/* On success, return 1 if the mapping object 'o' has the key 'key',
+   and 0 otherwise.
 
-      This is equivalent to the Python expression: key in o.
+   This is equivalent to the Python expression: key in o.
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyMapping_HasKeyString(PyObject *o, const char *key);
+   This function always succeeds. */
+PyAPI_FUNC(int) PyMapping_HasKeyString(PyObject *o, const char *key);
 
-   /* Return 1 if the mapping object has the key 'key', and 0 otherwise.
+/* Return 1 if the mapping object has the key 'key', and 0 otherwise.
 
-      This is equivalent to the Python expression: key in o.
+   This is equivalent to the Python expression: key in o.
 
-      This function always succeeds. */
-   PyAPI_FUNC(int) PyMapping_HasKey(PyObject *o, PyObject *key);
+   This function always succeeds. */
+PyAPI_FUNC(int) PyMapping_HasKey(PyObject *o, PyObject *key);
 
-   /* On success, return a list or tuple of the keys in mapping object 'o'.
-      On failure, return NULL. */
-   PyAPI_FUNC(uint64_t) PyMapping_Keys(PyObject *o);
+/* On success, return a list or tuple of the keys in mapping object 'o'.
+   On failure, return NULL. */
+PyAPI_FUNC(uint64_t) PyMapping_Keys(PyObject *o);
 
-   /* On success, return a list or tuple of the values in mapping object 'o'.
-      On failure, return NULL. */
-   PyAPI_FUNC(uint64_t) PyMapping_Values(PyObject *o);
+/* On success, return a list or tuple of the values in mapping object 'o'.
+   On failure, return NULL. */
+PyAPI_FUNC(uint64_t) PyMapping_Values(PyObject *o);
 
-   /* On success, return a list or tuple of the items in mapping object 'o',
-      where each item is a tuple containing a key-value pair. On failure, return
-      NULL. */
-   PyAPI_FUNC(uint64_t) PyMapping_Items(PyObject *o);
+/* On success, return a list or tuple of the items in mapping object 'o',
+   where each item is a tuple containing a key-value pair. On failure, return
+   NULL. */
+PyAPI_FUNC(uint64_t) PyMapping_Items(PyObject *o);
 
-   /* Return element of 'o' corresponding to the string 'key' or NULL on failure.
+/* Return element of 'o' corresponding to the string 'key' or NULL on failure.
 
-      This is the equivalent of the Python expression: o[key]. */
-   PyAPI_FUNC(uint64_t) PyMapping_GetItemString(PyObject *o,
-                                                const char *key);
+   This is the equivalent of the Python expression: o[key]. */
+PyAPI_FUNC(uint64_t) PyMapping_GetItemString(PyObject *o,
+                                               const char *key);
 
-   /* Map the string 'key' to the value 'v' in the mapping 'o'.
-      Returns -1 on failure.
+/* Map the string 'key' to the value 'v' in the mapping 'o'.
+   Returns -1 on failure.
 
-      This is the equivalent of the Python statement: o[key]=v. */
-   PyAPI_FUNC(int) PyMapping_SetItemString(PyObject *o, const char *key,
-                                           PyObject *value);
+   This is the equivalent of the Python statement: o[key]=v. */
+PyAPI_FUNC(int) PyMapping_SetItemString(PyObject *o, const char *key,
+                                        PyObject *value);
 
-   /* isinstance(object, typeorclass) */
-   PyAPI_FUNC(int) PyObject_IsInstance(PyObject *object, PyObject *typeorclass);
+/* isinstance(object, typeorclass) */
+PyAPI_FUNC(int) PyObject_IsInstance(PyObject *object, PyObject *typeorclass);
 
-   /* issubclass(object, typeorclass) */
-   PyAPI_FUNC(int) PyObject_IsSubclass(PyObject *object, PyObject *typeorclass);
+/* issubclass(object, typeorclass) */
+PyAPI_FUNC(int) PyObject_IsSubclass(PyObject *object, PyObject *typeorclass);
 
 #ifndef Py_LIMITED_API
-#define Py_CPYTHON_ABSTRACTOBJECT_H
-#include "cpython/abstract.h"
-#undef Py_CPYTHON_ABSTRACTOBJECT_H
+#  define Py_CPYTHON_ABSTRACTOBJECT_H
+#  include "cpython/abstract.h"
+#  undef Py_CPYTHON_ABSTRACTOBJECT_H
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 #endif /* Py_ABSTRACTOBJECT_H */
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/boolobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/codecs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/complexobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/cellobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/classobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/complexobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/descrobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/frameobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/funcobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/genobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/longintrepr.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/longobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/modsupport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/odictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/picklebufobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pthread_stubs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyctype.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pydebug.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pyframe.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pythread.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/pytime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/setobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/cpython/weakrefobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/datetime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/descrobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/dynamic_annotations.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/errcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/exports.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_accu.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_asdl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ast_state.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_atomic.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bitutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_call.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_condvar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_dict.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_dtoa.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_exceptions.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_frame.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_gc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_genobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_gil.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_global_objects.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_global_strings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_hamt.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_hashtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_interp.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_list.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_long.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_opcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_parser.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pathconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pyarena.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pymath.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_runtime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_runtime_init.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_signal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_strhex.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_structseq.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_symtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_tuple.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_typeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_ucnhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_unionobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/internal/pycore_warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/intrcheck.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/iterobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/longobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/marshal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/memoryobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/modsupport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/opcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/osdefs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/patchlevel.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/py_curses.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pybuffer.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pycapsule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pydtrace.d` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pydtrace.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyexpat.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyframe.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymacconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymacro.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymath.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pyport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pystrtod.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pythread.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/pytypedefs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/rangeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/setobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/sliceobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/structmember.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/structseq.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/token.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/tracemalloc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/typeslots.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/unicodeobject.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_UNICODEOBJECT_H
 #define Py_UNICODEOBJECT_H
 
-#include <stdarg.h>               // va_list
+#include <stdarg.h>
 
 /*
 
 Unicode implementation based on original code by Fredrik Lundh,
 modified by Marc-Andre Lemburg (mal@lemburg.com) according to the
 Unicode Integration Proposal. (See
 http://www.egenix.com/files/python/unicode-proposal.txt).
@@ -108,16 +108,16 @@
 #endif
 
 
 PyAPI_DATA(PyTypeObject) PyUnicode_Type;
 PyAPI_DATA(PyTypeObject) PyUnicodeIter_Type;
 
 #define PyUnicode_Check(op) \
-    PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
-#define PyUnicode_CheckExact(op) Py_IS_TYPE(op, &PyUnicode_Type)
+                 PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
+#define PyUnicode_CheckExact(op) (Py_TYPE(op) == &PyUnicode_Type)
 
 /* --- Constants ---------------------------------------------------------- */
 
 /* This Unicode character will be used as replacement character during
    decoding if the errors argument is set to "replace". Note: the
    Unicode character U+FFFD is the official REPLACEMENT CHARACTER in
    Unicode 3.0. */
@@ -147,24 +147,24 @@
 
 #if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
 /* Copy the string into a UCS4 buffer including the null character if copy_null
    is set. Return NULL and raise an exception on error. Raise a SystemError if
    the buffer is smaller than the string. Return buffer on success.
 
    buflen is the length of the buffer in (Py_UCS4) characters. */
-PyAPI_FUNC(uint64_t) PyUnicode_AsUCS4(
+PyAPI_FUNC(uint64_t)) PyUnicode_AsUCS4(
     PyObject *unicode,
     Py_UCS4* buffer,
     Py_ssize_t buflen,
     int copy_null);
 
 /* Copy the string into a UCS4 buffer. A new buffer is allocated using
  * PyMem_Malloc; if this fails, NULL is returned with a memory error
    exception set. */
-PyAPI_FUNC(uint64_t) PyUnicode_AsUCS4Copy(PyObject *unicode);
+PyAPI_FUNC(uint64_t)) PyUnicode_AsUCS4Copy(PyObject *unicode);
 #endif
 
 #if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
 /* Get the length of the Unicode object. */
 
 PyAPI_FUNC(Py_ssize_t) PyUnicode_GetLength(
     PyObject *unicode
@@ -257,21 +257,22 @@
     );
 PyAPI_FUNC(uint64_t) PyUnicode_FromFormat(
     const char *format,   /* ASCII-encoded string  */
     ...
     );
 
 PyAPI_FUNC(void) PyUnicode_InternInPlace(PyObject **);
+PyAPI_FUNC(void) PyUnicode_InternImmortal(PyObject **);
 PyAPI_FUNC(uint64_t) PyUnicode_InternFromString(
     const char *u              /* UTF-8 encoded string */
     );
 
-// PyUnicode_InternImmortal() is deprecated since Python 3.10
-// and will be removed in Python 3.12. Use PyUnicode_InternInPlace() instead.
-Py_DEPRECATED(3.10) PyAPI_FUNC(void) PyUnicode_InternImmortal(PyObject **);
+/* Use only if you know it's a string */
+#define PyUnicode_CHECK_INTERNED(op) \
+    (((PyASCIIObject *)(op))->state.interned)
 
 /* --- wchar_t support for platforms which support it --------------------- */
 
 #ifdef HAVE_WCHAR_H
 
 /* Create a Unicode Object from the wchar_t buffer w of the given
    size.
@@ -323,14 +324,25 @@
    The ordinal must be in range(0x110000). A ValueError is
    raised in case it is not.
 
 */
 
 PyAPI_FUNC(uint64_t) PyUnicode_FromOrdinal(int ordinal);
 
+/* --- Free-list management ----------------------------------------------- */
+
+/* Clear the free list used by the Unicode implementation.
+
+   This can be used to release memory used for objects on the free
+   list back to the Python memory allocator.
+
+*/
+
+PyAPI_FUNC(int) PyUnicode_ClearFreeList(void);
+
 /* === Builtin Codecs =====================================================
 
    Many of these APIs take two arguments encoding and errors. These
    parameters encoding and errors have the same semantics as the ones
    of the builtin str() API.
 
    Setting encoding to NULL causes the default encoding (UTF-8) to be used.
@@ -460,31 +472,14 @@
     Py_ssize_t *consumed        /* bytes consumed */
     );
 
 PyAPI_FUNC(uint64_t) PyUnicode_AsUTF8String(
     PyObject *unicode           /* Unicode object */
     );
 
-/* Returns a pointer to the default encoding (UTF-8) of the
-   Unicode object unicode and the size of the encoded representation
-   in bytes stored in *size.
-
-   In case of an error, no *size is set.
-
-   This function caches the UTF-8 encoded string in the unicodeobject
-   and subsequent calls will return the same string.  The memory is released
-   when the unicodeobject is deallocated.
-*/
-
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x030A0000
-PyAPI_FUNC(uint64_t) PyUnicode_AsUTF8AndSize(
-    PyObject *unicode,
-    Py_ssize_t *size);
-#endif
-
 /* --- UTF-32 Codecs ------------------------------------------------------ */
 
 /* Decodes length bytes from a UTF-32 encoded buffer string and returns
    the corresponding Unicode object.
 
    errors (if non-NULL) defines the error handling. It defaults
    to "strict".
@@ -1035,15 +1030,15 @@
 
 PyAPI_FUNC(int) PyUnicode_IsIdentifier(PyObject *s);
 
 /* === Characters Type APIs =============================================== */
 
 #ifndef Py_LIMITED_API
 #  define Py_CPYTHON_UNICODEOBJECT_H
-#  include "cpython/unicodeobject.h"
+#  include  "cpython/unicodeobject.h"
 #  undef Py_CPYTHON_UNICODEOBJECT_H
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 #endif /* !Py_UNICODEOBJECT_H */
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp311/weakrefobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/LICENSE` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/Python-ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/Python.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/asdl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/boolobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytes_methods.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cellobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/classobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/codecs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/complexobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/cpython/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/datetime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/descrobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/dynamic_annotations.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/errcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/eval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/frameobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/funcobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/genobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/graminit.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/grammar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_accu.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_atomic.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_condvar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_gil.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_hamt.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_long.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pathconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/internal/pycore_warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/intrcheck.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/iterobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/longintrepr.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/longobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/marshal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/memoryobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/modsupport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/node.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/odictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/opcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/osdefs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/parsetok.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/patchlevel.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/picklebufobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/py_curses.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyarena.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pycapsule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyctype.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydebug.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydtrace.d` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pydtrace.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyexpat.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymacconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymacro.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymath.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pyport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystrhex.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pystrtod.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pythread.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/pytime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/rangeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/setobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/sliceobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/structmember.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/structseq.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/symtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/token.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/tracemalloc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/typeslots.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/ucnhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/unicodeobject.h`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 PyAPI_DATA(PyTypeObject) PyUnicode_Type;
 PyAPI_DATA(PyTypeObject) PyUnicodeIter_Type;
 
 #define PyUnicode_Check(op) \
                  PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
-#define PyUnicode_CheckExact(op) (Py_TYPE(op) == &PyUnicode_Type)
+#define PyUnicode_CheckExact(op) Py_IS_TYPE(op, &PyUnicode_Type)
 
 /* --- Constants ---------------------------------------------------------- */
 
 /* This Unicode character will be used as replacement character during
    decoding if the errors argument is set to "replace". Note: the
    Unicode character U+FFFD is the official REPLACEMENT CHARACTER in
    Unicode 3.0. */
@@ -324,25 +324,14 @@
    The ordinal must be in range(0x110000). A ValueError is
    raised in case it is not.
 
 */
 
 PyAPI_FUNC(uint64_t) PyUnicode_FromOrdinal(int ordinal);
 
-/* --- Free-list management ----------------------------------------------- */
-
-/* Clear the free list used by the Unicode implementation.
-
-   This can be used to release memory used for objects on the free
-   list back to the Python memory allocator.
-
-*/
-
-PyAPI_FUNC(int) PyUnicode_ClearFreeList(void);
-
 /* === Builtin Codecs =====================================================
 
    Many of these APIs take two arguments encoding and errors. These
    parameters encoding and errors have the same semantics as the ones
    of the builtin str() API.
 
    Setting encoding to NULL causes the default encoding (UTF-8) to be used.
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp38/weakrefobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp38/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/LICENSE` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/Python-ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/Python.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/asdl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/ast.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/boolobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cellobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/classobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/codecs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/compile.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/complexobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/abstract.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/bytearrayobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/bytesobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/frameobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/cpython/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/datetime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/descrobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/dictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/dynamic_annotations.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/errcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/eval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/exports.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/fileobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/floatobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/funcobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/genobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/graminit.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/grammar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/import.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pegen_interface.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pegen_interface.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_accu.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_atomic.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_byteswap.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_call.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_ceval.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_code.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_condvar.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_context.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_dtoa.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_fileutils.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_gc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_gil.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_hamt.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_hashtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_initconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_interp.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_long.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pathconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_runtime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/internal/pycore_warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/intrcheck.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/iterobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/listobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/longintrepr.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/longobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/marshal.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/memoryobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/methodobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/modsupport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/moduleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/node.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/object.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/objimpl.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/odictobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/opcode.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/osdefs.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/parsetok.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/patchlevel.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/picklebufobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/py_curses.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyarena.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pycapsule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyctype.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydebug.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydtrace.d` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pydtrace.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyerrors.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyexpat.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pylifecycle.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymacconfig.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymacro.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymath.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pymem.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pyport.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystate.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystrhex.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pystrtod.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pythonrun.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pythread.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/pytime.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/rangeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/setobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/sliceobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/structmember.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/structseq.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/symtable.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/sysmodule.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/token.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/traceback.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/tracemalloc.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/tupleobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/typeslots.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/ucnhash.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/unicodeobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp311/unicodeobject.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_UNICODEOBJECT_H
 #define Py_UNICODEOBJECT_H
 
-#include <stdarg.h>
+#include <stdarg.h> // va_list
 
 /*
 
 Unicode implementation based on original code by Fredrik Lundh,
 modified by Marc-Andre Lemburg (mal@lemburg.com) according to the
 Unicode Integration Proposal. (See
 http://www.egenix.com/files/python/unicode-proposal.txt).
@@ -84,950 +84,958 @@
 /* #define HAVE_USABLE_WCHAR_T */
 
 /* If the compiler provides a wchar_t type we try to support it
    through the interface functions PyUnicode_FromWideChar(),
    PyUnicode_AsWideChar() and PyUnicode_AsWideCharString(). */
 
 #ifdef HAVE_USABLE_WCHAR_T
-# ifndef HAVE_WCHAR_H
-#  define HAVE_WCHAR_H
-# endif
+#ifndef HAVE_WCHAR_H
+#define HAVE_WCHAR_H
+#endif
 #endif
 
 #ifdef HAVE_WCHAR_H
-#  include <wchar.h>
+#include <wchar.h>
 #endif
 
 /* Py_UCS4 and Py_UCS2 are typedefs for the respective
    unicode representations. */
 typedef uint32_t Py_UCS4;
 typedef uint16_t Py_UCS2;
 typedef uint8_t Py_UCS1;
 
 #ifdef __cplusplus
-extern "C" {
+extern "C"
+{
 #endif
 
-
-PyAPI_DATA(PyTypeObject) PyUnicode_Type;
-PyAPI_DATA(PyTypeObject) PyUnicodeIter_Type;
+    PyAPI_DATA(PyTypeObject) PyUnicode_Type;
+    PyAPI_DATA(PyTypeObject) PyUnicodeIter_Type;
 
 #define PyUnicode_Check(op) \
-                 PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
+    PyType_FastSubclass(Py_TYPE(op), Py_TPFLAGS_UNICODE_SUBCLASS)
 #define PyUnicode_CheckExact(op) Py_IS_TYPE(op, &PyUnicode_Type)
 
-/* --- Constants ---------------------------------------------------------- */
+    /* --- Constants ---------------------------------------------------------- */
 
-/* This Unicode character will be used as replacement character during
-   decoding if the errors argument is set to "replace". Note: the
-   Unicode character U+FFFD is the official REPLACEMENT CHARACTER in
-   Unicode 3.0. */
+    /* This Unicode character will be used as replacement character during
+       decoding if the errors argument is set to "replace". Note: the
+       Unicode character U+FFFD is the official REPLACEMENT CHARACTER in
+       Unicode 3.0. */
 
-#define Py_UNICODE_REPLACEMENT_CHARACTER ((Py_UCS4) 0xFFFD)
+#define Py_UNICODE_REPLACEMENT_CHARACTER ((Py_UCS4)0xFFFD)
 
-/* === Public API ========================================================= */
+    /* === Public API ========================================================= */
 
-/* Similar to PyUnicode_FromUnicode(), but u points to UTF-8 encoded bytes */
-PyAPI_FUNC(uint64_t) PyUnicode_FromStringAndSize(
-    const char *u,             /* UTF-8 encoded string */
-    Py_ssize_t size            /* size of buffer */
+    /* Similar to PyUnicode_FromUnicode(), but u points to UTF-8 encoded bytes */
+    PyAPI_FUNC(uint64_t) PyUnicode_FromStringAndSize(
+        const char *u,  /* UTF-8 encoded string */
+        Py_ssize_t size /* size of buffer */
     );
 
-/* Similar to PyUnicode_FromUnicode(), but u points to null-terminated
-   UTF-8 encoded bytes.  The size is determined with strlen(). */
-PyAPI_FUNC(uint64_t) PyUnicode_FromString(
-    const char *u              /* UTF-8 encoded string */
+    /* Similar to PyUnicode_FromUnicode(), but u points to null-terminated
+       UTF-8 encoded bytes.  The size is determined with strlen(). */
+    PyAPI_FUNC(uint64_t) PyUnicode_FromString(
+        const char *u /* UTF-8 encoded string */
     );
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-PyAPI_FUNC(uint64_t) PyUnicode_Substring(
-    PyObject *str,
-    Py_ssize_t start,
-    Py_ssize_t end);
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    PyAPI_FUNC(uint64_t) PyUnicode_Substring(
+        PyObject *str,
+        Py_ssize_t start,
+        Py_ssize_t end);
 #endif
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-/* Copy the string into a UCS4 buffer including the null character if copy_null
-   is set. Return NULL and raise an exception on error. Raise a SystemError if
-   the buffer is smaller than the string. Return buffer on success.
-
-   buflen is the length of the buffer in (Py_UCS4) characters. */
-PyAPI_FUNC(uint64_t)) PyUnicode_AsUCS4(
-    PyObject *unicode,
-    Py_UCS4* buffer,
-    Py_ssize_t buflen,
-    int copy_null);
-
-/* Copy the string into a UCS4 buffer. A new buffer is allocated using
- * PyMem_Malloc; if this fails, NULL is returned with a memory error
-   exception set. */
-PyAPI_FUNC(uint64_t)) PyUnicode_AsUCS4Copy(PyObject *unicode);
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    /* Copy the string into a UCS4 buffer including the null character if copy_null
+       is set. Return NULL and raise an exception on error. Raise a SystemError if
+       the buffer is smaller than the string. Return buffer on success.
+
+       buflen is the length of the buffer in (Py_UCS4) characters. */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUCS4(
+        PyObject *unicode,
+        Py_UCS4 *buffer,
+        Py_ssize_t buflen,
+        int copy_null);
+
+    /* Copy the string into a UCS4 buffer. A new buffer is allocated using
+     * PyMem_Malloc; if this fails, NULL is returned with a memory error
+       exception set. */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUCS4Copy(PyObject *unicode);
 #endif
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-/* Get the length of the Unicode object. */
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    /* Get the length of the Unicode object. */
 
-PyAPI_FUNC(Py_ssize_t) PyUnicode_GetLength(
-    PyObject *unicode
-);
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_GetLength(
+        PyObject *unicode);
 #endif
 
-/* Get the number of Py_UNICODE units in the
-   string representation. */
+    /* Get the number of Py_UNICODE units in the
+       string representation. */
 
-Py_DEPRECATED(3.3) PyAPI_FUNC(Py_ssize_t) PyUnicode_GetSize(
-    PyObject *unicode           /* Unicode object */
+    Py_DEPRECATED(3.3) PyAPI_FUNC(Py_ssize_t) PyUnicode_GetSize(
+        PyObject *unicode /* Unicode object */
     );
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-/* Read a character from the string. */
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    /* Read a character from the string. */
 
-PyAPI_FUNC(Py_UCS4) PyUnicode_ReadChar(
-    PyObject *unicode,
-    Py_ssize_t index
-    );
+    PyAPI_FUNC(Py_UCS4) PyUnicode_ReadChar(
+        PyObject *unicode,
+        Py_ssize_t index);
 
-/* Write a character to the string. The string must have been created through
-   PyUnicode_New, must not be shared, and must not have been hashed yet.
+    /* Write a character to the string. The string must have been created through
+       PyUnicode_New, must not be shared, and must not have been hashed yet.
 
-   Return 0 on success, -1 on error. */
+       Return 0 on success, -1 on error. */
 
-PyAPI_FUNC(int) PyUnicode_WriteChar(
-    PyObject *unicode,
-    Py_ssize_t index,
-    Py_UCS4 character
-    );
+    PyAPI_FUNC(int) PyUnicode_WriteChar(
+        PyObject *unicode,
+        Py_ssize_t index,
+        Py_UCS4 character);
 #endif
 
-/* Resize a Unicode object. The length is the number of characters, except
-   if the kind of the string is PyUnicode_WCHAR_KIND: in this case, the length
-   is the number of Py_UNICODE characters.
+    /* Resize a Unicode object. The length is the number of characters, except
+       if the kind of the string is PyUnicode_WCHAR_KIND: in this case, the length
+       is the number of Py_UNICODE characters.
 
-   *unicode is modified to point to the new (resized) object and 0
-   returned on success.
+       *unicode is modified to point to the new (resized) object and 0
+       returned on success.
 
-   Try to resize the string in place (which is usually faster than allocating
-   a new string and copy characters), or create a new string.
+       Try to resize the string in place (which is usually faster than allocating
+       a new string and copy characters), or create a new string.
 
-   Error handling is implemented as follows: an exception is set, -1
-   is returned and *unicode left untouched.
+       Error handling is implemented as follows: an exception is set, -1
+       is returned and *unicode left untouched.
 
-   WARNING: The function doesn't check string content, the result may not be a
-            string in canonical representation. */
+       WARNING: The function doesn't check string content, the result may not be a
+                string in canonical representation. */
 
-PyAPI_FUNC(int) PyUnicode_Resize(
-    PyObject **unicode,         /* Pointer to the Unicode object */
-    Py_ssize_t length           /* New length */
+    PyAPI_FUNC(int) PyUnicode_Resize(
+        PyObject **unicode, /* Pointer to the Unicode object */
+        Py_ssize_t length   /* New length */
     );
 
-/* Decode obj to a Unicode object.
+    /* Decode obj to a Unicode object.
 
-   bytes, bytearray and other bytes-like objects are decoded according to the
-   given encoding and error handler. The encoding and error handler can be
-   NULL to have the interface use UTF-8 and "strict".
+       bytes, bytearray and other bytes-like objects are decoded according to the
+       given encoding and error handler. The encoding and error handler can be
+       NULL to have the interface use UTF-8 and "strict".
 
-   All other objects (including Unicode objects) raise an exception.
+       All other objects (including Unicode objects) raise an exception.
 
-   The API returns NULL in case of an error. The caller is responsible
-   for decref'ing the returned objects.
+       The API returns NULL in case of an error. The caller is responsible
+       for decref'ing the returned objects.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_FromEncodedObject(
-    PyObject *obj,              /* Object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_FromEncodedObject(
+        PyObject *obj,        /* Object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Copy an instance of a Unicode subtype to a new true Unicode object if
-   necessary. If obj is already a true Unicode object (not a subtype), return
-   the reference with *incremented* refcount.
+    /* Copy an instance of a Unicode subtype to a new true Unicode object if
+       necessary. If obj is already a true Unicode object (not a subtype), return
+       the reference with *incremented* refcount.
 
-   The API returns NULL in case of an error. The caller is responsible
-   for decref'ing the returned objects.
+       The API returns NULL in case of an error. The caller is responsible
+       for decref'ing the returned objects.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_FromObject(
-    PyObject *obj      /* Object */
+    PyAPI_FUNC(uint64_t) PyUnicode_FromObject(
+        PyObject *obj /* Object */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_FromFormatV(
-    const char *format,   /* ASCII-encoded string  */
-    va_list vargs
-    );
-PyAPI_FUNC(uint64_t) PyUnicode_FromFormat(
-    const char *format,   /* ASCII-encoded string  */
-    ...
-    );
+    PyAPI_FUNC(uint64_t) PyUnicode_FromFormatV(
+        const char *format, /* ASCII-encoded string  */
+        va_list vargs);
+    PyAPI_FUNC(uint64_t) PyUnicode_FromFormat(
+        const char *format, /* ASCII-encoded string  */
+        ...);
 
-PyAPI_FUNC(void) PyUnicode_InternInPlace(PyObject **);
-PyAPI_FUNC(void) PyUnicode_InternImmortal(PyObject **);
-PyAPI_FUNC(uint64_t) PyUnicode_InternFromString(
-    const char *u              /* UTF-8 encoded string */
+    PyAPI_FUNC(void) PyUnicode_InternInPlace(PyObject **);
+    PyAPI_FUNC(uint64_t) PyUnicode_InternFromString(
+        const char *u /* UTF-8 encoded string */
     );
 
-/* Use only if you know it's a string */
-#define PyUnicode_CHECK_INTERNED(op) \
-    (((PyASCIIObject *)(op))->state.interned)
+    // PyUnicode_InternImmortal() is deprecated since Python 3.10
+    // and will be removed in Python 3.12. Use PyUnicode_InternInPlace() instead.
+    Py_DEPRECATED(3.10) PyAPI_FUNC(void) PyUnicode_InternImmortal(PyObject **);
 
-/* --- wchar_t support for platforms which support it --------------------- */
+    /* --- wchar_t support for platforms which support it --------------------- */
 
 #ifdef HAVE_WCHAR_H
 
-/* Create a Unicode Object from the wchar_t buffer w of the given
-   size.
+    /* Create a Unicode Object from the wchar_t buffer w of the given
+       size.
 
-   The buffer is copied into the new object. */
+       The buffer is copied into the new object. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_FromWideChar(
-    const wchar_t *w,           /* wchar_t buffer */
-    Py_ssize_t size             /* size of buffer */
+    PyAPI_FUNC(uint64_t) PyUnicode_FromWideChar(
+        const wchar_t *w, /* wchar_t buffer */
+        Py_ssize_t size   /* size of buffer */
     );
 
-/* Copies the Unicode Object contents into the wchar_t buffer w.  At
-   most size wchar_t characters are copied.
+    /* Copies the Unicode Object contents into the wchar_t buffer w.  At
+       most size wchar_t characters are copied.
 
-   Note that the resulting wchar_t string may or may not be
-   0-terminated.  It is the responsibility of the caller to make sure
-   that the wchar_t string is 0-terminated in case this is required by
-   the application.
+       Note that the resulting wchar_t string may or may not be
+       0-terminated.  It is the responsibility of the caller to make sure
+       that the wchar_t string is 0-terminated in case this is required by
+       the application.
 
-   Returns the number of wchar_t characters copied (excluding a
-   possibly trailing 0-termination character) or -1 in case of an
-   error. */
+       Returns the number of wchar_t characters copied (excluding a
+       possibly trailing 0-termination character) or -1 in case of an
+       error. */
 
-PyAPI_FUNC(Py_ssize_t) PyUnicode_AsWideChar(
-    PyObject *unicode,          /* Unicode object */
-    wchar_t *w,                 /* wchar_t buffer */
-    Py_ssize_t size             /* size of buffer */
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_AsWideChar(
+        PyObject *unicode, /* Unicode object */
+        wchar_t *w,        /* wchar_t buffer */
+        Py_ssize_t size    /* size of buffer */
     );
 
-/* Convert the Unicode object to a wide character string. The output string
-   always ends with a nul character. If size is not NULL, write the number of
-   wide characters (excluding the null character) into *size.
+    /* Convert the Unicode object to a wide character string. The output string
+       always ends with a nul character. If size is not NULL, write the number of
+       wide characters (excluding the null character) into *size.
 
-   Returns a buffer allocated by PyMem_Malloc() (use PyMem_Free() to free it)
-   on success. On error, returns NULL, *size is undefined and raises a
-   MemoryError. */
+       Returns a buffer allocated by PyMem_Malloc() (use PyMem_Free() to free it)
+       on success. On error, returns NULL, *size is undefined and raises a
+       MemoryError. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsWideCharString(
-    PyObject *unicode,          /* Unicode object */
-    Py_ssize_t *size            /* number of characters of the result */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsWideCharString(
+        PyObject *unicode, /* Unicode object */
+        Py_ssize_t *size   /* number of characters of the result */
     );
 
 #endif
 
-/* --- Unicode ordinals --------------------------------------------------- */
+    /* --- Unicode ordinals --------------------------------------------------- */
 
-/* Create a Unicode Object from the given Unicode code point ordinal.
+    /* Create a Unicode Object from the given Unicode code point ordinal.
 
-   The ordinal must be in range(0x110000). A ValueError is
-   raised in case it is not.
+       The ordinal must be in range(0x110000). A ValueError is
+       raised in case it is not.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_FromOrdinal(int ordinal);
+    PyAPI_FUNC(uint64_t) PyUnicode_FromOrdinal(int ordinal);
 
-/* === Builtin Codecs =====================================================
+    /* === Builtin Codecs =====================================================
 
-   Many of these APIs take two arguments encoding and errors. These
-   parameters encoding and errors have the same semantics as the ones
-   of the builtin str() API.
+       Many of these APIs take two arguments encoding and errors. These
+       parameters encoding and errors have the same semantics as the ones
+       of the builtin str() API.
 
-   Setting encoding to NULL causes the default encoding (UTF-8) to be used.
+       Setting encoding to NULL causes the default encoding (UTF-8) to be used.
 
-   Error handling is set by errors which may also be set to NULL
-   meaning to use the default handling defined for the codec. Default
-   error handling for all builtin codecs is "strict" (ValueErrors are
-   raised).
+       Error handling is set by errors which may also be set to NULL
+       meaning to use the default handling defined for the codec. Default
+       error handling for all builtin codecs is "strict" (ValueErrors are
+       raised).
 
-   The codecs all use a similar interface. Only deviation from the
-   generic ones are documented.
+       The codecs all use a similar interface. Only deviation from the
+       generic ones are documented.
 
-*/
+    */
 
-/* --- Manage the default encoding ---------------------------------------- */
+    /* --- Manage the default encoding ---------------------------------------- */
 
-/* Returns "utf-8".  */
-PyAPI_FUNC(uint64_t) PyUnicode_GetDefaultEncoding(void);
+    /* Returns "utf-8".  */
+    PyAPI_FUNC(uint64_t) PyUnicode_GetDefaultEncoding(void);
 
-/* --- Generic Codecs ----------------------------------------------------- */
+    /* --- Generic Codecs ----------------------------------------------------- */
 
-/* Create a Unicode object by decoding the encoded string s of the
-   given size. */
+    /* Create a Unicode object by decoding the encoded string s of the
+       given size. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Decode(
-    const char *s,              /* encoded string */
-    Py_ssize_t size,            /* size of buffer */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_Decode(
+        const char *s,        /* encoded string */
+        Py_ssize_t size,      /* size of buffer */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Decode a Unicode object unicode and return the result as Python
-   object.
+    /* Decode a Unicode object unicode and return the result as Python
+       object.
 
-   This API is DEPRECATED. The only supported standard encoding is rot13.
-   Use PyCodec_Decode() to decode with rot13 and non-standard codecs
-   that decode from str. */
+       This API is DEPRECATED. The only supported standard encoding is rot13.
+       Use PyCodec_Decode() to decode with rot13 and non-standard codecs
+       that decode from str. */
 
-Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsDecodedObject(
-    PyObject *unicode,          /* Unicode object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsDecodedObject(
+        PyObject *unicode,    /* Unicode object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Decode a Unicode object unicode and return the result as Unicode
-   object.
+    /* Decode a Unicode object unicode and return the result as Unicode
+       object.
 
-   This API is DEPRECATED. The only supported standard encoding is rot13.
-   Use PyCodec_Decode() to decode with rot13 and non-standard codecs
-   that decode from str to str. */
+       This API is DEPRECATED. The only supported standard encoding is rot13.
+       Use PyCodec_Decode() to decode with rot13 and non-standard codecs
+       that decode from str to str. */
 
-Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsDecodedUnicode(
-    PyObject *unicode,          /* Unicode object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsDecodedUnicode(
+        PyObject *unicode,    /* Unicode object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Encodes a Unicode object and returns the result as Python
-   object.
+    /* Encodes a Unicode object and returns the result as Python
+       object.
 
-   This API is DEPRECATED.  It is superseded by PyUnicode_AsEncodedString()
-   since all standard encodings (except rot13) encode str to bytes.
-   Use PyCodec_Encode() for encoding with rot13 and non-standard codecs
-   that encode form str to non-bytes. */
+       This API is DEPRECATED.  It is superseded by PyUnicode_AsEncodedString()
+       since all standard encodings (except rot13) encode str to bytes.
+       Use PyCodec_Encode() for encoding with rot13 and non-standard codecs
+       that encode form str to non-bytes. */
 
-Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedObject(
-    PyObject *unicode,          /* Unicode object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedObject(
+        PyObject *unicode,    /* Unicode object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Encodes a Unicode object and returns the result as Python string
-   object. */
+    /* Encodes a Unicode object and returns the result as Python string
+       object. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedString(
-    PyObject *unicode,          /* Unicode object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedString(
+        PyObject *unicode,    /* Unicode object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Encodes a Unicode object and returns the result as Unicode
-   object.
+    /* Encodes a Unicode object and returns the result as Unicode
+       object.
 
-   This API is DEPRECATED.  The only supported standard encodings is rot13.
-   Use PyCodec_Encode() to encode with rot13 and non-standard codecs
-   that encode from str to str. */
+       This API is DEPRECATED.  The only supported standard encodings is rot13.
+       Use PyCodec_Encode() to encode with rot13 and non-standard codecs
+       that encode from str to str. */
 
-Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedUnicode(
-    PyObject *unicode,          /* Unicode object */
-    const char *encoding,       /* encoding */
-    const char *errors          /* error handling */
+    Py_DEPRECATED(3.6) PyAPI_FUNC(uint64_t) PyUnicode_AsEncodedUnicode(
+        PyObject *unicode,    /* Unicode object */
+        const char *encoding, /* encoding */
+        const char *errors    /* error handling */
     );
 
-/* Build an encoding map. */
+    /* Build an encoding map. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_BuildEncodingMap(
-    PyObject* string            /* 256 character map */
-   );
+    PyAPI_FUNC(uint64_t) PyUnicode_BuildEncodingMap(
+        PyObject *string /* 256 character map */
+    );
 
-/* --- UTF-7 Codecs ------------------------------------------------------- */
+    /* --- UTF-7 Codecs ------------------------------------------------------- */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF7(
-    const char *string,         /* UTF-7 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF7(
+        const char *string, /* UTF-7 encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF7Stateful(
-    const char *string,         /* UTF-7 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    Py_ssize_t *consumed        /* bytes consumed */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF7Stateful(
+        const char *string,  /* UTF-7 encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        Py_ssize_t *consumed /* bytes consumed */
     );
 
-/* --- UTF-8 Codecs ------------------------------------------------------- */
+    /* --- UTF-8 Codecs ------------------------------------------------------- */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF8(
-    const char *string,         /* UTF-8 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF8(
+        const char *string, /* UTF-8 encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF8Stateful(
-    const char *string,         /* UTF-8 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    Py_ssize_t *consumed        /* bytes consumed */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF8Stateful(
+        const char *string,  /* UTF-8 encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        Py_ssize_t *consumed /* bytes consumed */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsUTF8String(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUTF8String(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- UTF-32 Codecs ------------------------------------------------------ */
+    /* Returns a pointer to the default encoding (UTF-8) of the
+       Unicode object unicode and the size of the encoded representation
+       in bytes stored in *size.
 
-/* Decodes length bytes from a UTF-32 encoded buffer string and returns
-   the corresponding Unicode object.
+       In case of an error, no *size is set.
 
-   errors (if non-NULL) defines the error handling. It defaults
-   to "strict".
+       This function caches the UTF-8 encoded string in the unicodeobject
+       and subsequent calls will return the same string.  The memory is released
+       when the unicodeobject is deallocated.
+    */
 
-   If byteorder is non-NULL, the decoder starts decoding using the
-   given byte order:
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x030A0000
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUTF8AndSize(
+        PyObject *unicode,
+        Py_ssize_t *size);
+#endif
 
-    *byteorder == -1: little endian
-    *byteorder == 0:  native order
-    *byteorder == 1:  big endian
+    /* --- UTF-32 Codecs ------------------------------------------------------ */
 
-   In native mode, the first four bytes of the stream are checked for a
-   BOM mark. If found, the BOM mark is analysed, the byte order
-   adjusted and the BOM skipped.  In the other modes, no BOM mark
-   interpretation is done. After completion, *byteorder is set to the
-   current byte order at the end of input data.
+    /* Decodes length bytes from a UTF-32 encoded buffer string and returns
+       the corresponding Unicode object.
 
-   If byteorder is NULL, the codec starts in native order mode.
+       errors (if non-NULL) defines the error handling. It defaults
+       to "strict".
 
-*/
+       If byteorder is non-NULL, the decoder starts decoding using the
+       given byte order:
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF32(
-    const char *string,         /* UTF-32 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    int *byteorder              /* pointer to byteorder to use
-                                   0=native;-1=LE,1=BE; updated on
-                                   exit */
+        *byteorder == -1: little endian
+        *byteorder == 0:  native order
+        *byteorder == 1:  big endian
+
+       In native mode, the first four bytes of the stream are checked for a
+       BOM mark. If found, the BOM mark is analysed, the byte order
+       adjusted and the BOM skipped.  In the other modes, no BOM mark
+       interpretation is done. After completion, *byteorder is set to the
+       current byte order at the end of input data.
+
+       If byteorder is NULL, the codec starts in native order mode.
+
+    */
+
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF32(
+        const char *string, /* UTF-32 encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors, /* error handling */
+        int *byteorder      /* pointer to byteorder to use
+                               0=native;-1=LE,1=BE; updated on
+                               exit */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF32Stateful(
-    const char *string,         /* UTF-32 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    int *byteorder,             /* pointer to byteorder to use
-                                   0=native;-1=LE,1=BE; updated on
-                                   exit */
-    Py_ssize_t *consumed        /* bytes consumed */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF32Stateful(
+        const char *string,  /* UTF-32 encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        int *byteorder,      /* pointer to byteorder to use
+                                0=native;-1=LE,1=BE; updated on
+                                exit */
+        Py_ssize_t *consumed /* bytes consumed */
     );
 
-/* Returns a Python string using the UTF-32 encoding in native byte
-   order. The string always starts with a BOM mark.  */
+    /* Returns a Python string using the UTF-32 encoding in native byte
+       order. The string always starts with a BOM mark.  */
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsUTF32String(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUTF32String(
+        PyObject *unicode /* Unicode object */
     );
 
-/* Returns a Python string object holding the UTF-32 encoded value of
-   the Unicode data.
+    /* Returns a Python string object holding the UTF-32 encoded value of
+       the Unicode data.
 
-   If byteorder is not 0, output is written according to the following
-   byte order:
+       If byteorder is not 0, output is written according to the following
+       byte order:
 
-   byteorder == -1: little endian
-   byteorder == 0:  native byte order (writes a BOM mark)
-   byteorder == 1:  big endian
+       byteorder == -1: little endian
+       byteorder == 0:  native byte order (writes a BOM mark)
+       byteorder == 1:  big endian
 
-   If byteorder is 0, the output string will always start with the
-   Unicode BOM mark (U+FEFF). In the other two modes, no BOM mark is
-   prepended.
+       If byteorder is 0, the output string will always start with the
+       Unicode BOM mark (U+FEFF). In the other two modes, no BOM mark is
+       prepended.
 
-*/
+    */
 
-/* --- UTF-16 Codecs ------------------------------------------------------ */
+    /* --- UTF-16 Codecs ------------------------------------------------------ */
 
-/* Decodes length bytes from a UTF-16 encoded buffer string and returns
-   the corresponding Unicode object.
+    /* Decodes length bytes from a UTF-16 encoded buffer string and returns
+       the corresponding Unicode object.
 
-   errors (if non-NULL) defines the error handling. It defaults
-   to "strict".
+       errors (if non-NULL) defines the error handling. It defaults
+       to "strict".
 
-   If byteorder is non-NULL, the decoder starts decoding using the
-   given byte order:
+       If byteorder is non-NULL, the decoder starts decoding using the
+       given byte order:
 
-    *byteorder == -1: little endian
-    *byteorder == 0:  native order
-    *byteorder == 1:  big endian
+        *byteorder == -1: little endian
+        *byteorder == 0:  native order
+        *byteorder == 1:  big endian
 
-   In native mode, the first two bytes of the stream are checked for a
-   BOM mark. If found, the BOM mark is analysed, the byte order
-   adjusted and the BOM skipped.  In the other modes, no BOM mark
-   interpretation is done. After completion, *byteorder is set to the
-   current byte order at the end of input data.
+       In native mode, the first two bytes of the stream are checked for a
+       BOM mark. If found, the BOM mark is analysed, the byte order
+       adjusted and the BOM skipped.  In the other modes, no BOM mark
+       interpretation is done. After completion, *byteorder is set to the
+       current byte order at the end of input data.
 
-   If byteorder is NULL, the codec starts in native order mode.
+       If byteorder is NULL, the codec starts in native order mode.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF16(
-    const char *string,         /* UTF-16 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    int *byteorder              /* pointer to byteorder to use
-                                   0=native;-1=LE,1=BE; updated on
-                                   exit */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF16(
+        const char *string, /* UTF-16 encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors, /* error handling */
+        int *byteorder      /* pointer to byteorder to use
+                               0=native;-1=LE,1=BE; updated on
+                               exit */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF16Stateful(
-    const char *string,         /* UTF-16 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    int *byteorder,             /* pointer to byteorder to use
-                                   0=native;-1=LE,1=BE; updated on
-                                   exit */
-    Py_ssize_t *consumed        /* bytes consumed */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUTF16Stateful(
+        const char *string,  /* UTF-16 encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        int *byteorder,      /* pointer to byteorder to use
+                                0=native;-1=LE,1=BE; updated on
+                                exit */
+        Py_ssize_t *consumed /* bytes consumed */
     );
 
-/* Returns a Python string using the UTF-16 encoding in native byte
-   order. The string always starts with a BOM mark.  */
+    /* Returns a Python string using the UTF-16 encoding in native byte
+       order. The string always starts with a BOM mark.  */
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsUTF16String(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUTF16String(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- Unicode-Escape Codecs ---------------------------------------------- */
+    /* --- Unicode-Escape Codecs ---------------------------------------------- */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeUnicodeEscape(
-    const char *string,         /* Unicode-Escape encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeUnicodeEscape(
+        const char *string, /* Unicode-Escape encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsUnicodeEscapeString(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsUnicodeEscapeString(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- Raw-Unicode-Escape Codecs ------------------------------------------ */
+    /* --- Raw-Unicode-Escape Codecs ------------------------------------------ */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeRawUnicodeEscape(
-    const char *string,         /* Raw-Unicode-Escape encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeRawUnicodeEscape(
+        const char *string, /* Raw-Unicode-Escape encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsRawUnicodeEscapeString(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsRawUnicodeEscapeString(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- Latin-1 Codecs -----------------------------------------------------
+    /* --- Latin-1 Codecs -----------------------------------------------------
 
-   Note: Latin-1 corresponds to the first 256 Unicode ordinals. */
+       Note: Latin-1 corresponds to the first 256 Unicode ordinals. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeLatin1(
-    const char *string,         /* Latin-1 encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeLatin1(
+        const char *string, /* Latin-1 encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsLatin1String(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsLatin1String(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- ASCII Codecs -------------------------------------------------------
+    /* --- ASCII Codecs -------------------------------------------------------
 
-   Only 7-bit ASCII data is excepted. All other codes generate errors.
+       Only 7-bit ASCII data is excepted. All other codes generate errors.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeASCII(
-    const char *string,         /* ASCII encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeASCII(
+        const char *string, /* ASCII encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsASCIIString(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsASCIIString(
+        PyObject *unicode /* Unicode object */
     );
 
-/* --- Character Map Codecs -----------------------------------------------
+    /* --- Character Map Codecs -----------------------------------------------
 
-   This codec uses mappings to encode and decode characters.
+       This codec uses mappings to encode and decode characters.
 
-   Decoding mappings must map byte ordinals (integers in the range from 0 to
-   255) to Unicode strings, integers (which are then interpreted as Unicode
-   ordinals) or None.  Unmapped data bytes (ones which cause a LookupError)
-   as well as mapped to None, 0xFFFE or '\ufffe' are treated as "undefined
-   mapping" and cause an error.
+       Decoding mappings must map byte ordinals (integers in the range from 0 to
+       255) to Unicode strings, integers (which are then interpreted as Unicode
+       ordinals) or None.  Unmapped data bytes (ones which cause a LookupError)
+       as well as mapped to None, 0xFFFE or '\ufffe' are treated as "undefined
+       mapping" and cause an error.
 
-   Encoding mappings must map Unicode ordinal integers to bytes objects,
-   integers in the range from 0 to 255 or None.  Unmapped character
-   ordinals (ones which cause a LookupError) as well as mapped to
-   None are treated as "undefined mapping" and cause an error.
+       Encoding mappings must map Unicode ordinal integers to bytes objects,
+       integers in the range from 0 to 255 or None.  Unmapped character
+       ordinals (ones which cause a LookupError) as well as mapped to
+       None are treated as "undefined mapping" and cause an error.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeCharmap(
-    const char *string,         /* Encoded string */
-    Py_ssize_t length,          /* size of string */
-    PyObject *mapping,          /* decoding mapping */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeCharmap(
+        const char *string, /* Encoded string */
+        Py_ssize_t length,  /* size of string */
+        PyObject *mapping,  /* decoding mapping */
+        const char *errors  /* error handling */
     );
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsCharmapString(
-    PyObject *unicode,          /* Unicode object */
-    PyObject *mapping           /* encoding mapping */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsCharmapString(
+        PyObject *unicode, /* Unicode object */
+        PyObject *mapping  /* encoding mapping */
     );
 
-/* --- MBCS codecs for Windows -------------------------------------------- */
+    /* --- MBCS codecs for Windows -------------------------------------------- */
 
 #ifdef MS_WINDOWS
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeMBCS(
-    const char *string,         /* MBCS encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors          /* error handling */
-    );
-
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeMBCSStateful(
-    const char *string,         /* MBCS encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    Py_ssize_t *consumed        /* bytes consumed */
-    );
-
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeCodePageStateful(
-    int code_page,              /* code page number */
-    const char *string,         /* encoded string */
-    Py_ssize_t length,          /* size of string */
-    const char *errors,         /* error handling */
-    Py_ssize_t *consumed        /* bytes consumed */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeMBCS(
+        const char *string, /* MBCS encoded string */
+        Py_ssize_t length,  /* size of string */
+        const char *errors  /* error handling */
+    );
+
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeMBCSStateful(
+        const char *string,  /* MBCS encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        Py_ssize_t *consumed /* bytes consumed */
+    );
+
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeCodePageStateful(
+        int code_page,       /* code page number */
+        const char *string,  /* encoded string */
+        Py_ssize_t length,   /* size of string */
+        const char *errors,  /* error handling */
+        Py_ssize_t *consumed /* bytes consumed */
     );
 #endif
 
-PyAPI_FUNC(uint64_t) PyUnicode_AsMBCSString(
-    PyObject *unicode           /* Unicode object */
+    PyAPI_FUNC(uint64_t) PyUnicode_AsMBCSString(
+        PyObject *unicode /* Unicode object */
     );
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-PyAPI_FUNC(uint64_t) PyUnicode_EncodeCodePage(
-    int code_page,              /* code page number */
-    PyObject *unicode,          /* Unicode object */
-    const char *errors          /* error handling */
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    PyAPI_FUNC(uint64_t) PyUnicode_EncodeCodePage(
+        int code_page,     /* code page number */
+        PyObject *unicode, /* Unicode object */
+        const char *errors /* error handling */
     );
 #endif
 
 #endif /* MS_WINDOWS */
 
-/* --- Locale encoding --------------------------------------------------- */
+    /* --- Locale encoding --------------------------------------------------- */
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-/* Decode a string from the current locale encoding. The decoder is strict if
-   *surrogateescape* is equal to zero, otherwise it uses the 'surrogateescape'
-   error handler (PEP 383) to escape undecodable bytes. If a byte sequence can
-   be decoded as a surrogate character and *surrogateescape* is not equal to
-   zero, the byte sequence is escaped using the 'surrogateescape' error handler
-   instead of being decoded. *str* must end with a null character but cannot
-   contain embedded null characters. */
-
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeLocaleAndSize(
-    const char *str,
-    Py_ssize_t len,
-    const char *errors);
-
-/* Similar to PyUnicode_DecodeLocaleAndSize(), but compute the string
-   length using strlen(). */
-
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeLocale(
-    const char *str,
-    const char *errors);
-
-/* Encode a Unicode object to the current locale encoding. The encoder is
-   strict is *surrogateescape* is equal to zero, otherwise the
-   "surrogateescape" error handler is used. Return a bytes object. The string
-   cannot contain embedded null characters. */
-
-PyAPI_FUNC(uint64_t) PyUnicode_EncodeLocale(
-    PyObject *unicode,
-    const char *errors
-    );
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    /* Decode a string from the current locale encoding. The decoder is strict if
+       *surrogateescape* is equal to zero, otherwise it uses the 'surrogateescape'
+       error handler (PEP 383) to escape undecodable bytes. If a byte sequence can
+       be decoded as a surrogate character and *surrogateescape* is not equal to
+       zero, the byte sequence is escaped using the 'surrogateescape' error handler
+       instead of being decoded. *str* must end with a null character but cannot
+       contain embedded null characters. */
+
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeLocaleAndSize(
+        const char *str,
+        Py_ssize_t len,
+        const char *errors);
+
+    /* Similar to PyUnicode_DecodeLocaleAndSize(), but compute the string
+       length using strlen(). */
+
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeLocale(
+        const char *str,
+        const char *errors);
+
+    /* Encode a Unicode object to the current locale encoding. The encoder is
+       strict is *surrogateescape* is equal to zero, otherwise the
+       "surrogateescape" error handler is used. Return a bytes object. The string
+       cannot contain embedded null characters. */
+
+    PyAPI_FUNC(uint64_t) PyUnicode_EncodeLocale(
+        PyObject *unicode,
+        const char *errors);
 #endif
 
-/* --- File system encoding ---------------------------------------------- */
+    /* --- File system encoding ---------------------------------------------- */
 
-/* ParseTuple converter: encode str objects to bytes using
-   PyUnicode_EncodeFSDefault(); bytes objects are output as-is. */
+    /* ParseTuple converter: encode str objects to bytes using
+       PyUnicode_EncodeFSDefault(); bytes objects are output as-is. */
 
-PyAPI_FUNC(int) PyUnicode_FSConverter(PyObject*, void*);
+    PyAPI_FUNC(int) PyUnicode_FSConverter(PyObject *, void *);
 
-/* ParseTuple converter: decode bytes objects to unicode using
-   PyUnicode_DecodeFSDefaultAndSize(); str objects are output as-is. */
+    /* ParseTuple converter: decode bytes objects to unicode using
+       PyUnicode_DecodeFSDefaultAndSize(); str objects are output as-is. */
 
-PyAPI_FUNC(int) PyUnicode_FSDecoder(PyObject*, void*);
+    PyAPI_FUNC(int) PyUnicode_FSDecoder(PyObject *, void *);
 
-/* Decode a null-terminated string using Py_FileSystemDefaultEncoding
-   and the "surrogateescape" error handler.
+    /* Decode a null-terminated string using Py_FileSystemDefaultEncoding
+       and the "surrogateescape" error handler.
 
-   If Py_FileSystemDefaultEncoding is not set, fall back to the locale
-   encoding.
+       If Py_FileSystemDefaultEncoding is not set, fall back to the locale
+       encoding.
 
-   Use PyUnicode_DecodeFSDefaultAndSize() if the string length is known.
-*/
+       Use PyUnicode_DecodeFSDefaultAndSize() if the string length is known.
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeFSDefault(
-    const char *s               /* encoded string */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeFSDefault(
+        const char *s /* encoded string */
     );
 
-/* Decode a string using Py_FileSystemDefaultEncoding
-   and the "surrogateescape" error handler.
+    /* Decode a string using Py_FileSystemDefaultEncoding
+       and the "surrogateescape" error handler.
 
-   If Py_FileSystemDefaultEncoding is not set, fall back to the locale
-   encoding.
-*/
+       If Py_FileSystemDefaultEncoding is not set, fall back to the locale
+       encoding.
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_DecodeFSDefaultAndSize(
-    const char *s,               /* encoded string */
-    Py_ssize_t size              /* size */
+    PyAPI_FUNC(uint64_t) PyUnicode_DecodeFSDefaultAndSize(
+        const char *s,  /* encoded string */
+        Py_ssize_t size /* size */
     );
 
-/* Encode a Unicode object to Py_FileSystemDefaultEncoding with the
-   "surrogateescape" error handler, and return bytes.
+    /* Encode a Unicode object to Py_FileSystemDefaultEncoding with the
+       "surrogateescape" error handler, and return bytes.
 
-   If Py_FileSystemDefaultEncoding is not set, fall back to the locale
-   encoding.
-*/
+       If Py_FileSystemDefaultEncoding is not set, fall back to the locale
+       encoding.
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_EncodeFSDefault(
-    PyObject *unicode
-    );
+    PyAPI_FUNC(uint64_t) PyUnicode_EncodeFSDefault(
+        PyObject *unicode);
 
-/* --- Methods & Slots ----------------------------------------------------
+    /* --- Methods & Slots ----------------------------------------------------
 
-   These are capable of handling Unicode objects and strings on input
-   (we refer to them as strings in the descriptions) and return
-   Unicode objects or integers as appropriate. */
+       These are capable of handling Unicode objects and strings on input
+       (we refer to them as strings in the descriptions) and return
+       Unicode objects or integers as appropriate. */
 
-/* Concat two strings giving a new Unicode string. */
+    /* Concat two strings giving a new Unicode string. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Concat(
-    PyObject *left,             /* Left string */
-    PyObject *right             /* Right string */
+    PyAPI_FUNC(uint64_t) PyUnicode_Concat(
+        PyObject *left, /* Left string */
+        PyObject *right /* Right string */
     );
 
-/* Concat two strings and put the result in *pleft
-   (sets *pleft to NULL on error) */
+    /* Concat two strings and put the result in *pleft
+       (sets *pleft to NULL on error) */
 
-PyAPI_FUNC(void) PyUnicode_Append(
-    PyObject **pleft,           /* Pointer to left string */
-    PyObject *right             /* Right string */
+    PyAPI_FUNC(void) PyUnicode_Append(
+        PyObject **pleft, /* Pointer to left string */
+        PyObject *right   /* Right string */
     );
 
-/* Concat two strings, put the result in *pleft and drop the right object
-   (sets *pleft to NULL on error) */
+    /* Concat two strings, put the result in *pleft and drop the right object
+       (sets *pleft to NULL on error) */
 
-PyAPI_FUNC(void) PyUnicode_AppendAndDel(
-    PyObject **pleft,           /* Pointer to left string */
-    PyObject *right             /* Right string */
+    PyAPI_FUNC(void) PyUnicode_AppendAndDel(
+        PyObject **pleft, /* Pointer to left string */
+        PyObject *right   /* Right string */
     );
 
-/* Split a string giving a list of Unicode strings.
+    /* Split a string giving a list of Unicode strings.
 
-   If sep is NULL, splitting will be done at all whitespace
-   substrings. Otherwise, splits occur at the given separator.
+       If sep is NULL, splitting will be done at all whitespace
+       substrings. Otherwise, splits occur at the given separator.
 
-   At most maxsplit splits will be done. If negative, no limit is set.
+       At most maxsplit splits will be done. If negative, no limit is set.
 
-   Separators are not included in the resulting list.
+       Separators are not included in the resulting list.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Split(
-    PyObject *s,                /* String to split */
-    PyObject *sep,              /* String separator */
-    Py_ssize_t maxsplit         /* Maxsplit count */
+    PyAPI_FUNC(uint64_t) PyUnicode_Split(
+        PyObject *s,        /* String to split */
+        PyObject *sep,      /* String separator */
+        Py_ssize_t maxsplit /* Maxsplit count */
     );
 
-/* Dito, but split at line breaks.
+    /* Dito, but split at line breaks.
 
-   CRLF is considered to be one line break. Line breaks are not
-   included in the resulting list. */
+       CRLF is considered to be one line break. Line breaks are not
+       included in the resulting list. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Splitlines(
-    PyObject *s,                /* String to split */
-    int keepends                /* If true, line end markers are included */
+    PyAPI_FUNC(uint64_t) PyUnicode_Splitlines(
+        PyObject *s, /* String to split */
+        int keepends /* If true, line end markers are included */
     );
 
-/* Partition a string using a given separator. */
+    /* Partition a string using a given separator. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Partition(
-    PyObject *s,                /* String to partition */
-    PyObject *sep               /* String separator */
+    PyAPI_FUNC(uint64_t) PyUnicode_Partition(
+        PyObject *s,  /* String to partition */
+        PyObject *sep /* String separator */
     );
 
-/* Partition a string using a given separator, searching from the end of the
-   string. */
+    /* Partition a string using a given separator, searching from the end of the
+       string. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_RPartition(
-    PyObject *s,                /* String to partition */
-    PyObject *sep               /* String separator */
+    PyAPI_FUNC(uint64_t) PyUnicode_RPartition(
+        PyObject *s,  /* String to partition */
+        PyObject *sep /* String separator */
     );
 
-/* Split a string giving a list of Unicode strings.
+    /* Split a string giving a list of Unicode strings.
 
-   If sep is NULL, splitting will be done at all whitespace
-   substrings. Otherwise, splits occur at the given separator.
+       If sep is NULL, splitting will be done at all whitespace
+       substrings. Otherwise, splits occur at the given separator.
 
-   At most maxsplit splits will be done. But unlike PyUnicode_Split
-   PyUnicode_RSplit splits from the end of the string. If negative,
-   no limit is set.
+       At most maxsplit splits will be done. But unlike PyUnicode_Split
+       PyUnicode_RSplit splits from the end of the string. If negative,
+       no limit is set.
 
-   Separators are not included in the resulting list.
+       Separators are not included in the resulting list.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_RSplit(
-    PyObject *s,                /* String to split */
-    PyObject *sep,              /* String separator */
-    Py_ssize_t maxsplit         /* Maxsplit count */
+    PyAPI_FUNC(uint64_t) PyUnicode_RSplit(
+        PyObject *s,        /* String to split */
+        PyObject *sep,      /* String separator */
+        Py_ssize_t maxsplit /* Maxsplit count */
     );
 
-/* Translate a string by applying a character mapping table to it and
-   return the resulting Unicode object.
+    /* Translate a string by applying a character mapping table to it and
+       return the resulting Unicode object.
 
-   The mapping table must map Unicode ordinal integers to Unicode strings,
-   Unicode ordinal integers or None (causing deletion of the character).
+       The mapping table must map Unicode ordinal integers to Unicode strings,
+       Unicode ordinal integers or None (causing deletion of the character).
 
-   Mapping tables may be dictionaries or sequences. Unmapped character
-   ordinals (ones which cause a LookupError) are left untouched and
-   are copied as-is.
+       Mapping tables may be dictionaries or sequences. Unmapped character
+       ordinals (ones which cause a LookupError) are left untouched and
+       are copied as-is.
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Translate(
-    PyObject *str,              /* String */
-    PyObject *table,            /* Translate table */
-    const char *errors          /* error handling */
+    PyAPI_FUNC(uint64_t) PyUnicode_Translate(
+        PyObject *str,     /* String */
+        PyObject *table,   /* Translate table */
+        const char *errors /* error handling */
     );
 
-/* Join a sequence of strings using the given separator and return
-   the resulting Unicode string. */
+    /* Join a sequence of strings using the given separator and return
+       the resulting Unicode string. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Join(
-    PyObject *separator,        /* Separator string */
-    PyObject *seq               /* Sequence object */
+    PyAPI_FUNC(uint64_t) PyUnicode_Join(
+        PyObject *separator, /* Separator string */
+        PyObject *seq        /* Sequence object */
     );
 
-/* Return 1 if substr matches str[start:end] at the given tail end, 0
-   otherwise. */
+    /* Return 1 if substr matches str[start:end] at the given tail end, 0
+       otherwise. */
 
-PyAPI_FUNC(Py_ssize_t) PyUnicode_Tailmatch(
-    PyObject *str,              /* String */
-    PyObject *substr,           /* Prefix or Suffix string */
-    Py_ssize_t start,           /* Start index */
-    Py_ssize_t end,             /* Stop index */
-    int direction               /* Tail end: -1 prefix, +1 suffix */
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_Tailmatch(
+        PyObject *str,    /* String */
+        PyObject *substr, /* Prefix or Suffix string */
+        Py_ssize_t start, /* Start index */
+        Py_ssize_t end,   /* Stop index */
+        int direction     /* Tail end: -1 prefix, +1 suffix */
     );
 
-/* Return the first position of substr in str[start:end] using the
-   given search direction or -1 if not found. -2 is returned in case
-   an error occurred and an exception is set. */
+    /* Return the first position of substr in str[start:end] using the
+       given search direction or -1 if not found. -2 is returned in case
+       an error occurred and an exception is set. */
 
-PyAPI_FUNC(Py_ssize_t) PyUnicode_Find(
-    PyObject *str,              /* String */
-    PyObject *substr,           /* Substring to find */
-    Py_ssize_t start,           /* Start index */
-    Py_ssize_t end,             /* Stop index */
-    int direction               /* Find direction: +1 forward, -1 backward */
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_Find(
+        PyObject *str,    /* String */
+        PyObject *substr, /* Substring to find */
+        Py_ssize_t start, /* Start index */
+        Py_ssize_t end,   /* Stop index */
+        int direction     /* Find direction: +1 forward, -1 backward */
     );
 
-#if !defined(Py_LIMITED_API) || Py_LIMITED_API+0 >= 0x03030000
-/* Like PyUnicode_Find, but search for single character only. */
-PyAPI_FUNC(Py_ssize_t) PyUnicode_FindChar(
-    PyObject *str,
-    Py_UCS4 ch,
-    Py_ssize_t start,
-    Py_ssize_t end,
-    int direction
-    );
+#if !defined(Py_LIMITED_API) || Py_LIMITED_API + 0 >= 0x03030000
+    /* Like PyUnicode_Find, but search for single character only. */
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_FindChar(
+        PyObject *str,
+        Py_UCS4 ch,
+        Py_ssize_t start,
+        Py_ssize_t end,
+        int direction);
 #endif
 
-/* Count the number of occurrences of substr in str[start:end]. */
+    /* Count the number of occurrences of substr in str[start:end]. */
 
-PyAPI_FUNC(Py_ssize_t) PyUnicode_Count(
-    PyObject *str,              /* String */
-    PyObject *substr,           /* Substring to count */
-    Py_ssize_t start,           /* Start index */
-    Py_ssize_t end              /* Stop index */
+    PyAPI_FUNC(Py_ssize_t) PyUnicode_Count(
+        PyObject *str,    /* String */
+        PyObject *substr, /* Substring to count */
+        Py_ssize_t start, /* Start index */
+        Py_ssize_t end    /* Stop index */
     );
 
-/* Replace at most maxcount occurrences of substr in str with replstr
-   and return the resulting Unicode object. */
+    /* Replace at most maxcount occurrences of substr in str with replstr
+       and return the resulting Unicode object. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Replace(
-    PyObject *str,              /* String */
-    PyObject *substr,           /* Substring to find */
-    PyObject *replstr,          /* Substring to replace */
-    Py_ssize_t maxcount         /* Max. number of replacements to apply;
-                                   -1 = all */
+    PyAPI_FUNC(uint64_t) PyUnicode_Replace(
+        PyObject *str,      /* String */
+        PyObject *substr,   /* Substring to find */
+        PyObject *replstr,  /* Substring to replace */
+        Py_ssize_t maxcount /* Max. number of replacements to apply;
+                               -1 = all */
     );
 
-/* Compare two strings and return -1, 0, 1 for less than, equal,
-   greater than resp.
-   Raise an exception and return -1 on error. */
+    /* Compare two strings and return -1, 0, 1 for less than, equal,
+       greater than resp.
+       Raise an exception and return -1 on error. */
 
-PyAPI_FUNC(int) PyUnicode_Compare(
-    PyObject *left,             /* Left string */
-    PyObject *right             /* Right string */
+    PyAPI_FUNC(int) PyUnicode_Compare(
+        PyObject *left, /* Left string */
+        PyObject *right /* Right string */
     );
 
-/* Compare a Unicode object with C string and return -1, 0, 1 for less than,
-   equal, and greater than, respectively.  It is best to pass only
-   ASCII-encoded strings, but the function interprets the input string as
-   ISO-8859-1 if it contains non-ASCII characters.
-   This function does not raise exceptions. */
+    /* Compare a Unicode object with C string and return -1, 0, 1 for less than,
+       equal, and greater than, respectively.  It is best to pass only
+       ASCII-encoded strings, but the function interprets the input string as
+       ISO-8859-1 if it contains non-ASCII characters.
+       This function does not raise exceptions. */
 
-PyAPI_FUNC(int) PyUnicode_CompareWithASCIIString(
-    PyObject *left,
-    const char *right           /* ASCII-encoded string */
+    PyAPI_FUNC(int) PyUnicode_CompareWithASCIIString(
+        PyObject *left,
+        const char *right /* ASCII-encoded string */
     );
 
-/* Rich compare two strings and return one of the following:
+    /* Rich compare two strings and return one of the following:
 
-   - NULL in case an exception was raised
-   - Py_True or Py_False for successful comparisons
-   - Py_NotImplemented in case the type combination is unknown
+       - NULL in case an exception was raised
+       - Py_True or Py_False for successful comparisons
+       - Py_NotImplemented in case the type combination is unknown
 
-   Possible values for op:
+       Possible values for op:
 
-     Py_GT, Py_GE, Py_EQ, Py_NE, Py_LT, Py_LE
+         Py_GT, Py_GE, Py_EQ, Py_NE, Py_LT, Py_LE
 
-*/
+    */
 
-PyAPI_FUNC(uint64_t) PyUnicode_RichCompare(
-    PyObject *left,             /* Left string */
-    PyObject *right,            /* Right string */
-    int op                      /* Operation: Py_EQ, Py_NE, Py_GT, etc. */
+    PyAPI_FUNC(uint64_t) PyUnicode_RichCompare(
+        PyObject *left,  /* Left string */
+        PyObject *right, /* Right string */
+        int op           /* Operation: Py_EQ, Py_NE, Py_GT, etc. */
     );
 
-/* Apply an argument tuple or dictionary to a format string and return
-   the resulting Unicode string. */
+    /* Apply an argument tuple or dictionary to a format string and return
+       the resulting Unicode string. */
 
-PyAPI_FUNC(uint64_t) PyUnicode_Format(
-    PyObject *format,           /* Format string */
-    PyObject *args              /* Argument tuple or dictionary */
+    PyAPI_FUNC(uint64_t) PyUnicode_Format(
+        PyObject *format, /* Format string */
+        PyObject *args    /* Argument tuple or dictionary */
     );
 
-/* Checks whether element is contained in container and return 1/0
-   accordingly.
+    /* Checks whether element is contained in container and return 1/0
+       accordingly.
 
-   element has to coerce to a one element Unicode string. -1 is
-   returned in case of an error. */
+       element has to coerce to a one element Unicode string. -1 is
+       returned in case of an error. */
 
-PyAPI_FUNC(int) PyUnicode_Contains(
-    PyObject *container,        /* Container string */
-    PyObject *element           /* Element string */
+    PyAPI_FUNC(int) PyUnicode_Contains(
+        PyObject *container, /* Container string */
+        PyObject *element    /* Element string */
     );
 
-/* Checks whether argument is a valid identifier. */
+    /* Checks whether argument is a valid identifier. */
 
-PyAPI_FUNC(int) PyUnicode_IsIdentifier(PyObject *s);
+    PyAPI_FUNC(int) PyUnicode_IsIdentifier(PyObject *s);
 
-/* === Characters Type APIs =============================================== */
+    /* === Characters Type APIs =============================================== */
 
 #ifndef Py_LIMITED_API
-#  define Py_CPYTHON_UNICODEOBJECT_H
-#  include  "cpython/unicodeobject.h"
-#  undef Py_CPYTHON_UNICODEOBJECT_H
+#define Py_CPYTHON_UNICODEOBJECT_H
+#include "cpython/unicodeobject.h"
+#undef Py_CPYTHON_UNICODEOBJECT_H
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 #endif /* !Py_UNICODEOBJECT_H */
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/warnings.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build/include/cp39/weakrefobject.h` & `wasmpy-build-0.4.1/wasmpy_build/include/cp39/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.4.0/wasmpy_build.egg-info/PKG-INFO` & `wasmpy-build-0.4.1/wasmpy_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.4.0
+Version: 0.4.1
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wasmpy-build-0.4.0/wasmpy_build.egg-info/SOURCES.txt` & `wasmpy-build-0.4.1/wasmpy_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

