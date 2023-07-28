# Comparing `tmp/MomentumX-2.7.0.tar.gz` & `tmp/MomentumX-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MomentumX-2.7.0.tar", last modified: Tue May  9 16:22:34 2023, max compression
+gzip compressed data, was "MomentumX-2.7.1.tar", last modified: Fri Jul 28 00:12:40 2023, max compression
```

## Comparing `MomentumX-2.7.0.tar` & `MomentumX-2.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.316607 MomentumX-2.7.0/
--rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.7.0/.clang-format
--rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.7.0/.dockerignore
--rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.7.0/.gitignore
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.307607 MomentumX-2.7.0/.vscode/
--rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.7.0/.vscode/settings.json
--rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.7.0/CMakeLists.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.7.0/LICENSE
--rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.7.0/Logo.png
--rw-rw-r--   0 developer  (1000) developer  (1000)     1513 2023-05-09 13:05:53.000000 MomentumX-2.7.0/Makefile
--rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-05-09 16:22:34.315707 MomentumX-2.7.0/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     6442 2023-05-09 13:07:32.000000 MomentumX-2.7.0/README.md
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.312107 MomentumX-2.7.0/examples/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/multi.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/stream_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/stream_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.7.0/examples/sync_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.7.0/examples/sync_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1024 2023-04-24 15:44:52.000000 MomentumX-2.7.0/examples/threaded.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.313007 MomentumX-2.7.0/ext/
--rw-rw-r--   0 developer  (1000) developer  (1000)    22135 2023-04-24 15:44:52.000000 MomentumX-2.7.0/ext/binding.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.7.0/ext/buffer.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.7.0/ext/buffer.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/context.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/context.h
--rw-rw-r--   0 developer  (1000) developer  (1000)    21069 2023-05-09 13:05:53.000000 MomentumX-2.7.0/ext/stream.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/stream.h
--rw-rw-r--   0 developer  (1000) developer  (1000)    11990 2023-05-09 13:05:53.000000 MomentumX-2.7.0/ext/utils.h
--rw-rw-r--   0 developer  (1000) developer  (1000)      133 2023-04-24 15:44:52.000000 MomentumX-2.7.0/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-05-09 16:22:34.316607 MomentumX-2.7.0/setup.cfg
--rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-05-09 13:06:09.000000 MomentumX-2.7.0/setup.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.303107 MomentumX-2.7.0/src/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.313907 MomentumX-2.7.0/src/MomentumX.egg-info/
--rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/top_level.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.314807 MomentumX-2.7.0/src/momentumx/
--rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.7.0/src/momentumx/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-05-09 16:14:07.000000 MomentumX-2.7.0/src/momentumx/_mx.pyi
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.7.0/src/momentumx/cli.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.314807 MomentumX-2.7.0/tests/
--rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.7.0/tests/test_scenarios.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.064725 MomentumX-2.7.1/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.7.1/.clang-format
+-rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.7.1/.dockerignore
+-rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.7.1/.gitignore
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.058713 MomentumX-2.7.1/.vscode/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.7.1/.vscode/settings.json
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.7.1/CMakeLists.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.7.1/LICENSE
+-rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.7.1/Logo.png
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1513 2023-07-27 21:02:22.000000 MomentumX-2.7.1/Makefile
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-07-28 00:12:40.064725 MomentumX-2.7.1/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6442 2023-07-27 23:58:45.000000 MomentumX-2.7.1/README.md
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.061719 MomentumX-2.7.1/examples/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.7.1/examples/multi.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.7.1/examples/stream_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.7.1/examples/stream_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.7.1/examples/sync_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.7.1/examples/sync_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1024 2023-04-24 15:44:52.000000 MomentumX-2.7.1/examples/threaded.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.062721 MomentumX-2.7.1/ext/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    22135 2023-07-27 20:36:27.000000 MomentumX-2.7.1/ext/binding.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7518 2023-07-27 23:56:40.000000 MomentumX-2.7.1/ext/buffer.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.7.1/ext/buffer.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4750 2023-07-27 23:56:40.000000 MomentumX-2.7.1/ext/context.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-07-27 21:12:59.000000 MomentumX-2.7.1/ext/context.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    22274 2023-07-27 23:56:40.000000 MomentumX-2.7.1/ext/stream.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-07-27 21:12:59.000000 MomentumX-2.7.1/ext/stream.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    11990 2023-07-27 20:00:16.000000 MomentumX-2.7.1/ext/utils.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)      133 2023-04-24 15:44:52.000000 MomentumX-2.7.1/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-07-28 00:12:40.064725 MomentumX-2.7.1/setup.cfg
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-07-27 23:58:45.000000 MomentumX-2.7.1/setup.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.055707 MomentumX-2.7.1/src/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.063723 MomentumX-2.7.1/src/MomentumX.egg-info/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-07-28 00:12:39.000000 MomentumX-2.7.1/src/MomentumX.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-07-28 00:12:39.000000 MomentumX-2.7.1/src/MomentumX.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-07-28 00:12:39.000000 MomentumX-2.7.1/src/MomentumX.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-07-28 00:12:39.000000 MomentumX-2.7.1/src/MomentumX.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-07-28 00:12:39.000000 MomentumX-2.7.1/src/MomentumX.egg-info/top_level.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.064725 MomentumX-2.7.1/src/momentumx/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.7.1/src/momentumx/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-07-28 00:01:19.000000 MomentumX-2.7.1/src/momentumx/_mx.pyi
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.7.1/src/momentumx/cli.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-07-28 00:12:40.064725 MomentumX-2.7.1/tests/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-07-27 20:00:14.000000 MomentumX-2.7.1/tests/test_scenarios.py
```

### Comparing `MomentumX-2.7.0/CMakeLists.txt` & `MomentumX-2.7.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/LICENSE` & `MomentumX-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/Logo.png` & `MomentumX-2.7.1/Logo.png`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/Makefile` & `MomentumX-2.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/PKG-INFO` & `MomentumX-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.7.0
+Version: 2.7.1
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.7.0/README.md` & `MomentumX-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/multi.py` & `MomentumX-2.7.1/examples/multi.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/stream_reader.py` & `MomentumX-2.7.1/examples/stream_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/stream_writer.py` & `MomentumX-2.7.1/examples/stream_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/sync_reader.py` & `MomentumX-2.7.1/examples/sync_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/sync_writer.py` & `MomentumX-2.7.1/examples/sync_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/examples/threaded.py` & `MomentumX-2.7.1/examples/threaded.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/ext/binding.cpp` & `MomentumX-2.7.1/ext/binding.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/ext/buffer.cpp` & `MomentumX-2.7.1/ext/buffer.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -34,38 +34,62 @@
                 throw std::runtime_error("Failed to open shared memory buffer for stream '" + _backing_filepath + "' [errno: " + std::to_string(errno) + "]");
             }
         }
         // do the ftruncate to resize and (re)mmap
         resize_remap(size);
 
         if (_is_create) {
-            Utils::Logger::get_logger().info(std::string("Created Producer Buffer (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(std::string("Created Producer Buffer (" + std::to_string((uint64_t)this) + ")"));
         } else {
-            Utils::Logger::get_logger().info(std::string("Created Consumer Buffer (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(std::string("Created Consumer Buffer (" + std::to_string((uint64_t)this) + ")"));
         }
     };
 
     Buffer::~Buffer() {
+        bool has_errors = false;
+        int return_val;
+        if (_address != MAP_FAILED) {
+            return_val = munmap(_address, _size);
+            if (return_val != 0) {
+                has_errors |= true;
+                Utils::Logger::get_logger().warning(std::string("Buffer Unmap Failed (" + std::to_string((uint64_t)this) + ")"));
+            } else {
+                Utils::Logger::get_logger().debug(std::string("Buffer Unmapped (" + std::to_string((uint64_t)this) + ")"));
+            }
+        }
+
         if (_fd > -1) {
-            close(_fd);
+            return_val = ::close(_fd);
+
+            if (return_val != 0) {
+                has_errors |= true;
+                Utils::Logger::get_logger().warning(std::string("Buffer Close Failed (" + std::to_string((uint64_t)this) + ")"));
+            } else {
+                Utils::Logger::get_logger().debug(std::string("Buffer Closed (" + std::to_string((uint64_t)this) + ")"));
+            }
 
             if (_is_create) {
-                int return_val = std::remove(_backing_filepath.c_str());
+                return_val = std::remove(_backing_filepath.c_str());
                 if (return_val != 0) {
+                    has_errors |= true;
                     std::stringstream ss;
                     ss << "Unable to delete buffer file \"" << _backing_filepath << "\" with error: " << return_val;
-                    Utils::Logger::get_logger().error(ss.str());
+                    Utils::Logger::get_logger().warning(ss.str());
                 }
             }
         }
 
-        if (_is_create) {
-            Utils::Logger::get_logger().info(std::string("Destroyed Producer Buffer (" + std::to_string((uint64_t)this) + ")"));
+        std::stringstream ss;
+        ss << "Destroyed " << (_is_create ? "Producer" : "Consumer") << " Buffer (" << std::to_string((uint64_t)this) << ")";
+
+        if (has_errors) {
+            ss << " [POSSIBLE MEMORY LEAK DETECTED!]";
+            Utils::Logger::get_logger().warning(ss.str());
         } else {
-            Utils::Logger::get_logger().info(std::string("Destroyed Consumer Buffer (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(ss.str());
         }
     }
 
     const uint16_t Buffer::id() {
         return _id;
     }
 
@@ -180,8 +204,8 @@
         return next_buffer;
     }
 
     std::shared_ptr<Buffer> BufferManager::peek_next(const Lock& lock, const Utils::PathConfig& paths) {
         return _buffers_by_stream[paths.stream_name].front();
     }
 
-}  // namespace MomentumX
+}  // namespace MomentumX
```

### Comparing `MomentumX-2.7.0/ext/buffer.h` & `MomentumX-2.7.1/ext/buffer.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/ext/context.cpp` & `MomentumX-2.7.1/ext/context.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #include "context.h"
 #include "stream.h"
 #include "utils.h"
 
 namespace MomentumX {
 
     Context::Context(const std::string& context_path) : _context_path(context_path), _buffer_manager(), _stream_manager(this, &_buffer_manager) {
-        Utils::Logger::get_logger().info(std::string("Created Context (" + std::to_string((uint64_t)this) + ")"));
+        Utils::Logger::get_logger().debug(std::string("Created Context (" + std::to_string((uint64_t)this) + ")"));
     };
 
     Context::~Context() {
-        Utils::Logger::get_logger().info(std::string("Destroyed Context (" + std::to_string((uint64_t)this) + ")"));
+        Utils::Logger::get_logger().debug(std::string("Destroyed Context (" + std::to_string((uint64_t)this) + ")"));
     }
 
     Stream* Context::stream(std::string stream_name, size_t buffer_size, size_t buffer_count, bool sync) {
         // Ensure valid stream name
         Utils::validate_stream(stream_name);
 
         const auto sm_lock = _stream_manager.get_stream_manager_lock();
```

### Comparing `MomentumX-2.7.0/ext/context.h` & `MomentumX-2.7.1/ext/context.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/ext/stream.cpp` & `MomentumX-2.7.1/ext/stream.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             new (_control) ControlBlock();  // placement construct into shared memory
 
             const auto control_lock = get_control_lock();
             _control->sync = sync;
             _control->buffer_size = buffer_size;
             _control->buffer_count = buffer_count;
 
-            Utils::Logger::get_logger().info(std::string("Created Producer Stream (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(std::string("Created Producer Stream (" + std::to_string((uint64_t)this) + ")"));
         } else {
             auto control_lock = get_control_lock();
             if (!_control->is_ready()) {
                 throw std::runtime_error("Attempt to open stream before it is ready");
             }
             _control->subscriber_count++;
             if (_control->sync) {
@@ -84,66 +84,92 @@
                         auto& bsync = _control->buffers.at(idx).buffer_sync;
                         bsync.inc_required(control_lock);
                     }
                 }
             }
             _subscribed = true;
 
-            Utils::Logger::get_logger().info(std::string("Created Consumer Stream (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(std::string("Created Consumer Stream (" + std::to_string((uint64_t)this) + ")"));
         }
 
         // Initialize any cached variables that will remain for the duration of the stream to prevent extraneous locking...
         _sync = _control->sync;
     };
 
     Stream::~Stream() {
-        auto control_lock = get_control_lock();
-        if (_role == Role::PRODUCER) {
-            Utils::Logger::get_logger().info("Producer stream signaling end of stream");
-            end(control_lock);
-        } else {
-            if (_subscribed) {
-                --_control->subscriber_count;
-
-                // If we are destructing while producer is still sending, claim and release all unmanaged buffers
-                // Since this happens with the control block lock, any currently checkout-out write buffers will
-                // submitted with the updated subscriber_count value
-                if (_control->sync) {
-                    const auto inc = [&](size_t idx) { return ControlBlock::wrapping_increment(idx, _control->buffer_count); };
-                    while (_last_iteration != _control->last_sent_iteration()) {
-                        _last_index = inc(_last_index);
-                        _last_iteration++;
-
-                        auto& b = _control->buffers.at(_last_index);
-                        auto& bsync = b.buffer_sync;
-                        if (bsync.checkout_read(control_lock) == BufferSync::CheckoutResult::SUCCESS) {
-                            bsync.checkin_read(control_lock);
+        {
+            auto control_lock = get_control_lock();
+            if (_role == Role::PRODUCER) {
+                Utils::Logger::get_logger().debug(std::string("Producer stream signaling end of stream (" + std::to_string((uint64_t)this) + ")"));
+                end(control_lock);
+            } else {
+                if (_subscribed) {
+                    --_control->subscriber_count;
+
+                    // If we are destructing while producer is still sending, claim and release all unmanaged buffers
+                    // Since this happens with the control block lock, any currently checkout-out write buffers will
+                    // submitted with the updated subscriber_count value
+                    if (_control->sync) {
+                        const auto inc = [&](size_t idx) { return ControlBlock::wrapping_increment(idx, _control->buffer_count); };
+                        while (_last_iteration != _control->last_sent_iteration()) {
+                            _last_index = inc(_last_index);
+                            _last_iteration++;
+
+                            auto& b = _control->buffers.at(_last_index);
+                            auto& bsync = b.buffer_sync;
+                            if (bsync.checkout_read(control_lock) == BufferSync::CheckoutResult::SUCCESS) {
+                                bsync.checkin_read(control_lock);
+                            }
                         }
                     }
                 }
             }
         }
 
+        bool has_errors = false;
+        int return_val;
+
+        if (_data != MAP_FAILED) {
+            return_val = munmap(_data, Utils::page_aligned_size(sizeof(ControlBlock)));
+            if (return_val != 0) {
+                has_errors |= true;
+                Utils::Logger::get_logger().warning(std::string("Stream Unmap Failed (" + std::to_string((uint64_t)this) + ")"));
+            } else {
+                Utils::Logger::get_logger().debug(std::string("Stream Unmapped (" + std::to_string((uint64_t)this) + ")"));
+            }
+        }
+
         if (_fd > -1) {
-            ::close(_fd);
+            return_val = ::close(_fd);
+            if (return_val != 0) {
+                has_errors |= true;
+                Utils::Logger::get_logger().warning(std::string("Stream Close Failed (" + std::to_string((uint64_t)this) + ")"));
+            } else {
+                Utils::Logger::get_logger().debug(std::string("Stream Closed (" + std::to_string((uint64_t)this) + ")"));
+            }
 
             if (_role == Role::PRODUCER) {
-                int return_val = std::remove(_paths.stream_path.c_str());
+                return_val = std::remove(_paths.stream_path.c_str());
                 if (return_val != 0) {
+                    has_errors |= true;
                     std::stringstream ss;
                     ss << "Unable to delete stream file \"" << _paths.stream_path << "\" with error: " << return_val;
-                    Utils::Logger::get_logger().error(ss.str());
+                    Utils::Logger::get_logger().warning(ss.str());
                 }
             }
         }
 
-        if (_role == PRODUCER) {
-            Utils::Logger::get_logger().info(std::string("Destroyed Producer Stream (" + std::to_string((uint64_t)this) + ")"));
+        std::stringstream ss;
+        ss << "Destroyed " << (_role == PRODUCER ? "Producer" : "Consumer") << " Stream (" << std::to_string((uint64_t)this) << ")";
+
+        if (has_errors) {
+            ss << " [POSSIBLE MEMORY LEAK DETECTED!]";
+            Utils::Logger::get_logger().warning(ss.str());
         } else {
-            Utils::Logger::get_logger().info(std::string("Destroyed Consumer Stream (" + std::to_string((uint64_t)this) + ")"));
+            Utils::Logger::get_logger().debug(ss.str());
         }
     }
 
     const std::string& Stream::name(const Utils::OmniWriteLock& control_lock) {
         return _paths.stream_name;
     }
 
@@ -471,8 +497,8 @@
         }
     }
 
     size_t StreamManager::subscriber_count(const Lock& lock, const Stream::Lock& control_lock, Stream* stream) {
         return stream->_control->subscriber_count;
     }
 
-}  // namespace MomentumX
+}  // namespace MomentumX
```

### Comparing `MomentumX-2.7.0/ext/stream.h` & `MomentumX-2.7.1/ext/stream.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/ext/utils.h` & `MomentumX-2.7.1/ext/utils.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/setup.py` & `MomentumX-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from skbuild import setup
 
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="MomentumX",
     version=__version__,
```

### Comparing `MomentumX-2.7.0/src/MomentumX.egg-info/PKG-INFO` & `MomentumX-2.7.1/src/MomentumX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.7.0
+Version: 2.7.1
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.7.0/src/MomentumX.egg-info/SOURCES.txt` & `MomentumX-2.7.1/src/MomentumX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/src/momentumx/_mx.pyi` & `MomentumX-2.7.1/src/momentumx/_mx.pyi`

 * *Files identical despite different names*

### Comparing `MomentumX-2.7.0/tests/test_scenarios.py` & `MomentumX-2.7.1/tests/test_scenarios.py`

 * *Files identical despite different names*

