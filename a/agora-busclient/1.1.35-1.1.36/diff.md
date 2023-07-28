# Comparing `tmp/agora_busclient-1.1.35-py2.py3-none-any.whl.zip` & `tmp/agora_busclient-1.1.36-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 14563 bytes, number of entries: 22
+Zip file size: 14462 bytes, number of entries: 22
 -rw-r--r--  2.0 fat      261 b- defN 23-Jul-28 12:34 agora_busclient/__init__.py
 -rw-r--r--  2.0 fat     2974 b- defN 23-Jul-27 15:56 agora_busclient/base_mqtt_client.py
 -rw-r--r--  2.0 fat     3220 b- defN 23-Jul-27 16:58 agora_busclient/bus_client.py
 -rw-r--r--  2.0 fat     4267 b- defN 23-Jul-28 10:49 agora_busclient/message_queue.py
 -rw-r--r--  2.0 fat     5115 b- defN 23-May-19 17:55 agora_busclient/mqtt_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 16:38 agora_busclient/version.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 19:32 agora_busclient/version.py
 -rw-r--r--  2.0 fat      432 b- defN 23-Jul-10 22:39 agora_busclient/messages/__init__.py
 -rw-r--r--  2.0 fat     1693 b- defN 23-Jul-27 17:21 agora_busclient/messages/event_msg.py
 -rw-r--r--  2.0 fat      233 b- defN 23-May-12 13:38 agora_busclient/messages/io_device_data.py
 -rw-r--r--  2.0 fat      678 b- defN 23-May-12 13:38 agora_busclient/messages/io_point.py
 -rw-r--r--  2.0 fat      565 b- defN 23-May-12 13:38 agora_busclient/messages/io_tag_data_dict.py
 -rw-r--r--  2.0 fat     1918 b- defN 23-May-12 13:38 agora_busclient/messages/iodatareport_message.py
 -rw-r--r--  2.0 fat      950 b- defN 23-Jul-27 17:24 agora_busclient/messages/media_data.py
 -rw-r--r--  2.0 fat      799 b- defN 23-May-12 13:38 agora_busclient/messages/message_header.py
--rw-r--r--  2.0 fat     8051 b- defN 23-Jul-28 16:35 agora_busclient/messages/msg_decoder.py
--rw-r--r--  2.0 fat     4122 b- defN 23-Jul-28 14:42 agora_busclient/messages/msg_encoder.py
+-rw-r--r--  2.0 fat     7575 b- defN 23-Jul-28 16:47 agora_busclient/messages/msg_decoder.py
+-rw-r--r--  2.0 fat     3811 b- defN 23-Jul-28 19:31 agora_busclient/messages/msg_encoder.py
 -rw-r--r--  2.0 fat      581 b- defN 23-May-12 13:38 agora_busclient/messages/request_msg.py
 -rw-r--r--  2.0 fat      129 b- defN 23-Jul-11 16:30 agora_busclient/messages/work_flow.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.35.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.35.dist-info/WHEEL
--rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.35.dist-info/METADATA
--rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.35.dist-info/RECORD
-22 files, 39369 bytes uncompressed, 11241 bytes compressed:  71.4%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.36.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.36.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.36.dist-info/METADATA
+-rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.36.dist-info/RECORD
+22 files, 38582 bytes uncompressed, 11140 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: agora_busclient/messages/request_msg.py
 Comment: 
 
 Filename: agora_busclient/messages/work_flow.py
 Comment: 
 
-Filename: agora_busclient-1.1.35.dist-info/LICENSE
+Filename: agora_busclient-1.1.36.dist-info/LICENSE
 Comment: 
 
-Filename: agora_busclient-1.1.35.dist-info/WHEEL
+Filename: agora_busclient-1.1.36.dist-info/WHEEL
 Comment: 
 
-Filename: agora_busclient-1.1.35.dist-info/METADATA
+Filename: agora_busclient-1.1.36.dist-info/METADATA
 Comment: 
 
-Filename: agora_busclient-1.1.35.dist-info/RECORD
+Filename: agora_busclient-1.1.36.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_busclient/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.35'
+__version__ = '1.1.36'
```

## agora_busclient/messages/msg_decoder.py

```diff
@@ -188,19 +188,8 @@
             try:
                 if 'Detected_tm' in d:
                     ret.Detected_tm = float(str(d['Detected_tm']))
             except:
                 ret.Detected_tm = -1           
             if 'Version' in d:
                 ret.Version = d['Version']
-            return ret
-        # if o == WorkFlow:                       
-        #     ret = WorkFlow()        
-        #     try:
-        #         if 'Type' in d:
-        #             ret.Type = d['Type']     
-        #         if 'Properties' in d:
-        #             ret.Properties = d['Properties']
-        #     except Exception as e:
-        #         logger.exception(
-        #             e, f"Cannot decode WorkFlow with 'Type' of '{d['Type']}'")
-        #     return ret
+            return ret
```

## agora_busclient/messages/msg_encoder.py

```diff
@@ -77,31 +77,24 @@
             d['DetectedEnd_tm'] = int(o.DetectedEnd_tm)
             return d
         elif isinstance(o, EventMsg):
             d = dict()            
             d['EventId'] = o.EventId
             d['GroupId'] = o.GroupId
             d['GatewayId'] = o.GatewayId
-            d['ControllerId'] = o.ControllerId
-            # d['ZoneId'] = o.ZoneId
-            # d['CameraId'] = o.CameraId
-            # d['MotTrackerId'] = o.MotTrackerId
-            # d['EdgeFilename'] = o.EdgeFilename
-            # d['MotEdgeFilename'] = o.MotEdgeFilename
-            # d['MIMEType'] = o.MIMEType
-            # d['AltText'] = o.AltText
+            d['ControllerId'] = o.ControllerId          
             d['Start_tm'] = int(o.Start_tm)
             d['End_tm'] = int(o.End_tm)
             d['DetectedStart_tm'] = int(o.DetectedStart_tm)
             d['DetectedEnd_tm'] = int(o.DetectedEnd_tm)            
             d['Sent_tm'] = int(o.Sent_tm)
             d['Created_tm'] = int(o.Created_tm)
             d['Detected_tm'] = int(o.Detected_tm)
           
             lst = list()
             for mediaData in o.mediaDataRef:
                 lst.append(self.default(mediaData))
-            d['mediaDataRef'] = lst            
+            d['mediaData'] = lst            
             d['workFlow'] = o.workFlow
             d['Version'] = o.Version            
             return d
         return super().default(o)
```

## Comparing `agora_busclient-1.1.35.dist-info/METADATA` & `agora_busclient-1.1.36.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: agora_busclient
-Version: 1.1.35
+Version: 1.1.36
 Summary: Bus Client libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.35
-Requires-Dist: agora_config == 1.1.35
-Requires-Dist: agora_utils == 1.1.35
+Requires-Dist: agora_logging == 1.1.36
+Requires-Dist: agora_config == 1.1.36
+Requires-Dist: agora_utils == 1.1.36
 Requires-Dist: paho-mqtt
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_busclient
 
  This package is the Bus Client library for the Agora Edge Apps SDK (Python) developed by SLB.
```

## Comparing `agora_busclient-1.1.35.dist-info/RECORD` & `agora_busclient-1.1.36.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agora_busclient/__init__.py,sha256=u5C1uUUYJLFPg8rdFdLLUBkNZjPznbShJPz_6k7T8nc,261
 agora_busclient/base_mqtt_client.py,sha256=3TOsWL_LOfnxtj73slPj-L3I1kqc1niqW3C_m8tuSjQ,2974
 agora_busclient/bus_client.py,sha256=9SypfvNAuv_Tct1uwDMgj7dg-BdoLvk3aEWi2FpTPS0,3220
 agora_busclient/message_queue.py,sha256=l5L6PQoF_OQU8Ed0ZKKk-ZEwSBaCOOAajuHQ1fdaxiI,4267
 agora_busclient/mqtt_client.py,sha256=I87pojxwhaAzIrjU1HSlXOL2XkK8m-YCT2SD9mFYEFU,5115
-agora_busclient/version.py,sha256=E2ul4vbaQXGiyEzHol15bobIMzs_borOossos6CNFVw,25
+agora_busclient/version.py,sha256=A1T3nFjNgan8hUUu6uBJkXNVFhN1WwzflM-VtP30JjY,25
 agora_busclient/messages/__init__.py,sha256=SXI28GSrnaOZxDpXYqH4emANTRWlGDjvKVsClgtQGqw,432
 agora_busclient/messages/event_msg.py,sha256=55cfh04jB9CeuIUZRlnUwb9wY9ijSbjtpkpJHKUmO0Y,1693
 agora_busclient/messages/io_device_data.py,sha256=6-IyVdps8AquyivHUzS5LU4iIpIMIxBSdmOWZ1l187E,233
 agora_busclient/messages/io_point.py,sha256=J9nqULZ09fQxUneB1zcXNk5poOR7Uf9JwqkwrlQkFe8,678
 agora_busclient/messages/io_tag_data_dict.py,sha256=1-hmLr6RTtkeHdqfr7A8kGom3ZxkC8lHOfw3yDHk2ic,565
 agora_busclient/messages/iodatareport_message.py,sha256=u3ckr4Wx8qk-ce2pNcd6D3nBIJ09YrBlid57V1BKe1A,1918
 agora_busclient/messages/media_data.py,sha256=qjPR53XXC3WHEJeAiobNm0zeGr3dwrDI7RHBABtnga8,950
 agora_busclient/messages/message_header.py,sha256=Hk0slDisem-mIlpeosHpj1AxNSQqz7uerH8yUj6_-Jw,799
-agora_busclient/messages/msg_decoder.py,sha256=wDHe7hnBayE7H26qHcF8Jt28NuSC361k_HcNCusOJyc,8051
-agora_busclient/messages/msg_encoder.py,sha256=ktPlVM4eLG44wZ56PKSuJ9iNJVgBzm9v-2qehqwqG0g,4122
+agora_busclient/messages/msg_decoder.py,sha256=MapLMBRtpY_h_QSjN5ivlmKI_5uNNyGMmoitNYGD6Zw,7575
+agora_busclient/messages/msg_encoder.py,sha256=9yjGbLTfxIhsX4R3vJnNSKRsmf-GnROw7qaQpDm8lUQ,3811
 agora_busclient/messages/request_msg.py,sha256=LdtaEHkf2M4aA0I-XILzw9EQK0XNPi3H7M_O2z3AuMs,581
 agora_busclient/messages/work_flow.py,sha256=u1a7i4Inins3w9qThnz4CUkB-eYp6mkVsukJqr9x-n8,129
-agora_busclient-1.1.35.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_busclient-1.1.35.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_busclient-1.1.35.dist-info/METADATA,sha256=d-dVtOz2Uek0ScPdSwQ6pBeva68IpWgdQXbLlGGyfHI,1123
-agora_busclient-1.1.35.dist-info/RECORD,,
+agora_busclient-1.1.36.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_busclient-1.1.36.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_busclient-1.1.36.dist-info/METADATA,sha256=Bvq3IE8gXWfrUEcXL7hhtKl41aaThJIFRI_15Dgz7Gg,1123
+agora_busclient-1.1.36.dist-info/RECORD,,
```

