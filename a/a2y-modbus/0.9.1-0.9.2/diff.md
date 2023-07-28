# Comparing `tmp/a2y_modbus-0.9.1-cp36-cp36m-win32.whl.zip` & `tmp/a2y_modbus-0.9.2-cp36-cp36m-win32.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 89912 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   261120 b- defN 23-Feb-25 03:14 a2y_modbus.cp36-win32.pyd
--rw-rw-rw-  2.0 fat      704 b- defN 23-Feb-25 03:14 a2y_modbus-0.9.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      983 b- defN 23-Feb-25 03:14 a2y_modbus-0.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Feb-25 03:14 a2y_modbus-0.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Feb-25 03:14 a2y_modbus-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      483 b- defN 23-Feb-25 03:14 a2y_modbus-0.9.1.dist-info/RECORD
-6 files, 263398 bytes uncompressed, 89036 bytes compressed:  66.2%
+Zip file size: 103834 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   298496 b- defN 23-Jul-28 02:20 a2y_modbus.cp36-win32.pyd
+-rw-rw-rw-  2.0 fat      718 b- defN 23-Jul-28 02:20 a2y_modbus-0.9.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      993 b- defN 23-Jul-28 02:20 a2y_modbus-0.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-28 02:20 a2y_modbus-0.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-28 02:20 a2y_modbus-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      483 b- defN 23-Jul-28 02:20 a2y_modbus-0.9.2.dist-info/RECORD
+6 files, 300798 bytes uncompressed, 102958 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: a2y_modbus.cp36-win32.pyd
 Comment: 
 
-Filename: a2y_modbus-0.9.1.dist-info/LICENSE
+Filename: a2y_modbus-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: a2y_modbus-0.9.1.dist-info/METADATA
+Filename: a2y_modbus-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: a2y_modbus-0.9.1.dist-info/WHEEL
+Filename: a2y_modbus-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: a2y_modbus-0.9.1.dist-info/top_level.txt
+Filename: a2y_modbus-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: a2y_modbus-0.9.1.dist-info/RECORD
+Filename: a2y_modbus-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `a2y_modbus-0.9.1.dist-info/LICENSE` & `a2y_modbus-0.9.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is private software.
-
-Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
+This is private software.
+
+Anyone without authorization is NOT allowed to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `a2y_modbus-0.9.1.dist-info/METADATA` & `a2y_modbus-0.9.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: a2y-modbus
-Version: 0.9.1
+Version: 0.9.2
 Summary: A module that implements partial function of Modbus protocol.
 Home-page: http://www.sorobust.com/a2y/modbus.html
 Author: Yu Han
 Author-email: hanjunyu@163.com
 License: Private
 Platform: Windows
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free For Educational Use
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: pyserial (>=3.0)
 
 # Python Module: a2y_modbus
 a2y_modbus模块实现了基本的Modbus通信协议，包括以下功能码：
 - 0x01，读多个连续的线圈。
 - 0x03，读多个连续的寄存器。
 - 0x05，写单个线圈。
 - 0x06，写单个寄存器。
```

