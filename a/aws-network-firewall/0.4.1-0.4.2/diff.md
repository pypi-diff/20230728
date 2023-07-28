# Comparing `tmp/aws_network_firewall-0.4.1.tar.gz` & `tmp/aws_network_firewall-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.4.1.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.4.2.tar", max compression
```

## Comparing `aws_network_firewall-0.4.1.tar` & `aws_network_firewall-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11335 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/README.md
--rw-r--r--   0        0        0       22 2023-07-26 15:40:44.873654 aws_network_firewall-0.4.1/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-26 15:40:43.921648 aws_network_firewall-0.4.1/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      589 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     3210 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1994 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2680 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      474 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1812 2023-07-26 15:40:43.925648 aws_network_firewall-0.4.1/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-26 15:40:44.873654 aws_network_firewall-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-28 12:31:40.242970 aws_network_firewall-0.4.2/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      589 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     3325 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     1994 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2680 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-28 12:31:39.402967 aws_network_firewall-0.4.2/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      474 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1812 2023-07-28 12:31:39.406967 aws_network_firewall-0.4.2/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-28 12:31:40.242970 aws_network_firewall-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.4.2/PKG-INFO
```

### Comparing `aws_network_firewall-0.4.1/LICENSE.txt` & `aws_network_firewall-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/README.md` & `aws_network_firewall-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/account.py` & `aws_network_firewall-0.4.2/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.4.2/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.4.2/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/destination.py` & `aws_network_firewall-0.4.2/aws_network_firewall/destination.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.4.2/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/rule.py` & `aws_network_firewall-0.4.2/aws_network_firewall/rule.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         return list(filter(None, map(convert_source, self.sources)))
 
     @staticmethod
     def __tls_endpoint_options(endpoint: str) -> List[SuricataOption]:
         options = [
             SuricataOption(name="tls.sni"),
             SuricataOption(name="tls.version", value="1.2", quoted_value=False),
-            SuricataOption(name="tls.version", value="1.3", quoted_value=False),
+            # When using multiple tls versions you need 2 rules
+            # openssl 1.1.1 is needed for tls1.3
+            # SuricataOption(name="tls.version", value="1.3", quoted_value=False),
         ]
 
         if endpoint.startswith("*"):
             options += [
                 SuricataOption(name="dotprefix"),
                 SuricataOption(name="content", value=endpoint[1:]),
                 SuricataOption(name="nocase"),
```

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.4.2/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.4.2/aws_network_firewall/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.4.2/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.4.1/pyproject.toml` & `aws_network_firewall-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.4.1/PKG-INFO` & `aws_network_firewall-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

