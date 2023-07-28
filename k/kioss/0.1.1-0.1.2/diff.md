# Comparing `tmp/kioss-0.1.1.tar.gz` & `tmp/kioss-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.1.1.tar", last modified: Thu Jul 27 17:10:58 2023, max compression
+gzip compressed data, was "kioss-0.1.2.tar", last modified: Fri Jul 28 08:04:24 2023, max compression
```

## Comparing `kioss-0.1.1.tar` & `kioss-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 17:10:48.000000 kioss-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 17:10:58.027750 kioss-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 17:10:48.000000 kioss-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 17:10:58.000000 kioss-0.1.1/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:10:58.027750 kioss-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 17:10:48.000000 kioss-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-27 17:10:48.000000 kioss-0.1.1/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 17:10:48.000000 kioss-0.1.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 08:04:14.000000 kioss-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 08:04:24.840126 kioss-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-28 08:04:14.000000 kioss-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-28 08:04:14.000000 kioss-0.1.2/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 08:04:24.000000 kioss-0.1.2/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:04:24.840126 kioss-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-28 08:04:14.000000 kioss-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:04:24.840126 kioss-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-28 08:04:14.000000 kioss-0.1.2/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-28 08:04:14.000000 kioss-0.1.2/test/test_util.py
```

### Comparing `kioss-0.1.1/LICENSE` & `kioss-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.1.1/README.md` & `kioss-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.1.1/kioss/pipe.py` & `kioss-0.1.2/kioss/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                 iterators,
                 Queue(self.MAX_NUM_WAITING_ELEMS_PER_THREAD * len(iterators)),
             )
         )
 
     @staticmethod
     def _concurrently_merging_iterable(
-        iterators: List[Iterator[T]], queue: Queue[T]
+        iterators: List[Iterator[T]], queue: Queue
     ) -> Iterator[T]:
         with ThreadPoolExecutor(max_workers=len(iterators)) as executor:
 
             def pull_job(iterator: Iterator[T]):
                 while True:
                     try:
                         queue.put(next(iterator))
@@ -391,16 +391,16 @@
             )
         )
 
     @staticmethod
     def _concurrently_mapping_iterable(
         func: Callable[[T], R], iterator: Iterator[T], n_threads, max_queue_size: int
     ) -> Iterator[T]:
-        input_queue: Queue[T] = Queue(maxsize=max_queue_size)
-        output_queue: Queue[R] = Queue(maxsize=max_queue_size)
+        input_queue: Queue = Queue(maxsize=max_queue_size)
+        output_queue: Queue = Queue(maxsize=max_queue_size)
 
         with ThreadPoolExecutor(max_workers=n_threads + 1) as executor:
             input_feeder_future = executor.submit(
                 lambda: util.iterate(map(input_queue.put, iterator))
             )
 
             def mapper_job():
```

### Comparing `kioss-0.1.1/test/test_pipe.py` & `kioss-0.1.2/test/test_pipe.py`

 * *Files identical despite different names*

