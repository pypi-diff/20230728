# Comparing `tmp/pylink-square-1.1.0.tar.gz` & `tmp/pylink-square-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylink-square-1.1.0.tar", last modified: Tue May  9 16:00:42 2023, max compression
+gzip compressed data, was "pylink-square-1.2.0.tar", last modified: Fri Jul 28 16:05:24 2023, max compression
```

## Comparing `pylink-square-1.1.0.tar` & `pylink-square-1.2.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-09 16:00:12.000000 pylink-square-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-09 16:00:12.000000 pylink-square-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 16:00:12.000000 pylink-square-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-09 16:00:42.781110 pylink-square-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-09 16:00:12.000000 pylink-square-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.769110 pylink-square-1.1.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5563 2023-05-09 16:00:12.000000 pylink-square-1.1.0/examples/pylink-rtt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3202 2023-05-09 16:00:12.000000 pylink-square-1.1.0/examples/pylink-swv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/binpacker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   168513 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/jlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/protocols/swd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38009 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/unlockers/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/unlockers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/unlockers/unlock_kinetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink_square.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-09 16:00:42.781110 pylink-square-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-09 16:00:12.000000 pylink-square-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/features/jlink/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/canary.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/debugger.feature
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/emulator.feature
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/flash.feature
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/license.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/memory.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/register.feature
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/rtt.feature
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/swd.feature
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/swo.feature
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/unlock.feature
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/update.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/features/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/rtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/swd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/swo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.769110 pylink-square-1.1.0/tests/functional/firmware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.c
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.c
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h
--rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swd/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/gcc.ld
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/main.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.c
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/protocols/test_swd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_binpacker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   197978 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_jlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    41451 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/unlockers/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/test_unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/test_unlock_kinetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.351856 pylink-square-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-07-28 16:04:56.000000 pylink-square-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-28 16:04:56.000000 pylink-square-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 16:04:56.000000 pylink-square-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-28 16:05:24.351856 pylink-square-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-28 16:04:56.000000 pylink-square-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.339856 pylink-square-1.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5563 2023-07-28 16:04:56.000000 pylink-square-1.2.0/examples/pylink-rtt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3202 2023-07-28 16:04:56.000000 pylink-square-1.2.0/examples/pylink-swv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/pylink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/binpacker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168437 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/jlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/pylink/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/protocols/swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38009 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/pylink/unlockers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/unlockers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/unlockers/unlock_kinetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-28 16:04:56.000000 pylink-square-1.2.0/pylink/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/pylink_square.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 16:05:24.000000 pylink-square-1.2.0/pylink_square.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-28 16:05:24.351856 pylink-square-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-07-28 16:04:56.000000 pylink-square-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/features/jlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/canary.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/debugger.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/emulator.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/flash.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/license.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/memory.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/register.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/rtt.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/swd.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/swo.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/unlock.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/jlink/update.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/rtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/swo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/steps/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/features/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.339856 pylink-square-1.2.0/tests/functional/firmware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/firmware/k21-canary/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/firmware/k21-canary/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.343856 pylink-square-1.2.0/tests/functional/firmware/k21-canary/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-canary/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-etm/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-etm/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/etm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/etm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/swo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/swo.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-loop/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-loop/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-loop/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-loop/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-swd/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/gcc.ld
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/main.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-swo/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-swo/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.347856 pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/swo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/swo.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.351856 pylink-square-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.351856 pylink-square-1.2.0/tests/unit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/protocols/test_swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_binpacker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197633 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_jlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41451 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:05:24.351856 pylink-square-1.2.0/tests/unit/unlockers/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/unlockers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/unlockers/test_unlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-07-28 16:04:56.000000 pylink-square-1.2.0/tests/unit/unlockers/test_unlock_kinetis.py
```

### Comparing `pylink-square-1.1.0/CHANGELOG.md` & `pylink-square-1.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [1.2.0]
+### Changed
+- @cpattenden-sq: Fixed bug in `flash()` where return value was being checked
+  against a `void` function; would lead to exceptions being raised
+  unexpectedly.
+
 ## [1.1.0]
 ### Added
 - @chanqueo: Added `use_tmpcpy` field to constructor for `JLink` and `Library`
   instances to workaround temporary files not been cleaned up; a future patch
   will change the default behaviour based on the version of the SDK. By
   default, temporary files are used for the SDK binary.
```

### Comparing `pylink-square-1.1.0/LICENSE.md` & `pylink-square-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/PKG-INFO` & `pylink-square-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylink-square
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python interface for SEGGER J-Link.
 Home-page: http://www.github.com/Square/pylink
 Author: Square Embedded Software Team
 Author-email: esw-team@squareup.com
 License: Apache 2.0
 Keywords: SEGGER J-Link
 License-File: LICENSE.md
```

### Comparing `pylink-square-1.1.0/README.md` & `pylink-square-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/examples/pylink-rtt` & `pylink-square-1.2.0/examples/pylink-rtt`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/examples/pylink-swv` & `pylink-square-1.2.0/examples/pylink-swv`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/__init__.py` & `pylink-square-1.2.0/pylink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 __title__ = 'pylink'
 __author__ = 'Square Embedded Software Team'
 __author_email__ = 'esw-team@squareup.com'
 __copyright__ = 'Copyright 2017 Square, Inc.'
 __license__ = 'Apache 2.0'
 __url__ = 'http://www.github.com/Square/pylink'
 __description__ = 'Python interface for SEGGER J-Link.'
```

### Comparing `pylink-square-1.1.0/pylink/__main__.py` & `pylink-square-1.2.0/pylink/__main__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/binpacker.py` & `pylink-square-1.2.0/pylink/binpacker.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/decorators.py` & `pylink-square-1.2.0/pylink/decorators.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/enums.py` & `pylink-square-1.2.0/pylink/enums.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/errors.py` & `pylink-square-1.2.0/pylink/errors.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/jlink.py` & `pylink-square-1.2.0/pylink/jlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -2190,17 +2190,15 @@
             # try-catch as the 'halted()' check may fail with an exception.
             if not self.halted():
                 self.halt()
         except errors.JLinkException:
             pass
 
         # Perform read-modify-write operation.
-        res = self._dll.JLINKARM_BeginDownload(flags=flags)
-        if res < 0:
-            raise errors.JLinkEraseException(res)
+        self._dll.JLINKARM_BeginDownload(flags=flags)
 
         if isinstance(data, list):
             data = bytes(data)
 
         bytes_flashed = self._dll.JLINKARM_WriteMem(addr, len(data), data)
 
         res = self._dll.JLINKARM_EndDownload()
```

### Comparing `pylink-square-1.1.0/pylink/jlock.py` & `pylink-square-1.2.0/pylink/jlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/library.py` & `pylink-square-1.2.0/pylink/library.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/protocols/__init__.py` & `pylink-square-1.2.0/pylink/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/protocols/swd.py` & `pylink-square-1.2.0/pylink/protocols/swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/registers.py` & `pylink-square-1.2.0/pylink/registers.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/structs.py` & `pylink-square-1.2.0/pylink/structs.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/threads.py` & `pylink-square-1.2.0/pylink/threads.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/unlockers/__init__.py` & `pylink-square-1.2.0/pylink/unlockers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/unlockers/unlock_kinetis.py` & `pylink-square-1.2.0/pylink/unlockers/unlock_kinetis.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink/util.py` & `pylink-square-1.2.0/pylink/util.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/pylink_square.egg-info/PKG-INFO` & `pylink-square-1.2.0/pylink_square.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylink-square
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python interface for SEGGER J-Link.
 Home-page: http://www.github.com/Square/pylink
 Author: Square Embedded Software Team
 Author-email: esw-team@squareup.com
 License: Apache 2.0
 Keywords: SEGGER J-Link
 License-File: LICENSE.md
```

### Comparing `pylink-square-1.1.0/pylink_square.egg-info/SOURCES.txt` & `pylink-square-1.2.0/pylink_square.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/setup.py` & `pylink-square-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/README.md` & `pylink-square-1.2.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/__init__.py` & `pylink-square-1.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/__init__.py` & `pylink-square-1.2.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/environment.py` & `pylink-square-1.2.0/tests/functional/features/environment.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/debugger.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/debugger.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/emulator.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/emulator.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/flash.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/flash.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/license.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/license.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/memory.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/memory.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/register.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/register.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/rtt.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/rtt.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/jlink/swd.feature` & `pylink-square-1.2.0/tests/functional/features/jlink/swd.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/__init__.py` & `pylink-square-1.2.0/tests/functional/features/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/common.py` & `pylink-square-1.2.0/tests/functional/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/debug.py` & `pylink-square-1.2.0/tests/functional/features/steps/debug.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/licenses.py` & `pylink-square-1.2.0/tests/functional/features/steps/licenses.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/memory.py` & `pylink-square-1.2.0/tests/functional/features/steps/memory.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/registers.py` & `pylink-square-1.2.0/tests/functional/features/steps/registers.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/rtt.py` & `pylink-square-1.2.0/tests/functional/features/steps/rtt.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/swd.py` & `pylink-square-1.2.0/tests/functional/features/steps/swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/swo.py` & `pylink-square-1.2.0/tests/functional/features/steps/swo.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/unlock.py` & `pylink-square-1.2.0/tests/functional/features/steps/unlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/steps/update.py` & `pylink-square-1.2.0/tests/functional/features/steps/update.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/features/utility.py` & `pylink-square-1.2.0/tests/functional/features/utility.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-canary/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-canary/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-canary/README.md` & `pylink-square-1.2.0/tests/functional/firmware/k21-canary/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-canary/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-canary/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/main.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-canary/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/README.md` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/etm.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.h` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/etm.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/main.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/swo.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.h` & `pylink-square-1.2.0/tests/functional/firmware/k21-etm/src/swo.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-loop/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-loop/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-loop/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-loop/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/main.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-loop/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/README.md` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/main.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swd/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-swd/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swd/README.md` & `pylink-square-1.2.0/tests/functional/firmware/k21-swd/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/main.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-swd/asm/main.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/Makefile` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/README.md` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/bootloader.s` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/gcc.ld` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/main.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.c` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/swo.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.h` & `pylink-square-1.2.0/tests/functional/firmware/k21-swo/src/swo.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/__init__.py` & `pylink-square-1.2.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/protocols/__init__.py` & `pylink-square-1.2.0/tests/unit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/protocols/test_swd.py` & `pylink-square-1.2.0/tests/unit/protocols/test_swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_binpacker.py` & `pylink-square-1.2.0/tests/unit/test_binpacker.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_decorators.py` & `pylink-square-1.2.0/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_enums.py` & `pylink-square-1.2.0/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_errors.py` & `pylink-square-1.2.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_jlink.py` & `pylink-square-1.2.0/tests/unit/test_jlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -2720,36 +2720,28 @@
         self.jlink.power_on = mock.Mock()
         self.jlink.erase = mock.Mock()
         self.jlink.memory_write = mock.Mock()
 
         self.jlink.halted = mock.Mock()
         self.jlink.halted.return_value = True
 
-        # BeginDownload failing
-        self.dll.JLINKARM_BeginDownload.return_value = -1
-        self.dll.JLINKARM_EndDownload.return_value = 0
-        with self.assertRaises(JLinkException):
-            self.jlink.flash([0], 0)
-
         # EndDownload failing
-        self.dll.JLINKARM_BeginDownload.return_value = 0
         self.dll.JLINKARM_EndDownload.return_value = -1
         with self.assertRaises(JLinkException):
             self.jlink.flash([0], 0)
 
     def test_jlink_flash_success(self):
         """Tests a successful flash.
 
         Args:
           self (TestJLink): the ``TestJLink`` instance
 
         Returns:
           ``None``
         """
-        self.dll.JLINKARM_BeginDownload.return_value = 0
         self.dll.JLINKARM_WriteMem.return_value = 0
         self.dll.JLINKARM_EndDownload.return_value = 0
 
         self.jlink.power_on = mock.Mock()
         self.jlink.erase = mock.Mock()
         self.jlink.memory_write = mock.Mock()
```

### Comparing `pylink-square-1.1.0/tests/unit/test_jlock.py` & `pylink-square-1.2.0/tests/unit/test_jlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_library.py` & `pylink-square-1.2.0/tests/unit/test_library.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_main.py` & `pylink-square-1.2.0/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_structs.py` & `pylink-square-1.2.0/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_threads.py` & `pylink-square-1.2.0/tests/unit/test_threads.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/test_util.py` & `pylink-square-1.2.0/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/unlockers/__init__.py` & `pylink-square-1.2.0/tests/unit/unlockers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/unlockers/test_unlock.py` & `pylink-square-1.2.0/tests/unit/unlockers/test_unlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.1.0/tests/unit/unlockers/test_unlock_kinetis.py` & `pylink-square-1.2.0/tests/unit/unlockers/test_unlock_kinetis.py`

 * *Files identical despite different names*

