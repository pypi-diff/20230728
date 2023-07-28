# Comparing `tmp/aws_network_firewall-0.5.0.tar.gz` & `tmp/aws_network_firewall-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.5.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.6.0.tar", max compression
```

## Comparing `aws_network_firewall-0.5.0.tar` & `aws_network_firewall-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    11335 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-07-28 13:28:50.864131 aws_network_firewall-0.5.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      616 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     3485 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     2032 2023-07-28 13:28:50.024129 aws_network_firewall-0.5.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2716 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1812 2023-07-28 13:28:50.028129 aws_network_firewall-0.5.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-28 13:28:50.868131 aws_network_firewall-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 17:35:51.650500 aws_network_firewall-0.6.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      318 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     3501 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     1992 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2673 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1812 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-28 17:35:51.650500 aws_network_firewall-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.6.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.5.0/LICENSE.txt` & `aws_network_firewall-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/README.md` & `aws_network_firewall-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/account.py` & `aws_network_firewall-0.6.0/aws_network_firewall/account.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from __future__ import annotations
-from typing import List, Optional
+
+import itertools
+from typing import List, Union
 from landingzone_organization import Account as LandingZoneAccount
 from aws_network_firewall.cidr_ranges import CidrRanges
+from aws_network_firewall.destination import Destination
 from aws_network_firewall.rule import Rule
+from aws_network_firewall.rule_set import RuleSet
+from aws_network_firewall.source import Source
 
 
 class Account(LandingZoneAccount):
-    __rules: List[Rule]
+    __rules: RuleSet
     __cidr_ranges: CidrRanges
 
     def __init__(
         self, name: str, account_id: str, cidr_ranges: CidrRanges, rules: List[Rule]
     ) -> None:
         super().__init__(name, account_id)
         self.__cidr_ranges = cidr_ranges
-        self.__rules = list(map(self.__enrich_rule, rules))
+        self.__rules = RuleSet(rules=list(map(self.__enrich_rule, rules)))
 
     def __enrich_rule(self, rule: Rule) -> Rule:
-        list(
-            map(
-                lambda source: source.resolve_region_cidr_ranges(self.__cidr_ranges),
-                rule.sources,
-            )
-        )
-        list(
-            map(
-                lambda destination: destination.resolve_region_cidr_ranges(
-                    self.__cidr_ranges
-                ),
-                rule.destinations,
-            )
-        )
+        cidr_range = self.__cidr_ranges.by_region(rule.region)
+
+        def update_cidr_if_not_set(entry: Source) -> None:
+            if cidr_range and not entry.cidr:
+                entry.cidr = cidr_range.value
+
+        list(map(update_cidr_if_not_set, rule.sources))
 
         return rule
 
     @property
-    def rules(self) -> List[Rule]:
+    def regions(self) -> List[str]:
+        return list(set(filter(None, map(lambda rule: rule.region, self.rules.all))))
+
+    def rules_by_region(self, region: str) -> RuleSet:
+        return RuleSet(
+            rules=list(filter(lambda rule: region == rule.region, self.rules.all))
+        )
+
+    @property
+    def rules(self) -> RuleSet:
         return self.__rules
 
     @property
     def inspection_rules(self) -> List[Rule]:
-        return list(filter(lambda rule: rule.is_inspection_rule, self.rules))
+        return list(filter(lambda rule: rule.is_inspection_rule, self.rules.all))
 
     @property
     def egress_rules(self) -> List[Rule]:
-        return list(filter(lambda rule: rule.is_egress_rule, self.rules))
+        return list(filter(lambda rule: rule.is_egress_rule, self.rules.all))
```

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.6.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.6.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/rule.py` & `aws_network_firewall-0.6.0/aws_network_firewall/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     """
     Understands a rule
     """
 
     workload: str
     name: str
     type: str
+    region: str
     description: str
     sources: List[Source]
     destinations: List[Destination]
 
     INSPECTION: ClassVar[str] = "Inspection"
     EGRESS: ClassVar[str] = "Egress"
```

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.6.0/aws_network_firewall/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,33 @@
 EnvironmentSchema = load_schema(os.path.join(schema_path, "environment.yaml"))
 
 
 def source_resolver(entry: dict) -> Source:
     return Source(
         description=entry["Description"],
         cidr=entry.get("Cidr"),
-        region=entry.get("Region"),
     )
 
 
 def destination_resolver(entry: dict) -> Destination:
     return Destination(
         description=entry["Description"],
         protocol=entry["Protocol"],
         port=entry.get("Port"),
         endpoint=entry.get("Endpoint"),
-        region=entry.get("Region"),
         cidr=entry.get("Cidr"),
         message=entry.get("Message"),
     )
 
 
 def rule_resolver(workload: str, entry: dict) -> Rule:
     return Rule(
         workload=workload,
         type=entry["Type"],
+        region=entry["Region"],
         name=entry["Name"],
         description=entry["Description"],
         sources=list(map(source_resolver, entry["Sources"])),
         destinations=list(map(destination_resolver, entry["Destinations"])),
     )
```

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.6.0/aws_network_firewall/schemas/environment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,27 @@
 definitions:
   Rule:
     type: object
     additionalProperties: False
     required:
       - Name
       - Type
+      - Region
       - Description
       - Sources
       - Destinations
     properties:
       Name:
         type: string
       Type:
         enum: [ "Egress", "Inspection" ]
       Description:
         type: string
+      Region:
+        type: string
       Sources:
         type: array
         items:
           $ref: "#/definitions/Source"
       Destinations:
         type: array
         items:
@@ -74,35 +77,32 @@
     required:
       - Description
     properties:
       Description:
         type: string
       Cidr:
         type: string
-      Region:
-        type: string
     examples:
       - Description: Allow access from `10.0.0.0/8` to the defined destinations.
         Cidr: 10.0.0.0/8
       - Description: Allow access from `eu-central-1` to the defined destinations.
         Region: eu-central-1
 
   Destination:
     type: object
     additionalProperties: False
     required:
       - Description
       - Protocol
     anyOf:
+      - required: ["Endpoint", "Cidr"]
       - required: ["Endpoint"]
-        not: { required: ["Region", "Cidr"] }
+        not: { required: ["Cidr"] }
       - required: ["Cidr"]
-        not: { required: ["Endpoint", "Region"] }
-      - required: ["Region"]
-        not: { required: ["Endpoint", "Cidr"] }
+        not: { required: ["Endpoint"] }
 #      Port is not required when Protocol is ICMP
     properties:
       Description:
         type: string
       Endpoint:
         type: string
       Cidr:
```

### Comparing `aws_network_firewall-0.5.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.6.0/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.5.0/pyproject.toml` & `aws_network_firewall-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.5.0/PKG-INFO` & `aws_network_firewall-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

