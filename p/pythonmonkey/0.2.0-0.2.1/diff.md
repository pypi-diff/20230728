# Comparing `tmp/pythonmonkey-0.2.0.tar.gz` & `tmp/pythonmonkey-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmonkey-0.2.0.tar", max compression
+gzip compressed data, was "pythonmonkey-0.2.1.tar", max compression
```

## Comparing `pythonmonkey-0.2.0.tar` & `pythonmonkey-0.2.1.tar`

### file list

```diff
@@ -1,136 +1,138 @@
--rw-r--r--   0        0        0     3284 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/CMakeLists.txt
--rw-r--r--   0        0        0     1075 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/LICENSE
--rw-r--r--   0        0        0    14866 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/README.md
--rw-r--r--   0        0        0     2157 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/build.py
--rw-r--r--   0        0        0      921 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/CMakeLists.txt
--rw-r--r--   0        0        0      243 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/Doxyfile.in
--rw-r--r--   0        0        0        0 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/docs/mainpage.md
--rw-r--r--   0        0        0      957 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/externals/autopep8/CMakeLists.txt
--rw-r--r--   0        0        0     1498 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/externals/uncrustify/CMakeLists.txt
--rw-r--r--   0        0        0     3571 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/format/CMakeLists.txt
--rw-r--r--   0        0        0     4714 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/format/uncrustify.cfg
--rw-r--r--   0        0        0     4957 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/cmake/modules/FindSpiderMonkey.cmake
--rw-r--r--   0        0        0      643 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/BoolType.hh
--rw-r--r--   0        0        0     2350 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/BufferType.hh
--rw-r--r--   0        0        0      951 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/DateType.hh
--rw-r--r--   0        0        0     1392 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/DictType.hh
--rw-r--r--   0        0        0     1136 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/ExceptionType.hh
--rw-r--r--   0        0        0      679 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/FloatType.hh
--rw-r--r--   0        0        0      643 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/FuncType.hh
--rw-r--r--   0        0        0     1071 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/IntType.hh
--rw-r--r--   0        0        0     5828 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/JSObjectProxy.hh
--rw-r--r--   0        0        0     3771 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/JobQueue.hh
--rw-r--r--   0        0        0     1220 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/ListType.hh
--rw-r--r--   0        0        0      506 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/NoneType.hh
--rw-r--r--   0        0        0      600 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/NullType.hh
--rw-r--r--   0        0        0     2001 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PromiseType.hh
--rw-r--r--   0        0        0     6866 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyEventLoop.hh
--rw-r--r--   0        0        0     7110 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyProxyHandler.hh
--rw-r--r--   0        0        0      655 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/PyType.hh
--rw-r--r--   0        0        0     1736 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/StrType.hh
--rw-r--r--   0        0        0      839 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/TupleType.hh
--rw-r--r--   0        0        0      554 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/TypeEnum.hh
--rw-r--r--   0        0        0      572 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/internalBinding.hh
--rw-r--r--   0        0        0     1852 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/jsTypeFactory.hh
--rw-r--r--   0        0        0     3591 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/modules/pythonmonkey/pythonmonkey.hh
--rw-r--r--   0        0        0     2112 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/pyTypeFactory.hh
--rw-r--r--   0        0        0      981 2023-07-21 13:59:26.607132 pythonmonkey-0.2.0/include/setSpiderMonkeyException.hh
--rw-r--r--   0        0        0     1896 2023-07-21 13:59:50.491216 pythonmonkey-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      908 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/__init__.py
--rw-r--r--   0        0        0      617 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.d.ts
--rw-r--r--   0        0        0      633 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.py
--rw-r--r--   0        0        0     2571 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/console.js
--rw-r--r--   0        0        0     1177 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts
--rw-r--r--   0        0        0      176 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/internal-binding.py
--rw-r--r--   0        0        0    28025 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/util.js
--rw-r--r--   0        0        0        0 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/cli/__init__.py
--rwxr-xr-x   0        0        0    13319 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/cli/pmjs.py
--rw-r--r--   0        0        0     2157 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/global.d.ts
--rw-r--r--   0        0        0     1743 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/lib/pmjs/global-init.js
--rw-r--r--   0        0        0     1383 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/pythonmonkey.pyi
--rw-r--r--   0        0        0    13456 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/require.py
--rw-r--r--   0        0        0      422 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/python/pythonmonkey/tsconfig.json
--rwxr-xr-x   0        0        0     3181 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/setup.sh
--rw-r--r--   0        0        0      302 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/BoolType.cc
--rw-r--r--   0        0        0     8782 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/BufferType.cc
--rw-r--r--   0        0        0     1386 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/CMakeLists.txt
--rw-r--r--   0        0        0     1988 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/DateType.cc
--rw-r--r--   0        0        0     1032 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/DictType.cc
--rw-r--r--   0        0        0     2137 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/ExceptionType.cc
--rw-r--r--   0        0        0      391 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/FloatType.cc
--rw-r--r--   0        0        0      256 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/FuncType.cc
--rw-r--r--   0        0        0     7990 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/IntType.cc
--rw-r--r--   0        0        0     8984 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/JSObjectProxy.cc
--rw-r--r--   0        0        0     3679 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/JobQueue.cc
--rw-r--r--   0        0        0      688 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/ListType.cc
--rw-r--r--   0        0        0      331 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/NoneType.cc
--rw-r--r--   0        0        0      419 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/NullType.cc
--rw-r--r--   0        0        0     7205 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PromiseType.cc
--rw-r--r--   0        0        0     6866 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyEventLoop.cc
--rw-r--r--   0        0        0     7947 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyProxyHandler.cc
--rw-r--r--   0        0        0      286 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/PyType.cc
--rw-r--r--   0        0        0     6252 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/StrType.cc
--rw-r--r--   0        0        0      577 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/TupleType.cc
--rw-r--r--   0        0        0     3990 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/internalBinding/utils.cc
--rw-r--r--   0        0        0     2404 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/internalBinding.cc
--rw-r--r--   0        0        0    10785 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/jsTypeFactory.cc
--rw-r--r--   0        0        0    18299 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/modules/pythonmonkey/pythonmonkey.cc
--rw-r--r--   0        0        0     7365 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/pyTypeFactory.cc
--rw-r--r--   0        0        0     3502 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/src/setSpiderMonkeyException.cc
--rwxr-xr-x   0        0        0     1249 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/commonjs-modules.bash
--rw-r--r--   0        0        0      602 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-smoke.simple
--rwxr-xr-x   0        0        0      935 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-stdio.bash
--rw-r--r--   0        0        0     1008 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/console-this.simple
--rw-r--r--   0        0        0      532 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/is-compilable-unit.simple
--rw-r--r--   0        0        0      962 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/array-change-index.simple
--rw-r--r--   0        0        0      873 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/arraybuffer.simple
--rw-r--r--   0        0        0      787 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/bigint.simple
--rw-r--r--   0        0        0      866 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/boolean.simple
--rw-r--r--   0        0        0     1175 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/datetime.simple
--rw-r--r--   0        0        0     2003 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/datetime2.simple
--rw-r--r--   0        0        0      810 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/function-curry.simple
--rw-r--r--   0        0        0      733 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/higher-order-function.simple
--rw-r--r--   0        0        0      846 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/promise-await-in-python.simple.failing
--rw-r--r--   0        0        0      718 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/promise.simple.failing
--rw-r--r--   0        0        0      699 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/string.simple
--rw-r--r--   0        0        0      519 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/js2py/trivial-function.simple
--rw-r--r--   0        0        0      278 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/load-cjs-module.simple
--rw-r--r--   0        0        0      368 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/load-cjs-python-module.simple
--rw-r--r--   0        0        0      268 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/cjs-module.js
--rw-r--r--   0        0        0       67 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/print-load.js
--rw-r--r--   0        0        0      246 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/python-cjs-module.py
--rw-r--r--   0        0        0      371 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/modules/vm-tools.py
--rw-r--r--   0        0        0      447 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/not-strict-mode.simple
--rwxr-xr-x   0        0        0      750 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-eopt.bash
--rwxr-xr-x   0        0        0     1211 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-global-arguments.bash
--rwxr-xr-x   0        0        0     1289 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-interactive-smoke.bash
--rwxr-xr-x   0        0        0      747 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-popt.bash
--rwxr-xr-x   0        0        0     1089 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-require-cache.bash
--rwxr-xr-x   0        0        0      753 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/pmjs-ropt.bash
--rw-r--r--   0        0        0     1169 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/program-module.simple
--rwxr-xr-x   0        0        0      635 2023-07-21 13:59:26.611132 pythonmonkey-0.2.0/tests/js/program.js
--rw-r--r--   0        0        0      639 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/array-change-index.simple
--rw-r--r--   0        0        0      681 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/arraybuffer.simple
--rw-r--r--   0        0        0     1026 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/boolean.simple
--rw-r--r--   0        0        0     1515 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/datetime.simple
--rw-r--r--   0        0        0      903 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/function-curry.simple.failing
--rw-r--r--   0        0        0      666 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/higher-order-function.simple
--rw-r--r--   0        0        0      591 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/integer.simple
--rw-r--r--   0        0        0      669 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/promise.simple.failing
--rw-r--r--   0        0        0      538 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/string.simple
--rw-r--r--   0        0        0      471 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/py2js/trivial-function.simple
--rwxr-xr-x   0        0        0      796 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/require-module-stack.bash.failing
--rw-r--r--   0        0        0     1672 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/test-atob-btoa.simple
--rw-r--r--   0        0        0      330 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/throw-filename.js
--rwxr-xr-x   0        0        0     1208 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/typeofs-segfaults.simple.failing
--rwxr-xr-x   0        0        0     1667 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/typeofs.simple
--rw-r--r--   0        0        0      432 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/js/use-strict.simple
--rw-r--r--   0        0        0      356 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/conftest.py
--rw-r--r--   0        0        0     6491 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_bigints.py
--rw-r--r--   0        0        0    11020 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_buffer_typed_array.py
--rw-r--r--   0        0        0     4135 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_dicts_lists.py
--rw-r--r--   0        0        0    14294 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_event_loop.py
--rw-r--r--   0        0        0    10622 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_pythonmonkey_eval.py
--rw-r--r--   0        0        0      576 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_reentrance_smoke.py
--rw-r--r--   0        0        0     9095 2023-07-21 13:59:26.615132 pythonmonkey-0.2.0/tests/python/test_strings.py
--rw-r--r--   0        0        0    15380 1970-01-01 00:00:00.000000 pythonmonkey-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3284 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1075 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/LICENSE
+-rw-r--r--   0        0        0    15488 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/README.md
+-rw-r--r--   0        0        0     2157 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/build.py
+-rw-r--r--   0        0        0      921 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/docs/CMakeLists.txt
+-rw-r--r--   0        0        0      243 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/docs/Doxyfile.in
+-rw-r--r--   0        0        0        0 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/docs/mainpage.md
+-rw-r--r--   0        0        0      957 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/externals/autopep8/CMakeLists.txt
+-rw-r--r--   0        0        0     1498 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/externals/uncrustify/CMakeLists.txt
+-rw-r--r--   0        0        0     3571 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/format/CMakeLists.txt
+-rw-r--r--   0        0        0     4714 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/format/uncrustify.cfg
+-rw-r--r--   0        0        0     4957 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/cmake/modules/FindSpiderMonkey.cmake
+-rw-r--r--   0        0        0      643 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/BoolType.hh
+-rw-r--r--   0        0        0     2350 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/BufferType.hh
+-rw-r--r--   0        0        0      951 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/DateType.hh
+-rw-r--r--   0        0        0     1392 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/DictType.hh
+-rw-r--r--   0        0        0     1136 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/ExceptionType.hh
+-rw-r--r--   0        0        0      679 2023-07-28 19:27:20.668786 pythonmonkey-0.2.1/include/FloatType.hh
+-rw-r--r--   0        0        0      643 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/FuncType.hh
+-rw-r--r--   0        0        0     1071 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/IntType.hh
+-rw-r--r--   0        0        0     5828 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/JSObjectProxy.hh
+-rw-r--r--   0        0        0     3771 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/JobQueue.hh
+-rw-r--r--   0        0        0     1220 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/ListType.hh
+-rw-r--r--   0        0        0      506 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/NoneType.hh
+-rw-r--r--   0        0        0      600 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/NullType.hh
+-rw-r--r--   0        0        0     2001 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/PromiseType.hh
+-rw-r--r--   0        0        0     6866 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/PyEventLoop.hh
+-rw-r--r--   0        0        0     7110 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/PyProxyHandler.hh
+-rw-r--r--   0        0        0      655 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/PyType.hh
+-rw-r--r--   0        0        0     1736 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/StrType.hh
+-rw-r--r--   0        0        0      839 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/TupleType.hh
+-rw-r--r--   0        0        0      554 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/TypeEnum.hh
+-rw-r--r--   0        0        0      572 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/internalBinding.hh
+-rw-r--r--   0        0        0     1852 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/jsTypeFactory.hh
+-rw-r--r--   0        0        0     3591 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/modules/pythonmonkey/pythonmonkey.hh
+-rw-r--r--   0        0        0     2112 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/pyTypeFactory.hh
+-rw-r--r--   0        0        0      981 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/include/setSpiderMonkeyException.hh
+-rw-r--r--   0        0        0     1930 2023-07-28 19:27:43.261115 pythonmonkey-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      982 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/base64.d.ts
+-rw-r--r--   0        0        0      633 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/base64.py
+-rw-r--r--   0        0        0     2571 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/console.js
+-rw-r--r--   0        0        0     1177 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/internal-binding.d.ts
+-rw-r--r--   0        0        0      176 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/internal-binding.py
+-rw-r--r--   0        0        0    28025 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/util.js
+-rw-r--r--   0        0        0        0 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/cli/__init__.py
+-rwxr-xr-x   0        0        0    13439 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/cli/pmjs.py
+-rw-r--r--   0        0        0     2157 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/global.d.ts
+-rw-r--r--   0        0        0     1592 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/helpers.py
+-rw-r--r--   0        0        0     6281 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/lib/pmdb.py
+-rw-r--r--   0        0        0     1743 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/lib/pmjs/global-init.js
+-rw-r--r--   0        0        0     1383 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/pythonmonkey.pyi
+-rw-r--r--   0        0        0    13566 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/require.py
+-rw-r--r--   0        0        0      422 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/python/pythonmonkey/tsconfig.json
+-rwxr-xr-x   0        0        0     3181 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/setup.sh
+-rw-r--r--   0        0        0      302 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/BoolType.cc
+-rw-r--r--   0        0        0     8782 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/BufferType.cc
+-rw-r--r--   0        0        0     1386 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/CMakeLists.txt
+-rw-r--r--   0        0        0     1988 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/DateType.cc
+-rw-r--r--   0        0        0     1032 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/DictType.cc
+-rw-r--r--   0        0        0     2137 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/ExceptionType.cc
+-rw-r--r--   0        0        0      391 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/FloatType.cc
+-rw-r--r--   0        0        0      256 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/FuncType.cc
+-rw-r--r--   0        0        0     7990 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/IntType.cc
+-rw-r--r--   0        0        0     8984 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/JSObjectProxy.cc
+-rw-r--r--   0        0        0     3551 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/JobQueue.cc
+-rw-r--r--   0        0        0      688 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/ListType.cc
+-rw-r--r--   0        0        0      331 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/NoneType.cc
+-rw-r--r--   0        0        0      419 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/NullType.cc
+-rw-r--r--   0        0        0     7205 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/PromiseType.cc
+-rw-r--r--   0        0        0     6866 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/PyEventLoop.cc
+-rw-r--r--   0        0        0     7947 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/PyProxyHandler.cc
+-rw-r--r--   0        0        0      286 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/PyType.cc
+-rw-r--r--   0        0        0     6252 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/StrType.cc
+-rw-r--r--   0        0        0      577 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/TupleType.cc
+-rw-r--r--   0        0        0     3990 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/internalBinding/utils.cc
+-rw-r--r--   0        0        0     2404 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/internalBinding.cc
+-rw-r--r--   0        0        0    10785 2023-07-28 19:27:20.672786 pythonmonkey-0.2.1/src/jsTypeFactory.cc
+-rw-r--r--   0        0        0    18726 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/src/modules/pythonmonkey/pythonmonkey.cc
+-rw-r--r--   0        0        0     7365 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/src/pyTypeFactory.cc
+-rw-r--r--   0        0        0     3502 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/src/setSpiderMonkeyException.cc
+-rwxr-xr-x   0        0        0     1249 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/commonjs-modules.bash
+-rw-r--r--   0        0        0      602 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/console-smoke.simple
+-rwxr-xr-x   0        0        0      935 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/console-stdio.bash
+-rw-r--r--   0        0        0     1008 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/console-this.simple
+-rw-r--r--   0        0        0      532 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/is-compilable-unit.simple
+-rw-r--r--   0        0        0      962 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/array-change-index.simple
+-rw-r--r--   0        0        0      873 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/arraybuffer.simple
+-rw-r--r--   0        0        0      787 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/bigint.simple
+-rw-r--r--   0        0        0      866 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/boolean.simple
+-rw-r--r--   0        0        0     1175 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/datetime.simple
+-rw-r--r--   0        0        0     2003 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/datetime2.simple
+-rw-r--r--   0        0        0      810 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/function-curry.simple
+-rw-r--r--   0        0        0      733 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/higher-order-function.simple
+-rw-r--r--   0        0        0      846 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/promise-await-in-python.simple.failing
+-rw-r--r--   0        0        0      718 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/promise.simple.failing
+-rw-r--r--   0        0        0      699 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/string.simple
+-rw-r--r--   0        0        0      519 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/js2py/trivial-function.simple
+-rw-r--r--   0        0        0      278 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/load-cjs-module.simple
+-rw-r--r--   0        0        0      368 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/load-cjs-python-module.simple
+-rw-r--r--   0        0        0      268 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/modules/cjs-module.js
+-rw-r--r--   0        0        0       67 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/modules/print-load.js
+-rw-r--r--   0        0        0      246 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/modules/python-cjs-module.py
+-rw-r--r--   0        0        0      371 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/modules/vm-tools.py
+-rw-r--r--   0        0        0      447 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/not-strict-mode.simple
+-rwxr-xr-x   0        0        0      750 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-eopt.bash
+-rwxr-xr-x   0        0        0     1211 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-global-arguments.bash
+-rwxr-xr-x   0        0        0     1289 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-interactive-smoke.bash
+-rwxr-xr-x   0        0        0      747 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-popt.bash
+-rwxr-xr-x   0        0        0     1089 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-require-cache.bash
+-rwxr-xr-x   0        0        0      753 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/pmjs-ropt.bash
+-rw-r--r--   0        0        0     1169 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/program-module.simple
+-rwxr-xr-x   0        0        0      635 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/program.js
+-rw-r--r--   0        0        0      639 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/array-change-index.simple
+-rw-r--r--   0        0        0      681 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/arraybuffer.simple
+-rw-r--r--   0        0        0     1026 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/boolean.simple
+-rw-r--r--   0        0        0     1515 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/datetime.simple
+-rw-r--r--   0        0        0      903 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/function-curry.simple.failing
+-rw-r--r--   0        0        0      666 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/higher-order-function.simple
+-rw-r--r--   0        0        0      591 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/integer.simple
+-rw-r--r--   0        0        0      669 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/promise.simple.failing
+-rw-r--r--   0        0        0      538 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/string.simple
+-rw-r--r--   0        0        0      471 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/py2js/trivial-function.simple
+-rwxr-xr-x   0        0        0      796 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/require-module-stack.bash.failing
+-rw-r--r--   0        0        0     1672 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/test-atob-btoa.simple
+-rw-r--r--   0        0        0      330 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/throw-filename.js
+-rwxr-xr-x   0        0        0     1208 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/typeofs-segfaults.simple.failing
+-rwxr-xr-x   0        0        0     1667 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/typeofs.simple
+-rw-r--r--   0        0        0      432 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/js/use-strict.simple
+-rw-r--r--   0        0        0      356 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/conftest.py
+-rw-r--r--   0        0        0     6491 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_bigints.py
+-rw-r--r--   0        0        0    11020 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_buffer_typed_array.py
+-rw-r--r--   0        0        0     4135 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_dicts_lists.py
+-rw-r--r--   0        0        0    14294 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_event_loop.py
+-rw-r--r--   0        0        0    10622 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_pythonmonkey_eval.py
+-rw-r--r--   0        0        0      576 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_reentrance_smoke.py
+-rw-r--r--   0        0        0     9095 2023-07-28 19:27:20.676786 pythonmonkey-0.2.1/tests/python/test_strings.py
+-rw-r--r--   0        0        0    16028 1970-01-01 00:00:00.000000 pythonmonkey-0.2.1/PKG-INFO
```

### Comparing `pythonmonkey-0.2.0/CMakeLists.txt` & `pythonmonkey-0.2.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/LICENSE` & `pythonmonkey-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/README.md` & `pythonmonkey-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -346,17 +346,42 @@
 ```
 
 # Troubleshooting Tips
 
 ## CommonJS (require)
 If you are having trouble with the CommonJS require function, set environment variable `DEBUG='ctx-module*'` and you can see the filenames it tries to laod.
 
+## pmdb
+
+PythonMonkey has a built-in gdb-like JavaScript command-line debugger called **pmdb**, which would be automatically triggered on `debugger;` statements and uncaught exceptions.
+
+To enable **pmdb**, simply call `from pythonmonkey.lib import pmdb; pmdb.enable()` before doing anything on PythonMonkey.
+
+```py
+import pythonmonkey as pm
+from pythonmonkey.lib import pmdb
+
+pmdb.enable()
+
+pm.eval("...")
+```
+
+Run `help` command in **pmdb** to see available commands.
+
+```console
+(pmdb) > help
+List of commands:
+• ...
+• ...
+```
+
 ## pmjs
 - there is a `.help` menu in the REPL
 - there is a `--help` command-line option
+- the `--inspect` option enables **pmdb**, a gdb-like JavaScript command-line debugger
 - the `-r` option can be used to load a module before your program or the REPL runs
 - the `-e` option can be used evaluate code -- e.g. define global variables -- before your program or the REPL runs
 - The REPL can evaluate Python expressions, storing them in variables named `$1`, `$2`, etc.
 
 ```console
 $ pmjs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pythonmonkey-0.2.0/build.py` & `pythonmonkey-0.2.1/build.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/docs/CMakeLists.txt` & `pythonmonkey-0.2.1/cmake/docs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/externals/autopep8/CMakeLists.txt` & `pythonmonkey-0.2.1/cmake/externals/autopep8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/externals/uncrustify/CMakeLists.txt` & `pythonmonkey-0.2.1/cmake/externals/uncrustify/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/format/CMakeLists.txt` & `pythonmonkey-0.2.1/cmake/format/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/format/uncrustify.cfg` & `pythonmonkey-0.2.1/cmake/format/uncrustify.cfg`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/cmake/modules/FindSpiderMonkey.cmake` & `pythonmonkey-0.2.1/cmake/modules/FindSpiderMonkey.cmake`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/BoolType.hh` & `pythonmonkey-0.2.1/include/BoolType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/BufferType.hh` & `pythonmonkey-0.2.1/include/BufferType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/DateType.hh` & `pythonmonkey-0.2.1/include/DateType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/DictType.hh` & `pythonmonkey-0.2.1/include/DictType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/ExceptionType.hh` & `pythonmonkey-0.2.1/include/ExceptionType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/FloatType.hh` & `pythonmonkey-0.2.1/include/FloatType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/FuncType.hh` & `pythonmonkey-0.2.1/include/FuncType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/IntType.hh` & `pythonmonkey-0.2.1/include/IntType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/JSObjectProxy.hh` & `pythonmonkey-0.2.1/include/JSObjectProxy.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/JobQueue.hh` & `pythonmonkey-0.2.1/include/JobQueue.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/ListType.hh` & `pythonmonkey-0.2.1/include/ListType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/NullType.hh` & `pythonmonkey-0.2.1/include/NullType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/PromiseType.hh` & `pythonmonkey-0.2.1/include/PromiseType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/PyEventLoop.hh` & `pythonmonkey-0.2.1/include/PyEventLoop.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/PyProxyHandler.hh` & `pythonmonkey-0.2.1/include/PyProxyHandler.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/PyType.hh` & `pythonmonkey-0.2.1/include/PyType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/StrType.hh` & `pythonmonkey-0.2.1/include/StrType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/TupleType.hh` & `pythonmonkey-0.2.1/include/TupleType.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/TypeEnum.hh` & `pythonmonkey-0.2.1/include/TypeEnum.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/internalBinding.hh` & `pythonmonkey-0.2.1/include/internalBinding.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/jsTypeFactory.hh` & `pythonmonkey-0.2.1/include/jsTypeFactory.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/modules/pythonmonkey/pythonmonkey.hh` & `pythonmonkey-0.2.1/include/modules/pythonmonkey/pythonmonkey.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/pyTypeFactory.hh` & `pythonmonkey-0.2.1/include/pyTypeFactory.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/include/setSpiderMonkeyException.hh` & `pythonmonkey-0.2.1/include/setSpiderMonkeyException.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/pyproject.toml` & `pythonmonkey-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythonmonkey"
-version = "0.2.0" # automatically set by poetry-dynamic-versioning
+version = "0.2.1" # automatically set by poetry-dynamic-versioning
 description = ""
 authors = ["Caleb Aikens <caleb@distributive.network>", "Tom Tang <xmader@distributive.network>", "Wes Garland <wes@distributive.network>", "Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [
   { include = "pythonmonkey", from = "python" },
 ]
 include = [
@@ -24,15 +24,15 @@
   { path = "CMakeLists.txt", format = "sdist" },
   { path = "*.sh", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pyreadline3 = "^3.4.1"
+pyreadline3 = { version = "^3.4.1", platform = "win32" }
 pminit = { version = "*", allow-prereleases = true }
 
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
```

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/__init__.py` & `pythonmonkey-0.2.1/python/pythonmonkey/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Export public PythonMonkey APIs
 from .pythonmonkey import *
+from .helpers import *
 from .require import *
 
 # Expose the package version
 import importlib.metadata
 __version__= importlib.metadata.version(__name__)
 del importlib
 
@@ -20,8 +21,8 @@
     get() {
       return () => makeList(...Object.keys(this))
     }
   }
   Object.defineProperty(Object.prototype, "keys", keysMethod)
   Object.defineProperty(Array.prototype, "keys", keysMethod)
 }
-""")(lambda *args: list(args))
+""", { 'filename': __file__, 'fromPythonFrame': True })(lambda *args: list(args))
```

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.d.ts` & `pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/base64.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/base64.py` & `pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/base64.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/console.js` & `pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/console.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts` & `pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/internal-binding.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/builtin_modules/util.js` & `pythonmonkey-0.2.1/python/pythonmonkey/builtin_modules/util.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/cli/pmjs.py` & `pythonmonkey-0.2.1/python/pythonmonkey/cli/pmjs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #! /usr/bin/env python3
 # @file         pmjs - PythonMonkey REPL
 # @author       Wes Garland, wes@distributive.network
 # @date         June 2023
 
 import sys, os, signal, getopt
-try:
-  import readline # Unix
-except ImportError:
-  import pyreadline3 as readline # Windows
+import readline
 import pythonmonkey as pm
+from pythonmonkey.lib import pmdb
+
 globalThis = pm.eval("globalThis")
 evalOpts = { 'filename': __file__, 'fromPythonFrame': True, 'strict': False } # type: pm.EvalOptions
 
 if (os.getenv('PMJS_PATH')):
     requirePath = list(map(os.path.abspath, os.getenv('PMJS_PATH').split(',')))
 else:
     requirePath = False;
@@ -286,14 +285,15 @@
   -e, --eval=...       evaluate script
   -h, --help           print pnode command line options (currently set)
   -i, --interactive    always enter the REPL even if stdin does not appear to be a terminal
   -p, --print [...]    evaluate script and print result
   -r, --require...     module to preload (option can be repeated)
   -v, --version        print PythonMonkey version
   --use-strict         evaluate -e, -p, and REPL code in strict mode
+  --inspect            enable pmdb, a gdb-like JavaScript debugger interface
   
 Environment variables:
 TZ                            specify the timezone configuration
 PMJS_PATH                     ':'-separated list of directories prefixed to the module search path
 PMJS_REPL_HISTORY             path to the persistent REPL history file"""
     )
 
@@ -319,15 +319,15 @@
     """
     enterRepl = sys.stdin.isatty()
     forceRepl = False
     globalInitModule = initGlobalThis()
     global requirePath
     
     try:
-        opts, args = getopt.getopt(sys.argv[1:], "hie:p:r:v", ["help", "eval=", "print=", "require=", "version", "use-strict"])
+        opts, args = getopt.getopt(sys.argv[1:], "hie:p:r:v", ["help", "eval=", "print=", "require=", "version", "interactive", "use-strict", "inspect"])
     except getopt.GetoptError as err:
         # print help information and exit:
         print(err)  # will print something like "option -a not recognized"
         usage()
         sys.exit(2)
     output = None
     verbose = False
@@ -346,14 +346,16 @@
             pm.eval(a, evalOpts)
             enterRepl = False
         elif o in ("-p", "--print"):
             print(pm.eval(a, evalOpts))
             enterRepl = False
         elif o in ("-r", "--require"):
             globalThis.require(a)
+        elif o in ("--inspect"):
+            pmdb.enable()
         else:
             assert False, "unhandled option"
 
     if (len(args) > 0):
         globalInitModule.patchGlobalRequire()
         pm.runProgramModule(args[0], args, requirePath)
     elif (enterRepl or forceRepl):
```

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/global.d.ts` & `pythonmonkey-0.2.1/python/pythonmonkey/global.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/lib/pmjs/global-init.js` & `pythonmonkey-0.2.1/python/pythonmonkey/lib/pmjs/global-init.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/pythonmonkey.pyi` & `pythonmonkey-0.2.1/python/pythonmonkey/pythonmonkey.pyi`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/python/pythonmonkey/require.py` & `pythonmonkey-0.2.1/python/pythonmonkey/require.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,32 +41,32 @@
     "node_modules"
   )
 )
 evalOpts = { 'filename': __file__, 'fromPythonFrame': True } # type: pm.EvalOptions
 
 # Force to use UTF-8 encoding
 # Windows may use other encodings / code pages that have many characters missing/unrepresentable
-# Error: Python UnicodeEncodeError: 'charmap' codec can't encode characters in position xx-xx: character maps to <undefined>
-sys.stdout.reconfigure(encoding='utf-8')
-sys.stderr.reconfigure(encoding='utf-8')
+if isinstance(sys.stdin,  io.TextIOWrapper): sys.stdin.reconfigure(encoding='utf-8')
+if isinstance(sys.stdout, io.TextIOWrapper): sys.stdout.reconfigure(encoding='utf-8')
+if isinstance(sys.stderr, io.TextIOWrapper): sys.stderr.reconfigure(encoding='utf-8')
 
 # Add some python functions to the global python object for code in this file to use.
 globalThis = pm.eval("globalThis;", evalOpts)
 pm.eval("globalThis.python = { pythonMonkey: {}, stdout: {}, stderr: {} }", evalOpts);
 globalThis.pmEval = pm.eval
 globalThis.python.pythonMonkey.dir = os.path.dirname(__file__)
 #globalThis.python.pythonMonkey.version = pm.__version__
 #globalThis.python.pythonMonkey.module = pm
 globalThis.python.pythonMonkey.isCompilableUnit = pm.isCompilableUnit
 globalThis.python.pythonMonkey.nodeModules = node_modules
 globalThis.python.print  = print
-globalThis.python.stdout.write = sys.stdout.write
-globalThis.python.stderr.write = sys.stderr.write
-globalThis.python.stdout.read = sys.stdout.read
-globalThis.python.stderr.read = sys.stderr.read
+globalThis.python.stdout.write = lambda s: sys.stdout.write(s)
+globalThis.python.stderr.write = lambda s: sys.stderr.write(s)
+globalThis.python.stdout.read = lambda n: sys.stdout.read(n)
+globalThis.python.stderr.read = lambda n: sys.stderr.read(n)
 globalThis.python.eval = eval
 globalThis.python.exec = exec
 globalThis.python.getenv = os.getenv
 globalThis.python.paths  = sys.path
 
 globalThis.python.exit = pm.eval("""'use strict';
 (exit) => function pythonExitWrapper(exitCode) {
@@ -348,9 +348,9 @@
     # Retrieve the caller’s filename from the call stack
     filename = inspect.stack()[1].filename
     # From the REPL, the filename is "<stdin>", which is not a valid path
     if not os.path.exists(filename):
       filename = os.path.join(os.getcwd(), "__main__") # use the CWD instead
     return createRequire(filename)(moduleIdentifier)
 
-# Restrict what are exposed to the pythonmonkey module.
+# Restrict what symbols are exposed to the pythonmonkey module.
 __all__ = ["globalThis", "require", "createRequire", "runProgramModule"]
```

### Comparing `pythonmonkey-0.2.0/setup.sh` & `pythonmonkey-0.2.1/setup.sh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/BufferType.cc` & `pythonmonkey-0.2.1/src/BufferType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/CMakeLists.txt` & `pythonmonkey-0.2.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/DateType.cc` & `pythonmonkey-0.2.1/src/DateType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/DictType.cc` & `pythonmonkey-0.2.1/src/DictType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/ExceptionType.cc` & `pythonmonkey-0.2.1/src/ExceptionType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/IntType.cc` & `pythonmonkey-0.2.1/src/IntType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/JSObjectProxy.cc` & `pythonmonkey-0.2.1/src/JSObjectProxy.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/JobQueue.cc` & `pythonmonkey-0.2.1/src/JobQueue.cc`

 * *Files 10% similar despite different names*

```diff
@@ -35,27 +35,26 @@
   if (!loop.initialized()) return false;
   loop.enqueue(callback);
 
   return true;
 }
 
 void JobQueue::runJobs(JSContext *cx) {
-  // TODO (Tom Tang):
-  throw std::logic_error("JobQueue::runJobs is not implemented.");
+  return;
 }
 
 // is empty
 bool JobQueue::empty() const {
   // TODO (Tom Tang): implement using `get_running_loop` and getting job count on loop???
   throw std::logic_error("JobQueue::empty is not implemented\n");
 }
 
 js::UniquePtr<JS::JobQueue::SavedJobQueue> JobQueue::saveJobQueue(JSContext *cx) {
-  // TODO (Tom Tang): implement this method way later
-  throw std::logic_error("JobQueue::saveJobQueue is not implemented\n");
+  auto saved = js::MakeUnique<JS::JobQueue::SavedJobQueue>();
+  return saved;
 }
 
 bool JobQueue::init(JSContext *cx) {
   JS::SetJobQueue(cx, this);
   JS::InitDispatchToEventLoop(cx, /* callback */ dispatchToEventLoop, /* closure */ cx);
   return true;
 }
```

### Comparing `pythonmonkey-0.2.0/src/ListType.cc` & `pythonmonkey-0.2.1/src/ListType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/PromiseType.cc` & `pythonmonkey-0.2.1/src/PromiseType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/PyEventLoop.cc` & `pythonmonkey-0.2.1/src/PyEventLoop.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/PyProxyHandler.cc` & `pythonmonkey-0.2.1/src/PyProxyHandler.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/StrType.cc` & `pythonmonkey-0.2.1/src/StrType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/TupleType.cc` & `pythonmonkey-0.2.1/src/TupleType.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/internalBinding/utils.cc` & `pythonmonkey-0.2.1/src/internalBinding/utils.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/internalBinding.cc` & `pythonmonkey-0.2.1/src/internalBinding.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/jsTypeFactory.cc` & `pythonmonkey-0.2.1/src/jsTypeFactory.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/modules/pythonmonkey/pythonmonkey.cc` & `pythonmonkey-0.2.1/src/modules/pythonmonkey/pythonmonkey.cc`

 * *Files 2% similar despite different names*

```diff
@@ -427,22 +427,30 @@
   static JSClass globalClass = {"global", JSCLASS_GLOBAL_FLAGS, &JS::DefaultGlobalClassOps};
   global = new JS::RootedObject(GLOBAL_CX, JS_NewGlobalObject(GLOBAL_CX, &globalClass, nullptr, JS::FireOnNewGlobalHook, options));
   if (!global) {
     PyErr_SetString(SpiderMonkeyError, "Spidermonkey could not create a global object.");
     return NULL;
   }
 
+  JS::RootedObject debuggerGlobal(GLOBAL_CX, JS_NewGlobalObject(GLOBAL_CX, &globalClass, nullptr, JS::FireOnNewGlobalHook, options));
+  {
+    JSAutoRealm r(GLOBAL_CX, debuggerGlobal);
+    JS_DefineProperty(GLOBAL_CX, debuggerGlobal, "mainGlobal", *global, JSPROP_READONLY);
+    JS_DefineDebuggerObject(GLOBAL_CX, debuggerGlobal);
+  }
+
   autoRealm = new JSAutoRealm(GLOBAL_CX, *global);
 
   if (!JS_DefineFunctions(GLOBAL_CX, *global, jsGlobalFunctions)) {
     PyErr_SetString(SpiderMonkeyError, "Spidermonkey could not define global functions.");
     return NULL;
   }
 
   JS_SetGCCallback(GLOBAL_CX, handleSharedPythonMonkeyMemory, NULL);
+  JS_DefineProperty(GLOBAL_CX, *global, "debuggerGlobal", debuggerGlobal, JSPROP_READONLY);
 
   // XXX: SpiderMonkey bug???
   // In https://hg.mozilla.org/releases/mozilla-esr102/file/3b574e1/js/src/jit/CacheIR.cpp#l317, trying to use the callback returned by `js::GetDOMProxyShadowsCheck()` even it's unset (nullptr)
   // Temporarily solved by explicitly setting the `domProxyShadowsCheck` callback here
   JS::SetDOMProxyInformation(nullptr,
     [](JSContext *, JS::HandleObject, JS::HandleId) {   // domProxyShadowsCheck
       return JS::DOMProxyShadowsResult::ShadowCheckFailed;
```

### Comparing `pythonmonkey-0.2.0/src/pyTypeFactory.cc` & `pythonmonkey-0.2.1/src/pyTypeFactory.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/src/setSpiderMonkeyException.cc` & `pythonmonkey-0.2.1/src/setSpiderMonkeyException.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/commonjs-modules.bash` & `pythonmonkey-0.2.1/tests/js/commonjs-modules.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/console-smoke.simple` & `pythonmonkey-0.2.1/tests/js/console-smoke.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/console-stdio.bash` & `pythonmonkey-0.2.1/tests/js/console-stdio.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/console-this.simple` & `pythonmonkey-0.2.1/tests/js/console-this.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/is-compilable-unit.simple` & `pythonmonkey-0.2.1/tests/js/is-compilable-unit.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/array-change-index.simple` & `pythonmonkey-0.2.1/tests/js/js2py/array-change-index.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/arraybuffer.simple` & `pythonmonkey-0.2.1/tests/js/js2py/arraybuffer.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/bigint.simple` & `pythonmonkey-0.2.1/tests/js/js2py/bigint.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/boolean.simple` & `pythonmonkey-0.2.1/tests/js/js2py/boolean.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/datetime.simple` & `pythonmonkey-0.2.1/tests/js/js2py/datetime.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/datetime2.simple` & `pythonmonkey-0.2.1/tests/js/js2py/datetime2.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/function-curry.simple` & `pythonmonkey-0.2.1/tests/js/js2py/function-curry.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/higher-order-function.simple` & `pythonmonkey-0.2.1/tests/js/js2py/higher-order-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/promise-await-in-python.simple.failing` & `pythonmonkey-0.2.1/tests/js/js2py/promise-await-in-python.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/promise.simple.failing` & `pythonmonkey-0.2.1/tests/js/js2py/promise.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/string.simple` & `pythonmonkey-0.2.1/tests/js/js2py/string.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/js2py/trivial-function.simple` & `pythonmonkey-0.2.1/tests/js/js2py/trivial-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-eopt.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-eopt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-global-arguments.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-global-arguments.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-interactive-smoke.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-interactive-smoke.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-popt.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-popt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-require-cache.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-require-cache.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/pmjs-ropt.bash` & `pythonmonkey-0.2.1/tests/js/pmjs-ropt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/program-module.simple` & `pythonmonkey-0.2.1/tests/js/program-module.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/program.js` & `pythonmonkey-0.2.1/tests/js/program.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/array-change-index.simple` & `pythonmonkey-0.2.1/tests/js/py2js/array-change-index.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/arraybuffer.simple` & `pythonmonkey-0.2.1/tests/js/py2js/arraybuffer.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/boolean.simple` & `pythonmonkey-0.2.1/tests/js/py2js/boolean.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/datetime.simple` & `pythonmonkey-0.2.1/tests/js/py2js/datetime.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/function-curry.simple.failing` & `pythonmonkey-0.2.1/tests/js/py2js/function-curry.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/higher-order-function.simple` & `pythonmonkey-0.2.1/tests/js/py2js/higher-order-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/integer.simple` & `pythonmonkey-0.2.1/tests/js/py2js/integer.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/promise.simple.failing` & `pythonmonkey-0.2.1/tests/js/py2js/promise.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/py2js/string.simple` & `pythonmonkey-0.2.1/tests/js/py2js/string.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/require-module-stack.bash.failing` & `pythonmonkey-0.2.1/tests/js/require-module-stack.bash.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/test-atob-btoa.simple` & `pythonmonkey-0.2.1/tests/js/test-atob-btoa.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/typeofs-segfaults.simple.failing` & `pythonmonkey-0.2.1/tests/js/typeofs-segfaults.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/js/typeofs.simple` & `pythonmonkey-0.2.1/tests/js/typeofs.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_bigints.py` & `pythonmonkey-0.2.1/tests/python/test_bigints.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_buffer_typed_array.py` & `pythonmonkey-0.2.1/tests/python/test_buffer_typed_array.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_dicts_lists.py` & `pythonmonkey-0.2.1/tests/python/test_dicts_lists.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_event_loop.py` & `pythonmonkey-0.2.1/tests/python/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_pythonmonkey_eval.py` & `pythonmonkey-0.2.1/tests/python/test_pythonmonkey_eval.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_reentrance_smoke.py` & `pythonmonkey-0.2.1/tests/python/test_reentrance_smoke.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/tests/python/test_strings.py` & `pythonmonkey-0.2.1/tests/python/test_strings.py`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.2.0/PKG-INFO` & `pythonmonkey-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pythonmonkey
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Caleb Aikens
 Author-email: caleb@distributive.network
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pminit
-Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0)
+Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform == "win32"
 Description-Content-Type: text/markdown
 
 # PythonMonkey
 
 ![Testing Suite](https://github.com/Kings-Distributed-Systems/PythonMonkey/actions/workflows/tests.yaml/badge.svg)
 
 ## About
@@ -362,17 +362,42 @@
 ```
 
 # Troubleshooting Tips
 
 ## CommonJS (require)
 If you are having trouble with the CommonJS require function, set environment variable `DEBUG='ctx-module*'` and you can see the filenames it tries to laod.
 
+## pmdb
+
+PythonMonkey has a built-in gdb-like JavaScript command-line debugger called **pmdb**, which would be automatically triggered on `debugger;` statements and uncaught exceptions.
+
+To enable **pmdb**, simply call `from pythonmonkey.lib import pmdb; pmdb.enable()` before doing anything on PythonMonkey.
+
+```py
+import pythonmonkey as pm
+from pythonmonkey.lib import pmdb
+
+pmdb.enable()
+
+pm.eval("...")
+```
+
+Run `help` command in **pmdb** to see available commands.
+
+```console
+(pmdb) > help
+List of commands:
+• ...
+• ...
+```
+
 ## pmjs
 - there is a `.help` menu in the REPL
 - there is a `--help` command-line option
+- the `--inspect` option enables **pmdb**, a gdb-like JavaScript command-line debugger
 - the `-r` option can be used to load a module before your program or the REPL runs
 - the `-e` option can be used evaluate code -- e.g. define global variables -- before your program or the REPL runs
 - The REPL can evaluate Python expressions, storing them in variables named `$1`, `$2`, etc.
 
 ```console
 $ pmjs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

