# Comparing `tmp/agora_busclient-1.1.31-py2.py3-none-any.whl.zip` & `tmp/agora_busclient-1.1.32-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 14358 bytes, number of entries: 22
--rw-r--r--  2.0 fat      240 b- defN 23-Jul-20 18:48 agora_busclient/__init__.py
+Zip file size: 14571 bytes, number of entries: 22
+-rw-r--r--  2.0 fat      261 b- defN 23-Jul-28 12:34 agora_busclient/__init__.py
 -rw-r--r--  2.0 fat     2974 b- defN 23-Jul-27 15:56 agora_busclient/base_mqtt_client.py
 -rw-r--r--  2.0 fat     3220 b- defN 23-Jul-27 16:58 agora_busclient/bus_client.py
 -rw-r--r--  2.0 fat     4267 b- defN 23-Jul-28 10:49 agora_busclient/message_queue.py
 -rw-r--r--  2.0 fat     5115 b- defN 23-May-19 17:55 agora_busclient/mqtt_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:13 agora_busclient/version.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:37 agora_busclient/version.py
 -rw-r--r--  2.0 fat      432 b- defN 23-Jul-10 22:39 agora_busclient/messages/__init__.py
 -rw-r--r--  2.0 fat     1693 b- defN 23-Jul-27 17:21 agora_busclient/messages/event_msg.py
 -rw-r--r--  2.0 fat      233 b- defN 23-May-12 13:38 agora_busclient/messages/io_device_data.py
 -rw-r--r--  2.0 fat      678 b- defN 23-May-12 13:38 agora_busclient/messages/io_point.py
 -rw-r--r--  2.0 fat      565 b- defN 23-May-12 13:38 agora_busclient/messages/io_tag_data_dict.py
 -rw-r--r--  2.0 fat     1918 b- defN 23-May-12 13:38 agora_busclient/messages/iodatareport_message.py
 -rw-r--r--  2.0 fat      950 b- defN 23-Jul-27 17:24 agora_busclient/messages/media_data.py
 -rw-r--r--  2.0 fat      799 b- defN 23-May-12 13:38 agora_busclient/messages/message_header.py
--rw-r--r--  2.0 fat     7572 b- defN 23-Jul-28 12:11 agora_busclient/messages/msg_decoder.py
--rw-r--r--  2.0 fat     3851 b- defN 23-Jul-28 12:12 agora_busclient/messages/msg_encoder.py
+-rw-r--r--  2.0 fat     8500 b- defN 23-Jul-28 12:33 agora_busclient/messages/msg_decoder.py
+-rw-r--r--  2.0 fat     4116 b- defN 23-Jul-28 12:30 agora_busclient/messages/msg_encoder.py
 -rw-r--r--  2.0 fat      581 b- defN 23-May-12 13:38 agora_busclient/messages/request_msg.py
 -rw-r--r--  2.0 fat      129 b- defN 23-Jul-11 16:30 agora_busclient/messages/work_flow.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.31.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.31.dist-info/WHEEL
--rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.31.dist-info/METADATA
--rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.31.dist-info/RECORD
-22 files, 38598 bytes uncompressed, 11036 bytes compressed:  71.4%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.32.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.32.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.32.dist-info/METADATA
+-rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.32.dist-info/RECORD
+22 files, 39812 bytes uncompressed, 11249 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: agora_busclient/messages/request_msg.py
 Comment: 
 
 Filename: agora_busclient/messages/work_flow.py
 Comment: 
 
-Filename: agora_busclient-1.1.31.dist-info/LICENSE
+Filename: agora_busclient-1.1.32.dist-info/LICENSE
 Comment: 
 
-Filename: agora_busclient-1.1.31.dist-info/WHEEL
+Filename: agora_busclient-1.1.32.dist-info/WHEEL
 Comment: 
 
-Filename: agora_busclient-1.1.31.dist-info/METADATA
+Filename: agora_busclient-1.1.32.dist-info/METADATA
 Comment: 
 
-Filename: agora_busclient-1.1.31.dist-info/RECORD
+Filename: agora_busclient-1.1.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_busclient/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .bus_client import bus_client
 from .base_mqtt_client import BaseMqttClient
 from .mqtt_client import MqttClient
 from .messages import IoDataReportMsg, RequestMsg, \
-    IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg
+    IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg, MediaData, WorkFlow
```

## agora_busclient/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.31'
+__version__ = '1.1.32'
```

## agora_busclient/messages/msg_decoder.py

```diff
@@ -150,39 +150,65 @@
             if 'mediaData' in d:
                 for d in d['mediaData']:
                     ret.mediaDataRef.append(self.__decode(d, MediaData))
             if 'workFlow' in d:                                
                 ret.workFlow = self.__decode(d['workFlow'], WorkFlow)
             # if 'ZoneId' in d:
             #     ret.ZoneId = d['ZoneId']
-            if 'CameraId' in d:
-                ret.CameraId = d['CameraId']
+            # if 'CameraId' in d:
+            #     ret.CameraId = d['CameraId']
+            # try:
+            #     if 'MotTrackerId' in d:
+            #         ret.MotTrackerId = int(str(d['MotTrackerId']))
+            # except:
+            #     ret.MotTrackerId = -1            
+            # if 'EdgeFilename' in d:
+            #     ret.EdgeFilename = d['EdgeFilename']                     
+            # if 'MotEdgeFilename' in d:
+            #     ret.MotEdgeFilename = d['MotEdgeFilename']
+            # if 'MIMEType' in d:
+            #     ret.MIMEType = d['MIMEType']
+            # if 'AltText' in d:
+            #     ret.AltText = d['AltText']
+
             try:
-                if 'MotTrackerId' in d:
-                    ret.MotTrackerId = int(str(d['MotTrackerId']))
+                if 'Start_tm' in d:
+                    ret.Start_tm = float(str(d['Start_tm']))
             except:
-                ret.MotTrackerId = -1            
-            if 'EdgeFilename' in d:
-                ret.EdgeFilename = d['EdgeFilename']                     
-            if 'MotEdgeFilename' in d:
-                ret.MotEdgeFilename = d['MotEdgeFilename']
-            if 'MIMEType' in d:
-                ret.MIMEType = d['MIMEType']
-            if 'AltText' in d:
-                ret.AltText = d['AltText']
+                ret.Start_tm = -1
+            try:
+                if 'End_tm' in d:
+                    ret.End_tm = float(str(d['End_tm']))
+            except:
+                ret.End_tm = -1
             try:
                 if 'DetectedStart_tm' in d:
                     ret.DetectedStart_tm = float(str(d['DetectedStart_tm']))
             except:
                 ret.DetectedStart_tm = -1
             try:
                 if 'DetectedEnd_tm' in d:
                     ret.DetectedEnd_tm = float(str(d['DetectedEnd_tm']))
             except:
                 ret.DetectedEnd_tm = -1
+            try:
+                if 'Sent_tm' in d:
+                    ret.Sent_tm = float(str(d['Sent_tm']))
+            except:
+                ret.Sent_tm = -1
+            try:
+                if 'Created_tm' in d:
+                    ret.Created_tm = float(str(d['Created_tm']))
+            except:
+                ret.Created_tm = -1            
+            try:
+                if 'Detected_tm' in d:
+                    ret.Detected_tm = float(str(d['Detected_tm']))
+            except:
+                ret.Detected_tm = -1           
             if 'Version' in d:
                 ret.Version = d['Version']
             return ret
         if o == WorkFlow:           
             ret = WorkFlow()        
             try:
                 if 'Type' in d:
```

## agora_busclient/messages/msg_encoder.py

```diff
@@ -79,22 +79,28 @@
         elif isinstance(o, EventMsg):
             d = dict()            
             d['EventId'] = o.EventId
             d['GroupId'] = o.GroupId
             d['GatewayId'] = o.GatewayId
             d['ControllerId'] = o.ControllerId
             # d['ZoneId'] = o.ZoneId
-            d['CameraId'] = o.CameraId
-            d['MotTrackerId'] = o.MotTrackerId
-            d['EdgeFilename'] = o.EdgeFilename
-            d['MotEdgeFilename'] = o.MotEdgeFilename
-            d['MIMEType'] = o.MIMEType
-            d['AltText'] = o.AltText
+            # d['CameraId'] = o.CameraId
+            # d['MotTrackerId'] = o.MotTrackerId
+            # d['EdgeFilename'] = o.EdgeFilename
+            # d['MotEdgeFilename'] = o.MotEdgeFilename
+            # d['MIMEType'] = o.MIMEType
+            # d['AltText'] = o.AltText
+            d['Start_tm'] = int(o.Start_tm)
+            d['End_tm'] = int(o.End_tm)
             d['DetectedStart_tm'] = int(o.DetectedStart_tm)
-            d['DetectedEnd_tm'] = int(o.DetectedEnd_tm)
+            d['DetectedEnd_tm'] = int(o.DetectedEnd_tm)            
+            d['Sent_tm'] = int(o.Sent_tm)
+            d['Created_tm'] = int(o.Created_tm)
+            d['Detected_tm'] = int(o.Detected_tm)
+          
             lst = list()
             for mediaData in o.mediaData:
                 lst.append(self.default(mediaData))
             d['mediaData'] = lst            
             d['workFlow'] = o.WorkFlow
             d['Version'] = o.Version            
             return d
```

## Comparing `agora_busclient-1.1.31.dist-info/METADATA` & `agora_busclient-1.1.32.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: agora_busclient
-Version: 1.1.31
+Version: 1.1.32
 Summary: Bus Client libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.31
-Requires-Dist: agora_config == 1.1.31
-Requires-Dist: agora_utils == 1.1.31
+Requires-Dist: agora_logging == 1.1.32
+Requires-Dist: agora_config == 1.1.32
+Requires-Dist: agora_utils == 1.1.32
 Requires-Dist: paho-mqtt
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_busclient
 
  This package is the Bus Client library for the Agora Edge Apps SDK (Python) developed by SLB.
```

## Comparing `agora_busclient-1.1.31.dist-info/RECORD` & `agora_busclient-1.1.32.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-agora_busclient/__init__.py,sha256=UamGaY7znMO5n1XEUhOEGO43HJhBHKSUUM7Nqqkxsic,240
+agora_busclient/__init__.py,sha256=u5C1uUUYJLFPg8rdFdLLUBkNZjPznbShJPz_6k7T8nc,261
 agora_busclient/base_mqtt_client.py,sha256=3TOsWL_LOfnxtj73slPj-L3I1kqc1niqW3C_m8tuSjQ,2974
 agora_busclient/bus_client.py,sha256=9SypfvNAuv_Tct1uwDMgj7dg-BdoLvk3aEWi2FpTPS0,3220
 agora_busclient/message_queue.py,sha256=l5L6PQoF_OQU8Ed0ZKKk-ZEwSBaCOOAajuHQ1fdaxiI,4267
 agora_busclient/mqtt_client.py,sha256=I87pojxwhaAzIrjU1HSlXOL2XkK8m-YCT2SD9mFYEFU,5115
-agora_busclient/version.py,sha256=m6Gwb-2J7qH0YItWdRx6poaAJYM2sVamUx_y8wEEcbI,25
+agora_busclient/version.py,sha256=g0EmYAMzvboJ32TdMNLZcoLdC3TIhGHXLgf4Ivquuds,25
 agora_busclient/messages/__init__.py,sha256=SXI28GSrnaOZxDpXYqH4emANTRWlGDjvKVsClgtQGqw,432
 agora_busclient/messages/event_msg.py,sha256=55cfh04jB9CeuIUZRlnUwb9wY9ijSbjtpkpJHKUmO0Y,1693
 agora_busclient/messages/io_device_data.py,sha256=6-IyVdps8AquyivHUzS5LU4iIpIMIxBSdmOWZ1l187E,233
 agora_busclient/messages/io_point.py,sha256=J9nqULZ09fQxUneB1zcXNk5poOR7Uf9JwqkwrlQkFe8,678
 agora_busclient/messages/io_tag_data_dict.py,sha256=1-hmLr6RTtkeHdqfr7A8kGom3ZxkC8lHOfw3yDHk2ic,565
 agora_busclient/messages/iodatareport_message.py,sha256=u3ckr4Wx8qk-ce2pNcd6D3nBIJ09YrBlid57V1BKe1A,1918
 agora_busclient/messages/media_data.py,sha256=qjPR53XXC3WHEJeAiobNm0zeGr3dwrDI7RHBABtnga8,950
 agora_busclient/messages/message_header.py,sha256=Hk0slDisem-mIlpeosHpj1AxNSQqz7uerH8yUj6_-Jw,799
-agora_busclient/messages/msg_decoder.py,sha256=wfQdtscxnUqE82S3f884UF3-8ghaUBXFNLZSNVmP6dY,7572
-agora_busclient/messages/msg_encoder.py,sha256=0aHrvSLMbXxy8AsjXNoRqJtx5wGvCqrUSsBOrHTih54,3851
+agora_busclient/messages/msg_decoder.py,sha256=xxZablnORrNESre3l9zZB_Dudshqcy743FiHRw6dKyY,8500
+agora_busclient/messages/msg_encoder.py,sha256=gN3XFVUgatFlFaDnNZIP6mfj6yYW9UqAs1bPTLqoMU4,4116
 agora_busclient/messages/request_msg.py,sha256=LdtaEHkf2M4aA0I-XILzw9EQK0XNPi3H7M_O2z3AuMs,581
 agora_busclient/messages/work_flow.py,sha256=u1a7i4Inins3w9qThnz4CUkB-eYp6mkVsukJqr9x-n8,129
-agora_busclient-1.1.31.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_busclient-1.1.31.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_busclient-1.1.31.dist-info/METADATA,sha256=CfRZR5n78EbutsvNY12A7KHdVwpJsAWP00hEVFgb0c0,1123
-agora_busclient-1.1.31.dist-info/RECORD,,
+agora_busclient-1.1.32.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_busclient-1.1.32.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_busclient-1.1.32.dist-info/METADATA,sha256=C21xMOPnorfI_Frno3kpPs_2Yus4Cv5JU6LM_I-Ghks,1123
+agora_busclient-1.1.32.dist-info/RECORD,,
```

