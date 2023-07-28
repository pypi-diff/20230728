# Comparing `tmp/memray-1.8.1.tar.gz` & `tmp/memray-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memray-1.8.1.tar", last modified: Tue Jun 20 15:33:21 2023, max compression
+gzip compressed data, was "memray-1.9.0.tar", last modified: Fri Jul 28 17:02:09 2023, max compression
```

## Comparing `memray-1.8.1.tar` & `memray-1.9.0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.937368 memray-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 15:33:07.000000 memray-1.8.1/.babelrc
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-20 15:33:07.000000 memray-1.8.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-20 15:33:07.000000 memray-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-20 15:33:07.000000 memray-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-20 15:33:07.000000 memray-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-20 15:33:07.000000 memray-1.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-06-20 15:33:07.000000 memray-1.8.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-06-20 15:33:21.937368 memray-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-06-20 15:33:07.000000 memray-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   529986 2023-06-20 15:33:07.000000 memray-1.8.1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 15:33:07.000000 memray-1.8.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-20 15:33:07.000000 memray-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:33:21.937368 memray-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-20 15:33:07.000000 memray-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.889365 memray-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.897365 memray-1.8.1/src/memray/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.897365 memray-1.8.1/src/memray/_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_ipython/flamegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.905366 memray-1.8.1/src/memray/_memray/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/algorithm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/alloc.h
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/alloc.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/compat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/elf_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/elf_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/frame_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/hooks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/hooks.h
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/hooks.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/inject.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/linker_shenanigans.h
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/lz4_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/macho_shenanigans.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/macho_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/native_resolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/native_resolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/native_resolver.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/pthread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/python_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/python_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_reader.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/record_writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/records.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/records.h
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/records.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/sink.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/sink.h
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/sink.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    34716 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/snapshot.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17955 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/snapshot.h
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/snapshot.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/socket_reader_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/socket_reader_thread.h
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/socket_reader_thread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/source.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/source.h
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/source.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    36803 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/tracking_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/tracking_api.h
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray/tracking_api.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54621 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_memray_test_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_test_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.909366 memray-1.8.1/src/memray/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/_attach.gdb
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/_attach.lldb
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/attach.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/commands/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.909366 memray-1.8.1/src/memray/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.909366 memray-1.8.1/src/memray/reporters/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/common.js
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/common.test.js
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/assets/temporal_flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/flamegraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/frame_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.913366 memray-1.8.1/src/memray/reporters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.913366 memray-1.8.1/src/memray/reporters/templates/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/flamegraph.css
--rw-r--r--   0 runner    (1001) docker     (123)    78020 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)    73346 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/flamegraph_common.js
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/table.css
--rw-r--r--   0 runner    (1001) docker     (123)    72863 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/table.js
--rw-r--r--   0 runner    (1001) docker     (123)    81214 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/assets/temporal_flamegraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/classic_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/flamegraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/templates/temporal_flamegraph.html
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-06-20 15:33:07.000000 memray-1.8.1/src/memray/reporters/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.897365 memray-1.8.1/src/memray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:33:21.000000 memray-1.8.1/src/memray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.913366 memray-1.8.1/src/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.933367 memray-1.8.1/src/vendor/libbacktrace/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/aclocal.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/allocfail.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/allocfail.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/atomic.c
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/backtrace-supported.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/backtrace.c
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/backtrace.h
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/btest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:21.937368 memray-1.8.1/src/vendor/libbacktrace/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/enable.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/lead-dot.m4
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/multi.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/override.m4
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/unwind_ipinfo.m4
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config/warnings.m4
--rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config.guess
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/config.sub
--rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/configure
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/configure.ac
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/debuginfod_support.h
--rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/dwarf.c
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/edtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/edtest2.c
--rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/elf.c
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/fileline.c
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/filenames.h
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/filetype.awk
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
--rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/install-sh
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/instrumented_alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/internal.h
--rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/libtool.m4
--rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ltmain.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ltoptions.m4
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ltsugar.m4
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ltversion.m4
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/lt~obsolete.m4
--rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/macho.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/missing
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/mmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/mmapio.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/move-if-change
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/mtest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/nounwind.c
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/pecoff.c
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/posix.c
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/print.c
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/read.c
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/simple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/sort.c
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/state.c
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/stest.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/test-driver
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/test_format.c
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/testlib.c
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/testlib.h
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ttest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/unittest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/unknown.c
--rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/xcoff.c
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/xztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace/ztest.c
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-06-20 15:33:07.000000 memray-1.8.1/src/vendor/regenerate_libbacktrace.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 15:33:07.000000 memray-1.8.1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.941002 memray-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 17:01:54.000000 memray-1.9.0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-28 17:01:54.000000 memray-1.9.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-28 17:01:54.000000 memray-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-28 17:01:54.000000 memray-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-28 17:01:54.000000 memray-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-28 17:01:54.000000 memray-1.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-28 17:01:54.000000 memray-1.9.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-07-28 17:02:09.941002 memray-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-28 17:01:54.000000 memray-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   529986 2023-07-28 17:01:54.000000 memray-1.9.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-28 17:01:54.000000 memray-1.9.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-28 17:01:54.000000 memray-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:02:09.941002 memray-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-28 17:01:54.000000 memray-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.900999 memray-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray/_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_ipython/flamegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.921000 memray-1.9.0/src/memray/_memray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/algorithm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/alloc.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/compat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/elf_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/elf_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/frame_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.h
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/hooks.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/inject.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/linker_shenanigans.h
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/lz4_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/macho_shenanigans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/macho_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/native_resolver.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/pthread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/python_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/python_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42922 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_reader.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/record_writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/records.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/sink.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34716 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17955 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/snapshot.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/socket_reader_thread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.h
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/source.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    36947 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray/tracking_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54621 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_memray_test_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_test_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.921000 memray-1.9.0/src/memray/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/_attach.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/_attach.lldb
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/commands/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/common.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/common.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/flamegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/frame_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/memray/reporters/templates/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.css
+-rw-r--r--   0 runner    (1001) docker     (123)    78020 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73346 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/flamegraph_common.js
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)    72863 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)    81214 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/assets/temporal_flamegraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/classic_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/templates/temporal_flamegraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-07-28 17:01:54.000000 memray-1.9.0/src/memray/reporters/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.909000 memray-1.9.0/src/memray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17178 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 17:02:09.000000 memray-1.9.0/src/memray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.925001 memray-1.9.0/src/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.937001 memray-1.9.0/src/vendor/libbacktrace/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   567198 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)   123456 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/aclocal.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/allocfail.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3135 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/allocfail.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/atomic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace-supported.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/backtrace.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/btest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7382 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:02:09.941002 memray-1.9.0/src/vendor/libbacktrace/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/enable.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/lead-dot.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/multi.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/override.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config/warnings.m4
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49446 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.guess
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35295 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/config.sub
+-rwxr-xr-x   0 runner    (1001) docker     (123)   452188 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/configure
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/debuginfod_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)   116397 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/dwarf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/edtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/edtest2.c
+-rw-r--r--   0 runner    (1001) docker     (123)   133952 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/elf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/fileline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/filenames.h
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/filetype.awk
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14675 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/install-sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/instrumented_alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)   263960 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/libtool.m4
+-rw-r--r--   0 runner    (1001) docker     (123)   249764 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltmain.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltoptions.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltsugar.m4
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ltversion.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/lt~obsolete.m4
+-rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/macho.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6872 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/missing
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mmapio.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/move-if-change
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/mtest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/nounwind.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/pecoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/posix.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/print.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/read.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/sort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/state.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/stest.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4641 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/test-driver
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/test_format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/testlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/testlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ttest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/unittest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/unknown.c
+-rw-r--r--   0 runner    (1001) docker     (123)    41385 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/xcoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/xztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace/ztest.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-07-28 17:01:54.000000 memray-1.9.0/src/vendor/regenerate_libbacktrace.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 17:01:54.000000 memray-1.9.0/webpack.config.js
```

### Comparing `memray-1.8.1/.pre-commit-config.yaml` & `memray-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/LICENSE` & `memray-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/MANIFEST.in` & `memray-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/Makefile` & `memray-1.9.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 		--cov=memray \
 		--cov=tests \
 		--cov-config=pyproject.toml \
 		--cov-report=term \
 		--cov-fail-under=90 \
 		--cov-append $(PYTEST_ARGS) \
 		tests
+	$(PYTHON) -m coverage lcov -i -o pycoverage.lcov
+	genhtml *coverage.lcov  --branch-coverage --output-directory memray-coverage $(GENHTMLOPTS)
 
 .PHONY: valgrind
 valgrind:  ## Run valgrind, with the correct configuration
 	PYTHONMALLOC=malloc valgrind \
 		--suppressions=./valgrind.supp \
 		--leak-check=full \
 		--show-leak-kinds=definite \
```

### Comparing `memray-1.8.1/NEWS.rst` & `memray-1.9.0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,30 @@
     fix problems like typo corrections or such.
 
 Changelog
 =========
 
 .. towncrier release notes start
 
+memray 1.9.0 (2023-07-28)
+-------------------------
+
+Features
+~~~~~~~~
+
+- Allow to report the current version of Memray via a ``--version/-V`` command line parameter (#420)
+- Add pause/unpause keybindings to the live reporter that allows the user to pause the live reporter to analyse the current results without pausing the running program (#418)
+
+
+Bug Fixes
+~~~~~~~~~
+
+- Support building with Cython 3 (#425)
+
+
 memray 1.8.1 (2023-06-20)
 -------------------------
 
 Features
 ~~~~~~~~
 
 - When the high water mark being shown by a temporal flame graph is before the first memory snapshot or after the last one, tell the user so by highlighting a region beyond the end of the memory usage plot. (#399)
```

### Comparing `memray-1.8.1/PKG-INFO` & `memray-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.8.1
+Version: 1.9.0
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -174,14 +174,15 @@
     parse               Debug a results file by parsing and printing each record in it
     summary             Generate a terminal-based summary report of the functions that allocate most memory
     stats               Generate high level stats of the memory usage in the terminal
 
 optional arguments:
   -h, --help            Show this help message and exit
   -v, --verbose         Increase verbosity. Option is additive and can be specified up to 3 times
+  -V, --version         Displays the current version of Memray
 
 Please submit feedback, ideas, and bug reports by filing a new issue at https://github.com/bloomberg/memray/issues
 ```
 
 To use Memray over a script or a single python file you can use
 
 ```shell
```

### Comparing `memray-1.8.1/README.md` & `memray-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     parse               Debug a results file by parsing and printing each record in it
     summary             Generate a terminal-based summary report of the functions that allocate most memory
     stats               Generate high level stats of the memory usage in the terminal
 
 optional arguments:
   -h, --help            Show this help message and exit
   -v, --verbose         Increase verbosity. Option is additive and can be specified up to 3 times
+  -V, --version         Displays the current version of Memray
 
 Please submit feedback, ideas, and bug reports by filing a new issue at https://github.com/bloomberg/memray/issues
 ```
 
 To use Memray over a script or a single python file you can use
 
 ```shell
```

### Comparing `memray-1.8.1/package-lock.json` & `memray-1.9.0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999361910828025%*

 * *Differences: {"'dependencies'": "{'word-wrap': {'version': '1.2.4', 'resolved': "*

 * *                   "'https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz', 'integrity': "*

 * *                   "'sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA=='}}",*

 * * "'packages'": "{'node_modules/word-wrap': {'version': '1.2.4', 'resolved': "*

 * *               "'https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz', 'integrity': "*

 * *               "'sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8j […]*

```diff
@@ -5624,17 +5624,17 @@
             "dev": true,
             "integrity": "sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==",
             "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.0.tgz",
             "version": "2.0.0"
         },
         "word-wrap": {
             "dev": true,
-            "integrity": "sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==",
-            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz",
-            "version": "1.2.3"
+            "integrity": "sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA==",
+            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz",
+            "version": "1.2.4"
         },
         "wrap-ansi": {
             "dependencies": {
                 "ansi-styles": {
                     "dev": true,
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
@@ -13254,17 +13254,17 @@
             "version": "2.0.0"
         },
         "node_modules/word-wrap": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==",
-            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz",
-            "version": "1.2.3"
+            "integrity": "sha512-2V81OA4ugVo5pRo46hAoD2ivUJx8jXmWXfUkY4KFNw0hEptvN0QfH3K4nHiwzGeKl5rFKedV48QVoqYavy4YpA==",
+            "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.4.tgz",
+            "version": "1.2.4"
         },
         "node_modules/wrap-ansi": {
             "dependencies": {
                 "ansi-styles": "^4.0.0",
                 "string-width": "^4.1.0",
                 "strip-ansi": "^6.0.0"
             },
```

### Comparing `memray-1.8.1/pyproject.toml` & `memray-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ]
 
 [tool.mypy]
 exclude="tests/integration/(native_extension|multithreaded_extension)/"
 
 [tool.cibuildwheel]
 build = ["cp38-*", "cp39-*", "cp310-*", "cp311-*"]
-skip = "*musllinux*i686*"
+skip = "*musllinux*{i686,aarch64}*"
 manylinux-x86_64-image = "manylinux2014"
 manylinux-i686-image = "manylinux2014"
 
 [[tool.cibuildwheel.overrides]]
 select = "cp3{7,8,9,10}-*"
 manylinux-x86_64-image = "manylinux2010"
 manylinux-i686-image = "manylinux2010"
```

### Comparing `memray-1.8.1/setup.py` & `memray-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
 test_requires = [
     "Cython",
     "greenlet; python_version < '3.11'",
     "pytest",
     "pytest-cov",
     "ipython",
+    "setuptools; python_version >= '3.12'",
 ]
 
 benchmark_requires = [
     "asv",
 ]
```

### Comparing `memray-1.8.1/src/memray/__init__.py` & `memray-1.9.0/src/memray/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/__init__.pyi` & `memray-1.9.0/src/memray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_destination.py` & `memray-1.9.0/src/memray/_destination.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_ipython/flamegraph.py` & `memray-1.9.0/src/memray/_ipython/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/CMakeLists.txt` & `memray-1.9.0/src/memray/_memray/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/alloc.pxd` & `memray-1.9.0/src/memray/_memray/alloc.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/compat.cpp` & `memray-1.9.0/src/memray/_memray/compat.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/compat.h` & `memray-1.9.0/src/memray/_memray/compat.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/elf_shenanigans.cpp` & `memray-1.9.0/src/memray/_memray/elf_shenanigans.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/elf_utils.h` & `memray-1.9.0/src/memray/_memray/elf_utils.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/frame_tree.h` & `memray-1.9.0/src/memray/_memray/frame_tree.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/hooks.cpp` & `memray-1.9.0/src/memray/_memray/hooks.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/hooks.h` & `memray-1.9.0/src/memray/_memray/hooks.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/inject.cpp` & `memray-1.9.0/src/memray/_memray/inject.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/logging.cpp` & `memray-1.9.0/src/memray/_memray/logging.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/logging.h` & `memray-1.9.0/src/memray/_memray/logging.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/lz4_stream.h` & `memray-1.9.0/src/memray/_memray/lz4_stream.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/macho_shenanigans.cpp` & `memray-1.9.0/src/memray/_memray/macho_shenanigans.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/macho_utils.h` & `memray-1.9.0/src/memray/_memray/macho_utils.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/native_resolver.cpp` & `memray-1.9.0/src/memray/_memray/native_resolver.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/native_resolver.h` & `memray-1.9.0/src/memray/_memray/native_resolver.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/pthread.pxd` & `memray-1.9.0/src/memray/_memray/pthread.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/python_helpers.cpp` & `memray-1.9.0/src/memray/_memray/python_helpers.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/record_reader.cpp` & `memray-1.9.0/src/memray/_memray/record_reader.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/record_reader.h` & `memray-1.9.0/src/memray/_memray/record_reader.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/record_reader.pxd` & `memray-1.9.0/src/memray/_memray/record_reader.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/record_writer.cpp` & `memray-1.9.0/src/memray/_memray/record_writer.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/record_writer.h` & `memray-1.9.0/src/memray/_memray/record_writer.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/records.cpp` & `memray-1.9.0/src/memray/_memray/records.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/records.h` & `memray-1.9.0/src/memray/_memray/records.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/records.pxd` & `memray-1.9.0/src/memray/_memray/records.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/sink.cpp` & `memray-1.9.0/src/memray/_memray/sink.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/sink.h` & `memray-1.9.0/src/memray/_memray/sink.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/snapshot.cpp` & `memray-1.9.0/src/memray/_memray/snapshot.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/snapshot.h` & `memray-1.9.0/src/memray/_memray/snapshot.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/snapshot.pxd` & `memray-1.9.0/src/memray/_memray/snapshot.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/socket_reader_thread.cpp` & `memray-1.9.0/src/memray/_memray/socket_reader_thread.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/socket_reader_thread.h` & `memray-1.9.0/src/memray/_memray/socket_reader_thread.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/source.cpp` & `memray-1.9.0/src/memray/_memray/source.cpp`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/source.h` & `memray-1.9.0/src/memray/_memray/source.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/tracking_api.cpp` & `memray-1.9.0/src/memray/_memray/tracking_api.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1143,14 +1143,16 @@
 {
     RecursionGuard guard;
     if (!Tracker::isActive()) {
         return 0;
     }
 
     if (frame != PyEval_GetFrame()) {
+        // This should only happen for the phony frames produced by Cython
+        // extension modules that were compiled with `profile=True`.
         return 0;
     }
 
     switch (what) {
         case PyTrace_CALL: {
             return PythonStackTracker::get().pushPythonFrame(frame);
         }
```

### Comparing `memray-1.8.1/src/memray/_memray/tracking_api.h` & `memray-1.9.0/src/memray/_memray/tracking_api.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray/tracking_api.pxd` & `memray-1.9.0/src/memray/_memray/tracking_api.pxd`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray.pyi` & `memray-1.9.0/src/memray/_memray.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray.pyx` & `memray-1.9.0/src/memray/_memray.pyx`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_memray_test_utils.pyx` & `memray-1.9.0/src/memray/_memray_test_utils.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from posix.mman cimport MAP_SHARED
 from posix.mman cimport PROT_WRITE
 from posix.mman cimport mmap
 from posix.mman cimport munmap
 from posix.unistd cimport read
 from posix.unistd cimport write
 
-cimport cython
 from _memray.alloc cimport PyMem_Calloc
 from _memray.alloc cimport PyMem_Free
 from _memray.alloc cimport PyMem_Malloc
 from _memray.alloc cimport PyMem_RawCalloc
 from _memray.alloc cimport PyMem_RawFree
 from _memray.alloc cimport PyMem_RawMalloc
 from _memray.alloc cimport PyMem_RawRealloc
@@ -62,63 +61,53 @@
 
 cdef class MemoryAllocator:
     cdef void* ptr
 
     def __cinit__(self):
         self.ptr = NULL
 
-    @cython.profile(True)
     def free(self):
         if self.ptr == NULL:
             raise RuntimeError("Pointer cannot be NULL")
         free(self.ptr)
         self.ptr = NULL
 
-    @cython.profile(True)
     def malloc(self, size_t size):
         self.ptr = malloc(size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def calloc(self, size_t size):
         self.ptr = calloc(1, size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def realloc(self, size_t size):
         self.ptr = malloc(1)
         self.ptr = realloc(self.ptr, size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def posix_memalign(self, size_t size):
         rc = posix_memalign(&self.ptr, sizeof(void*), size)
         return rc == 0 and self.ptr != NULL
 
-    @cython.profile(True)
     def aligned_alloc(self, size_t size):
         self.ptr = aligned_alloc(sizeof(void*), size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def memalign(self, size_t size):
         self.ptr = memalign(sizeof(void*), size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def valloc(self, size_t size):
         self.ptr = valloc(size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def pvalloc(self, size_t size):
         self.ptr = pvalloc(size)
         return self.ptr != NULL
 
-    @cython.profile(True)
     def run_in_pthread(self, callback):
         cdef pthread_t thread
         cdef int ret = pthread_create(&thread, NULL, &_pthread_worker, <void*>callback)
         if ret != 0:
             raise RuntimeError("Failed to create thread")
         with nogil:
             pthread_join(thread, NULL)
@@ -134,55 +123,51 @@
     cdef void* ptr
     cdef PymallocDomain domain
 
     def __cinit__(self, PymallocDomain domain):
         self.ptr = NULL
         self.domain = domain
 
-    @cython.profile(True)
     def free(self):
         if self.ptr == NULL:
             raise RuntimeError("Pointer cannot be NULL")
         if self.domain == PYMALLOC_RAW:
             PyMem_RawFree(self.ptr)
         elif self.domain == PYMALLOC_MEM:
             PyMem_Free(self.ptr)
         elif self.domain == PYMALLOC_OBJECT:
             PyObject_Free(self.ptr)
         else:
             raise RuntimeError("Invlid pymalloc domain")
         self.ptr = NULL
 
-    @cython.profile(True)
     def malloc(self, size_t size):
         if self.domain == PYMALLOC_RAW:
             self.ptr = PyMem_RawMalloc(size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Malloc(size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Malloc(size)
         else:
             raise RuntimeError("Invlid pymalloc domain")
 
         return self.ptr != NULL
 
-    @cython.profile(True)
     def calloc(self, size_t size):
         if self.domain == PYMALLOC_RAW:
             self.ptr = PyMem_RawCalloc(1, size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Calloc(1, size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Calloc(1, size)
         else:
             raise RuntimeError("Invlid pymalloc domain")
 
         return self.ptr != NULL
 
-    @cython.profile(True)
     def realloc(self, size_t size):
         if self.domain == PYMALLOC_RAW:
             self.ptr = PyMem_RawRealloc(self.ptr, size)
         elif self.domain == PYMALLOC_MEM:
             self.ptr = PyMem_Realloc(self.ptr, size)
         elif self.domain == PYMALLOC_OBJECT:
             self.ptr = PyObject_Realloc(self.ptr, size)
@@ -190,69 +175,60 @@
             raise RuntimeError("Invlid pymalloc domain")
 
         return self.ptr != NULL
 
 cdef do_not_optimize_ptr(void* ptr):
     return ptr == <void*>(1)
 
-@cython.profile(True)
 def _cython_nested_allocation(allocator_fn, size):
     allocator_fn(size)
     cdef void* p = valloc(size);
     do_not_optimize_ptr(p)
     free(p)
 
 cdef class MmapAllocator:
     cdef uintptr_t _address
 
-    @cython.profile(True)
     def __cinit__(self, size, address=0):
         cdef uintptr_t start_address = address
 
         self._address = <uintptr_t>mmap(<void *>start_address, size, PROT_WRITE, MAP_SHARED | MAP_ANONYMOUS, -1, 0)
         if <void *>self._address == MAP_FAILED:
             raise MemoryError
 
     @property
     def address(self):
         return self._address
 
-    @cython.profile(True)
     def munmap(self, length, offset=0):
         cdef uintptr_t addr = self._address + <uintptr_t> offset
         cdef int ret = munmap(<void *>addr, length)
         if ret != 0:
             raise MemoryError(f"munmap rcode: {ret} errno: {errno}")
 
-@cython.profile(True)
-cdef void* _pthread_worker(void* arg) with gil:
+cdef void* _pthread_worker(void* arg) noexcept with gil:
     (<object> arg)()
 
-@cython.profile(False)
 def _cython_allocate_in_two_places(size_t size):
     cdef void* a = allocation_place_a(size)
     do_not_optimize_ptr(a)
     cdef void* b = allocation_place_b(size)
     do_not_optimize_ptr(b)
     free(a)
     free(b)
 
-@cython.profile(False)
 cdef void* allocation_place_a(size_t size):
     return valloc(size)
 
-@cython.profile(False)
 cdef void* allocation_place_b(size_t size):
     return valloc(size)
 
-@cython.profile(True)
 def function_caller(func):
     func()
 
-@cython.profile(False)
 def allocate_without_gil_held(int wake_up_main_fd, int wake_up_thread_fd):
     cdef char buf = 0
     cdef int write_rc = 0
     cdef int read_rc = 0
     cdef void* p = NULL
     with nogil:
         while write_rc != 1:
@@ -262,23 +238,21 @@
         p = valloc(1234)
     do_not_optimize_ptr(p)
     free(p)
     p = valloc(4321)
     do_not_optimize_ptr(p)
     free(p)
 
-@cython.profile(True)
 def allocate_cpp_vector(size_t size):
     cdef vector[int] v;
     cdef size_t nelems = <size_t>(size / sizeof(int))
     v.reserve(nelems)
     return v.size()
 
 
-@cython.profile(True)
 def fill_cpp_vector(size_t size):
     cdef vector[int] v
     cdef size_t nelems = <size_t>(size / sizeof(int))
     for i in range(nelems):
         v.push_back(i)
     return v.size()
```

### Comparing `memray-1.8.1/src/memray/_test.py` & `memray-1.9.0/src/memray/_test.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/_test_utils.pyi` & `memray-1.9.0/src/memray/_test_utils.pyi`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/__init__.py` & `memray-1.9.0/src/memray/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import logging
 import sys
 import textwrap
 from typing import List
 from typing import Optional
 
+from memray._version import __version__
+
 try:
     from typing import Protocol
 except ImportError:
     from typing_extensions import Protocol  # type: ignore
 
 from memray._errors import MemrayCommandError
 from memray._errors import MemrayError
@@ -79,14 +81,21 @@
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
         default=0,
         help="Increase verbosity. Option is additive and can be specified up to 3 times",
     )
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=__version__,
+        help="Displays the current version of Memray",
+    )
 
     subparsers = parser.add_subparsers(
         help="Mode of operation",
         dest="command",
         required=True,
     )
```

### Comparing `memray-1.8.1/src/memray/commands/_attach.gdb` & `memray-1.9.0/src/memray/commands/_attach.gdb`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/_attach.lldb` & `memray-1.9.0/src/memray/commands/_attach.lldb`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/attach.py` & `memray-1.9.0/src/memray/commands/attach.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/common.py` & `memray-1.9.0/src/memray/commands/common.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/flamegraph.py` & `memray-1.9.0/src/memray/commands/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/live.py` & `memray-1.9.0/src/memray/commands/live.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from memray.reporters.tui import TUI
 
 KEYS = {
     "ESC": "\x1b",
     "CTRL_C": "\x03",
     "LEFT": "\x1b\x5b\x44",
     "RIGHT": "\x1b\x5b\x43",
+    "SPACEBAR": "\x20",
     "O": "o",
     "T": "t",
     "A": "a",
 }
 
 
 def _readchar() -> str:  # pragma: no cover
@@ -104,16 +105,18 @@
                 return tui.generate_layout()
 
             with Live(get_renderable=_get_renderable, screen=True):
                 while True:
                     char = readkey()
                     if char == KEYS["LEFT"]:
                         tui.previous_thread()
-                    if char == KEYS["RIGHT"]:
+                    elif char == KEYS["RIGHT"]:
                         tui.next_thread()
                     elif char in {"q", KEYS["ESC"]}:
                         break
+                    elif char == KEYS["SPACEBAR"]:
+                        tui.toggle_pause_state()
                     elif char.lower() in TUI.KEY_TO_COLUMN_ID.keys():
                         col_number = tui.KEY_TO_COLUMN_ID[char.lower()]
                         tui.update_sort_key(col_number)
                     elif char == KEYS["CTRL_C"]:
                         raise KeyboardInterrupt()
```

### Comparing `memray-1.8.1/src/memray/commands/parse.py` & `memray-1.9.0/src/memray/commands/parse.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/run.py` & `memray-1.9.0/src/memray/commands/run.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/stats.py` & `memray-1.9.0/src/memray/commands/stats.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/summary.py` & `memray-1.9.0/src/memray/commands/summary.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/transform.py` & `memray-1.9.0/src/memray/commands/transform.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/commands/tree.py` & `memray-1.9.0/src/memray/commands/tree.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/common.js` & `memray-1.9.0/src/memray/reporters/assets/common.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/common.test.js` & `memray-1.9.0/src/memray/reporters/assets/common.test.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/flamegraph.js` & `memray-1.9.0/src/memray/reporters/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/flamegraph_common.js` & `memray-1.9.0/src/memray/reporters/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/table.js` & `memray-1.9.0/src/memray/reporters/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/assets/temporal_flamegraph.js` & `memray-1.9.0/src/memray/reporters/assets/temporal_flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/flamegraph.py` & `memray-1.9.0/src/memray/reporters/flamegraph.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/frame_tools.py` & `memray-1.9.0/src/memray/reporters/frame_tools.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/stats.py` & `memray-1.9.0/src/memray/reporters/stats.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/summary.py` & `memray-1.9.0/src/memray/reporters/summary.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/table.py` & `memray-1.9.0/src/memray/reporters/table.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/__init__.py` & `memray-1.9.0/src/memray/reporters/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/assets/flamegraph.css` & `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.css`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/assets/flamegraph.js` & `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/assets/flamegraph_common.js` & `memray-1.9.0/src/memray/reporters/templates/assets/flamegraph_common.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/assets/table.js` & `memray-1.9.0/src/memray/reporters/templates/assets/table.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/assets/temporal_flamegraph.js` & `memray-1.9.0/src/memray/reporters/templates/assets/temporal_flamegraph.js`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/base.html` & `memray-1.9.0/src/memray/reporters/templates/base.html`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/classic_base.html` & `memray-1.9.0/src/memray/reporters/templates/classic_base.html`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/flamegraph.html` & `memray-1.9.0/src/memray/reporters/templates/flamegraph.html`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/table.html` & `memray-1.9.0/src/memray/reporters/templates/table.html`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/templates/temporal_flamegraph.html` & `memray-1.9.0/src/memray/reporters/templates/temporal_flamegraph.html`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/transform.py` & `memray-1.9.0/src/memray/reporters/transform.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/tree.py` & `memray-1.9.0/src/memray/reporters/tree.py`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/memray/reporters/tui.py` & `memray-1.9.0/src/memray/reporters/tui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from collections import defaultdict
 from collections import deque
+from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from math import ceil
 from typing import DefaultDict
 from typing import Deque
 from typing import Dict
 from typing import Iterable
@@ -179,14 +180,34 @@
             visited.add(location)
             frame.total_memory += allocation.size
             frame.n_allocations += allocation.n_allocations
             frame.thread_ids.add(allocation.tid)
     return processed_allocations
 
 
+class TUIData:
+    def __init__(self, pid: Optional[int], cmd_line: Optional[str], native: bool):
+        self.pid = pid or "???"
+        if not cmd_line:
+            cmd_line = "???"
+        if len(cmd_line) > 50:
+            cmd_line = cmd_line[:50] + "..."
+        self.command_line = escape(cmd_line)
+        self.native = native
+        self.n_samples = 0
+        self.start = datetime.now()
+        self.last_update = datetime.now()
+        self.snapshot_data: Dict[Location, AllocationEntry] = {}
+        self.current_memory_size = 0
+        self.max_memory_seen = 0
+        self.message = ""
+        self.stream = MemoryGraph(50, 4, 0.0, 1024.0)
+        self.total_allocations = 0
+
+
 class TUI:
     KEY_TO_COLUMN_NAME = {
         1: "total_memory",
         2: "total_memory",
         3: "own_memory",
         4: "own_memory",
         5: "n_allocations",
@@ -199,80 +220,103 @@
 
     # Start with a non-empty list of threads so that we always have something
     # to display. This avoids "Thread 1 of 0" and fixes a DivideByZeroError
     # when switching threads before the first allocation is seen.
     _DUMMY_THREAD_LIST = [0]
 
     def __init__(self, pid: Optional[int], cmd_line: Optional[str], native: bool):
-        self.pid = pid or "???"
-        if not cmd_line:
-            cmd_line = "???"
-        if len(cmd_line) > 50:
-            cmd_line = cmd_line[:50] + "..."
-        self.command_line = escape(cmd_line)
-        self._native = native
+        self.live_data = TUIData(pid, cmd_line, native)
+        self.paused_data: Optional[TUIData] = None
+        self.display_data = self.live_data
+
+        self.is_paused = False
+        self.active = True
         self._thread_idx = 0
         self._seen_threads: Set[int] = set()
-        self._threads: List[int] = self._DUMMY_THREAD_LIST
-        self.n_samples = 0
-        self.start = datetime.now()
-        self._last_update = datetime.now()
-        self._snapshot: Tuple[AllocationRecord, ...] = tuple()
-        self._current_memory_size = 0
-        self._max_memory_seen = 0
-        self._message = ""
-        self.active = True
         self._sort_field_name = "total_memory"
         self._sort_column_id = 1
         self._terminal_size = _get_terminal_lines()
-        self.stream = MemoryGraph(50, 4, 0.0, 1024.0)
+        self._threads: List[int] = self._DUMMY_THREAD_LIST
 
         layout = Layout(name="root")
         layout.split(
             Layout(name="header", size=7),
             Layout(name="heap_size", size=2),
             Layout(name="table", ratio=1),
             Layout(name="message", size=1),
             Layout(name="footer", size=1),
         )
-        layout["footer"].update(
-            "[bold grey93 on dodger_blue1] Q [/] Quit "
-            "[bold grey93 on dodger_blue1] ←  [/] Previous Thread "
-            "[bold grey93 on dodger_blue1] →  [/] Next Thread "
-            "[bold grey93 on dodger_blue1] T [/] Sort By Total "
-            "[bold grey93 on dodger_blue1] O [/] Sort By Own "
-            "[bold grey93 on dodger_blue1] A [/] Sort By Allocations "
-        )
         self.layout = layout
 
+        self.footer_paused_str = (
+            "[bold grey93 on dodger_blue1] SPACEBAR [/] Unpause View "
+        )
+        self.footer_running_str = (
+            "[bold grey93 on dodger_blue1] SPACEBAR [/] Pause View "
+        )
+
+        self.footer_dict = {
+            "quit": "[bold grey93 on dodger_blue1] Q [/] Quit ",
+            "prev_thread": "[bold grey93 on dodger_blue1] ←  [/] Previous Thread ",
+            "next_thread": "[bold grey93 on dodger_blue1] →  [/] Next Thread ",
+            "sort_tot": "[bold grey93 on dodger_blue1] T [/] Sort By Total ",
+            "sort_own": "[bold grey93 on dodger_blue1] O [/] Sort By Own ",
+            "sort_alloc": "[bold grey93 on dodger_blue1] A [/] Sort By Allocations ",
+            "pause": self.footer_running_str,
+        }
+
+    def footer(self) -> str:
+        return "".join(self.footer_dict.values())
+
+    def pause(self) -> None:
+        if not self.is_paused:
+            self.paused_data = deepcopy(self.live_data)
+            self.display_data = self.paused_data
+            self.footer_dict["pause"] = self.footer_paused_str
+            self.is_paused = True
+
+    def unpause(self) -> None:
+        if self.is_paused:
+            self.display_data = self.live_data
+            self.footer_dict["pause"] = self.footer_running_str
+            self.is_paused = False
+
+    def toggle_pause_state(self) -> None:
+        self.unpause() if self.is_paused else self.pause()
+
     def get_header(self) -> Table:
         header = Table.grid(expand=True)
         head = Table.grid(expand=True)
         head.add_column(justify="left", ratio=3)
         head.add_column(justify="right", ratio=7)
         head.add_row(
             "[b]Memray[/b] live tracking",
             datetime.now().ctime().replace(":", "[blink]:[/]"),
         )
 
         metadata = Table.grid(expand=False, padding=(0, 0, 0, 4))
         metadata.add_column(justify="left", ratio=5)
         metadata.add_column(justify="left", ratio=5)
         metadata.add_row("")
-        metadata.add_row(f"[b]PID[/]: {self.pid}", f"[b]CMD[/]: {self.command_line}")
+        metadata.add_row(
+            f"[b]PID[/]: {self.display_data.pid}",
+            f"[b]CMD[/]: {self.display_data.command_line}",
+        )
         metadata.add_row(
             f"[b]TID[/]: {hex(self.current_thread)}",
             f"[b]Thread[/] {self._thread_idx + 1} of {len(self._threads)}",
         )
         metadata.add_row(
-            f"[b]Samples[/]: {self.n_samples}",
-            f"[b]Duration[/]: {(self._last_update - self.start).total_seconds()} seconds",
+            f"[b]Samples[/]: {self.display_data.n_samples}",
+            f"[b]Duration[/]: "
+            f"{(self.display_data.last_update - self.display_data.start).total_seconds()}"
+            f" seconds",
         )
 
-        graph = "\n".join(self.stream.graph)
+        graph = "\n".join(self.display_data.stream.graph)
         plot = Panel(
             f"[color({2})]{graph}[/]",
             title="Memory",
             title_align="left",
             border_style="green",
             expand=False,
         )
@@ -289,21 +333,21 @@
 
     def get_heap_size(self) -> Table:
         heap_grid = Table.grid(expand=True)
         metadata = Table.grid(expand=True)
         metadata.add_column(justify="left", ratio=5)
         metadata.add_column(justify="right", ratio=5)
         metadata.add_row(
-            f"[bold]Current heap size[/]: {size_fmt(self._current_memory_size)}",
-            f"[bold]Max heap size seen[/]: {size_fmt(self._max_memory_seen)}",
+            f"[bold]Current heap size[/]: {size_fmt(self.display_data.current_memory_size)}",
+            f"[bold]Max heap size seen[/]: {size_fmt(self.display_data.max_memory_seen)}",
         )
         heap_grid.add_row(metadata)
         bar = ProgressBar(
-            completed=self._current_memory_size,
-            total=self._max_memory_seen + 1,
+            completed=self.display_data.current_memory_size,
+            total=self.display_data.max_memory_seen + 1,
             complete_style="blue",
         )
         heap_grid.add_row(bar)
         return heap_grid
 
     def get_body(self, *, max_rows: Optional[int] = None) -> Table:
         max_rows = max_rows or self._terminal_size
@@ -315,57 +359,58 @@
             Column("Own Memory % ", ratio=1, justify="right"),
             Column("Allocation Count", ratio=1, justify="right"),
             expand=True,
         )
         sort_column = table.columns[self._sort_column_id]
         sort_column.header = f"<{sort_column.header}>"
 
-        total_allocations = sum(record.n_allocations for record in self._snapshot)
-        allocation_entries = aggregate_allocations(
-            self._snapshot, MAX_MEMORY_RATIO * self._current_memory_size, self._native
-        )
-
         sorted_allocations = sorted(
-            allocation_entries.items(),
-            key=lambda item: getattr(  # type: ignore[no-any-return]
-                item[1], self._sort_field_name
-            ),
+            self.display_data.snapshot_data.items(),
+            key=lambda item: getattr(item[1], self._sort_field_name),
             reverse=True,
         )[:max_rows]
         for location, result in sorted_allocations:
             if self.current_thread not in result.thread_ids:
                 continue
             color_location = (
                 f"[bold magenta]{escape(location.function)}[/] at "
                 f"[cyan]{escape(location.file)}[/]"
             )
             total_color = _size_to_color(
-                result.total_memory / self._current_memory_size
+                result.total_memory / self.display_data.current_memory_size
+            )
+            own_color = _size_to_color(
+                result.own_memory / self.display_data.current_memory_size
+            )
+            allocation_colors = _size_to_color(
+                result.n_allocations / self.display_data.total_allocations
+            )
+            percent_total = (
+                result.total_memory / self.display_data.current_memory_size * 100
+            )
+            percent_own = (
+                result.own_memory / self.display_data.current_memory_size * 100
             )
-            own_color = _size_to_color(result.own_memory / self._current_memory_size)
-            allocation_colors = _size_to_color(result.n_allocations / total_allocations)
-            percent_total = result.total_memory / self._current_memory_size * 100
-            percent_own = result.own_memory / self._current_memory_size * 100
             table.add_row(
                 color_location,
                 f"[{total_color}]{size_fmt(result.total_memory)}[/{total_color}]",
                 f"[{total_color}]{percent_total:.2f}%[/{total_color}]",
                 f"[{own_color}]{size_fmt(result.own_memory)}[/{own_color}]",
                 f"[{own_color}]{percent_own:.2f}%[/{own_color}]",
                 f"[{allocation_colors}]{result.n_allocations}[/{allocation_colors}]",
             )
         return table
 
     @property
     def message(self) -> str:
-        return self._message
+        return self.display_data.message
 
     @message.setter
     def message(self, message: str) -> None:
-        self._message = message
+        self.display_data.message = message
 
     @property
     def current_thread(self) -> int:
         return self._threads[self._thread_idx]
 
     def next_thread(self) -> None:
         self._thread_idx = (self._thread_idx + 1) % len(self._threads)
@@ -374,29 +419,41 @@
         self._thread_idx = (self._thread_idx - 1) % len(self._threads)
 
     def generate_layout(self) -> Layout:
         self.layout["header"].update(self.get_header())
         self.layout["heap_size"].update(self.get_heap_size())
         self.layout["table"].update(self.get_body())
         self.layout["message"].update(self.message)
+        self.layout["footer"].update(self.footer())
         return self.layout
 
     def update_snapshot(self, snapshot: Iterable[AllocationRecord]) -> None:
-        self._snapshot = tuple(snapshot)
-        for record in self._snapshot:
+        for record in snapshot:
             if record.tid in self._seen_threads:
                 continue
             if self._threads is self._DUMMY_THREAD_LIST:
                 self._threads = []
             self._threads.append(record.tid)
             self._seen_threads.add(record.tid)
-        self.n_samples += 1
-        self._last_update = datetime.now()
-        self._current_memory_size = sum(record.size for record in self._snapshot)
-        if self._current_memory_size > self._max_memory_seen:
-            self._max_memory_seen = self._current_memory_size
-            self.stream.reset_max(self._max_memory_seen)
-        self.stream.add_value(self._current_memory_size)
+
+        self.live_data.n_samples += 1
+        self.live_data.last_update = datetime.now()
+        self.live_data.current_memory_size = sum(record.size for record in snapshot)
+
+        if self.live_data.current_memory_size > self.live_data.max_memory_seen:
+            self.live_data.max_memory_seen = self.live_data.current_memory_size
+            self.live_data.stream.reset_max(self.live_data.max_memory_seen)
+        self.live_data.stream.add_value(self.live_data.current_memory_size)
+
+        self.live_data.total_allocations = sum(
+            record.n_allocations for record in snapshot
+        )
+        allocation_entries = aggregate_allocations(
+            snapshot,
+            MAX_MEMORY_RATIO * self.live_data.current_memory_size,
+            self.live_data.native,
+        )
+        self.live_data.snapshot_data = allocation_entries
 
     def update_sort_key(self, col_number: int) -> None:
         self._sort_column_id = col_number
         self._sort_field_name = self.KEY_TO_COLUMN_NAME[col_number]
```

### Comparing `memray-1.8.1/src/memray.egg-info/PKG-INFO` & `memray-1.9.0/src/memray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memray
-Version: 1.8.1
+Version: 1.9.0
 Summary: A memory profiler for Python applications
 Home-page: https://github.com/bloomberg/memray
 Author: Pablo Galindo Salgado
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -174,14 +174,15 @@
     parse               Debug a results file by parsing and printing each record in it
     summary             Generate a terminal-based summary report of the functions that allocate most memory
     stats               Generate high level stats of the memory usage in the terminal
 
 optional arguments:
   -h, --help            Show this help message and exit
   -v, --verbose         Increase verbosity. Option is additive and can be specified up to 3 times
+  -V, --version         Displays the current version of Memray
 
 Please submit feedback, ideas, and bug reports by filing a new issue at https://github.com/bloomberg/memray/issues
 ```
 
 To use Memray over a script or a single python file you can use
 
 ```shell
```

### Comparing `memray-1.8.1/src/memray.egg-info/SOURCES.txt` & `memray-1.9.0/src/memray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt` & `memray-1.9.0/src/vendor/libbacktrace/Isaac.Newton-Opticks.txt`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/LICENSE` & `memray-1.9.0/src/vendor/libbacktrace/LICENSE`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/Makefile.am` & `memray-1.9.0/src/vendor/libbacktrace/Makefile.am`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/Makefile.in` & `memray-1.9.0/src/vendor/libbacktrace/Makefile.in`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/README.md` & `memray-1.9.0/src/vendor/libbacktrace/README.md`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/aclocal.m4` & `memray-1.9.0/src/vendor/libbacktrace/aclocal.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/alloc.c` & `memray-1.9.0/src/vendor/libbacktrace/alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/allocfail.c` & `memray-1.9.0/src/vendor/libbacktrace/allocfail.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/allocfail.sh` & `memray-1.9.0/src/vendor/libbacktrace/allocfail.sh`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/atomic.c` & `memray-1.9.0/src/vendor/libbacktrace/atomic.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/backtrace-supported.h.in` & `memray-1.9.0/src/vendor/libbacktrace/backtrace-supported.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/backtrace.c` & `memray-1.9.0/src/vendor/libbacktrace/backtrace.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/backtrace.h` & `memray-1.9.0/src/vendor/libbacktrace/backtrace.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/btest.c` & `memray-1.9.0/src/vendor/libbacktrace/btest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/compile` & `memray-1.9.0/src/vendor/libbacktrace/compile`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/enable.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/enable.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/lead-dot.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/lead-dot.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/libtool.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/ltoptions.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/ltsugar.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/ltversion.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/lt~obsolete.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/multi.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/multi.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/override.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/override.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/unwind_ipinfo.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/unwind_ipinfo.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config/warnings.m4` & `memray-1.9.0/src/vendor/libbacktrace/config/warnings.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config.guess` & `memray-1.9.0/src/vendor/libbacktrace/config.guess`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config.h.in` & `memray-1.9.0/src/vendor/libbacktrace/config.h.in`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/config.sub` & `memray-1.9.0/src/vendor/libbacktrace/config.sub`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/configure` & `memray-1.9.0/src/vendor/libbacktrace/configure`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/configure.ac` & `memray-1.9.0/src/vendor/libbacktrace/configure.ac`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/debuginfod_support.h` & `memray-1.9.0/src/vendor/libbacktrace/debuginfod_support.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/dwarf.c` & `memray-1.9.0/src/vendor/libbacktrace/dwarf.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/edtest.c` & `memray-1.9.0/src/vendor/libbacktrace/edtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/edtest2.c` & `memray-1.9.0/src/vendor/libbacktrace/edtest2.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/elf.c` & `memray-1.9.0/src/vendor/libbacktrace/elf.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/fileline.c` & `memray-1.9.0/src/vendor/libbacktrace/fileline.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/filenames.h` & `memray-1.9.0/src/vendor/libbacktrace/filenames.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/filetype.awk` & `memray-1.9.0/src/vendor/libbacktrace/filetype.awk`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in` & `memray-1.9.0/src/vendor/libbacktrace/install-debuginfo-for-buildid.sh.in`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/install-sh` & `memray-1.9.0/src/vendor/libbacktrace/install-sh`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/instrumented_alloc.c` & `memray-1.9.0/src/vendor/libbacktrace/instrumented_alloc.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/internal.h` & `memray-1.9.0/src/vendor/libbacktrace/internal.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/libtool.m4` & `memray-1.9.0/src/vendor/libbacktrace/libtool.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ltmain.sh` & `memray-1.9.0/src/vendor/libbacktrace/ltmain.sh`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ltoptions.m4` & `memray-1.9.0/src/vendor/libbacktrace/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ltsugar.m4` & `memray-1.9.0/src/vendor/libbacktrace/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ltversion.m4` & `memray-1.9.0/src/vendor/libbacktrace/ltversion.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/lt~obsolete.m4` & `memray-1.9.0/src/vendor/libbacktrace/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/macho.c` & `memray-1.9.0/src/vendor/libbacktrace/macho.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/missing` & `memray-1.9.0/src/vendor/libbacktrace/missing`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/mmap.c` & `memray-1.9.0/src/vendor/libbacktrace/mmap.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/mmapio.c` & `memray-1.9.0/src/vendor/libbacktrace/mmapio.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/move-if-change` & `memray-1.9.0/src/vendor/libbacktrace/move-if-change`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/mtest.c` & `memray-1.9.0/src/vendor/libbacktrace/mtest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/nounwind.c` & `memray-1.9.0/src/vendor/libbacktrace/nounwind.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/pecoff.c` & `memray-1.9.0/src/vendor/libbacktrace/pecoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/posix.c` & `memray-1.9.0/src/vendor/libbacktrace/posix.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/print.c` & `memray-1.9.0/src/vendor/libbacktrace/print.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/read.c` & `memray-1.9.0/src/vendor/libbacktrace/read.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/simple.c` & `memray-1.9.0/src/vendor/libbacktrace/simple.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/sort.c` & `memray-1.9.0/src/vendor/libbacktrace/sort.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/state.c` & `memray-1.9.0/src/vendor/libbacktrace/state.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/stest.c` & `memray-1.9.0/src/vendor/libbacktrace/stest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/test-driver` & `memray-1.9.0/src/vendor/libbacktrace/test-driver`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/test_format.c` & `memray-1.9.0/src/vendor/libbacktrace/test_format.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/testlib.c` & `memray-1.9.0/src/vendor/libbacktrace/testlib.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/testlib.h` & `memray-1.9.0/src/vendor/libbacktrace/testlib.h`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ttest.c` & `memray-1.9.0/src/vendor/libbacktrace/ttest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/unittest.c` & `memray-1.9.0/src/vendor/libbacktrace/unittest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/unknown.c` & `memray-1.9.0/src/vendor/libbacktrace/unknown.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/xcoff.c` & `memray-1.9.0/src/vendor/libbacktrace/xcoff.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/xztest.c` & `memray-1.9.0/src/vendor/libbacktrace/xztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace/ztest.c` & `memray-1.9.0/src/vendor/libbacktrace/ztest.c`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff` & `memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_debuginfod_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff` & `memray-1.9.0/src/vendor/libbacktrace_2446c66076480ce07a6bd868badcbceb3eeecc2e_patch.diff`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/src/vendor/regenerate_libbacktrace.sh` & `memray-1.9.0/src/vendor/regenerate_libbacktrace.sh`

 * *Files identical despite different names*

### Comparing `memray-1.8.1/webpack.config.js` & `memray-1.9.0/webpack.config.js`

 * *Files identical despite different names*

