# Comparing `tmp/aws_network_firewall-0.4.2.tar.gz` & `tmp/aws_network_firewall-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.4.2.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.5.0.tar", max compression
```

## Comparing `aws_network_firewall-0.4.2.tar` & `aws_network_firewall-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11335 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/README.md
--rw-r--r--   0        0        0       22 2023-07-28 12:31:40.242970 aws_network_firewall-0.4.2/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      589 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     3325 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1994 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2680 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      474 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1812 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-28 12:31:40.242970 aws_network_firewall-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 13:28:50.864131 aws_network_firewall-0.5.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      616 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     3485 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     2032 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2716 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1812 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-28 13:28:50.868131 aws_network_firewall-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.5.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.4.2/LICENSE.txt` & `aws_network_firewall-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/README.md` & `aws_network_firewall-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/account.py` & `aws_network_firewall-0.5.0/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.5.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/destination.py` & `aws_network_firewall-0.5.0/aws_network_firewall/destination.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 
     description: str
     protocol: str
     port: Optional[int]
     endpoint: Optional[str]
     region: Optional[str]
     cidr: Optional[str]
+    message: Optional[str]
 
     def resolve_region_cidr_ranges(self, ranges: CidrRanges) -> None:
         if self.region and not self.cidr:
             cidr = ranges.by_region(self.region)
             self.cidr = cidr.value if cidr else None
```

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.5.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/rule.py` & `aws_network_firewall-0.5.0/aws_network_firewall/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,22 @@
 
     def __resolve_options(self, destination: Destination) -> List[SuricataOption]:
         options = []
 
         if destination.protocol == "TLS" and destination.endpoint:
             options = self.__tls_endpoint_options(destination.endpoint)
 
+        message = (
+            f"{destination.message} | {self.workload} | {self.name}"
+            if destination.message
+            else f"{self.workload} | {self.name}"
+        )
+
         return options + [
-            SuricataOption(name="msg", value=f"{self.workload} | {self.name}"),
+            SuricataOption(name="msg", value=message),
             SuricataOption(name="rev", value="1", quoted_value=False),
             SuricataOption(name="sid", value="XXX", quoted_value=False),
         ]
 
     def __resolve_rule(self, destination: Destination) -> SuricataRule:
         return SuricataRule(
             action="pass",
```

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.5.0/aws_network_firewall/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     return Destination(
         description=entry["Description"],
         protocol=entry["Protocol"],
         port=entry.get("Port"),
         endpoint=entry.get("Endpoint"),
         region=entry.get("Region"),
         cidr=entry.get("Cidr"),
+        message=entry.get("Message"),
     )
 
 
 def rule_resolver(workload: str, entry: dict) -> Rule:
     return Rule(
         workload=workload,
         type=entry["Type"],
```

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.5.0/aws_network_firewall/schemas/environment.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,16 @@
         type: string
       Region:
         type: string
       Protocol:
         enum: [ "TCP", "TLS", "ICMP" ]
       Port:
         type: integer
+      Message:
+        type: string
     examples:
       - Description: Website of Xebia
         Protocol: TLS
         Endpoint: xebia.com
         Region: eu-central-1
         Port: 443
```

### Comparing `aws_network_firewall-0.4.2/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.5.0/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.2/pyproject.toml` & `aws_network_firewall-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.4.2"
+version = "0.5.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.4.2/PKG-INFO` & `aws_network_firewall-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.4.2
+Version: 0.5.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

