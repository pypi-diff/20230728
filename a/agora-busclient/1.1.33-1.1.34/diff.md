# Comparing `tmp/agora_busclient-1.1.33-py2.py3-none-any.whl.zip` & `tmp/agora_busclient-1.1.34-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 14582 bytes, number of entries: 22
+Zip file size: 14573 bytes, number of entries: 22
 -rw-r--r--  2.0 fat      261 b- defN 23-Jul-28 12:34 agora_busclient/__init__.py
 -rw-r--r--  2.0 fat     2974 b- defN 23-Jul-27 15:56 agora_busclient/base_mqtt_client.py
 -rw-r--r--  2.0 fat     3220 b- defN 23-Jul-27 16:58 agora_busclient/bus_client.py
 -rw-r--r--  2.0 fat     4267 b- defN 23-Jul-28 10:49 agora_busclient/message_queue.py
 -rw-r--r--  2.0 fat     5115 b- defN 23-May-19 17:55 agora_busclient/mqtt_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 13:00 agora_busclient/version.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 13:30 agora_busclient/version.py
 -rw-r--r--  2.0 fat      432 b- defN 23-Jul-10 22:39 agora_busclient/messages/__init__.py
 -rw-r--r--  2.0 fat     1693 b- defN 23-Jul-27 17:21 agora_busclient/messages/event_msg.py
 -rw-r--r--  2.0 fat      233 b- defN 23-May-12 13:38 agora_busclient/messages/io_device_data.py
 -rw-r--r--  2.0 fat      678 b- defN 23-May-12 13:38 agora_busclient/messages/io_point.py
 -rw-r--r--  2.0 fat      565 b- defN 23-May-12 13:38 agora_busclient/messages/io_tag_data_dict.py
 -rw-r--r--  2.0 fat     1918 b- defN 23-May-12 13:38 agora_busclient/messages/iodatareport_message.py
 -rw-r--r--  2.0 fat      950 b- defN 23-Jul-27 17:24 agora_busclient/messages/media_data.py
 -rw-r--r--  2.0 fat      799 b- defN 23-May-12 13:38 agora_busclient/messages/message_header.py
--rw-r--r--  2.0 fat     8526 b- defN 23-Jul-28 12:59 agora_busclient/messages/msg_decoder.py
--rw-r--r--  2.0 fat     4122 b- defN 23-Jul-28 12:41 agora_busclient/messages/msg_encoder.py
+-rw-r--r--  2.0 fat     8516 b- defN 23-Jul-28 13:29 agora_busclient/messages/msg_decoder.py
+-rw-r--r--  2.0 fat     4122 b- defN 23-Jul-28 13:26 agora_busclient/messages/msg_encoder.py
 -rw-r--r--  2.0 fat      581 b- defN 23-May-12 13:38 agora_busclient/messages/request_msg.py
 -rw-r--r--  2.0 fat      129 b- defN 23-Jul-11 16:30 agora_busclient/messages/work_flow.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.33.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.33.dist-info/WHEEL
--rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.33.dist-info/METADATA
--rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.33.dist-info/RECORD
-22 files, 39844 bytes uncompressed, 11260 bytes compressed:  71.7%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.34.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.34.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.34.dist-info/METADATA
+-rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.34.dist-info/RECORD
+22 files, 39834 bytes uncompressed, 11251 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: agora_busclient/messages/request_msg.py
 Comment: 
 
 Filename: agora_busclient/messages/work_flow.py
 Comment: 
 
-Filename: agora_busclient-1.1.33.dist-info/LICENSE
+Filename: agora_busclient-1.1.34.dist-info/LICENSE
 Comment: 
 
-Filename: agora_busclient-1.1.33.dist-info/WHEEL
+Filename: agora_busclient-1.1.34.dist-info/WHEEL
 Comment: 
 
-Filename: agora_busclient-1.1.33.dist-info/METADATA
+Filename: agora_busclient-1.1.34.dist-info/METADATA
 Comment: 
 
-Filename: agora_busclient-1.1.33.dist-info/RECORD
+Filename: agora_busclient-1.1.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_busclient/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.33'
+__version__ = '1.1.34'
```

## agora_busclient/messages/msg_decoder.py

```diff
@@ -204,19 +204,18 @@
                 if 'Detected_tm' in d:
                     ret.Detected_tm = float(str(d['Detected_tm']))
             except:
                 ret.Detected_tm = -1           
             if 'Version' in d:
                 ret.Version = d['Version']
             return ret
-        if o == WorkFlow:           
-            print(d)
+        if o == WorkFlow:                       
             ret = WorkFlow()        
             try:
                 if 'Type' in d:
                     ret.Type = d['Type']     
                 if 'Properties' in d:
-                    ret.properties = d['Properties']
+                    ret.Properties = d['Properties']
             except Exception as e:
                 logger.exception(
                     e, f"Cannot decode WorkFlow with 'Type' of '{d['Type']}'")
             return ret
```

## agora_busclient/messages/msg_encoder.py

```diff
@@ -55,17 +55,17 @@
             for device in o.device:
                 lst.append(self.default(device))
             d['device'] = lst
             d['response'] = o.response
             return d
         elif isinstance(o, WorkFlow):
             d = dict()         
-            d['properties'] = o.properties         
+            d['Properties'] = o.Properties         
             if o.type != None:
-                d['type'] = o.type               
+                d['Type'] = o.Type               
             return d
         elif isinstance(o, MediaData):
             d = dict()
             d['Id'] = o.Id
             d['ZoneId'] = o.ZoneId
             d['CameraId'] = o.CameraId
             d['MotTrackerId'] = o.MotTrackerId
@@ -97,11 +97,11 @@
             d['Created_tm'] = int(o.Created_tm)
             d['Detected_tm'] = int(o.Detected_tm)
           
             lst = list()
             for mediaData in o.mediaDataRef:
                 lst.append(self.default(mediaData))
             d['mediaDataRef'] = lst            
-            d['workFlow'] = o.WorkFlow
+            d['workFlow'] = o.workFlow
             d['Version'] = o.Version            
             return d
         return super().default(o)
```

## Comparing `agora_busclient-1.1.33.dist-info/RECORD` & `agora_busclient-1.1.34.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agora_busclient/__init__.py,sha256=u5C1uUUYJLFPg8rdFdLLUBkNZjPznbShJPz_6k7T8nc,261
 agora_busclient/base_mqtt_client.py,sha256=3TOsWL_LOfnxtj73slPj-L3I1kqc1niqW3C_m8tuSjQ,2974
 agora_busclient/bus_client.py,sha256=9SypfvNAuv_Tct1uwDMgj7dg-BdoLvk3aEWi2FpTPS0,3220
 agora_busclient/message_queue.py,sha256=l5L6PQoF_OQU8Ed0ZKKk-ZEwSBaCOOAajuHQ1fdaxiI,4267
 agora_busclient/mqtt_client.py,sha256=I87pojxwhaAzIrjU1HSlXOL2XkK8m-YCT2SD9mFYEFU,5115
-agora_busclient/version.py,sha256=EScuLwcq-3hy2HikwoaxRp9r-IW-958r6RvFXuDxof4,25
+agora_busclient/version.py,sha256=__M-p52YVK0wENk52iWt5ZNTtYNC5XyWOlrQ3P8OVMU,25
 agora_busclient/messages/__init__.py,sha256=SXI28GSrnaOZxDpXYqH4emANTRWlGDjvKVsClgtQGqw,432
 agora_busclient/messages/event_msg.py,sha256=55cfh04jB9CeuIUZRlnUwb9wY9ijSbjtpkpJHKUmO0Y,1693
 agora_busclient/messages/io_device_data.py,sha256=6-IyVdps8AquyivHUzS5LU4iIpIMIxBSdmOWZ1l187E,233
 agora_busclient/messages/io_point.py,sha256=J9nqULZ09fQxUneB1zcXNk5poOR7Uf9JwqkwrlQkFe8,678
 agora_busclient/messages/io_tag_data_dict.py,sha256=1-hmLr6RTtkeHdqfr7A8kGom3ZxkC8lHOfw3yDHk2ic,565
 agora_busclient/messages/iodatareport_message.py,sha256=u3ckr4Wx8qk-ce2pNcd6D3nBIJ09YrBlid57V1BKe1A,1918
 agora_busclient/messages/media_data.py,sha256=qjPR53XXC3WHEJeAiobNm0zeGr3dwrDI7RHBABtnga8,950
 agora_busclient/messages/message_header.py,sha256=Hk0slDisem-mIlpeosHpj1AxNSQqz7uerH8yUj6_-Jw,799
-agora_busclient/messages/msg_decoder.py,sha256=8XeMP4kSFuUNobEWECnn3s43RB_3BMmPWvUFH6Tls6w,8526
-agora_busclient/messages/msg_encoder.py,sha256=fGJoumGIkAVWRw1FXhuXMGtHkFWKWJP0BcijGJ6fRV4,4122
+agora_busclient/messages/msg_decoder.py,sha256=t6X3l6LOWkl6__bae5IDGWD_mxJhHM-pF0uRp96vVwc,8516
+agora_busclient/messages/msg_encoder.py,sha256=Bvz0Q7_l9Cu7EARN8QxMnl0c6NnJl6sBnO1NB0j0pEc,4122
 agora_busclient/messages/request_msg.py,sha256=LdtaEHkf2M4aA0I-XILzw9EQK0XNPi3H7M_O2z3AuMs,581
 agora_busclient/messages/work_flow.py,sha256=u1a7i4Inins3w9qThnz4CUkB-eYp6mkVsukJqr9x-n8,129
-agora_busclient-1.1.33.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_busclient-1.1.33.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_busclient-1.1.33.dist-info/METADATA,sha256=5jKr7S8KVN9DfJlofMFcpNM9R1f9II8DzqdORqPpOUM,1123
-agora_busclient-1.1.33.dist-info/RECORD,,
+agora_busclient-1.1.34.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_busclient-1.1.34.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_busclient-1.1.34.dist-info/METADATA,sha256=Msa2qPQsNM-CHtKi9AjQyQ5CXNe52UEvKHP6k-iOYRU,1123
+agora_busclient-1.1.34.dist-info/RECORD,,
```

