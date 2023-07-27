# Comparing `tmp/datatransport-3.0.6.tar.gz` & `tmp/datatransport-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransport-3.0.6.tar", last modified: Thu Jul 13 20:00:21 2023, max compression
+gzip compressed data, was "datatransport-3.0.7.tar", last modified: Thu Jul 27 22:31:25 2023, max compression
```

## Comparing `datatransport-3.0.6.tar` & `datatransport-3.0.7.tar`

### file list

```diff
@@ -1,212 +1,215 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/
--rw-rw-r--   0 valentic   (500) valentic   (500)    49678 2023-07-12 23:31:21.000000 datatransport-3.0.6/CHANGES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.6/INSTALL
--rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.6/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.6/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.6/MIGRATION
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-13 20:00:21.000000 datatransport-3.0.6/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.6/README.rst
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/
--rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/.coverage
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2351 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/archivegroups/archivegroups.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2340 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/component/component.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1759 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/environ/environ.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1098 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/environ/environ.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.6/contrib/examples/examples.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/filewatch/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1654 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/getbytes/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      896 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/hello/
--rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.6/contrib/examples/hello/hello.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      799 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/hello/helloworld.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/init/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      973 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/init/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/init/init.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/messagebox/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/messagebox.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/poll_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/poll_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/post_file.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/messagebox/post_text.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/postpoll/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1009 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/poll_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      836 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/poll_text.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1125 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/post_file.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      957 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/post_text.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/postpoll/postpoll.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/rotatelogs/
--rwxrwxr-x   0 valentic   (500) valentic   (500)      861 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/service/
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1175 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/client.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/directory.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/echo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/service/service.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/spawn/spawn.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     1284 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples/watchdog/
--rwxr-xr-x   0 valentic   (500) valentic   (500)     1054 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/crasher.py
--rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/init_crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/README
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/archivegroups.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/archivegroups/postdata.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/component/
--rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/component/component.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/component/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/config/config.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/config/config.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/diskmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/diskmonitor/diskmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/environ/
--rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/environ/environ.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/environ/environ.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/eventmonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/eventmonitor/serverstate.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/createdata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/filewatch/filewatch.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/getbytes/getbytes.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/plugin.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/instrumentstatus/postdata
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/
--rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/README
--rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/multipoll.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/reader.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/multipoll/writer.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/plottool/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/plottool/datasource.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/plottool/plottool.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/checkdate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/postdatafiles/postdatafiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/resourcemonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/
--rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/counter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/rotatelogs/rotatelogs.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/spawn/
--rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/spawn/spawn.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/spawn/spawner.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/createfiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/splitfiles/splitfiles.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/
--rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/poller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/source.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/syncpoller/syncpoller.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/test.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/wait/
--rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/wait/timer.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/wait/wait.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/
--rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/crasher.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/examples.v2/watchdog/watchdog.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/contrib/utils/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/createnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/getarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/postarticle
--rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/rebuilddatabase
--rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/relaynewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/rmnewsgroup
--rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.6/contrib/utils/watchtransport
--rw-rw-r--   0 valentic   (500) valentic   (500)     2611 2023-07-10 06:31:17.000000 datatransport-3.0.6/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-13 20:00:21.000000 datatransport-3.0.6/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/
--rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1584 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/accessmixin.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/commands/
--rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/cancelnewsgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/console.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/listnewsgroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transport_create_app.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportctl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportd.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/commands/transportps.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.6/src/datatransport/commands/viewlog.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)    50983 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/ArchiveGroups.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2405 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/DirectoryService.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5325 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/DiskMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6212 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/EventMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4130 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FilePost.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     9573 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FileStore.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5460 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/FileWatch.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5213 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/GroupControl.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/InstrumentStatus.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4364 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/NewsGateway.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7859 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/NewsgroupMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PageKit.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PlotTool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    12588 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/PostDataFiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/RealTimeFeed.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/ResourceMonitor.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     6851 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/Scheduler.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/SyncPoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11920 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/WatchURL.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      645 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/components/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1335 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/configcomponent.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     3058 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/directory.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-12 23:30:41.000000 datatransport-3.0.6/src/datatransport/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    10437 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newspoller.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     7928 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newsposter.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    33842 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/newstool.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    15514 2023-07-09 19:28:31.000000 datatransport-3.0.6/src/datatransport/processclient.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    13288 2023-07-09 19:27:51.000000 datatransport-3.0.6/src/datatransport/processgroup.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/root.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/etc/
--rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/etc/transportd.conf
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/groups/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/
--rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
--rw-rw-r--   0 valentic   (500) valentic   (500)     4679 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/watchdog.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.6/src/datatransport/transportconfig.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportlogger.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportmanager.py
--rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/transportserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport/utilities/
--rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4012 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/patterntemplate.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/removefile.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/sizedesc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/utilities/xmlrpcdeferred.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     4498 2023-07-07 20:20:45.000000 datatransport-3.0.6/src/datatransport/xmlrpcserver.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)     6282 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)     1330 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/entry_points.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-13 20:00:21.000000 datatransport-3.0.6/src/datatransport.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-13 20:00:21.000000 datatransport-3.0.6/tests/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_datefunc.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_makepath.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1443 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_pattern.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_removefiles.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.6/tests/test_utilities_sizedesc.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    50206 2023-07-27 21:23:37.000000 datatransport-3.0.7/CHANGES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)    32333 2023-07-07 20:20:45.000000 datatransport-3.0.7/INSTALL
+-rw-rw-r--   0 valentic   (500) valentic   (500)    35149 2023-07-07 20:20:45.000000 datatransport-3.0.7/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)      231 2023-07-07 20:20:45.000000 datatransport-3.0.7/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3721 2023-07-07 20:20:45.000000 datatransport-3.0.7/MIGRATION
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-27 22:31:25.000000 datatransport-3.0.7/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      155 2023-07-07 20:20:45.000000 datatransport-3.0.7/README.rst
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    53248 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/.coverage
+-rw-rw-r--   0 valentic   (500) valentic   (500)      121 2023-07-27 16:34:01.000000 datatransport-3.0.7/contrib/examples/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2333 2023-07-26 23:11:05.000000 datatransport-3.0.7/contrib/examples/archivegroups/archivegroups.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2345 2023-07-26 21:56:24.000000 datatransport-3.0.7/contrib/examples/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      753 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/component/component.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1854 2023-07-27 04:14:34.000000 datatransport-3.0.7/contrib/examples/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      418 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/environ/environ.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1097 2023-07-26 20:31:33.000000 datatransport-3.0.7/contrib/examples/environ/environ.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       28 2023-07-09 19:21:24.000000 datatransport-3.0.7/contrib/examples/examples.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/filewatch/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1682 2023-07-26 21:29:22.000000 datatransport-3.0.7/contrib/examples/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      459 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/getbytes/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      874 2023-07-26 21:19:37.000000 datatransport-3.0.7/contrib/examples/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      530 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/hello/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      268 2023-07-09 20:00:03.000000 datatransport-3.0.7/contrib/examples/hello/hello.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      876 2023-07-26 20:27:09.000000 datatransport-3.0.7/contrib/examples/hello/helloworld.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/init/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1020 2023-07-26 20:28:47.000000 datatransport-3.0.7/contrib/examples/init/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      108 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/init/init.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/messagebox/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1220 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/messagebox.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      970 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/poll_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      930 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/poll_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1108 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/post_file.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      989 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/messagebox/post_text.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/postpoll/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1090 2023-07-26 21:11:35.000000 datatransport-3.0.7/contrib/examples/postpoll/poll_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      918 2023-07-26 20:43:33.000000 datatransport-3.0.7/contrib/examples/postpoll/poll_text.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1162 2023-07-26 20:46:08.000000 datatransport-3.0.7/contrib/examples/postpoll/post_file.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1010 2023-07-26 20:34:43.000000 datatransport-3.0.7/contrib/examples/postpoll/post_text.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1111 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/postpoll/postpoll.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/rotatelogs/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      868 2023-07-26 21:20:22.000000 datatransport-3.0.7/contrib/examples/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/service/
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1194 2023-07-27 16:36:41.000000 datatransport-3.0.7/contrib/examples/service/client.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      447 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/directory.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      915 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/echo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      613 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/service/service.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      345 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/spawn/spawn.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     1304 2023-07-26 21:26:34.000000 datatransport-3.0.7/contrib/examples/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples/watchdog/
+-rwxr-xr-x   0 valentic   (500) valentic   (500)     1061 2023-07-26 21:27:53.000000 datatransport-3.0.7/contrib/examples/watchdog/crasher.py
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      754 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/watchdog/init_crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      246 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1031 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/README
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2367 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/archivegroups.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1348 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/archivegroups/postdata.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/component/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      752 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/component/component.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1447 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/component/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      301 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/config/config.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)      901 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/config/config.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/diskmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      460 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/diskmonitor/diskmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/environ/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      407 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/environ/environ.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      805 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/environ/environ.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/eventmonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4620 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/eventmonitor/serverstate.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1367 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/createdata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      458 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/filewatch/filewatch.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1228 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      410 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/getbytes/getbytes.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/instrumentstatus.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      235 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/plugin.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1320 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/instrumentstatus/postdata
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      197 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/README
+-rw-rw-r--   0 valentic   (500) valentic   (500)      629 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/multipoll.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      427 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/reader.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      534 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/multipoll/writer.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      839 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/plottool/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1726 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/plottool/datasource.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2269 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/plottool/plottool.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      339 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/checkdate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      913 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      562 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/postdatafiles/postdatafiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/resourcemonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      261 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/resourcemonitor/resourcemonitor.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      806 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/counter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      349 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/rotatelogs/rotatelogs.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/spawn/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      195 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/spawn/spawn.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)      962 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/spawn/spawner.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1128 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/createfiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      832 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/splitfiles/splitfiles.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      360 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/poller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      648 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/source.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      653 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/syncpoller/syncpoller.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)       70 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/test.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/wait/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      863 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/wait/timer.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      176 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/wait/wait.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      889 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/crasher.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      166 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/examples.v2/watchdog/watchdog.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/contrib/utils/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1476 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/createnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1741 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/getarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1432 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/postarticle
+-rw-rw-r--   0 valentic   (500) valentic   (500)      711 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/rebuilddatabase
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2789 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/relaynewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)      614 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/rmnewsgroup
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3753 2023-07-07 20:20:45.000000 datatransport-3.0.7/contrib/utils/watchtransport
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2611 2023-07-27 16:43:31.000000 datatransport-3.0.7/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-27 22:31:25.000000 datatransport-3.0.7/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      547 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1539 2023-07-27 20:11:25.000000 datatransport-3.0.7/src/datatransport/accessmixin.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/commands/
+-rw-rw-r--   0 valentic   (500) valentic   (500)        0 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1110 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/cancelnewsgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8443 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/console.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1656 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/listnewsgroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3307 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transport_create_app.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10912 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportctl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3584 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportd.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1356 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/commands/transportps.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7918 2023-07-12 23:39:58.000000 datatransport-3.0.7/src/datatransport/commands/viewlog.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5325 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/DiskMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6212 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/EventMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4130 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/FilePost.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     9573 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/FileStore.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5308 2023-07-27 07:14:43.000000 datatransport-3.0.7/src/datatransport/components/GroupControl.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    20030 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/InstrumentStatus.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4975 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/NewsGateway.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7859 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/NewsgroupMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5778 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/PageKit.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    30535 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/PlotTool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    12712 2023-07-27 07:14:43.000000 datatransport-3.0.7/src/datatransport/components/PostDataFiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3926 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/RealTimeFeed.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     7552 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/ResourceMonitor.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6942 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/Scheduler.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4420 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/components/SyncPoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11743 2023-07-27 07:14:44.000000 datatransport-3.0.7/src/datatransport/components/WatchURL.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      645 2023-07-27 16:42:50.000000 datatransport-3.0.7/src/datatransport/components/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    52705 2023-07-26 23:57:41.000000 datatransport-3.0.7/src/datatransport/components/archivegroups.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2736 2023-07-27 16:48:23.000000 datatransport-3.0.7/src/datatransport/components/directoryservice.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5651 2023-07-26 21:50:04.000000 datatransport-3.0.7/src/datatransport/components/filewatch.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1304 2023-07-27 18:05:17.000000 datatransport-3.0.7/src/datatransport/configcomponent.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     3065 2023-07-26 20:39:27.000000 datatransport-3.0.7/src/datatransport/directory.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-25 17:37:52.000000 datatransport-3.0.7/src/datatransport/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    10799 2023-07-27 21:09:07.000000 datatransport-3.0.7/src/datatransport/newspoller.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8209 2023-07-27 21:58:14.000000 datatransport-3.0.7/src/datatransport/newsposter.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    34275 2023-07-27 21:22:50.000000 datatransport-3.0.7/src/datatransport/newstool.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    15543 2023-07-27 22:31:13.000000 datatransport-3.0.7/src/datatransport/processclient.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    13509 2023-07-20 22:01:05.000000 datatransport-3.0.7/src/datatransport/processgroup.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      173 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/root.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/etc/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2057 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/templates/etc/transportd.conf
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/groups/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      508 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4747 2023-07-27 05:02:15.000000 datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/watchdog.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2949 2023-07-09 19:12:21.000000 datatransport-3.0.7/src/datatransport/transportconfig.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2197 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportlogger.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2542 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportmanager.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)    11136 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/transportserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport/utilities/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      170 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1420 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1000 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4170 2023-07-27 03:27:27.000000 datatransport-3.0.7/src/datatransport/utilities/patterntemplate.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1375 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/removefile.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2947 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/sizedesc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5357 2023-07-07 20:20:45.000000 datatransport-3.0.7/src/datatransport/utilities/xmlrpcdeferred.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     4505 2023-07-27 16:47:53.000000 datatransport-3.0.7/src/datatransport/xmlrpcserver.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    41258 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)     6376 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1330 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/entry_points.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)      151 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       14 2023-07-27 22:31:25.000000 datatransport-3.0.7/src/datatransport.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-27 22:31:25.000000 datatransport-3.0.7/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     8651 2023-07-27 01:45:55.000000 datatransport-3.0.7/tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1772 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_datefunc.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      813 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_makepath.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     2113 2023-07-27 01:45:50.000000 datatransport-3.0.7/tests/test_utilities_pattern.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1168 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_removefiles.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1667 2023-07-07 20:20:45.000000 datatransport-3.0.7/tests/test_utilities_sizedesc.py
```

### Comparing `datatransport-3.0.6/CHANGES.txt` & `datatransport-3.0.7/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+2023-07-20  Todd Valentic
+    - Process group. Do not log error if no clients listed
+    - Process group. Change default shutdown timeout to be 30s
+    - Process group. Change shutdown timeout to be a timedelta
+    - Process client. Add stop() to request process to stop.
+    - NewsTool. Ensure enable is boolean
+    - PatternTemplate. Missing pattern check. Update test.
+    - NewsPoller. Code cleanup. Use AccessMixin
+    - NewsPoster. Code cleanup. Use AccessMixin
+    - NewsTool. Fix host/port setting
+
+    - Release 3.0.7
+
 2023-07-12  Todd Valentic
     - Make sure viewlog opens new files
     - Release 3.0.6
 
 2023-07-09  Todd Valentic
     - Add find_config_files() method to TransportConfig()
     - Allow hostname config files now on all configs
```

### Comparing `datatransport-3.0.6/INSTALL` & `datatransport-3.0.7/INSTALL`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/LICENSE` & `datatransport-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/MIGRATION` & `datatransport-3.0.7/MIGRATION`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/PKG-INFO` & `datatransport-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.6
+Version: 3.0.7
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.6/contrib/examples/.coverage` & `datatransport-3.0.7/contrib/examples/.coverage`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/archivegroups/archivegroups.conf` & `datatransport-3.0.7/contrib/examples/archivegroups/archivegroups.conf`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,14 @@
 summary.period:			60s
 
 [MultipleFiles]
 
 command:				archivegroups
 label:					Concatenate three files together
 
-log.level: debug
-
 input.pollrate:			5s	
 input.timeout:			30s
 input.timegap:			20s
 input.newsgroups:		%(news.data)s
 input.filenames:		*.txt *.out
 
 output.path:            ./data/multiple
```

### Comparing `datatransport-3.0.6/contrib/examples/archivegroups/postdata.py` & `datatransport-3.0.7/contrib/examples/archivegroups/postdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #   Post test data files
 #
 #   2022-11-04  Todd Valentic
 #               Initial implementation
 #
 ##########################################################################
 
+import bz2
+import gzip
 import pathlib
 import sys
 import zipfile
-import gzip
-import bz2
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport.utilities import remove_file, make_path
 
 
 class PostData(ProcessClient):
@@ -27,15 +27,15 @@
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def init(self):
         super().init()
 
         self.news_poster = NewsPoster(self)
-        self.filenames = self.get_list("filenames")
+        self.filenames = self.config.get_list("filenames")
 
     def save_zip(self, filename, message):
         """Save as zip file"""
 
         with zipfile.ZipFile(filename, "w") as archive:
             archive.writestr("content", message)
 
@@ -51,21 +51,21 @@
         with bz2.open(filename, "wt") as archive:
             archive.write(message)
 
 
     def main(self):
         """Main loop"""
 
-        rate = self.get_rate("rate", 60)
+        rate = self.config.get_rate("rate", 60)
 
         counter = 0
 
         while self.wait(rate):
 
-            now = self.current_time()
+            now = self.now()
             message = f"Index: {counter}"
 
             postnames = []
 
             for name in self.filenames:
 
                 filename = pathlib.Path(now.strftime(name))
```

### Comparing `datatransport-3.0.6/contrib/examples/component/component.conf` & `datatransport-3.0.7/contrib/examples/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/component/demo.py` & `datatransport-3.0.7/contrib/examples/component/demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,39 +24,38 @@
     """Component Class"""
 
     def __init__(self, name, config, parent, **kw):
         ConfigComponent.__init__(self, "watch", name, config, parent, **kw)
 
         self.news_poster = NewsPoster(self)
 
-        self.path = self.get_path("path", ".")
-        self.label = self.get("label", "")
-        self.host = self.get("host", "")
-        self.option = self.get("option", "")
-        self.desc = self.get("desc", "")
-        self.subject = self.get("subject", "")
+        self.path = self.config.get_path("path", ".")
+        self.label = self.config.get("label", "")
+        self.host = self.config.get("host", "")
+        self.option = self.config.get("option", "")
+        self.desc = self.config.get("desc", "")
+        self.subject = self.config.get("subject", "")
 
-        self.log.info("Component: %s", name)
+        self.log.info("Component: %s", self.name)
         self.log.info("  path:    %s", self.path)
         self.log.info("  label:   %s", self.label)
         self.log.info("  host:    %s", self.host)
         self.log.info("  option:  %s", self.option)
         self.log.info("  desc:    %s", self.desc)
         self.log.info("  subject: %s", self.subject)
+        self.log.info("  options: %s", self.config.options())
 
 
 class Demo(ProcessClient):
     """Parent Class"""
 
     def __init__(self, args):
         ProcessClient.__init__(self, args)
 
-    def init(self):
-
-        self.components = self.get_components("watches", factory=Watch)
+        self.components = self.config.get_components("watches", factory=Watch)
 
         self.log.info("Loaded %d components:", len(self.components))
 
         for name in self.components:
             self.log.info("  %s", name)
 
 if __name__ == "__main__":
```

### Comparing `datatransport-3.0.6/contrib/examples/environ/environ.py` & `datatransport-3.0.7/contrib/examples/environ/environ.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class DisplayEnviron(ProcessClient):
     """Display environment"""
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
-    def init(self): 
+    def init(self):
         super().init()
 
         self.print_environ()
 
     def print_environ(self):
         """Print environment to log"""
```

### Comparing `datatransport-3.0.6/contrib/examples/filewatch/createdata.py` & `datatransport-3.0.7/contrib/examples/filewatch/createdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def init(self):
         super().init()
 
-        self.rate = self.get_rate("rate", 60)
-        self.path = self.get_path("output.path")
-        self.names = self.get_list("output.names")
-        self.maxbytes = self.get_bytes("output.maxsize", "10KB")
+        self.rate = self.config.get_rate("rate", 60)
+        self.path = self.config.get_path("output.path")
+        self.names = self.config.get_list("output.names")
+        self.maxbytes = self.config.get_bytes("output.maxsize", "10KB")
 
         if not self.names:
             self.abort("No output names (output.names)")
 
     def main(self):
         """Main loop"""
```

### Comparing `datatransport-3.0.6/contrib/examples/getbytes/demo.py` & `datatransport-3.0.7/contrib/examples/getbytes/demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,20 +17,16 @@
 
 class Demo(ProcessClient):
     """Test program"""
 
     def __init__(self, args):
         ProcessClient.__init__(self, args)
 
-    def init(self):
-        super().init()
-
         for key in self.options():
             if key.startswith('test.'):
                 try:
-                    value = self.get_bytes(key)
-                    self.log.info("%s: %s", key, self.get_bytes(key))
-                except:
-                    self.log.error('Problem parsing %s' % key)
+                    self.log.info("%s: %s", key, self.config.get_bytes(key))
+                except Exception as e:  # pylint: disable=broad-exception-caught
+                    self.log.error('Problem parsing %s: %s', key, e)
 
 if __name__ == "__main__":
     Demo(sys.argv).run()
```

### Comparing `datatransport-3.0.6/contrib/examples/getbytes/getbytes.conf` & `datatransport-3.0.7/contrib/examples/getbytes/getbytes.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/hello/helloworld.py` & `datatransport-3.0.7/contrib/examples/hello/helloworld.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 #!/usr/bin/env python3
+"""Hello World example"""
 
 ##########################################################################
 #
 #   Hello World example
 #
 #   Periodically print a message to the log file.
 #
 #   2022-10-07  Todd Valentic
 #               Initial implementation
 #
 ##########################################################################
 
+import sys
+
 from datatransport import ProcessClient
 
-import sys
 
-class Client (ProcessClient):
+class Client(ProcessClient):
+    """Process Client"""
 
     def __init__(self, args):
         ProcessClient.__init__(self, args)
 
-    def init(self):
+        self.rate = self.config.get_rate("rate")
+        self.text = self.config.get("text")
 
-        self.rate = self.get_rate('rate')
-        self.text = self.get('text')
-
-        self.log.info(f'Log message every {self.rate.period}')
+        self.log.info("Log message every: %s", self.rate.period)
 
     def main(self):
+        """Main application"""
 
         while self.wait(self.rate):
             self.log.info(self.text)
 
-if __name__ == '__main__':
-    Client(sys.argv).run()
 
+if __name__ == "__main__":
+    Client(sys.argv).run()
```

### Comparing `datatransport-3.0.6/contrib/examples/init/demo.py` & `datatransport-3.0.7/contrib/examples/init/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 #!/usr/bin/env python
 """Test Inherited init()"""
 
 ##############################################################
 #
-#   Test init() call chain in inherited classes 
+#   Test init() call chain in inherited classes
 #
 #   2023-07-03  Todd Valentic
 #               Initial implementation.
 #
 ##############################################################
 
 import sys
 
 from datatransport import Root, ProcessClient
 
+
 class MixinA(Root):
-    
+    """Mixin class A"""
+
     def init(self):
         super().init()
         self.log.info("MixinA.init()")
 
+
 class MixinB(Root):
+    """Mixin class B"""
 
     def init(self):
         super().init()
         self.log.info("MixinB.init()")
 
+
 class Demo(MixinA, MixinB, ProcessClient):
     """Parent Class"""
 
-    def __init__(self, args, **kwargs):
+    def __init__(self, args, **_kwargs):
         ProcessClient.__init__(self, args)
         MixinA.__init__(self)
         MixinB.__init__(self)
 
-        self.log.info('Demo.mro(): %s' % Demo.mro())
+        self.log.info("Demo.mro(): %s", Demo.mro())
 
     def init(self):
         super().init()
 
         self.log.info("Demo.init()")
 
+
 if __name__ == "__main__":
     Demo(sys.argv).run()
```

### Comparing `datatransport-3.0.6/contrib/examples/messagebox/messagebox.conf` & `datatransport-3.0.7/contrib/examples/messagebox/messagebox.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/messagebox/poll_file.py` & `datatransport-3.0.7/contrib/examples/messagebox/poll_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/messagebox/poll_text.py` & `datatransport-3.0.7/contrib/examples/messagebox/poll_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/messagebox/post_file.py` & `datatransport-3.0.7/contrib/examples/messagebox/post_file.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/messagebox/post_text.py` & `datatransport-3.0.7/contrib/examples/messagebox/post_text.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/postpoll/poll_file.py` & `datatransport-3.0.7/contrib/examples/postpoll/poll_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 #!/usr/bin/env python3
+"""File polling example"""
 
 ##########################################################################
 #
 #   Polling example (file attachment)
 #
-#   Periodically poll for messages from a news group 
+#   Periodically poll for messages from a news group
 #
 #   2022-10-10  Todd Valentic
 #               Initial implementation
 #
 ##########################################################################
 
+import sys
+
 from datatransport import ProcessClient
 from datatransport import NewsPoller
 from datatransport import newstool
 from datatransport.utilities import remove_file
 
-import sys
 
-class Client (ProcessClient):
+class Client(ProcessClient):
+    """Process client"""
 
     def __init__(self, args):
         ProcessClient.__init__(self, args)
 
         self.poller = NewsPoller(self, callback=self.process)
         self.main = self.poller.main
 
-        self.log.info(f'Poll for messages')
+        self.log.info("Poll for messages")
 
     def process(self, message):
+        """Process handler"""
 
         filenames = newstool.save_files(message)
-        self.log.info(f'Received files: {[str(f) for f in filenames]}')
+        self.log.info("Received files: %s", [str(f) for f in filenames])
 
         remove_file(filenames)
 
-if __name__ == '__main__':
-    Client(sys.argv).run()
 
+if __name__ == "__main__":
+    Client(sys.argv).run()
```

### Comparing `datatransport-3.0.6/contrib/examples/postpoll/poll_text.py` & `datatransport-3.0.7/contrib/examples/postpoll/poll_text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #!/usr/bin/env python3
+"""Text polling example"""
 
 ##########################################################################
 #
 #   Polling example
 #
-#   Periodically poll for messages from a news group 
+#   Periodically poll for messages from a news group
 #
 #   2022-10-10  Todd Valentic
 #               Initial implementation
 #
 ##########################################################################
 
+import sys
+
 from datatransport import ProcessClient
 from datatransport import NewsPoller
 
-import sys
 
-class Client (ProcessClient):
+class Client(ProcessClient):
+    """Process client"""
 
     def __init__(self, args):
         ProcessClient.__init__(self, args)
 
         self.poller = NewsPoller(self, callback=self.process)
         self.main = self.poller.main
 
-        self.log.info(f'Poll for messages')
+        self.log.info("Poll for messages")
 
     def process(self, message):
+        """Process handler"""
 
         text = message.get_payload()
-        self.log.info(f'Received "{text}"')
+        self.log.info('Received: "%s"', text)
 
-if __name__ == '__main__':
-    Client(sys.argv).run()
 
+if __name__ == "__main__":
+    Client(sys.argv).run()
```

### Comparing `datatransport-3.0.6/contrib/examples/postpoll/post_file.py` & `datatransport-3.0.7/contrib/examples/postpoll/post_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 #!/usr/bin/env python3
+"""Text posting example"""
 
 ##########################################################################
 #
-#   File post example
+#   Posting example
 #
-#   Periodically post a file to a news group 
+#   Periodically post a message to a news group
 #
 #   2022-10-10  Todd Valentic
 #               Initial implementation
 #
 ##########################################################################
 
+import sys
+
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 
-import sys
-import pathlib
 
-class Client (ProcessClient):
+class Client(ProcessClient):
+    """Process Client"""
 
-    def __init__(self, args):
-        ProcessClient.__init__(self, args)
+    def __init__(self, argv):
+        ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
 
-    def init(self):
-
-        self.rate = self.get_rate('rate')
-        self.text = self.get('text')
+        self.rate = self.config.get_rate("rate")
+        self.text = self.config.get("text")
 
-        self.log.info(f'Post message every {self.rate.period}')
+        self.log.info("Post message every %s", self.rate.period)
 
     def main(self):
-
-        filename = pathlib.Path('data.txt')
+        """Main application"""
 
         while self.wait(self.rate):
+            self.news_poster.post_text(self.text)
+            self.log.info("Posted message")
 
-            with filename.open(mode='w') as message:
-                message.write(self.text)
-
-            self.news_poster.post(str(filename))
-            self.log.info('Posted %s' % filename)
 
-            filename.unlink()
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     Client(sys.argv).run()
-
```

### Comparing `datatransport-3.0.6/contrib/examples/postpoll/postpoll.conf` & `datatransport-3.0.7/contrib/examples/postpoll/postpoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/rotatelogs/counter.py` & `datatransport-3.0.7/contrib/examples/rotatelogs/counter.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def main(self):
         """Main loop"""
 
-        rate = self.get_rate("rate", 1)
+        rate = self.config.get_rate("rate", 1)
         counter = 0
 
         while self.wait(rate):
             self.log.info("Counter = %d", counter)
             counter += 1
```

### Comparing `datatransport-3.0.6/contrib/examples/service/client.py` & `datatransport-3.0.7/contrib/examples/service/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 class EchoClient(ProcessClient):
     """Client calling the echo service"""
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
-        self.connect = Directory(self)
+        self.directory = Directory(self)
 
-        self.rate = self.get_rate("rate", "10s")
+        self.rate = self.config.get_rate("rate", "10s")
 
         self.log.info('echo client')
 
-        self.echo = self.connect("echo")
+        self.echo = self.directory.connect("echo")
 
     def run(self):
         self.log.info("Starting")
         try:
             self._run()
         except BaseException as err:
             self.log.exception(str(err))
```

### Comparing `datatransport-3.0.6/contrib/examples/service/echo.py` & `datatransport-3.0.7/contrib/examples/service/echo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/service/service.conf` & `datatransport-3.0.7/contrib/examples/service/service.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples/spawn/spawner.py` & `datatransport-3.0.7/contrib/examples/spawn/spawner.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def main(self):
         """Main loop"""
 
-        rate = self.get_rate("spawn.rate", 10)
-        cmd = self.get("spawn.command", "pwd")
+        rate = self.config.get_rate("spawn.rate", 10)
+        cmd = self.config.get("spawn.command", "pwd")
 
         while self.wait(rate):
 
             self.log.info("Running command: %s", cmd)
 
             try:
                 status, output = subprocess.getstatusoutput(cmd)
-            except BaseException: # pylint: disable=broad-except
+            except Exception: # pylint: disable=broad-exception-caught
                 self.log.exception("Problem starting child")
                 self.abort("Exiting")
 
             self.log.info("  Status=%d", status)
             self.log.info("  Output=%s", output)
```

### Comparing `datatransport-3.0.6/contrib/examples/watchdog/crasher.py` & `datatransport-3.0.7/contrib/examples/watchdog/crasher.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def main(self):
         """Main loop"""
 
-        lifetime = self.get_rate("lifetime", 10)
+        lifetime = self.config.get_rate("lifetime", 10)
 
         while self.wait(lifetime):
             self.log.info("About to crash!")
             self.log.info("badness = %f", 1 / 0)
 
 
 if __name__ == "__main__":
```

### Comparing `datatransport-3.0.6/contrib/examples/watchdog/init_crasher.py` & `datatransport-3.0.7/contrib/examples/watchdog/init_crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/README` & `datatransport-3.0.7/contrib/examples.v2/README`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/archivegroups/archivegroups.conf` & `datatransport-3.0.7/contrib/examples.v2/archivegroups/archivegroups.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/archivegroups/postdata.py` & `datatransport-3.0.7/contrib/examples.v2/archivegroups/postdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/component/component.conf` & `datatransport-3.0.7/contrib/examples.v2/component/component.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/component/demo.py` & `datatransport-3.0.7/contrib/examples.v2/component/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/config/config.py` & `datatransport-3.0.7/contrib/examples.v2/config/config.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/environ/environ.py` & `datatransport-3.0.7/contrib/examples.v2/environ/environ.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/eventmonitor/eventmonitor.conf` & `datatransport-3.0.7/contrib/examples.v2/eventmonitor/eventmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/eventmonitor/serverstate.py` & `datatransport-3.0.7/contrib/examples.v2/eventmonitor/serverstate.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/filewatch/createdata.py` & `datatransport-3.0.7/contrib/examples.v2/filewatch/createdata.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/getbytes/demo.py` & `datatransport-3.0.7/contrib/examples.v2/getbytes/demo.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/instrumentstatus/instrumentstatus.conf` & `datatransport-3.0.7/contrib/examples.v2/instrumentstatus/instrumentstatus.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/instrumentstatus/postdata` & `datatransport-3.0.7/contrib/examples.v2/instrumentstatus/postdata`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/multipoll/multipoll.conf` & `datatransport-3.0.7/contrib/examples.v2/multipoll/multipoll.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/multipoll/writer.py` & `datatransport-3.0.7/contrib/examples.v2/multipoll/writer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf` & `datatransport-3.0.7/contrib/examples.v2/newsgroupmonitor/newsgroupmonitor.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/plottool/datasource.py` & `datatransport-3.0.7/contrib/examples.v2/plottool/datasource.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/plottool/plottool.conf` & `datatransport-3.0.7/contrib/examples.v2/plottool/plottool.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/postdatafiles/createfiles.py` & `datatransport-3.0.7/contrib/examples.v2/postdatafiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/postdatafiles/postdatafiles.conf` & `datatransport-3.0.7/contrib/examples.v2/postdatafiles/postdatafiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/rotatelogs/counter.py` & `datatransport-3.0.7/contrib/examples.v2/rotatelogs/counter.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/spawn/spawner.py` & `datatransport-3.0.7/contrib/examples.v2/spawn/spawner.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/splitfiles/createfiles.py` & `datatransport-3.0.7/contrib/examples.v2/splitfiles/createfiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/splitfiles/splitfiles.conf` & `datatransport-3.0.7/contrib/examples.v2/splitfiles/splitfiles.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/syncpoller/source.py` & `datatransport-3.0.7/contrib/examples.v2/syncpoller/source.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/syncpoller/syncpoller.conf` & `datatransport-3.0.7/contrib/examples.v2/syncpoller/syncpoller.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/wait/timer.py` & `datatransport-3.0.7/contrib/examples.v2/wait/timer.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/examples.v2/watchdog/crasher.py` & `datatransport-3.0.7/contrib/examples.v2/watchdog/crasher.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/createnewsgroup` & `datatransport-3.0.7/contrib/utils/createnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/getarticle` & `datatransport-3.0.7/contrib/utils/getarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/postarticle` & `datatransport-3.0.7/contrib/utils/postarticle`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/rebuilddatabase` & `datatransport-3.0.7/contrib/utils/rebuilddatabase`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/relaynewsgroup` & `datatransport-3.0.7/contrib/utils/relaynewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/rmnewsgroup` & `datatransport-3.0.7/contrib/utils/rmnewsgroup`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/contrib/utils/watchtransport` & `datatransport-3.0.7/contrib/utils/watchtransport`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/pyproject.toml` & `datatransport-3.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
     ]
 
 [project.urls]
 homepage="https://github.com/valentic/datatransport"
 repository="https://github.com/valentic/datatransport"
 
 [project.scripts]
-    archivegroups = "datatransport.components.ArchiveGroups:main"
-    directoryservice = "datatransport.components.DirectoryService:main"
+    archivegroups = "datatransport.components.archivegroups:main"
+    directoryservice = "datatransport.components.directoryservice:main"
     diskmonitor = "datatransport.components.DiskMonitor:main"
     filepost = "datatransport.components.FilePost:main"
     filestore = "datatransport.components.FileStore:main"
-    filewatch = "datatransport.components.FileWatch:main"
+    filewatch = "datatransport.components.filewatch:main"
     groupcontrol = "datatransport.components.GroupControl:main"
     instrumentstatus = "datatransport.components.InstrumentStatus:main"
     newsgateway = "datatransport.components.NewsGateway:main"
     newsgroupmonitor = "datatransport.components.NewsgroupMonitor:main"
     plottool = "datatransport.components.PlotTool:main"
     postdatafiles = "datatransport.components.PostDataFiles:main"
     realtimefeed = "datatransport.components.RealTimeFeed:main"
```

### Comparing `datatransport-3.0.6/src/datatransport/__init__.py` & `datatransport-3.0.7/src/datatransport/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/cancelnewsgroup.py` & `datatransport-3.0.7/src/datatransport/commands/cancelnewsgroup.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/console.py` & `datatransport-3.0.7/src/datatransport/commands/console.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/listnewsgroups.py` & `datatransport-3.0.7/src/datatransport/commands/listnewsgroups.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/transport_create_app.py` & `datatransport-3.0.7/src/datatransport/commands/transport_create_app.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/transportctl.py` & `datatransport-3.0.7/src/datatransport/commands/transportctl.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/transportd.py` & `datatransport-3.0.7/src/datatransport/commands/transportd.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/transportps.py` & `datatransport-3.0.7/src/datatransport/commands/transportps.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/commands/viewlog.py` & `datatransport-3.0.7/src/datatransport/commands/viewlog.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/ArchiveGroups.py` & `datatransport-3.0.7/src/datatransport/components/archivegroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#!/usr/bin/env python3
+"""ArchiveGroups Component"""
+
+# pylint: disable=bare-except
+
 ##############################################################################
 #
 #  ArchiveGroups
 #
 #  Archives messages held in multiple newsgroups.
 #
 #  History:
@@ -206,15 +211,15 @@
 #
 #   2.1.29  2004-04-08  Todd Valentic
 #           Add wait_on_start option (defaults on) to pause on startup
 #               (prevents a lot of thrashing the news server when all
 #               the processes are starting), but for long waits, it can
 #               be annoying for debugging.
 #
-#           Added start_currentReset (defaults on) to prevent reseting
+#           Added start_current_reset (defaults on) to prevent reseting
 #               the start_current counter, allowing you to "catchup"
 #               each time the news server is queried. Therefore, you
 #               can now do something like wake up each hour and just
 #               process the last message to give you an hourly sample.
 #
 #   2.1.30  2004-08-17  Todd Valentic
 #           Change to new logging interface.
@@ -342,51 +347,55 @@
 #                   removeFile -> remove_file
 #                   sizeDesc -> size_desc
 #                   getInt -> get_int
 #                   getDeltaTime -> get_timedelta
 #                   getboolean -> get_boolean
 #                   NewsPoster
 #
+#   2023-07-26  Todd Valentic
+#               Updated for transport3 / python3
+#
 ##############################################################################
 
 import email
 import fnmatch
 import glob
 import math
 import os
-import pathlib
 import shelve
 import shutil
 import stat
 import sys
 import subprocess
 import traceback
-import types
 
 from datetime import datetime, timezone
 from hashlib import md5
+from pathlib import Path
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport import newstool
 
 from datatransport.utilities import size_desc
 from datatransport.utilities import remove_file
 from datatransport.utilities import PatternTemplate
 from datatransport.utilities import datefunc
 from datatransport.utilities import make_path
 
 
 def now():
+    """Return current time"""
     return datetime.now(timezone.utc)
 
 
 class Checkpoint:
-    def __init__(self, newsgroup, low_mark, max_history, keep_summary):
+    """Track newsgroup state"""
 
+    def __init__(self, newsgroup, low_mark, max_history, keep_summary):
         self.newsgroup = newsgroup
         self.last_message = low_mark - 1
 
         self.keep_summary = keep_summary
         self.summary_max_files = 1000
         self.reset_summary()
 
@@ -398,38 +407,43 @@
         self.start_time = now()
         self.poll_time = now()
 
         self.history = []
         self.max_history = max_history
 
     def update_message(self, msg_num, date=None):
+        """Update current state"""
 
         self.num_messages = self.num_messages + 1
         self.last_message = msg_num
         self.poll_time = now()
 
         if date:
             self.last_time = date
 
     def touch_message(self, msg_num):
+        """Mark message time"""
 
         self.last_message = msg_num
         self.poll_time = now()
 
     def update_file(self, filename, numbytes):
+        """Update file stats"""
+
         if filename in self.filenames:
-            (prevMsgs, prevBytes) = self.filenames[filename]
+            (prev_msgs, prev_bytes) = self.filenames[filename]
         else:
-            prevMsgs = 0
-            prevBytes = 0
+            prev_msgs = 0
+            prev_bytes = 0
 
-        self.filenames[filename] = (prevMsgs + 1, prevBytes + numbytes)
+        self.filenames[filename] = (prev_msgs + 1, prev_bytes + numbytes)
         self.num_bytes = self.num_bytes + numbytes
 
     def reset(self, date=None, last_message=0):
+        """Reset state"""
 
         if not date:
             date = now()
 
         if self.filenames:
             self.history.insert(0, (self.filenames, self.last_time))
             self.history = self.history[0 : self.max_history + 1]
@@ -444,112 +458,118 @@
         self.last_time = date
         self.num_messages = 0
         self.num_bytes = 0
         self.filenames = {}
         self.last_message = last_message
 
     def is_active(self):
+        """Is newsgroup active"""
+
         return self.num_messages > 0
 
     def in_span(self, curtime, timespan):
+        """Check if time in span"""
 
         lastsecs = self.last_time.timestamp()
         cursecs = curtime.timestamp()
         interval = timespan.total_seconds()
 
         lastblock = int(math.floor(lastsecs / interval))
         curblock = int(math.floor(cursecs / interval))
 
         return lastblock == curblock
 
     def reset_summary(self):
+        """Reset summary counts"""
 
         self.summary_files = []
         self.summary_start = now()
         self.summary_bytes = 0
         self.summary_msgs = 0
 
     def get_report(self, title, reason):
+        """Generate report"""
 
         message = []
 
         fmt = "%c %Z %z"
 
         message.append("_" * 75)
-        message.append("%s" % title)
+        message.append(title)
         message.append("")
-        message.append("    Newsgroup     : %s" % self.newsgroup)
-        message.append("    Beginning     : %s" % self.start_time.strftime(fmt))
-        message.append("    Ending        : %s" % self.last_time.strftime(fmt))
-        message.append("    Messages      : %d" % self.num_messages)
-        message.append("    Total bytes   : %s" % size_desc(self.num_bytes))
-        message.append("    Reason        : %s" % reason)
+        message.append(f"    Newsgroup     : {self.newsgroup}")
+        message.append(f"    Beginning     : {self.start_time.strftime(fmt)}")
+        message.append(f"    Ending        : {self.last_time.strftime(fmt)}")
+        message.append(f"    Messages      : {self.num_messages}")
+        message.append(f"    Total bytes   : {size_desc(self.num_bytes)}")
+        message.append(f"    Reason        : {reason}")
         message.append("")
 
         if self.filenames:
             message.append("    Filenames")
             message.append("    ---------")
 
             for filename in sorted(self.filenames):
                 msgs, numbytes = self.filenames[filename]
                 if msgs > 1:
                     units = "msgs"
                 else:
                     units = "msg"
                 message.append(
-                    "    %s: %s (%d %s)" % (filename, size_desc(numbytes), msgs, units)
+                    f"    {filename}: {size_desc(numbytes)} ({msgs} {units})"
                 )
 
         message.append("_" * 75)
         message = "\n".join(message)
 
         return message
 
     def get_summary(self, title):
+        """Get summary report"""
 
         message = []
 
         fmt = "%c %Z %z"
 
         message.append("_" * 75)
-        message.append("%s" % title)
+        message.append(title)
         message.append("")
-        message.append("    Newsgroup     : %s" % self.newsgroup)
-        message.append("    Beginning     : %s" % self.summary_start.strftime(fmt))
-        message.append("    Ending        : %s" % now().strftime(fmt))
-        message.append("    Messages      : %d" % self.summary_msgs)
-        message.append("    Total bytes   : %s" % size_desc(self.summary_bytes))
+        message.append(f"    Newsgroup     : {self.newsgroup}")
+        message.append(f"    Beginning     : {self.summary_start.strftime(fmt)}")
+        message.append(f"    Ending        : {now().strftime(fmt)}")
+        message.append(f"    Messages      : {self.summary_msgs}")
+        message.append(f"    Total bytes   : {size_desc(self.summary_bytes)}")
         message.append("")
 
         if self.summary_files:
             message.append("    Filenames")
             message.append("    ---------")
 
             for filegroup in self.summary_files:
-
                 prefix = "-"
                 for filename in sorted(filegroup):
                     msgs, numbytes = filegroup[filename]
                     if msgs > 1:
                         units = "msgs"
                     else:
                         units = "msg"
                     message.append(
-                        "  %s %s: %s (%d %s)"
-                        % (prefix, filename, size_desc(numbytes), msgs, units)
+                        f"  {prefix} {filename}: {size_desc(numbytes)} ({msgs} {units})"
                     )
                     prefix = " "
 
         message.append("_" * 75)
         message = "\n".join(message)
 
         return message
 
 
 class ArchiveGroups(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.report_poster = NewsPoster(self, prefix="report", quiet=True)
         self.summary_poster = NewsPoster(self, prefix="summary", quiet=True)
         self.trouble_poster = NewsPoster(self, prefix="trouble", quiet=True)
 
@@ -559,149 +579,162 @@
         self.replace_client_name = PatternTemplate("clientname", "/")
         self.replace_newsgroup = PatternTemplate("newsgroup", ".")
         self.replace_filename = PatternTemplate("filename", ".")
         self.replace_rule = PatternTemplate("rule")
         self.replace_history = PatternTemplate("history")
         self.replace_header = PatternTemplate("header")
 
-        self.time_offset = self.get_timedelta("timeoffset", 0)
-        self.pollrate = self.get_rate("input.pollrate", 60)
-        self.wait_on_start = self.get_boolean("input.wait_on_start", True)
-
-        self.pollserver_host = self.get("input.server", "localhost")
-        self.pollserver_port = self.get_int("input.server.port", 119)
-        self.timeout = self.get_timedelta("input.timeout", None)
-        self.timegap = self.get_timedelta("input.timegap", None)
-        self.timespan = self.get_timedelta("input.timespan", None)
-        self.start_time = self.get("input.start_time", None)
-        self.stop_time = self.get("input.stop_time", None)
-        self.start_current = self.get_int("input.start_current", 1)
-        self.start_currentReset = self.get_boolean("input.start_current.reset", True)
-
-        self.dest_path = self.get("output.path", "")
-        self.dest_name = self.get("output.name", "<rule>")
-        self.dest_file_mode = self.get_int("output.mode.file", "0o644")
-        self.dest_path_mode = self.get_int("output.mode.path", "0o755")
-        self.max_messages = self.get_int("output.max_messages", 1)
-        self.expire = self.get_timedelta("output.expire", None)
-        self.history = self.get_int("output.history", 0)
-        self.plain_text_name = self.get("output.plain_text_name", "noname.txt")
-        self.uncompress = self.get_boolean("output.uncompress", False)
-        self.overwrite = self.get_boolean("output.overwrite", True)
+        self.time_offset = self.config.get_timedelta("timeoffset", 0)
+        self.pollrate = self.config.get_rate("input.pollrate", 60)
+        self.wait_on_start = self.config.get_boolean("input.wait_on_start", True)
+
+        self.pollserver_host = self.config.get("input.server", "localhost")
+        self.pollserver_port = self.config.get_int("input.server.port", 119)
+        self.timeout = self.config.get_timedelta("input.timeout", None)
+        self.timegap = self.config.get_timedelta("input.timegap", None)
+        self.timespan = self.config.get_timedelta("input.timespan", None)
+        self.start_time = self.config.get("input.start_time", None)
+        self.stop_time = self.config.get("input.stop_time", None)
+        self.start_current = self.config.get_int("input.start_current", 1)
+        self.start_current_reset = self.config.get_boolean(
+            "input.start_current.reset", True
+        )
+
+        self.dest_path = self.config.get("output.path", "")
+        self.dest_name = self.config.get("output.name", "<rule>")
+        self.dest_file_mode = self.config.get_int("output.mode.file", "0o644")
+        self.dest_path_mode = self.config.get_int("output.mode.path", "0o755")
+        self.max_messages = self.config.get_int("output.max_messages", 1)
+        self.expire = self.config.get_timedelta("output.expire", None)
+        self.history = self.config.get_int("output.history", 0)
+        self.plain_text_name = self.config.get("output.plain_text_name", "noname.txt")
+        self.uncompress = self.config.get_boolean("output.uncompress", False)
+        self.overwrite = self.config.get_boolean("output.overwrite", True)
 
-        self.report_subject = self.get("report.subject", "Newsgroup archive report")
-        self.report_title = self.get("report.title", "Newsgroup archive report")
+        self.report_subject = self.config.get(
+            "report.subject", "Newsgroup archive report"
+        )
+        self.report_title = self.config.get("report.title", "Newsgroup archive report")
 
         enable = self.report_poster.enabled
-        self.report_max_messages = self.get_boolean("report.enable.max_messages", enable)
-        self.report_timeout = self.get_boolean("report.enable.timeout", enable)
-        self.report_timegap = self.get_boolean("report.enable.timegap", enable)
-        self.report_timespan = self.get_boolean("report.enable.timespan", enable)
-
-        self.summary_subject = self.get("summary.subject", "Newsgroup summary report")
-        self.summary_title = self.get("summary.title", "Newsgroup summary report")
-        self.summary_enable = self.get_boolean(
+        self.report_max_messages = self.config.get_boolean(
+            "report.enable.max_messages", enable
+        )
+        self.report_timeout = self.config.get_boolean("report.enable.timeout", enable)
+        self.report_timegap = self.config.get_boolean("report.enable.timegap", enable)
+        self.report_timespan = self.config.get_boolean("report.enable.timespan", enable)
+
+        self.summary_subject = self.config.get(
+            "summary.subject", "Newsgroup summary report"
+        )
+        self.summary_title = self.config.get(
+            "summary.title", "Newsgroup summary report"
+        )
+        self.summary_enable = self.config.get_boolean(
             "summary.enable", self.summary_poster.enabled
         )
-        self.summary_period = self.get_timedelta("summary.period", 60 * 60 * 24)
-        self.summary_offset = self.get_timedelta("summary.offset", 0)
-        self.summary_max_files = self.get_int("summary.max_files", 1000)
-
-        self.debug = self.get_boolean("debug", False)
-
-        self.include_newsgroups = self.get_list("input.newsgroups")
-        self.exclude_newsgroups = self.get_list("input.newsgroups.exclude")
-        self.include_filenames = self.get_list("input.filenames", "*")
-        self.exclude_filenames = self.get_list("input.filenames.exclude")
+        self.summary_period = self.config.get_timedelta("summary.period", 60 * 60 * 24)
+        self.summary_offset = self.config.get_timedelta("summary.offset", 0)
+        self.summary_max_files = self.config.get_int("summary.max_files", 1000)
+
+        self.debug = self.config.get_boolean("debug", False)
+
+        self.include_newsgroups = self.config.get_list("input.newsgroups")
+        self.exclude_newsgroups = self.config.get_list("input.newsgroups.exclude")
+        self.include_filenames = self.config.get_list("input.filenames", "*")
+        self.exclude_filenames = self.config.get_list("input.filenames.exclude")
 
         try:
-            self.callback = self.get_callback("callback")
+            self.callback = self.config.get_callback("callback")
         except:
             self.log.exception("Problem loading callback")
             self.abort()
 
         try:
-            self.rules = eval(self.get("output.rules", "[('*','*','<filename>')]"))
+            self.rules = eval(
+                self.config.get("output.rules", "[('*','*','<filename>')]")
+            )
         except:
             self.log.exception("There was a problem parsing output.rules.")
             self.abort()
 
         self.validate_setup()
         self.setup_database()
 
     def __del__(self):
         try:
             self.database.close()
         except:
             pass
 
     def setup_database(self):
+        """Setup checkpoint database"""
 
         self.database = shelve.open("checkpoint.db")
 
         # Update the config parameters in the database to new values.
 
-        for key in self.database.keys():
-            checkpoint = self.database[key]
+        for key, checkpoint in self.database.items():
             checkpoint.max_history = self.history
             checkpoint.keep_summary = self.summary_enable
             checkpoint.summary_max_files = self.summary_max_files
             self.database[key] = checkpoint
 
         # Make sure that the on-disk files are initialized, otherwise they will
         # be zero-length and cause problems next time if opened that way.
 
         self.database.sync()
 
     def validate_setup(self):
+        """Validate setup"""
 
         if self.start_time:
             try:
                 self.start_time = datefunc.strptime(
                     self.start_time, self.time_fmt, timezone.utc
                 )
-                self.log.info("Only processing messages past %s" % self.start_time)
+                self.log.info("Only processing messages past %s", self.start_time)
             except:
                 self.log.exception(
                     "The start time format is bad. It should be YYYY JJJ HH:MM:SS"
                 )
                 self.abort("Exiting")
 
         if self.stop_time:
             try:
                 self.stop_time = datefunc.strptime(
                     self.stop_time, self.time_fmt, timezone.utc
                 )
-                self.log.info("Only processing messages before  %s" % self.stop_time)
+                self.log.info("Only processing messages before  %s", self.stop_time)
             except:
                 self.log.exception(
                     "The stop time format is bad. It should be YYYY JJJ HH:MM:SS"
                 )
                 self.abort("Exiting")
 
         self.log.debug("Watching these newsgroups (+ = include, - = exclude):")
         for newsgroup in self.include_newsgroups:
-            self.log.debug("  + %s" % newsgroup)
+            self.log.debug("  + %s", newsgroup)
         for newsgroup in self.exclude_newsgroups:
-            self.log.debug("  - %s" % newsgroup)
+            self.log.debug("  - %s", newsgroup)
 
         self.log.debug("Watching these filenames (+ = include, - = exclude):")
         for filename in self.include_filenames:
-            self.log.debug("  + %s" % filename)
+            self.log.debug("  + %s", filename)
         for filename in self.exclude_filenames:
-            self.log.debug("  - %s" % filename)
+            self.log.debug("  - %s", filename)
 
     def get_groups(self, newsserver):
+        """Get newsgroup list"""
 
         groups = []
 
-        response, list = newsserver.list()
-
-        for newsgroup, high_mark, low_mark, flag in list:
+        _response, newsgroup_list = newsserver.list()
 
+        for newsgroup, high_mark, low_mark, _flag in newsgroup_list:
             high_mark = int(high_mark)
             low_mark = int(low_mark)
 
             for incgroup in self.include_newsgroups:
                 if fnmatch.fnmatch(newsgroup, incgroup):
                     keep = 1
                     for excgroup in self.exclude_newsgroups:
@@ -716,79 +749,82 @@
                             )
                             self.database[newsgroup] = checkpoint
                             self.database.sync()
 
         return groups
 
     def filter_filenames(self, filenames):
+        """Filter filenames"""
 
         goodfiles = []
 
         for filename in filenames:
-
             for incpattern in self.include_filenames:
                 if fnmatch.fnmatch(filename, incpattern):
                     keep = 1
                     for excpattern in self.exclude_filenames:
                         if fnmatch.fnmatch(filename, excpattern):
                             keep = 0
                             break
                     if keep:
                         goodfiles.append(filename)
 
         return goodfiles
 
-    def get_file_time(self, newsgroup, filename):
+    def get_file_time(self, _newsgroup, _filename):
+        """Get timestamp from filename"""
         return None
 
     def compute_name(self, filename, checkpoint):
+        """Compute filename"""
 
         rule = self.find_rule(checkpoint.newsgroup, filename)
 
         path = os.path.join(self.dest_path, self.dest_name)
         path = self.replace_rule(path, rule)
 
         try:
-            filetime = self.get_file_time(checkpoint.newsgroup, filename)
+            filetime = self.config.get_file_time(checkpoint.newsgroup, filename)
         except:
             filetime = None
 
         if filetime is None:
-
             if self.max_messages == 1:
                 filetime = checkpoint.last_time
             else:
                 filetime = checkpoint.start_time
 
         # NOTE - Potential breakage with long paths and versions
         #        of python < 2.4.4 where strftime is limited to
-        #        127 character strings. Miving it to the end
+        #        127 character strings. Moving it to the end
         #        of the expansion here, helped, but I need to
         #        figure out a better way of doing this...
 
         path = self.replace_newsgroup(path, checkpoint.newsgroup)
         path = self.replace_proc_group(path, self.groupname)
         path = self.replace_client_name(path, self.name)
         path = self.replace_filename(path, str(filename))
         path = self.replace_header(path)
         path = filetime.strftime(path)
 
         return path
 
     def find_rule(self, newsgroup, filename):
+        """Find matching rule"""
 
         for rule in self.rules:
             if fnmatch.fnmatch(newsgroup, rule[0]) and fnmatch.fnmatch(
                 filename, rule[1]
             ):
                 return rule[2]
 
         return ""
 
     def post_report(self, checkpoint, reason):
+        """Post report"""
 
         title = self.report_title
         title = self.replace_newsgroup(title, checkpoint.newsgroup)
         title = self.replace_proc_group(title, self.groupname)
         title = self.replace_client_name(title, self.name)
 
         header = self.report_subject
@@ -797,19 +833,20 @@
         header = self.replace_client_name(header, self.name)
 
         message = checkpoint.get_report(title, reason)
 
         try:
             self.report_poster.set_subject(header)
             self.report_poster.post_text(message)
-            self.log.info("%s, posting report (%s)" % (reason, checkpoint.newsgroup))
+            self.log.info("%s, posting report (%s)", reason, checkpoint.newsgroup)
         except:
-            self.log.error("Error posting report message")
+            self.log.exception("Error posting report message")
 
     def post_summary(self, checkpoint):
+        """Post summary report"""
 
         title = self.summary_title
         title = self.replace_newsgroup(title, checkpoint.newsgroup)
         title = self.replace_proc_group(title, self.groupname)
         title = self.replace_client_name(title, self.name)
 
         header = self.summary_subject
@@ -818,92 +855,92 @@
         header = self.replace_client_name(header, self.name)
 
         message = checkpoint.get_summary(title)
 
         try:
             self.summary_poster.set_subject(header)
             self.summary_poster.post_text(message)
-            self.log.info("Posting summary report (%s)" % (checkpoint.newsgroup))
+            self.log.info("Posting summary report (%s)", checkpoint.newsgroup)
         except:
             self.log.error("Error posting summary message")
 
     def roll_files(self, checkpoint):
+        """Only keep N files"""
 
         self.log.debug("Rolling file history:")
-        self.log.debug("  history length: %d" % len(checkpoint.history))
-        self.log.debug("  max history: %d" % checkpoint.max_history)
+        self.log.debug("  history length: %d", len(checkpoint.history))
+        self.log.debug("  max history: %d", checkpoint.max_history)
 
         if not checkpoint.history or checkpoint.max_history == 0:
             self.log.debug("  no files to roll")
             return
 
-        historyIndex = list(range(len(checkpoint.history)))
-        historyIndex.reverse()
-
-        for index in historyIndex:
+        history_index = list(range(len(checkpoint.history)))
+        history_index.reverse()
 
+        for index in history_index:
             filenames = checkpoint.history[index][0].keys()
 
             for filename in filenames:
-
                 oldname = self.replace_history(filename, index)
                 newname = self.replace_history(filename, index + 1)
 
                 try:
                     if index < checkpoint.max_history:
                         if oldname == newname:
-                            self.log.debug("  keeping  %s" % oldname)
+                            self.log.debug("  keeping  %s", oldname)
                         else:
                             os.rename(oldname, newname)
-                            self.log.debug("  copying  %s -> %s" % (oldname, newname))
+                            self.log.debug("  copying  %s -> %s", oldname, newname)
                     else:
                         os.remove(oldname)
-                        self.log.debug("  removing %s" % oldname)
+                        self.log.debug("  removing %s", oldname)
                 except:
                     pass
 
     def save_callback(self, filename):
+        """Save callback"""
 
         # Used by derived classes to do something interesting with
         # the newly saved file such as creating a thumbnail of images.
 
-        pass
-
     def save_handler(self, srcname, destname, mode):
-        srcfile = open(srcname, "r")
+        """Save handler"""
+
+        srcfile = open(srcname, "rb")
         destfile = open(destname, mode)
         shutil.copyfileobj(srcfile, destfile)
         srcfile.close()
         destfile.close()
         os.chmod(destname, self.dest_file_mode)
 
     def save_file(self, srcname, checkpoint):
+        """Save single file"""
 
         num_bytes = os.stat(srcname)[stat.ST_SIZE]
         name = self.compute_name(srcname, checkpoint)
-        destname = self.replace_history(name, 0)
+        destname = self.replace_history(name, str(0))
         destname = os.path.abspath(destname)
-        dirname = os.path.dirname(destname)
 
-        self.log.debug("Saving %s" % srcname)
-        self.log.debug("  dest: %s" % destname)
-        self.log.debug("  maxmessages: %d" % self.max_messages)
-        self.log.debug("  nummessages: %d" % checkpoint.num_messages)
-        self.log.debug("  is_active: %s" % checkpoint.is_active())
+        self.log.debug("Saving %s", srcname)
+        self.log.debug("  dest: %s", destname)
+        self.log.debug("  maxmessages: %d", self.max_messages)
+        self.log.debug("  nummessages: %d", checkpoint.num_messages)
+        self.log.debug("  is_active: %s", checkpoint.is_active())
 
         if not self.overwrite and os.path.exists(destname):
             self.log.debug("  destination exists - not saving")
             return
 
         if self.max_messages != 1 and checkpoint.is_active():
-            mode = "a"
-            self.log.info("Concat: %s -> %s" % (srcname, destname))
+            mode = "ab"
+            self.log.info("Concat: %s -> %s", srcname, destname)
         else:
-            mode = "w"
-            self.log.info("Start : %s -> %s" % (srcname, destname))
+            mode = "wb"
+            self.log.info("Start : %s -> %s", srcname, destname)
 
         try:
             make_path(destname, self.dest_path_mode)
         except BaseException as err:
             self.log.exception("Problem creating the path.")
             raise err
 
@@ -921,54 +958,61 @@
             self.save_callback(destname)
         except:
             self.log.exception("Problem running the save callback")
 
         checkpoint.update_file(name, num_bytes)
 
     def uncompress_file(self, cmd, filename):
+        """Uncompress file if needed"""
 
-        uncompressname = filename.stem 
+        uncompressname = filename.stem
 
         try:
-            status, output = subprocess.getstatusoutput("%s %s" % (cmd, filename))
+            status, output = subprocess.getstatusoutput(f"{cmd} {filename}")
         except IOError:
-            self.abort("Error running uncompression: %s" % cmd)
+            self.abort("Error running uncompression: %s", cmd)
 
         if status == 0:
-            self.log.debug("  uncompressing: %s" % filename)
+            self.log.debug("  uncompressing: %s", filename)
         else:
             subject = "Archive: Error umcompressing file"
             note = []
             note.append("Error trying to uncompress file")
-            note.append("   command: %s" % cmd)
-            note.append("   status:  %d" % status)
-            note.append("   output:  %s" % output)
+            note.append("   command: %s", cmd)
+            note.append("   status:  %d", status)
+            note.append("   output:  %s", output)
             self.post_error(subject, note)
             return None
 
-        return pathlib.Path(uncompressname)
+        return Path(uncompressname)
 
     def last_tracback(self):
+        """Format last traceback"""
+
         return traceback.format_tb(sys.exc_traceback)[-1]
 
     def post_error(self, subject, note):
+        """Post error message"""
+
         for line in note:
             self.log.error(line)
 
         try:
             self.trouble_poster.set_subject(subject)
             self.trouble_poster.post_text("\n".join(note))
             self.log.info("Sent trouble message")
         except:
             self.log.exception("Failed to post trouble message")
 
-    def validate_file(self, filename):
+    def validate_file(self, _filename):
+        """Validate file"""
         return True
 
     def process_files(self, filenames, checkpoint, msg_num, msg_time):
+        """Process files"""
 
         # Hack alert - the callbacks sometimes want access to
         # the message time.
         self.msg_time = msg_time
 
         # Roll old files
 
@@ -977,33 +1021,30 @@
             checkpoint.reset(msg_time, msg_num)
 
         # Uncompress any files that need it
 
         uncompressedfiles = []
 
         for filename in filenames:
-
             if self.uncompress:
-
-                if filename.suffix == ".zip":
-                    filename = self.uncompress_file("unzip -o", filename)
-                elif filename.suffix == ".gz":
+                # if filename.suffix == ".zip":
+                #    filename = self.uncompress_file("unzip -o", filename)
+                if filename.suffix == ".gz":
                     filename = self.uncompress_file("gunzip -f", filename)
                 elif filename.suffix == ".bz2":
                     filename = self.uncompress_file("bunzip2 -f", filename)
 
             if filename:
                 uncompressedfiles.append(filename)
 
         # Run the callback function if needed
 
         savefiles = []
 
         for filename in uncompressedfiles:
-
             if not self.validate_file(filename):
                 continue
 
             if self.callback:
                 try:
                     filename = self.callback(self, filename)
                     # filename can now be the same name, a new name
@@ -1019,49 +1060,51 @@
 
             if isinstance(filename, (list, tuple)):
                 savefiles.extend(filename)
             else:
                 savefiles.append(filename)
 
         for filename in savefiles:
-
             try:
                 self.save_file(filename, checkpoint)
             except:
                 note = []
                 note.append("Problem storing file:")
-                note.append("  filename    = %s" % filename)
-                note.append("  path        = %s" % self.dest_path)
-                note.append("  message num = %d" % msg_num)
-                note.append("  newsgroup   = %s" % checkpoint.newsgroup)
-                note.append("  file mode   = %o" % self.dest_file_mode)
-                note.append("  path mode   = %o" % self.dest_path_mode)
+                note.append(f"  filename    = {filename}")
+                note.append(f"  path        = {self.dest_path}")
+                note.append(f"  message num = {msg_num}")
+                note.append(f"  newsgroup   = {checkpoint.newsgroup}")
+                note.append(f"  file mode   = {oct(self.dest_file_mode)}")
+                note.append(f"  path mode   = {oct(self.dest_path_mode)}")
                 note.append("")
                 note.append(traceback.format_exc())
 
-                subject = "Archive: problem saving %s" % filename
+                subject = f"Archive: problem saving {filename}"
 
                 self.post_error(subject, note)
 
                 if self.debug:
                     self.log.error("Exiting on error (debug mode on)")
                     raise
-                else:
-                    self.abort("Exiting on error")
-                    break
+
+                self.abort("Exiting on error")
+                break
 
             remove_file(filename)
 
             if self.is_stopped():
                 break
 
     def modify_message(self, message):
+        """Modify message"""
+
         return message
 
     def process_message(self, newsserver, msg_num, checkpoint):
+        """Process message"""
 
         try:
             article = newsserver.article(str(msg_num))[1]
             message = email.message_from_bytes(b"\n".join(article.lines))
         except:
             self.log.exception("    unable to retrieve article body")
             checkpoint.touch_message(msg_num)
@@ -1080,22 +1123,22 @@
         for key in message.keys():
             headers[key] = message[key]
 
         self.replace_header.set_value(headers)
 
         if self.start_time and msg_time < self.start_time:
             self.log.debug(
-                "    rejecting - too old (%s)" % msg_time.strftime(self.time_fmt)
+                "    rejecting - too old (%s)", msg_time.strftime(self.time_fmt)
             )
             checkpoint.reset(msg_time, msg_num)
             return
 
         if self.stop_time and msg_time > self.stop_time:
             self.log.debug(
-                "    rejecting - too new (%s)" % msg_time.strftime(self.time_fmt)
+                "    rejecting - too new (%s)", msg_time.strftime(self.time_fmt)
             )
             checkpoint.reset(msg_time, msg_num)
             return
 
         if self.timegap and (msg_time - checkpoint.last_time) >= self.timegap:
             self.log.info("    time gap between messages exceeds limit")
             if self.report_timegap and checkpoint.is_active():
@@ -1118,15 +1161,14 @@
             filenames = newstool.save_files(message)
         except:
             self.log.exception("    rejecting - unable to parse message body")
             checkpoint.touch_message(msg_num)
             return
 
         if "x-transport-part" in message:
-
             # Assumes that there is only one part attached
 
             part, total = map(int, message["X-Transport-Part"].split("/"))
             srcname = os.path.basename(filenames[0])
             destname = os.path.basename(message["X-Transport-Filename"])
             workdir = os.path.join("work", checkpoint.newsgroup, destname)
             workname = os.path.join(workdir, srcname)
@@ -1135,108 +1177,113 @@
                 os.makedirs(workdir)
 
             shutil.move(srcname, workname)
 
             parts = sorted(glob.glob(os.path.join(workdir, "*")))
 
             if len(parts) == total:
-
-                destfile = open(destname, "w")
-
-                for filepart in parts:
-                    destfile.write(open(filepart).read())
-
-                destfile.close()
+                with Path(destname).open("wb") as destfile:
+                    for filepart in parts:
+                        contents = Path(filepart).read_bytes()
+                        destfile.write(contents)
 
                 remove_file(parts)
                 os.rmdir(workdir)
 
-                self.log.debug("Joined split message: %d parts" % total)
+                self.log.debug("Joined split message: %d parts", total)
 
                 if "x-transport-md5" in message:
                     orgmd5 = message["x-transport-md5"]
-                    newmd5 = md5(open(destname).read()).hexdigest()
+                    newmd5 = md5(Path(destname).read_bytes()).hexdigest()
                     if orgmd5 == newmd5:
                         self.log.debug("  MD5 checksum matches")
                         filenames = [destname]
                     else:
                         subject = "Archive: MD5 mismatch"
 
                         note = []
                         note.append("MD5 mistmatch in file")
-                        note.append("  message ID: %s" % message["Xref"])
-                        note.append("  filename:   %s" % destname)
-                        note.append("  expected:   %s" % orgmd5)
-                        note.append("  found:      %s" % newmd5)
+                        note.append(f"  message ID: {message['Xref']}")
+                        note.append(f"  filename:   {destname}")
+                        note.append(f"  expected:   {orgmd5}")
+                        note.append(f"  found:      {newmd5}")
                         self.post_error(subject, note)
 
                         filenames = []
                 else:
                     self.log.debug("  No MD5 checksum to compare")
                     filenames = [destname]
 
             else:
                 filenames = []
-                self.log.debug("Joining split message: part %d of %d" % (part, total))
+                self.log.debug("Joining split message: part %d of %d", part, total)
 
         goodfiles = self.filter_filenames(filenames)
         self.log.debug(
-            "    message contains %d file(s), saving %d:"
-            % (len(filenames), len(goodfiles))
+            "    message contains %d file(s), saving %d:",
+            len(filenames),
+            len(goodfiles),
         )
         for filename in filenames:
             if filename in goodfiles:
-                self.log.debug("      + %s" % filename)
+                self.log.debug("      + %s", filename)
             else:
-                self.log.debug("      - %s" % filename)
+                self.log.debug("      - %s", filename)
 
         if goodfiles:
             self.process_files(goodfiles, checkpoint, msg_num, msg_time)
             checkpoint.update_message(msg_num, msg_time)
 
         remove_file(filenames)
 
         self.log.debug(
-            "    after writing files, message count=%d, max=%d"
-            % (checkpoint.num_messages, self.max_messages)
+            "    after writing files, message count=%d, max=%d",
+            checkpoint.num_messages,
+            self.max_messages,
         )
 
         if self.max_messages and checkpoint.num_messages >= self.max_messages:
             if self.max_messages > 1:
                 self.log.info("    max message count reached")
             if self.report_max_messages:
                 self.post_report(checkpoint, "Max message count reached")
             if not self.timespan and not self.timegap:
                 checkpoint.reset(msg_time, msg_num)
 
     def process_group(self, newsserver, checkpoint, low_mark, high_mark):
+        """Process newsgroup"""
 
-        self.log.debug("Processing newsgroup: %s" % checkpoint.newsgroup)
+        self.log.debug("Processing newsgroup: %s", checkpoint.newsgroup)
         self.log.debug(
-            "  available message numbers: %d - %d, last processed: %d"
-            % (low_mark, high_mark, checkpoint.last_message)
+            "  available message numbers: %d - %d, last processed: %d",
+            low_mark,
+            high_mark,
+            checkpoint.last_message,
         )
 
         if self.start_current == 1:
             self.log.debug("  catching up")
             checkpoint.reset(last_message=high_mark)
 
         elif self.start_current < 0:
-            lastMsg = max(low_mark - 1, high_mark + self.start_current)
-            lastMsg = max(lastMsg, checkpoint.last_message)
+            last_msg = max(low_mark - 1, high_mark + self.start_current)
+            last_msg = max(last_msg, checkpoint.last_message)
             self.log.debug(
-                "  starting with last %d message(s)" % abs(high_mark - lastMsg)
+                "  starting with last %d message(s)", abs(high_mark - last_msg)
             )
-            checkpoint.reset(last_message=lastMsg)
+            checkpoint.reset(last_message=last_msg)
 
         elif low_mark > high_mark:
             self.log.debug("  no messages on server")
             return
 
-        elif checkpoint.last_message < low_mark - 1 or checkpoint.last_message > high_mark:
+        elif (
+            checkpoint.last_message < low_mark - 1
+            or checkpoint.last_message > high_mark
+        ):
             self.log.info("  message count reset")
             checkpoint.reset(last_message=low_mark - 1)
 
         if checkpoint.last_message == high_mark:
             self.log.debug("  no new messages")
 
             if self.timeout and checkpoint.is_active():
@@ -1247,135 +1294,137 @@
                     checkpoint.reset(last_message=high_mark)
 
                 return
 
         newsserver.group(checkpoint.newsgroup)
 
         for msg_num in range(checkpoint.last_message + 1, high_mark + 1):
-
-            self.log.debug("  processing message %d" % msg_num)
+            self.log.debug("  processing message %d", msg_num)
 
             self.process_message(newsserver, msg_num, checkpoint)
             self.database[checkpoint.newsgroup] = checkpoint
             self.database.sync()
 
             if self.is_stopped():
                 break
 
     def check_groups(self):
+        """Check newsgroups"""
 
         host = self.pollserver_host
         port = self.pollserver_port
 
         with newstool.NewsTool().open_server(host, port) as newsserver:
-
             for newsgroup, low_mark, high_mark in self.get_groups(newsserver):
                 checkpoint = self.database[newsgroup]
                 self.process_group(newsserver, checkpoint, low_mark, high_mark)
                 self.database[newsgroup] = checkpoint
                 self.database.sync()
 
                 if self.is_stopped():
                     break
 
-        if self.start_currentReset:
+        if self.start_current_reset:
             self.start_current = 0
 
     def expire_files(self):
+        """Expire old files"""
 
         self.log.debug("Expiring old files")
 
-        for key in self.database.keys():
-            self.log.debug("  - %s" % key)
-            checkpoint = self.database[key]
+        for key, checkpoint in self.database.items():
+            self.log.debug("  - %s", key)
 
             if len(checkpoint.history) > 0:
-
                 self.log.debug("    checking file history expire times:")
 
-                historyIndex = list(range(len(checkpoint.history)))
-                historyIndex.reverse()
-
-                for index in historyIndex:
+                history_index = list(range(len(checkpoint.history)))
+                history_index.reverse()
 
+                for index in history_index:
                     filenames, lastdate = checkpoint.history[index]
 
                     diff = now() - lastdate
                     expire = diff > self.expire
 
                     self.log.debug(
-                        "      %d: time=%s, diff=%s, expire? %d"
-                        % (index, lastdate, diff, expire)
+                        "      %d: time=%s, diff=%s, expire? %d",
+                        index,
+                        lastdate,
+                        diff,
+                        expire,
                     )
 
                     if expire:
                         for filename in filenames.keys():
                             filename = self.replace_history(filename, index)
-                            self.log.debug("         %s" % filename)
+                            self.log.debug("         %s", filename)
                             try:
                                 os.remove(filename)
                             except:
                                 pass
                         del checkpoint.history[index]
                     else:
                         break
 
             self.database[key] = checkpoint
 
         self.database.sync()
 
     def check_summary(self):
+        """Check if time for summary report"""
 
         if not self.summary_enable:
             return
 
         self.log.debug("Checking summary reporting")
 
-        for key in self.database.keys():
-            self.log.debug("  - %s" % key)
-            checkpoint = self.database[key]
+        for key, checkpoint in self.database.items():
+            self.log.debug("  - %s", key)
 
             secs = checkpoint.summary_start.timestamp()
             interval = self.summary_period.total_seconds()
             offset = self.summary_offset.total_seconds()
 
-            nextTime = (math.floor(secs / interval) + 1) * interval + offset
-            nextTime = datetime.fromtimestamp(nextTime, tz=timezone.utc)
+            next_time = (math.floor(secs / interval) + 1) * interval + offset
+            next_time = datetime.fromtimestamp(next_time, tz=timezone.utc)
 
-            self.log.debug("    - interval = %s" % self.summary_period)
-            self.log.debug("    - offset   = %s" % self.summary_offset)
-            self.log.debug("    - start_time= %s" % checkpoint.summary_start)
-            self.log.debug("    - nextTime = %s" % nextTime)
+            self.log.debug("    - interval = %s", self.summary_period)
+            self.log.debug("    - offset   = %s", self.summary_offset)
+            self.log.debug("    - start_time= %s", checkpoint.summary_start)
+            self.log.debug("    - next_time = %s", next_time)
 
-            if now() >= nextTime:
+            if now() >= next_time:
                 self.log.info("Summary time reached")
                 self.post_summary(checkpoint)
                 checkpoint.reset_summary()
 
             self.database[key] = checkpoint
 
         self.database.sync()
 
     def main(self):
+        """Main application"""
 
-        self.log.info('Starting')
+        self.log.info("Starting")
 
         while self.wait(self.pollrate):
-
             try:
                 self.check_groups()
             except SystemExit:
-                self.log.info('TAV *** SYSTEM EXIT exception')
+                self.log.info("TAV *** SYSTEM EXIT exception")
                 break
             except:
                 note = [traceback.format_exc()]
                 self.post_error("Archive: problem checking groups", note)
 
             self.check_summary()
 
             if self.expire:
                 self.expire_files()
 
-        self.log.info('Finished')
+        self.log.info("Finished")
+
 
 def main():
+    """Script entry point"""
     ArchiveGroups(sys.argv).run()
```

### Comparing `datatransport-3.0.6/src/datatransport/components/DirectoryService.py` & `datatransport-3.0.7/src/datatransport/components/directoryservice.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+"""Directory Service"""
 
 ##########################################################################
 #
 #   Directory Service
 #
 #   The directory is used to return information about the
 #   various services. It is used primarily in bootstraping
@@ -22,64 +23,74 @@
 #
 #   2013-01-30  Todd Valentic
 #               Make sure port has a value.
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #
+#   2023-07-27  Todd Valentic
+#               Updated for transport3 / python3
+#
 ##########################################################################
 
-import os
 import sys
 
 from datatransport import ProcessClient
 from datatransport import ConfigComponent
 from datatransport import XMLRPCServer
 
 
 class Service(ConfigComponent):
+    """Service Component"""
+
     def __init__(self, name, config, parent, **kw):
         ConfigComponent.__init__(self, "service", name, config, parent, **kw)
 
-        self.host = self.get("host", "localhost")
-        self.port = self.get_int("port")
-        self.label = self.get("label")
-        self.url = "http://%s:%s" % (self.host, self.port)
-        self.hold = self.get_boolean("hold", True)
+        self.host = self.config.get("host", "localhost")
+        self.port = self.config.get_int("port")
+        self.scheme = self.config.get("scheme", "http")
+        self.label = self.config.get("label")
+        self.url = f"{self.scheme}://{self.host}:{self.port}"
+        self.hold = self.config.get_boolean("hold", True)
 
         if not self.port:
             raise ValueError("No port specified")
 
 
 class DirectoryService(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
-        port = self.get_int("directory.port", 8411)
+        port = self.config.get_int("directory.port", 8411)
 
-        self.xmlserver = XMLRPCServer(self, 
-            queue_size=100, port=port, label="Directory"
+        self.xmlserver = XMLRPCServer(
+            self, queue_size=100, port=port, label="Directory"
         )
         self.main = self.xmlserver.main
 
         self.xmlserver.register_function(self.list)
         self.xmlserver.register_function(self.lookup, "get")
 
-        self.services = self.get_components("services", factory=Service)
+        self.services = self.config.get_components("services", factory=Service)
 
         self.log.info("Services:")
         for service in self.services.values():
-            self.log.info(f"  - {service.label} ({service.host}:{service.port})")
+            self.log.info("  - %s (%s:%s)", service.label, service.host, service.port)
 
     def list(self):
+        """List services"""
+
         return list(self.services)
 
     def lookup(self, name, key):
+        """Lookup data on service component"""
 
         if name in self.services:
             return getattr(self.services[name], key)
 
-        raise KeyError("Unknown service: %s" % name)
+        raise KeyError(f"Unknown service: {name}")
 
 
 def main():
     DirectoryService(sys.argv).run()
```

### Comparing `datatransport-3.0.6/src/datatransport/components/DiskMonitor.py` & `datatransport-3.0.7/src/datatransport/components/DiskMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/EventMonitor.py` & `datatransport-3.0.7/src/datatransport/components/EventMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/FilePost.py` & `datatransport-3.0.7/src/datatransport/components/FilePost.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/FileStore.py` & `datatransport-3.0.7/src/datatransport/components/FileStore.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/FileWatch.py` & `datatransport-3.0.7/src/datatransport/components/filewatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+#!/usr/bin/env python3
+"""FileWatch component"""
+
+# pylint: disable=broad-exception-caught
+
 ##########################################################################
 #
 #   FileWatch
 #
 #   This transport component script watches for new files to appear in
 #   a specified directory and posts them into a given newsgroup. If the
 #   newsgroup does not exist when the script starts, it will try to
@@ -70,92 +75,90 @@
 #
 #   2022-10-07  Todd Valentic
 #               Python3 port:
 #                   Reorder imports
 #                   removeFile -> remove_file
 #                   NewsPoster
 #
+#   2023-07026  Todd Valentic
+#               Use new config interface
+#
 ##########################################################################
 
-import os
-import glob
 import sys
-import time
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport.utilities import remove_file
 
 
 class FileWatch(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
 
-        self.pollrate = self.get_timedelta("watch.rate", 60)
-        self.remove_files = self.get_boolean("watch.removefiles", True)
-        self.group_files = self.get_boolean("watch.groupfiles", False)
+        self.pollrate = self.config.get_rate("watch.rate", 60)
+        self.remove_files = self.config.get_boolean("watch.removefiles", True)
+        self.group_files = self.config.get_boolean("watch.groupfiles", False)
 
-        path = self.get("watch.path", "")
-        files = self.get("watch.files", "").split()
+        self.watchpath = self.config.get_path("watch.path", ".")
+        self.filespecs = self.config.get_list("watch.files")
 
-        if not files:
+        if not self.filespecs:
             self.abort("No watch files listed in the config file.")
 
-        try:
-            self.watchfiles = [os.path.join(path, file) for file in files]
-        except:
-            self.log.exception("Problem parsing watchfiles list")
-            self.abort("Aborting")
-
-        self.log.info("Posting to %s" % self.get("post.newsgroup"))
-        self.log.info("Watching for: %s" % self.watchfiles)
+        self.log.info("Posting to %s", self.config.get("post.newsgroup"))
+        self.log.info("Watching path: %s", self.watchpath)
+        self.log.info("Watching for: %s", self.filespecs)
 
-    def watch_files(self):
+    def find_files(self):
+        """Find files to post"""
 
         readyfiles = []
 
-        for filespec in self.watchfiles:
-            files = [f for f in glob.glob(filespec) if os.path.isfile(f)]
+        for filespec in self.filespecs:
+            files = [f for f in self.watchpath.glob(filespec) if f.is_file()]
             readyfiles.extend(files)
 
-        readyfiles.sort()
-
-        return readyfiles
+        return sorted(readyfiles)
 
     def process(self):
+        """Process files ready to post"""
 
-        files = self.watch_files()
+        files = self.find_files()
 
         if not files:
             self.log.debug("No files present, sleeping")
             return
 
         if self.group_files:
             files = [files]
 
         for filegroup in files:
-
             try:
-                starttime = time.time()
+                starttime = self.now()
                 self.news_poster.post(filegroup)
-                elapsed = time.time() - starttime
-                self.log.info("Files posted (%.2f s): %s" % (elapsed, filegroup))
-            except:
+                elapsed = self.now() - starttime
+                self.log.info("Files posted (%s): %s", elapsed, filegroup)
+            except Exception:
                 self.log.exception("Problem posting files")
                 return
 
             if self.remove_files:
                 try:
                     remove_file(filegroup)
-                except:
-                    self.log.exception("Problem deleting file: %s" % filegroup)
+                except Exception:
+                    self.log.exception("Problem deleting file: %s", filegroup)
 
     def main(self):
+        """Main application"""
 
         while self.wait(self.pollrate):
             self.process()
 
 
 def main():
+    """Script entry"""
     FileWatch(sys.argv).run()
```

### Comparing `datatransport-3.0.6/src/datatransport/components/GroupControl.py` & `datatransport-3.0.7/src/datatransport/components/GroupControl.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #               Python3 migration:
 #                   exception handling
 #                   NewsPoller, NewsPoster
 #
+#   2023-07-28  Todd Valentic
+#               Updated for transport3 / python3
+#
 ###########################################################################
 
 import os
 import socket
 import sys
 
 from datatransport import ProcessClient
@@ -84,16 +87,16 @@
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
         self.news_poller = NewsPoller(self, callback=self.process)
         self.main = self.news_poller.main
 
-        self.prefix = self.get("prefix", "")
-        self.postfix = self.get("postfix", "")
+        self.prefix = self.config.get("prefix", "")
+        self.postfix = self.config.get("postfix", "")
 
         self.connect()
 
     def connect(self):
 
         self.log.info("Connecting to transport server")
```

### Comparing `datatransport-3.0.6/src/datatransport/components/InstrumentStatus.py` & `datatransport-3.0.7/src/datatransport/components/InstrumentStatus.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/NewsGateway.py` & `datatransport-3.0.7/src/datatransport/components/NewsGateway.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+"""Newsgroup Gateway Component"""
 
 #########################################################################
 #
 #   News group gateway service
 #
 #   This service provides an XML-RPC gateway to news groups.
 #   The contents of the latest available message in a group
@@ -17,14 +18,17 @@
 #   2009-11-24  Todd Valentic
 #               Use currentTime instead of datetime.now()
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #               NewsPoller
 #
+#   2023-07-26  Todd Valentic
+#               Updated for transport3 / python3
+#
 #########################################################################
 
 import pickle
 import shelve
 import sys
 
 from threading import Thread, Lock
@@ -34,67 +38,85 @@
 from datatransport import ProcessClient
 from datatransport import XMLRPCServerMixin
 from datatransport import NewsPoller
 from datatransport import AccessMixin
 
 
 def synchronized(lock):
+    """Lock decorator"""
+
     def wrap(f):
         def new_function(*args, **kw):
             lock.acquire()
             try:
                 return f(*args, **kw)
             finally:
                 lock.release()
 
         return new_function
 
     return wrap
 
 
 class Data(AccessMixin):
+    """Data cache"""
 
     lock = Lock()
 
     def __init__(self, parent):
         AccessMixin.__init__(self, parent)
         self.messages = shelve.open("cache")
 
     @synchronized(lock)
     def write(self, message):
+        """Store message into cache"""
+
         newsgroup = message["Newsgroups"]
         self.messages[newsgroup] = self.write_handler(newsgroup, message)
         self.messages.sync()
 
     def write_handler(self, newsgroup, message):
+        """What to cache"""
         return message
 
     @synchronized(lock)
     def clear(self):
+        """Clear the cache"""
+
         self.messages.clear()
         self.messages.sync()
 
     @synchronized(lock)
     def read(self, newsgroup):
-        return self.messages[newsgroup]
+        """Read entry from cache"""
+     
+     return self.messages[newsgroup]
 
     @synchronized(lock)
     def list(self):
-        return self.messages.keys()
+        """List cache"""
+      
+      return self.messages.keys()
 
     @synchronized(lock)
     def get_string(self, newsgroup):
-        return self.messages[newsgroup].as_string()
+        """Reture message as string"""
+       
+       return self.messages[newsgroup].as_string()
 
     @synchronized(lock)
     def unpickle(self, newsgroup):
+        """Unpickle message"""
+        
         return pickle.loads(self.messages[newsgroup].get_payload())
 
 
 class Server(Thread, AccessMixin):
+    """XMLRPC Server Interface"""
+
     def __init__(self, parent, data):
         Thread.__init__(self)
         AccessMixin.__init__(self, parent)
 
         self.xmlserver = XMLRPCServerMixin(self)
         self.main = self.xmlserver.main
 
@@ -106,57 +128,65 @@
         self.xmlserver.register_function(self.data.unpickle, "unpickle")
         self.xmlserver.register_function(self.data.list, "list")
         self.xmlserver.register_function(self.data.get_string, "message")
 
         self.add_handlers()
 
     def add_handlers(self):
+        """Used by derived classes to add handlers"""
         return
 
     def read(self, newsgroup):
+        """Read message from newsgroup"""
+
         message = self.data.read(newsgroup)
         headers = {}
         for key, value in message.items():
             headers[key] = value
         return {"headers": headers, "body": message.get_payload()}
 
 
 class NewsGateway(ProcessClient):
+    """Process Client"""
+
     def __init__(self, dataFactory, serverFactory, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poller = NewsPoller(self, callback=self.process, idle=self.idle)
         self.main = self.news_poller.main
 
         self.data = dataFactory(self)
-        self.timeout = self.get_timedelta("timeout")
+        self.timeout = self.config.get_timedelta("timeout")
         self.in_timeout = False
 
         if self.timeout:
-            self.log.info("Timeout set to %s" % self.timeout)
-            self.next_time = self.current_time() + self.timeout
+            self.log.info("Timeout set to %s", self.timeout)
+            self.next_time = self.now() + self.timeout
         else:
             self.log.info("No timeout set")
 
         serverFactory(self, self.data).start()
 
     def process(self, message):
-        self.log.info("Set from %s" % message["Newsgroups"])
+        """Process handler"""
+
+        self.log.info("Set from %s", message["Newsgroups"])
         self.data.write(message)
 
         if self.timeout:
-            self.next_time = self.current_time() + self.timeout
+            self.next_time = self.now() + self.timeout
             self.in_timeout = False
 
     def idle(self):
+        """Idle handler"""
 
         if self.in_timeout:
             return
 
-        if self.timeout and self.current_time() > self.next_time:
+        if self.timeout and self.now() > self.next_time:
             self.log.info("timeout reached, clearing values")
             self.data.clear()
             self.in_timeout = True
 
 
 def main():
     NewsGateway(Data, Server, sys.argv).run()
```

### Comparing `datatransport-3.0.6/src/datatransport/components/NewsgroupMonitor.py` & `datatransport-3.0.7/src/datatransport/components/NewsgroupMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/PageKit.py` & `datatransport-3.0.7/src/datatransport/components/PageKit.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/PlotTool.py` & `datatransport-3.0.7/src/datatransport/components/PlotTool.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/PostDataFiles.py` & `datatransport-3.0.7/src/datatransport/components/PostDataFiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+"""Post data files component"""
+
 ############################################################################
 #
 #   PostDataFiles
 #
 #   This script watches for new radar data files to appear and posts them
 #   to the newsserver. There is an option not to remove the original file
 #   under the assumption that someone else will in the future. It can also
@@ -110,32 +113,35 @@
 #           Fix bug when timestamp file not present.
 #           Changed a number of config parameters to booleans
 #
 #   2006-10-14  Todd Valentic
 #               Convert headers in post to a dict from a list
 #
 #   2009-11-24  Todd Valentic
-#               Use current_time()
+#               Use now()
 #
 #   2015-11-23  Todd Valentic
 #               Add md5 checksum header.
 #
 #   2015-11-30  Todd Valentic
 #               Use get_rate() for pollrate
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #               Use get_ config methods
 #               Python3 updates:
 #                   commands -> subprocess
 #                   removeFile -> remove_file
 #                   sizeDesc -> size_desc
-#                   currentTime -> current_time
+#                   currentTime -> now
 #                   NewsPoster
 #
+#   2023-07-26  Todd Valentic
+#               Updated for transport3 / python3 
+#
 ############################################################################
 
 import bz2
 import glob
 import math
 import os
 import subprocess
@@ -146,42 +152,44 @@
 
 from datatransport import ProcessClient
 from datatransport import NewsPoster
 from datatransport.utilities import size_desc
 
 
 class PostDataFiles(ProcessClient):
+    """Process Client"""
+
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
 
         self.input_name = self.get("input.name", "*.DAT")
         self.input_path = self.get("input.path", ".")
         self.include_current = self.get_boolean("include_current", False)
-        self.compress = self.get_boolean("compress", 1)
+        self.compress = self.get_boolean("compress", True)
         self.remove_files = self.get_boolean("remove_files", False)
-        self.max_files = self.get_int("max_files", None)
+        self.max_files = self.get_int("max_files")
         self.max_size = self.get_bytes("max_size", "20Mb")
         self.check_index = self.get_boolean("check_index", True)
         self.check_size = self.get_boolean("check_size", True)
 
-        self.pollrate = self.get_rate("pollrate", "5:00")
+        self.pollrate = self.get_rate("pollrate", "5")
         self.filedate = self.get_callback("filedate", self.filedate_callback)
 
         self.timefile = "timestamp"
         self.indexfile = "index"
 
         if not os.path.isfile(self.timefile):
             # Default to sometime long ago
             open(self.timefile, "w").write("0")
             t = time.mktime((1975, 1, 1, 0, 0, 0, 0, 0, 0))
             os.utime(self.timefile, (t, t))
 
-        if self.get_boolean("startCurrent", 0) == 1:
+        if self.get_boolean("startCurrent", False) == 1:
             os.utime(self.timefile, None)
 
         if not os.path.isfile(self.indexfile):
             open(self.indexfile, "w").write("0")
 
         self.log.info("Input path: %s" % self.input_path)
         self.log.info("Input name: %s" % self.input_name)
@@ -198,38 +206,38 @@
 
         numchunks = int(math.ceil(filesize / float(self.max_size)))
         chunks = []
         file = open(filename, "rb")
 
         for chunk in range(numchunks):
             data = file.read(self.max_size)
-            chunkname = "chunk.%03d" % chunk
+            chunkname = f"chunk.{chunk:03d}"
             open(chunkname, "wb").write(data)
             chunks.append(chunkname)
 
         self.log.info("  - split into %d parts" % numchunks)
 
         return chunks
 
-    def get_checksumg(self, filename):
+    def get_checksum(self, filename):
         # Shell out - some files might be quite large
         status, output = subprocess.getstatusoutput("md5sum %s" % filename)
 
         if status != 0:
             return None
 
         return output.split()[0]
 
     def post(self, filename, timestamp):
 
         files = self.split(filename)
         part = 1
         numparts = len(files)
         basename = os.path.basename(filename)
-        checksum = self.get_checksumg(filename)
+        checksum = self.get_checksum(filename)
 
         for file in files:
 
             headers = {}
             if numparts > 1:
                 headers["X-Transport-Part"] = "%d/%d" % (part, numparts)
                 headers["X-Transport-Filename"] = basename
@@ -279,29 +287,29 @@
                 self.log.debug("  - file date: %s" % date)
         except:
             self.log.exception("Error calling routine to determine file date")
             return
 
         if self.compress and not isCompressed:
 
-            starttime = self.current_time()
+            starttime = self.now()
 
             self.log.debug("  - compressing file")
             data = open(file).read()
             open(zipname, "w").write(bz2.compress(data))
 
             orgsize = os.path.getsize(file)
             zipsize = os.path.getsize(zipname)
 
             if orgsize > 0:
                 zippct = (zipsize / float(orgsize)) * 100
             else:
                 zippct = 0
 
-            totaltime = self.current_time() - starttime
+            totaltime = self.now() - starttime
             self.log.info(
                 "  - %s -> %s (%d%%) %s"
                 % (size_desc(orgsize), size_desc(zipsize), zippct, totaltime)
             )
 
             postfile = zipname
```

### Comparing `datatransport-3.0.6/src/datatransport/components/RealTimeFeed.py` & `datatransport-3.0.7/src/datatransport/components/RealTimeFeed.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/ResourceMonitor.py` & `datatransport-3.0.7/src/datatransport/components/ResourceMonitor.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/Scheduler.py` & `datatransport-3.0.7/src/datatransport/components/Scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,28 +57,31 @@
 #
 #   2009-11-24  Todd Valentic
 #               Use currentTime()
 #
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #
+#   2023-07-26  Todd Valentic
+#               Updated for transport3 / python3
+#
 #############################################################################
 
 import datetime
 import sys
 
 from datatransport import ProcessClient
 from datatransprot import ConfigComponent
 from datatransport.utilities import datefunc
 
 
 class Event(ConfigComponent):
     def __init__(self, name, parent):
         ConfigComponent.__init__(self, "event", name, parent)
-        self.startearly = self.get_boolean("startearly", False)
+        self.startearly = self.config.get_boolean("startearly", False)
 
     def __getrunning(self):
         return self.parent.running
 
     running = property(__getrunning)
 
     def start(self):
@@ -91,24 +94,24 @@
         pass
 
 
 class Scheduler(ProcessClient):
     def __init__(self, argv, EventFactory):
         ProcessClient.__init__(self, argv)
 
-        self.rate = self.get_timedelta("repeat.rate", ":60")
-        self.offset = self.get_timedelta("repeat.offset")
-        self.sync = self.get_boolean("repeat.sync", True)
-        self.whole = self.get_boolean("repeat.whole", False)
-        self.exit_on_error = self.get_boolean("exitOnError", False)
+        self.rate = self.config.get_timedelta("repeat.rate", 60)
+        self.offset = self.config.get_timedelta("repeat.offset")
+        self.sync = self.config.get_boolean("repeat.sync", True)
+        self.whole = self.config.get_boolean("repeat.whole", False)
+        self.exit_on_error = self.config.get_boolean("exitOnError", False)
 
         self.events = {}
         self.schedule = []
 
-        for entry in self.get("repeat.events").split("\n"):
+        for entry in self.config.get("repeat.events").split("\n"):
 
             try:
                 start, duration, name = entry.split("|")
 
                 start = datefunc.parse_timedelta(start)
                 duration = datefunc.parse_timedelta(duration)
                 name = name.strip()
@@ -133,16 +136,16 @@
             self.log.info("  %s: %s - %s" % (name, start, start + duration))
 
     def waituntil(self, starttime):
 
         # Sometimes small rounding errors creep in, so spin
         # around until we are really at the target time
 
-        while self.current_time() < starttime:
-            if not self.wait(starttime - self.current_time()):
+        while self.now() < starttime:
+            if not self.wait(starttime - self.now()):
                 return False
 
         return True
 
     def main(self):
 
         for event in self.events.values():
@@ -154,15 +157,15 @@
             self.log.info("Waiting to sync whole event sequence")
             self.wait(self.rate, self.offset, self.sync)
         else:
             self.log.info("Starting in middle of event sequence")
 
         while not error and self.is_running():
 
-            basetime = self.current_time()
+            basetime = self.now()
 
             if self.sync:
                 rate = self.rate.total_seconds()
                 inset = datetime.timedelta(seconds=basetime.timestamp() % rate)
                 basetime = basetime - inset + self.offset
 
             self.log.info("---- Starting event cycle ----")
@@ -178,15 +181,15 @@
 
                 if not event.startearly:
                     if not self.waituntil(starttime):
                         break
 
                 self.log.info("Processing %s" % name)
 
-                if self.current_time() >= endtime:
+                if self.now() >= endtime:
                     self.log.info("  past end time, skipping")
                     continue
 
                 try:
                     event.run(endtime)
                 except:
                     self.log.exception("Problem running event")
```

### Comparing `datatransport-3.0.6/src/datatransport/components/SyncPoller.py` & `datatransport-3.0.7/src/datatransport/components/SyncPoller.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/components/WatchURL.py` & `datatransport-3.0.7/src/datatransport/components/WatchURL.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+"""WatchURL Component"""
+
 #####################################################################
 #
 #   WatchURL
 #
 #   This script watches a URL (which, for example, can be a web
 #   page or an image) and posts it to the specified newsgroup when
 #   a new version appears.
@@ -63,14 +66,17 @@
 #                   commands -> subprocess
 #                   <> -> !=
 #                   htmllib -> html.parser
 #                   urlparse -> urllib.parse
 #                   removeFile -> remove_file
 #                   NewsPoster
 #
+#   2023-07-26  Todd Valentic
+#               Updated for transport3 / python3
+#
 #####################################################################
 
 import datetime
 import fnmatch
 import os
 import socket
 import subprocess
@@ -142,49 +148,47 @@
 
 class WatchURL(ProcessClient):
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
         self.news_poster = NewsPoster(self)
 
-        self.pollrate = self.get_timedelta("pollrate", 600).seconds
-        self.sync = self.get_boolean("pollrate.sync", False)
-        self.offset = self.get_timedelta("pollrate.offset", 0).seconds
-        self.retryrate = self.get_timedelta("retryrate", 60).seconds
-        self.timeout = self.get_timedelta("timeout", 60).seconds
-
-        self.url = self.get("url", None)
-        self.include_names = self.get("images", "*").split()
-        self.exclude_names = self.get("images.exclude", "").split()
-        self.check_headers = self.get_boolean("headers.enable", True)
-        self.exclude_headers = self.get("headers.exclude", "Date").split()
-        self.rename_rules = self.get("rename", "[]")
-        self.save_body = self.get_boolean("save.body", True)
-        self.save_images = self.get_boolean("save.images", False)
-        self.save_thumbnails = self.get_boolean("save.thumbnails", False)
-        self.thumbnail_cmd = self.get(
+        self.pollrate = self.config.get_rate("pollrate", '10m')
+        self.retryrate = self.config.get_rate("retryrate", 60)
+        self.timeout = self.config.get_timedelta("timeout", 60)
+
+        self.url = self.config.get("url", None)
+        self.include_names = self.config.get_list("images", "*")
+        self.exclude_names = self.config.get_list("images.exclude", "")
+        self.check_headers = self.config.get_boolean("headers.enable", True)
+        self.exclude_headers = self.config.get_list("headers.exclude", "Date")
+        self.rename_rules = self.config.get("rename", "[]")
+        self.save_body = self.config.get_boolean("save.body", True)
+        self.save_images = self.config.get_boolean("save.images", False)
+        self.save_thumbnails = self.config.get_boolean("save.thumbnails", False)
+        self.thumbnail_cmd = self.config.get(
             "thumbnails.cmd", "convert -geometry 125x125 -sharpen 2x2"
         )
-        self.thumbnail_exts = self.get("thumbnails.ext", ".jpg .png .gif").split()
-        self.thumbnail_name = self.get("thumbnails.name", "%s-thumbnail.jpg")
+        self.thumbnail_exts = self.config.get_list("thumbnails.ext", ".jpg .png .gif")
+        self.thumbnail_name = self.config.get("thumbnails.name", "%s-thumbnail.jpg")
 
-        socket.setdefaulttimeout(self.timeout)
+        socket.setdefaulttimeout(self.timeout.total_seconds())
 
         try:
             self.rename_rules = eval(self.rename_rules)
         except:
             self.log.exception("Problem parsing the rename rules:")
             self.abort("Aborting")
 
         if self.url is None:
             self.abort("No URL specified")
 
         scheme = urlparse(self.url)[0]
 
-        if self.save_images and scheme != "http":
+        if self.save_images and not scheme.startswith("http"):
             self.abort("Can only save images from http sites")
 
         self.parser = Parser(self.include_names, self.exclude_names)
 
     def gather_urls(self):
 
         urls = []
@@ -267,15 +271,15 @@
             self.log.debug("  files are the same")
             return 0
 
     def remap(self, filename):
 
         for pattern, result in self.rename_rules:
             if fnmatch.fnmatch(filename, pattern):
-                return self.current_time().strftime(result)
+                return self.now().strftime(result)
 
         return filename
 
     def retrieve_files(self, urls):
 
         filenames = []
         unknownext = 0
@@ -325,40 +329,37 @@
                     self.log.error("Problem running thumbnail command: %s" % cmd)
                     self.log.error("Output: %s" % output)
 
         return thumbnails
 
     def main(self):
 
-        if self.sync:
-            self.wait(self.pollrate, sync=True, offset=self.offset)
+        self.wait(self.pollrate)
 
         while self.is_running():
 
             try:
                 urls = self.gather_urls()
             except:
-                self.log.error("Problem gathering URLs")
-                self.log.exception("Traceback:")
+                self.log.exception("Problem gathering URLs")
                 self.wait(self.retryrate)
                 continue
 
             if not urls:
                 self.log.debug("No urls to check")
-                self.wait(self.pollrate, sync=self.sync, offset=self.offset)
+                self.wait(self.pollrate)
                 continue
 
             try:
                 if self.check_headers and not self.headers_changed(urls):
                     self.log.debug("The headers have not changed")
-                    self.wait(self.pollrate, sync=self.sync, offset=self.offset)
+                    self.wait(self.pollrate)
                     continue
             except:
-                self.log.error("Problem checking headers")
-                self.log.exception("Traceback:")
+                self.log.exception("Problem checking headers")
                 self.wait(self.retryrate)
                 continue
 
             filenames, checksum = self.retrieve_files(urls)
 
             if self.files_changed(checksum):
                 if self.save_thumbnails:
@@ -366,22 +367,22 @@
                         filenames.extend(self.make_thumbnails(filenames))
                     except:
                         self.log.exception("Problem making thumbnails")
 
                 if filenames:
                     try:
                         self.news_poster.post(filenames)
-                        self.log.info("New files detected, posting %s" % filenames)
+                        self.log.info("New files detected, posting %s", filenames)
                     except:
                         self.log.exception("Error posting to the news server")
                 else:
                     self.log.info(
                         "Strange, filenames detected, but none listed for posting..."
                     )
 
             remove_file(filenames)
 
-            self.wait(self.pollrate, sync=self.sync, offset=self.offset)
+            self.wait(self.pollrate)
 
 
 def main():
     WatchURL(sys.argv).run()
```

### Comparing `datatransport-3.0.6/src/datatransport/components/__init__.py` & `datatransport-3.0.7/src/datatransport/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .ArchiveGroups	    import ArchiveGroups
-from .DirectoryService  import DirectoryService
+from .archivegroups	    import ArchiveGroups
+from .directoryservice  import DirectoryService
 from .DiskMonitor	    import DiskMonitor
-from .FileWatch         import FileWatch
+from .filewatch         import FileWatch
 from .FilePost          import FilePost
 from .FileStore         import FileStore
 from .GroupControl	    import GroupControl
 from .InstrumentStatus	import InstrumentStatus
 from .NewsgroupMonitor  import NewsgroupMonitor
 from .PlotTool          import PlotTool
 from .PostDataFiles	    import PostDataFiles
```

### Comparing `datatransport-3.0.6/src/datatransport/configcomponent.py` & `datatransport-3.0.7/src/datatransport/configcomponent.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #   DataTransport version of the Sapphire ConfigComponent.
 #
 #   2023-06-28  Todd Valentic
 #               Initial implementation. Based on transport v2 version.
 #
 ##########################################################################
 
-import functools
+from functools import partial
 from .accessmixin import AccessMixin
 
 import sapphire_config as sapphire
 
 
 class ComponentLog:
     """Prefix log entries with the component name"""
@@ -36,14 +36,12 @@
 class ConfigComponent(sapphire.Component, AccessMixin):
     """Component class for config file entries"""
 
     # pylint: disable=too-many-arguments
 
     def __init__(self, prefix, name, config, parent, **kw):
         sapphire.Component.__init__(self, prefix, name, config, parent, **kw)
-        AccessMixin.__init__(self, parent, getters=False)
+        AccessMixin.__init__(self, parent)
 
         self.log = ComponentLog(f"{prefix}.{name}", parent.log)
 
-        setattr(
-            self, "get_components", functools.partial(self.get_components, parent=self)
-        )
+        self.config.get_components = partial(self.config.get_components, parent=self)
```

### Comparing `datatransport-3.0.6/src/datatransport/directory.py` & `datatransport-3.0.7/src/datatransport/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class Directory:
     """Add methods to connect to the XMLRPC directory service"""
 
     def __init__(self, parent):
         self.parent = parent
 
-        url = parent.get("directory.url")
+        url = parent.config.get("directory.url")
         kwargs = {"allow_none": True, "use_builtin_types": True}
         self.directory = xmlrpc.client.ServerProxy(url, **kwargs)
 
         # Wait for the directory service to become ready
 
         self._waiton(self.directory, "directory")
```

### Comparing `datatransport-3.0.6/src/datatransport/newspoller.py` & `datatransport-3.0.7/src/datatransport/newspoller.py`

 * *Files 9% similar despite different names*

```diff
@@ -131,167 +131,183 @@
 #   2022-10-19  Todd Valentic
 #               Remove deprecated idleFunc
 #               Port to transport3 / python3
 #
 #   2023-07-04  Todd Valentic
 #               Convert from being a mixin class
 #
+#   2023-07-27  Todd Valentic
+#               Use AccessMixin
+#
 ###########################################################################
 
 from datatransport import newstool
+from datatransport import AccessMixin
 
 
-class NewsPoller:
+class NewsPoller(AccessMixin):
     """News poller"""
 
     def __init__(self, parent, prefix="poll", callback=None, idle=None):
-        self.parent = parent
+        AccessMixin.__init__(self, parent)
+
         self.prefix = prefix
         self.idle = idle
-        self.rate = parent.get_rate(f"{prefix}.rate", 60)
+        self.rate = self.config.get_rate(f"{prefix}.rate", 60)
 
-        self.news_pollers = self._create_pollers(parent, prefix, callback)
+        self.news_pollers = self.create_pollers(prefix, callback)
 
     # pylint: disable=inconsistent-return-statements
-    def _connect_to_server(self, parent, host, port):
+    def connect_to_server(self, host, port):
+        """Open a connection to the news server"""
+
         server = newstool.NewsTool()
         server.set_server(host, port)
 
-        while parent.is_running():
+        while self.is_running():
             try:
                 server.open_server()
                 return server
             except:  # pylint: disable=bare-except
-                parent.log.exception(f"Failed to connect to {host}:{port}")
-                parent.wait(15)
+                self.log.exception(f"Failed to connect to {host}:{port}")
+                self.wait(15)
 
-        parent.abort("Exiting")
+        self.abort("Exiting")
 
-    def _get_newsgoups(self, parent, prefix, server):
-        targetgroup = parent.get(f"{prefix}.newsgroup", "")
-        targetgroups = parent.get_list(f"{prefix}.newsgroups", targetgroup)
-        excludegroup = parent.get(f"{prefix}.newsgroup.exclude", "")
-        excludegroups = parent.get_list(f"{prefix}.newsgroups.exclude", excludegroup)
+    def get_newsgoups(self, prefix, server):
+        """Get a list of newsgroups"""
+
+        targetgroup = self.config.get(f"{prefix}.newsgroup", "")
+        targetgroups = self.config.get_list(f"{prefix}.newsgroups", targetgroup)
+        excludegroup = self.config.get(f"{prefix}.newsgroup.exclude", "")
+        excludegroups = self.config.get_list(f"{prefix}.newsgroups.exclude", excludegroup)
 
         newsgroups = []
 
         for groupspec in targetgroups:
             if "*" in groupspec or "?" in groupspec:
                 try:
                     matches = server.list_newsgroups(groupspec, excludegroups)
                     newsgroups.extend(matches)
                 except:  # pylint: disable=bare-except
-                    parent.log.info(f"Problem matching '{groupspec}'")
+                    self.log.info(f"Problem matching '{groupspec}'")
                     continue
             else:
                 newsgroups.append(groupspec)
 
         return newsgroups
 
-    def _create_pollers(self, parent, prefix, callback):
-        host = parent.get(f"{prefix}.newsserver", "localhost")
-        port = parent.get_int(f"{prefix}.newsserver.port", 119)
+    def create_pollers(self, prefix, callback):
+        """Create a news poller for each newsgroup"""
+
+        host = self.config.get(f"{prefix}.newsserver", "localhost")
+        port = self.config.get_int(f"{prefix}.newsserver.port", 119)
 
-        exit_on_error = parent.get_boolean(f"{prefix}.exit_on_error", False)
-        retry_wait = parent.get_timedelta(f"{prefix}.retry_wait", 60)
+        exit_on_error = self.config.get_boolean(f"{prefix}.exit_on_error", False)
+        retry_wait = self.config.get_timedelta(f"{prefix}.retry_wait", 60)
 
         # Prefix the tracking file when used in ConfigComponent
         # because we might have multiple references to the same group
 
-        if hasattr(parent, "prefix") and hasattr(parent, "name"):
-            last_read_prefix = f"{parent.prefix}-{parent.name}"
+        if hasattr(self.parent, "prefix") and hasattr(self.parent, "name"):
+            last_read_prefix = f"{self.parent.prefix}-{self.parent.name}"
         else:
             last_read_prefix = ""
 
-        server = self._connect_to_server(parent, host, port)
-        newsgroups = self._get_newsgoups(parent, prefix, server)
+        server = self.connect_to_server(host, port)
+        newsgroups = self.get_newsgoups(prefix, server)
 
-        parent.log.debug("Creating news pollers:")
+        self.log.debug("Creating news pollers:")
 
         pollers = []
 
         for newsgroup in newsgroups:
             poller = newstool.NewsPoller()
             poller.set_server(host, port)
             poller.set_newsgroup(newsgroup)
-            poller.set_log(parent.log)
+            poller.set_log(self.log)
             poller.set_callback(callback)
-            poller.set_stop_func(parent.is_stopped)
+            poller.set_stop_func(self.is_stopped)
             poller.set_retry_wait(retry_wait.total_seconds())
             poller.set_debug(exit_on_error)
             poller.set_last_read_prefix(last_read_prefix)
 
             pollers.append(poller)
 
-            parent.log.debug(f" - {newsgroup}")
+            self.log.debug(" - [%s:%s] %s", host, port, newsgroup)
 
         return pollers
 
-    def _run_pollers(self, catchup, reset):
+    def run_pollers(self, catchup, reset):
+        """Run each poller"""
+
         for poller in self.news_pollers:
             if reset and catchup != 0:
                 poller.mark_read(catchup, reset=reset)
 
             poller.poll()
 
-    def _run_idle(self):
-        if self.idle and self.parent.is_running():
+    def run_idle(self):
+        """Run the idle handler"""
+
+        if self.idle and self.is_running():
             self.idle()
 
-    def _mark_read(self, catchup, reset):
+    def mark_read(self, catchup, reset):
+        """Mark each newsgroup as read"""
+
         for poller in self.news_pollers:
             while not poller.has_newsgroup():
-                self.parent.log.error(
+                self.self.log.error(
                     f"The polling group ({poller.newsgroup_header}) "
                     f"does not exist on "
                     f"{poller.server_host}:{poller.server_port}, "
                     f"waiting 60 seconds ..."
                 )
-                if not self.parent.wait(60):
+                if not self.wait(60):
                     return
 
             if catchup != 0:
                 poller.mark_read(catchup, reset)
 
-    def _loop(self):
-        parent = self.parent
-        prefix = self.prefix
-
-        catchup = parent.get_int(f"{prefix}.catchup", 0)
-        catchup_reset = parent.get_boolean(f"{prefix}.catchup.reset", False)
-        exit_on_error = parent.get_boolean(f"{prefix}.exit_on_error", False)
+    def process(self):
+        """Process messages"""
+
+        catchup = self.config.get_int(f"{self.prefix}.catchup", 0)
+        catchup_reset = self.config.get_boolean(f"{self.prefix}.catchup.reset", False)
+        exit_on_error = self.config.get_boolean(f"{self.prefix}.exit_on_error", False)
 
         if catchup == 0:
-            parent.log.debug("Starting with first article in last read file")
+            self.log.debug("Starting with first article in last read file")
         else:
-            self._mark_read(catchup, catchup_reset)
+            self.mark_read(catchup, catchup_reset)
 
-        while parent.is_running():
+        while self.is_running():
             try:
-                self._run_pollers(catchup, catchup_reset)
+                self.run_pollers(catchup, catchup_reset)
             except:  # pylint: disable=bare-except
-                parent.log.exception("Error detected during polling")
+                self.log.exception("Error detected during polling")
                 if exit_on_error:
-                    parent.abort("Exiting on error")
+                    self.abort("Exiting on error")
 
             try:
-                self._run_idle()
+                self.run_idle()
             except:  # pylint: disable=bare-except
-                parent.log.exception("Error detected during idle")
+                self.log.exception("Error detected during idle")
                 if exit_on_error:
-                    parent.abort("Exiting on error")
+                    self.abort("Exiting on error")
 
             yield 1
 
     def main(self):
         """Main loop"""
 
-        if not self.parent.wait(self.rate):
+        if not self.wait(self.rate):
             return
 
-        for _step in self._loop():
-            self.parent.wait(self.rate)
+        for _step in self.process():
+            self.wait(self.rate)
 
     def run_step(self):
         """Run one step in main loop"""
 
-        next(self._loop())
+        next(self.process())
```

### Comparing `datatransport-3.0.6/src/datatransport/newstool.py` & `datatransport-3.0.7/src/datatransport/newstool.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,17 +339,21 @@
 #                   setTimeout - set_timeout
 #                   openServer -> open_server
 #                   groupExists -> group_exists
 #                   datetime - > get_datetime
 #                   listArticles -> list_articles
 #                   listGroups -> list_newsgroups
 #
+#   2023-07-26  Todd Valentic
+#               Support pathlib in poster
+#
 #
 ###########################################################################
 
+import collections
 import datetime
 import email
 import logging
 import mimetypes
 import nntplib
 import pathlib
 import time
@@ -519,16 +523,16 @@
 
     def open_server(self, host=None, port=119):
         """Initialize instance"""
 
         if host:
             self.set_server(host, port)
 
-        return nntplib.NNTP(host, 
-                            port=port, 
+        return nntplib.NNTP(self.server_host, 
+                            port=self.server_port, 
                             readermode=True, 
                             timeout=self.timeout)
 
     def has_newsgroup(self, newsgroup=None):
         """Check if newsgroup exists"""
 
         if not newsgroup:
@@ -704,16 +708,19 @@
         part.add_header("Content-Disposition", "attachment", filename=basename)
 
         msg.attach(part)
 
     def post(self, filenames=None, comment=None, date=None, headers=None):
         """Post files to newsgroup"""
 
-        if isinstance(filenames, str):
-            filenames = [filenames]
+        if filenames is not None:
+            if isinstance(filenames, str):
+                filenames = [filenames]
+            elif not isinstance(filenames, collections.abc.Iterable): 
+                filenames = [filenames]
 
         if not filenames:
             msg = MIMEText(comment)
         else:
             msg = MIMEMultipart()
             msg.preable = comment
 
@@ -976,16 +983,19 @@
 
     def get_next_message(self):
         """Get the next message from the newsgroup"""
 
         try:
             server = self.open_server()
             _resp, count, low, high, name = server.group(self.newsgroup_header)
-        except:  # pylint: disable=bare-except
-            self.log.debug("Failed to get message numbers")
+        except nntplib.NNTPError as e:
+            self.log.debug("Failed to get message numbers: %s", e)
+            return None
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            self.log.debug("Failed to get message numbers: %s", e)
             return None
 
         self.log.debug(f"Group {name} has {count} articles from {low} to {high}")
 
         try:
             lastid = self.load_last_read()
             self.log.debug(f"  last message read was {lastid}")
```

### Comparing `datatransport-3.0.6/src/datatransport/processclient.py` & `datatransport-3.0.7/src/datatransport/processclient.py`

 * *Files 9% similar despite different names*

```diff
@@ -160,29 +160,34 @@
 #               Make running a property
 #               Convert API to snake case naming
 #                   CurrentTime -> current_time
 #
 #   2023-07-09  Todd Valentic
 #               Use TransportConfig find_config_files()
 #
+#   2023-07-25  Todd Valentic
+#               Add set() and options() to config proxy
+#               Do not map getters from config, use config object               
+#               current_time() renamed to now()
+#
 ###########################################################################
 
 import atexit
 import datetime
 import fnmatch
-import functools
 import glob
 import logging
 import os
 import signal
 import sys
 import threading
 import time
 import xmlrpc.client
 
+from functools import partial
 from logging.handlers import RotatingFileHandler
 from logging.handlers import SocketHandler
 
 import sapphire_config as sapphire
 
 from . import Root
 from . import TransportConfig
@@ -255,61 +260,61 @@
             for proc in self.subprocs:
                 if proc.poll() is None:
                     proc.send_signal(signum)
 
     def _setup_log_socket_handler(self, formatter):
         """Add a socket log handler"""
 
-        host = self.get("log.socket.host", fallback="localhost")
-        port = self.get_int("log.socket.port", fallback=9020)
+        host = self.config.get("log.socket.host", fallback="localhost")
+        port = self.config.get_int("log.socket.port", fallback=9020)
 
         socket_handler = SocketHandler(host, port)
         socket_handler.setFormatter(formatter)
 
         return socket_handler
 
     def _setup_log_file_handler(self, formatter):
         """Add a rotating file log handler"""
 
-        filename = self.get("log.file")
-        maxbytes = self.get_bytes("log.maxbytes", fallback="100kb")
-        backup_count = self.get_int("log.backupcount", fallback=3)
+        filename = self.config.get("log.file")
+        maxbytes = self.config.get_bytes("log.maxbytes", fallback="100kb")
+        backup_count = self.config.get_int("log.backupcount", fallback=3)
 
         rotating_handler = RotatingFileHandler(filename, "a", maxbytes, backup_count)
         rotating_handler.setFormatter(formatter)
 
         return rotating_handler
 
     def setup_log_formatter(self):
         """Initialize a log formatter"""
 
         msgfmt = "[%(asctime)s.%(msecs)03d %(levelname)7s] %(name)s"
 
-        if self.get_boolean("log.showthread", fallback=False):
+        if self.config.get_boolean("log.showthread", fallback=False):
             msgfmt += " [%(threadName)s]"
 
         msgfmt = msgfmt + ": %(message)s"
 
         datefmt = "%Y-%m-%d %H:%M:%S"
 
         return logging.Formatter(msgfmt, datefmt)
 
     def setup_log(self):
         """Setup log handlers"""
 
-        level = self.get("log.level", "info")
+        level = self.config.get("log.level", "info")
         formatter = self.setup_log_formatter()
 
         root_logger = logging.getLogger("")
         self.log = logging.getLogger(f"{self.groupname}/{self.name}")
 
-        if self.get_boolean("log.file.enable", True):
+        if self.config.get_boolean("log.file.enable", True):
             root_logger.addHandler(self._setup_log_file_handler(formatter))
 
-        if self.get_boolean("log.socket.enable", True):
+        if self.config.get_boolean("log.socket.enable", True):
             root_logger.addHandler(self._setup_log_socket_handler(formatter))
 
         if level == "warning":
             root_logger.setLevel(logging.WARNING)
         elif level == "info":
             root_logger.setLevel(logging.INFO)
         else:
@@ -332,50 +337,44 @@
 
         # Read one at a time so we know if one has an error
 
         for filename in config_files:
             config.read(filename)
 
         self.config = config[self.name]
+        self.config.set = self.config.__setitem__
+        self.config.options = self.config._options
+        self.config.get_components = partial(self.config.get_components, parent=self)
 
         self.hostname = config.get("DEFAULT", "hostname")
 
-        # Map the config section proxy get() methods onto this class
-
-        for key in dir(self.config):
-            method = getattr(self.config, key)
-            if key.startswith("get") and callable(method):
-                setattr(self, key, method)
-
-        self.get_components = functools.partial(self.config.get_components, parent=self)
-
         return config_files
 
     def setup_environment(self):
         """Setup up environment variables"""
 
         self.log.debug("Setting environment variables:")
 
-        os.environ["PATH"] = self.get("path.exec", "/usr/local/bin:/bin:/usr/bin")
-        os.environ["PATH"] += ":" + self.get("group.bin")
-        os.environ["PATH"] += ":" + self.get("path.bin")
+        os.environ["PATH"] = self.config.get("path.exec", "/usr/local/bin:/bin:/usr/bin")
+        os.environ["PATH"] += ":" + self.config.get("group.bin")
+        os.environ["PATH"] += ":" + self.config.get("path.bin")
 
-        options = self.options()
+        options = self.config.options()
 
         setoptions = fnmatch.filter(options, "environ.set.*")
         addoptions = fnmatch.filter(options, "environ.add.*")
 
         for option in setoptions:
-            value = self.get(option)
+            value = self.config.get(option)
             var = option.split(".")[2].upper()
             os.environ[var] = value
             self.log.debug("  set: [%s] = %s", var, value)
 
         for option in addoptions:
-            value = self.get(option)
+            value = self.config.get(option)
             var = option.split(".")[2].upper()
             if var in os.environ:
                 # only add if not there
                 if os.environ[var].find(value) == -1:
                     os.environ[var] += ":" + value
             else:
                 os.environ[var] = value
@@ -387,49 +386,46 @@
 
         for key in keys:
             self.log.debug("  [%s] = %s", key, os.environ[key])
 
     def setup_working_dir(self):
         """Change to working directory"""
 
-        workingdir = os.path.join(self.get("group.work"), self.name)
+        workingdir = os.path.join(self.config.get("group.work"), self.name)
 
         if not os.path.exists(workingdir):
             os.makedirs(workingdir)
 
         os.chdir(workingdir)
 
-    def put(self, option, value):
-        """Put item info configuration"""
-        self.config.parser.set(self.name, option, value)
-
-    def options(self):
-        """Get all configuration options"""
-        return self.config.parser.options(self.name)
-
     def abort(self, msg="Exiting", status=1):
         """Exit process with error"""
         self.log.error(msg)
+        self.exit_event.set()
         sys.exit(status)
 
     def exit(self, msg="Exiting", status=0):
         """Exit process"""
         self.log.info(msg)
         self.exit_event.set()
         sys.exit(status)
 
+    def stop(self):
+        """Request to stop"""
+        self.exit_event.set()
+
     def is_running(self):
         """Indicate the process is running"""
         return self.running
 
     def is_stopped(self):
         """Indicate the processes has stopped"""
         return not self.running
 
-    def current_time(self):
+    def now(self):
         """Return current time as datetime with UTC timezone"""
         return datetime.datetime.now(self.utc)
 
     def wait(self, pollrate, offset=None, sync=False):
         """Wait for a given time, short circuit if we have stopped running"""
 
         if not self.running:
```

### Comparing `datatransport-3.0.6/src/datatransport/processgroup.py` & `datatransport-3.0.7/src/datatransport/processgroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 #   2022-10-07  Todd Valentic
 #               Reorder imports
 #
 #   2023-07-09  Todd Valentic
 #               Use TransportConfig find_config_files()
 #               Use place holde {client.name} when showing config in debug 
 #
+#   2023-07-20  Todd Valentic
+#               Change error to debug if no clients listed
+#               Reduce default shutdown_timeout to 30s
+#               Change shutdown_timeout to timedelta 
+#
 #############################################################################
 
 import configparser
 import copy
 import fnmatch
 import glob
 import logging
@@ -236,15 +241,15 @@
 
         processgroup = self.config["ProcessGroup"]
 
         self.autostart = processgroup.get_boolean("autostart", False)
         self.grouplabel = processgroup.get("label", self.name)
         self.start_priority = processgroup.get_int("priority.start", 50)
         self.stop_priority = processgroup.get_int("priority.stop", 50)
-        self.shutdown_timeout = processgroup.get_int("shutdown.timeout", 120)
+        self.shutdown_timeout = processgroup.get_timedelta("shutdown.timeout", 30)
         self.report_rate = processgroup.get_int("shutdown.report.rate", 15)
 
         return config_files
 
     def load_clients(self):
         """Load clients"""
 
@@ -322,15 +327,15 @@
             try:
                 clientnames = self.config["ProcessGroup"].get("clients.start")
                 clientnames = clientnames.split()
             except (configparser.Error, AttributeError):
                 clientnames = self.clients.keys()
 
         if not clientnames:
-            self.log.error("No clients listed")
+            self.log.debug("No clients listed")
             return
 
         clientnames = set(clientnames).intersection(self.clients)
 
         for clientname in clientnames:
             cmd = self.find_command(clientname)
             args = [cmd, self.name, clientname]
@@ -349,15 +354,15 @@
 
         for name in names:
             if self.clients[name].alive():
                 self.parent_log.info("Stopping client %s", name)
                 self.clients[name].stop()
                 num_running += 1
 
-        timeout = time.time() + self.shutdown_timeout
+        timeout = time.time() + self.shutdown_timeout.total_seconds()
         report_time = time.time() + self.report_rate
 
         while time.time() < timeout and num_running > 0:
             time.sleep(1)
             num_running = 0
             for name in names:
                 if self.clients[name].alive():
```

### Comparing `datatransport-3.0.6/src/datatransport/templates/etc/transportd.conf` & `datatransport-3.0.7/src/datatransport/templates/etc/transportd.conf`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/templates/groups/ServerMonitor/watchdog.py` & `datatransport-3.0.7/src/datatransport/templates/groups/ServerMonitor/watchdog.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 #               Converted to directly reading /proc instead of using ps
 #
 #   2004-12-30  Todd Valentic
 #               Convert from mx.DateTime to datetime
 #
 #   2022-10-06  Todd Valentic
 #               Updated for transport3/python3
+#   
+#   2023-07-26  Todd Valentic
+#               Use config getters
 #
 ############################################################################
 
 import pathlib
 import sys
 
 from datatransport import ProcessClient
@@ -66,15 +69,15 @@
     def __init__(self, argv):
         ProcessClient.__init__(self, argv)
 
     def init(self):
         super().init()
 
         self.news_poster = NewsPoster(self)
-        self.rate = self.get_rate("rate", "5m")
+        self.rate = self.config.get_rate("rate", "5m")
 
     def get_client_pids(self):
         """Query server for expected client PIDs"""
 
         pids = {}
 
         for group in self.server.listgroups():
@@ -99,15 +102,15 @@
         body.append(
             "  The watchdog has detected the following client has stopped running:"
         )
         body.append("")
         body.append(f"      Client name: {client_name}")
         body.append(f"       Group name: {group_name}")
         body.append(f"       Process ID: {pid}")
-        body.append(f"       Time stamp: {self.current_time()}")
+        body.append(f"       Time stamp: {self.now()}")
         body.append("")
         body.append("  The client has been restarted.")
         body.append("")
 
         header = f"Watchdog restart {client_name}"
 
         try:
```

### Comparing `datatransport-3.0.6/src/datatransport/transportconfig.py` & `datatransport-3.0.7/src/datatransport/transportconfig.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/transportlogger.py` & `datatransport-3.0.7/src/datatransport/transportlogger.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/transportmanager.py` & `datatransport-3.0.7/src/datatransport/transportmanager.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/transportserver.py` & `datatransport-3.0.7/src/datatransport/transportserver.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/utilities/datefunc.py` & `datatransport-3.0.7/src/datatransport/utilities/datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/utilities/makepath.py` & `datatransport-3.0.7/src/datatransport/utilities/makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/utilities/patterntemplate.py` & `datatransport-3.0.7/src/datatransport/utilities/patterntemplate.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 #
 #   2022-10-12  Todd Valentic
 #               Python3 port
 #               Use parse_slice (https://stackoverflow.com/a/68899290)
 #               Rework implementation with regex instead of eval
 #               setValue -> set_value
 #
+#   2023-07-26  Todd Valentic
+#               Missing check for pattern 
+#
 #   SPDX-License-Identifier: GPL-3.0-or-later
 #   Copyright (C) 1999-2022 Todd Valentic
 #
 ###########################################################################
 
 import re
 
@@ -77,20 +80,20 @@
     Return a unique list of patterns (<name>) found in the string
     """
     return list(set(re_pattern.findall(string)))
 
 class PatternTemplate:
     """String pattern replacement"""
 
-    def __init__(self, patttern: str, sep: str=None):
-        self.patttern = patttern
+    def __init__(self, pattern: str, sep: str=None):
+        self.pattern = pattern
         self.sep = sep
         self.value = None
 
-    def set_value(self, value: str) -> None:
+    def set_value(self, value: Union[str, list, dict]) -> None:
         """Cache the value of the replacement string"""
 
         self.value = value
 
     def lookup_value(self, entry: str, value: Union[str, list, dict], sep: str='') -> str:
         """Look up the entry in the value str, list or dict"""
 
@@ -120,25 +123,27 @@
 
             return entry
 
         return value
 
 
     def __call__(self, src: str, value: str=None) -> str:
-        """Replace <patttern> with value"""
+        """Replace <pattern> with value"""
 
-        if value is None:
-            value = self.value
-        else:
+        if value is not None:
             self.set_value(value)
 
+        value = self.value
+
         if value is None:
             return src
 
         if self.sep:
             value = value.split(self.sep)
 
         for entry in parse_patterns(src):
+            if not entry.startswith(self.pattern):
+                continue
             v = self.lookup_value(entry, value, self.sep)
-            src = src.replace(f'<{entry}>', v)
+            src = src.replace(f'<{entry}>', str(v))
 
         return src
```

### Comparing `datatransport-3.0.6/src/datatransport/utilities/removefile.py` & `datatransport-3.0.7/src/datatransport/utilities/removefile.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/utilities/sizedesc.py` & `datatransport-3.0.7/src/datatransport/utilities/sizedesc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/utilities/xmlrpcdeferred.py` & `datatransport-3.0.7/src/datatransport/utilities/xmlrpcdeferred.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/src/datatransport/xmlrpcserver.py` & `datatransport-3.0.7/src/datatransport/xmlrpcserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.timeout = timeout
 
         if port is None:
             # This is a normal service client
 
             self.directory = Directory(parent)
 
-            servicename = parent.get("service.name")
+            servicename = parent.config.get("service.name")
 
             if not servicename:
                 parent.abort("No service.name found")
 
             port = self.directory.get(servicename, "port")
 
             try:
```

### Comparing `datatransport-3.0.6/src/datatransport.egg-info/PKG-INFO` & `datatransport-3.0.7/src/datatransport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatransport
-Version: 3.0.6
+Version: 3.0.7
 Summary: Data Transport Network
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `datatransport-3.0.6/src/datatransport.egg-info/SOURCES.txt` & `datatransport-3.0.7/src/datatransport.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 INSTALL
 LICENSE
 MANIFEST.in
 MIGRATION
 README.rst
 pyproject.toml
 contrib/examples/.coverage
+contrib/examples/README
 contrib/examples/examples.conf
 contrib/examples.v2/README
 contrib/examples.v2/test.conf
 contrib/examples.v2/archivegroups/archivegroups.conf
 contrib/examples.v2/archivegroups/postdata.py
 contrib/examples.v2/component/component.conf
 contrib/examples.v2/component/demo.py
@@ -120,42 +121,43 @@
 src/datatransport/commands/console.py
 src/datatransport/commands/listnewsgroups.py
 src/datatransport/commands/transport_create_app.py
 src/datatransport/commands/transportctl.py
 src/datatransport/commands/transportd.py
 src/datatransport/commands/transportps.py
 src/datatransport/commands/viewlog.py
-src/datatransport/components/ArchiveGroups.py
-src/datatransport/components/DirectoryService.py
 src/datatransport/components/DiskMonitor.py
 src/datatransport/components/EventMonitor.py
 src/datatransport/components/FilePost.py
 src/datatransport/components/FileStore.py
-src/datatransport/components/FileWatch.py
 src/datatransport/components/GroupControl.py
 src/datatransport/components/InstrumentStatus.py
 src/datatransport/components/NewsGateway.py
 src/datatransport/components/NewsgroupMonitor.py
 src/datatransport/components/PageKit.py
 src/datatransport/components/PlotTool.py
 src/datatransport/components/PostDataFiles.py
 src/datatransport/components/RealTimeFeed.py
 src/datatransport/components/ResourceMonitor.py
 src/datatransport/components/Scheduler.py
 src/datatransport/components/SyncPoller.py
 src/datatransport/components/WatchURL.py
 src/datatransport/components/__init__.py
+src/datatransport/components/archivegroups.py
+src/datatransport/components/directoryservice.py
+src/datatransport/components/filewatch.py
 src/datatransport/templates/etc/transportd.conf
 src/datatransport/templates/groups/ServerMonitor/ServerMonitor.conf
 src/datatransport/templates/groups/ServerMonitor/watchdog.py
 src/datatransport/utilities/__init__.py
 src/datatransport/utilities/datefunc.py
 src/datatransport/utilities/makepath.py
 src/datatransport/utilities/patterntemplate.py
 src/datatransport/utilities/removefile.py
 src/datatransport/utilities/sizedesc.py
 src/datatransport/utilities/xmlrpcdeferred.py
 tests/test_utilities_datefunc.py
 tests/test_utilities_makepath.py
 tests/test_utilities_pattern.py
 tests/test_utilities_removefiles.py
-tests/test_utilities_sizedesc.py
+tests/test_utilities_sizedesc.py
+tests/__pycache__/test_utilities_pattern.cpython-311-pytest-7.4.0.pyc
```

### Comparing `datatransport-3.0.6/src/datatransport.egg-info/entry_points.txt` & `datatransport-3.0.7/src/datatransport.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [console_scripts]
-archivegroups = datatransport.components.ArchiveGroups:main
+archivegroups = datatransport.components.archivegroups:main
 cancelnewsgroup = datatransport.commands.cancelnewsgroup:main
 console = datatransport.commands.console:main
-directoryservice = datatransport.components.DirectoryService:main
+directoryservice = datatransport.components.directoryservice:main
 diskmonitor = datatransport.components.DiskMonitor:main
 filepost = datatransport.components.FilePost:main
 filestore = datatransport.components.FileStore:main
-filewatch = datatransport.components.FileWatch:main
+filewatch = datatransport.components.filewatch:main
 groupcontrol = datatransport.components.GroupControl:main
 instrumentstatus = datatransport.components.InstrumentStatus:main
 listnewsgroups = datatransport.commands.listnewsgroups:main
 newsgateway = datatransport.components.NewsGateway:main
 newsgroupmonitor = datatransport.components.NewsgroupMonitor:main
 plottool = datatransport.components.PlotTool:main
 postdatafiles = datatransport.components.PostDataFiles:main
```

### Comparing `datatransport-3.0.6/tests/test_utilities_datefunc.py` & `datatransport-3.0.7/tests/test_utilities_datefunc.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/tests/test_utilities_makepath.py` & `datatransport-3.0.7/tests/test_utilities_makepath.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/tests/test_utilities_removefiles.py` & `datatransport-3.0.7/tests/test_utilities_removefiles.py`

 * *Files identical despite different names*

### Comparing `datatransport-3.0.6/tests/test_utilities_sizedesc.py` & `datatransport-3.0.7/tests/test_utilities_sizedesc.py`

 * *Files identical despite different names*

