# Comparing `tmp/dbl_discoverx-0.0.3.tar.gz` & `tmp/dbl_discoverx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbl_discoverx-0.0.3.tar", last modified: Wed Jul  5 14:35:20 2023, max compression
+gzip compressed data, was "dbl_discoverx-0.0.4.tar", last modified: Fri Jul 28 11:53:47 2023, max compression
```

## Comparing `dbl_discoverx-0.0.3.tar` & `dbl_discoverx-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.388141 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 14:35:20.000000 dbl_discoverx-0.0.3/dbl_discoverx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/discoverx/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/discoverx/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/dx.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/msql.py
--rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/discoverx/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:35:20.392141 dbl_discoverx-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-05 14:35:07.000000 dbl_discoverx-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:53:47.160015 dbl_discoverx-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-28 11:53:47.160015 dbl_discoverx-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:53:47.156015 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-28 11:53:47.000000 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-28 11:53:47.000000 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:53:47.000000 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-28 11:53:47.000000 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 11:53:47.000000 dbl_discoverx-0.0.4/dbl_discoverx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:53:47.160015 dbl_discoverx-0.0.4/discoverx/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:53:47.160015 dbl_discoverx-0.0.4/discoverx/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/dx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/msql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20619 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/discoverx/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 11:53:47.160015 dbl_discoverx-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-28 11:53:35.000000 dbl_discoverx-0.0.4/setup.py
```

### Comparing `dbl_discoverx-0.0.3/LICENSE` & `dbl_discoverx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.3/PKG-INFO` & `dbl_discoverx-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl_discoverx
-Version: 0.0.3
+Version: 0.0.4
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -43,24 +43,26 @@
 Check out the [scan parameters](#scan-parameters) for more details.
 
 The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
 ### Available classes
 
 The supported classes are:
-- IP v4 addresses
-- IP v6 addresses
-- Email addresses
-- URLs
-- fqdn (Fully qualified domain names)
+- IP v4 address
+- IP v6 address
+- Email address
+- URL
+- fqdn (Fully qualified domain name)
 - Credit card number
 - Credit card expiration date
 - Iso date
 - Iso date time
 - Mac address
+- Integer number as string
+- Decimal number as string
 
 US locale specific classes
 - us_mailing_address
 - us_phone_number
 - us_social_security_number
 - us_state
 - us_state_abbreviation
@@ -171,24 +173,27 @@
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
 ```
+from discoverx.rules import RegexRule
+from discoverx import DX
+
 custom_rules = [
-    {
-        'name': 'resource_request_id',
-        'type': 'regex',
-        'description': 'Resource request ID',
-        'definition': r'^AR-\d{9}$',
-        'match_example': ['AR-123456789'],
-        'nomatch_example': ['CD-123456789']
-    }
+  RegexRule(
+    name = "resource_request_id",
+    description = "Resource request ID",
+    definition = r"^AR-\d{9}$",
+    match_example = ["AR-123456789"],
+    nomatch_example = ["R-123"],
+  )
 ]
+
 dx = DX(custom_rules=custom_rules)
 ```
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
```

### Comparing `dbl_discoverx-0.0.3/README.md` & `dbl_discoverx-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,26 @@
 Check out the [scan parameters](#scan-parameters) for more details.
 
 The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
 ### Available classes
 
 The supported classes are:
-- IP v4 addresses
-- IP v6 addresses
-- Email addresses
-- URLs
-- fqdn (Fully qualified domain names)
+- IP v4 address
+- IP v6 address
+- Email address
+- URL
+- fqdn (Fully qualified domain name)
 - Credit card number
 - Credit card expiration date
 - Iso date
 - Iso date time
 - Mac address
+- Integer number as string
+- Decimal number as string
 
 US locale specific classes
 - us_mailing_address
 - us_phone_number
 - us_social_security_number
 - us_state
 - us_state_abbreviation
@@ -156,24 +158,27 @@
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
 ```
+from discoverx.rules import RegexRule
+from discoverx import DX
+
 custom_rules = [
-    {
-        'name': 'resource_request_id',
-        'type': 'regex',
-        'description': 'Resource request ID',
-        'definition': r'^AR-\d{9}$',
-        'match_example': ['AR-123456789'],
-        'nomatch_example': ['CD-123456789']
-    }
+  RegexRule(
+    name = "resource_request_id",
+    description = "Resource request ID",
+    definition = r"^AR-\d{9}$",
+    match_example = ["AR-123456789"],
+    nomatch_example = ["R-123"],
+  )
 ]
+
 dx = DX(custom_rules=custom_rules)
 ```
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
```

### Comparing `dbl_discoverx-0.0.3/dbl_discoverx.egg-info/PKG-INFO` & `dbl_discoverx-0.0.4/dbl_discoverx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbl-discoverx
-Version: 0.0.3
+Version: 0.0.4
 Summary: DiscoverX - Map and Search your Lakehouse
 Home-page: https://databricks.com/learn/labs
 Author: Erni Durdevic, David Tempelmann
 Author-email: labs@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -43,24 +43,26 @@
 Check out the [scan parameters](#scan-parameters) for more details.
 
 The scan result is a dataset with a `score` column, which defines the fraction of matched records against the total records scanned for each rule.
 
 ### Available classes
 
 The supported classes are:
-- IP v4 addresses
-- IP v6 addresses
-- Email addresses
-- URLs
-- fqdn (Fully qualified domain names)
+- IP v4 address
+- IP v6 address
+- Email address
+- URL
+- fqdn (Fully qualified domain name)
 - Credit card number
 - Credit card expiration date
 - Iso date
 - Iso date time
 - Mac address
+- Integer number as string
+- Decimal number as string
 
 US locale specific classes
 - us_mailing_address
 - us_phone_number
 - us_social_security_number
 - us_state
 - us_state_abbreviation
@@ -171,24 +173,27 @@
 ```
 
 ### Custom rules
 
 You can provide your custom scanning rules based on regex expressions.
 
 ```
+from discoverx.rules import RegexRule
+from discoverx import DX
+
 custom_rules = [
-    {
-        'name': 'resource_request_id',
-        'type': 'regex',
-        'description': 'Resource request ID',
-        'definition': r'^AR-\d{9}$',
-        'match_example': ['AR-123456789'],
-        'nomatch_example': ['CD-123456789']
-    }
+  RegexRule(
+    name = "resource_request_id",
+    description = "Resource request ID",
+    definition = r"^AR-\d{9}$",
+    match_example = ["AR-123456789"],
+    nomatch_example = ["R-123"],
+  )
 ]
+
 dx = DX(custom_rules=custom_rules)
 ```
 
 You should now see your rules added to the default ones with
 
 ```
 dx.display_rules()
```

### Comparing `dbl_discoverx-0.0.3/discoverx/common/helper.py` & `dbl_discoverx-0.0.4/discoverx/common/helper.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.3/discoverx/dx.py` & `dbl_discoverx-0.0.4/discoverx/dx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from delta.tables import DeltaTable
 import pandas as pd
 from pyspark.sql import SparkSession
-import pyspark.sql.functions as func
 from typing import List, Optional, Union
 from discoverx import logging
 from discoverx.msql import Msql
 from discoverx.rules import Rules, Rule
 from discoverx.scanner import Scanner, ScanResult
 
 
@@ -235,30 +233,27 @@
                 by_class = search_matching_rules[0]
             self.logger.friendly(f"Discoverx will search your lakehouse using the class {by_class}")
         elif isinstance(by_class, str):
             search_matching_rules = [by_class]
         else:
             raise ValueError(f"The provided by_class {by_class} must be of string type.")
 
-        sql_filter = f"[{search_matching_rules[0]}] = '{search_term}'"
+        sql_filter = f"`[{search_matching_rules[0]}]` = '{search_term}'"
         select_statement = (
             "named_struct("
             + ", ".join(
                 [
                     f"'{rule_name}', named_struct('column_name', '[{rule_name}]', 'value', `[{rule_name}]`)"
                     for rule_name in search_matching_rules
                 ]
             )
             + ") AS search_result"
         )
 
-        if search_term is None:
-            where_statement = ""
-        else:
-            where_statement = f"WHERE {sql_filter}"
+        where_statement = f"WHERE {sql_filter}"
 
         return self._msql(
             f"SELECT {select_statement}, to_json(struct(*)) AS row_content FROM {from_tables} {where_statement}",
             min_score=min_score,
         )
 
     def select_by_classes(
```

### Comparing `dbl_discoverx-0.0.3/discoverx/logging.py` & `dbl_discoverx-0.0.4/discoverx/logging.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.3/discoverx/msql.py` & `dbl_discoverx-0.0.4/discoverx/msql.py`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.3/discoverx/rules.py` & `dbl_discoverx-0.0.4/discoverx/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 """
 
 from dataclasses import dataclass
 from enum import Enum
 from fnmatch import fnmatch
 import re
 from typing import Union, Optional, List
-from pydantic import BaseModel, field_validator
 
 
 class RuleTypes(str, Enum):
     """Allowed types/choices for Rules"""
 
     REGEX = "regex"
 
 
-class Rule(BaseModel):
+class Rule:
     """Parent class for rules
     Attributes:
         type (RuleTypes): Defines the type of Rule, e.g. Regex
     """
 
     type: RuleTypes
 
@@ -37,70 +36,46 @@
         match_example (str, optional): It is possible to provide an example of
             a string/expression to be matched by the Rule. This example
             is used to validate the Rule upon instantiation.
         class_name (str, optional): Name of the class used to select columns in unity
             catalog
     """
 
+    def __init__(self, name, description, definition, match_example=[], nomatch_example=[], class_name=None):
+        self.name = name
+        self.description = description
+        self.definition = definition
+        self.match_example = match_example
+        self.nomatch_example = nomatch_example
+        self.class_name = class_name
+        self.type = RuleTypes.REGEX
+
+        self.validate_rule(self.match_example, self.definition, self.name, False)
+        self.validate_rule(self.nomatch_example, self.definition, self.name, True)
+
     type: RuleTypes = RuleTypes.REGEX
 
     name: str
     description: str
     definition: str
     match_example: Optional[Union[str, List[str]]] = None
     nomatch_example: Optional[Union[str, List[str]]] = None
     class_name: Optional[str] = None
 
-    # pylint: disable=no-self-argument
-    @field_validator("match_example")
-    def validate_match_example(cls, match_example, values):
-        """Validate regular expression
-        This validator checks that the regular expression matches
-        the provided match_example.
-
-        Args:
-            match_example (List): A list of strings supposed to match the
-                defined regular expression
-            values (ValidationInfo): values.data provides dictionary of
-            remaining fields
-
-        Returns: List of specified examples
-        """
-        return cls.validate_rule(match_example, values, False)
-
-    # pylint: disable=no-self-argument
-    @field_validator("nomatch_example")
-    def validate_nomatch_example(cls, nomatch_example, values):
-        """Validate regular expression
-        This validator checks that the regular expression does not match
-        the provided nomatch_example.
-
-        Args:
-            nomatch_example (List): A list of strings supposed to not
-                match the defined regular expression
-            values (ValidationInfo): values.data provides dictionary of
-                remaining fields
-
-        Returns: List of specified examples
-        """
-        return cls.validate_rule(nomatch_example, values, True)
-
     @staticmethod
-    def validate_rule(example, values, fail_match: bool):
+    def validate_rule(example, definition, name, fail_match: bool):
         """Validates that given example is matched by defined pattern"""
         if not isinstance(example, list):
             validation_example = [example]
         else:
             validation_example = example
 
         for ex in validation_example:
-            if (not re.match(values.data["definition"], ex)) != fail_match:
-                raise ValueError(
-                    f"The definition of the rule {values.data['name']} does not match the provided example {ex}"
-                )
+            if (not re.match(definition, ex)) != fail_match:
+                raise ValueError(f"The definition of the rule {name} does not match the provided example {ex}")
         return example
 
 
 @dataclass
 class RulesList:
     """A list of rules with added properties
     Attributes:
@@ -148,14 +123,34 @@
         name="credit_card_number",
         description="Credit Card Number",
         definition=r"^\d{4}-\d{4}-\d{4}-\d{4}$",
         match_example=["1234-5678-9012-3456", "9876-5432-1098-7654"],
         nomatch_example=["1234-5678-9012-345", "1234-5678-9012-34567", "1234-5678-9012-3456-7890"],
     ),
     RegexRule(
+        name="decimal_number",
+        description="Decimal Number",
+        definition=r"^-?\d+(?:[.,]\d*)?[eE]?-?\d{0,3}$",
+        match_example=[
+            "123.45",
+            "-123.45",
+            "1.1E2",
+            "1.1E-1",
+            "123,45",
+            "-123,45",
+            "123,0123",
+            "-123,0",
+            "123.",
+            "123,",
+            "-123.",
+            "-123,",
+        ],
+        nomatch_example=["", "123,456,789", "1$", "123,456.789"],
+    ),
+    RegexRule(
         name="email",
         description="Email address",
         definition=r"^.+@[^\.].*\.[a-z]{2,}$",
         match_example=[
             "whatever@somewhere.museum",
             "foreignchars@myforeigncharsdomain.nu",
             "me+mysomething@mydomain.com",
@@ -177,14 +172,21 @@
             "label.name.321",
             "1234567890-1234567890-1234567890-1234567890-12345678901234567890.123.com",
             "abc.cdf@mydoamain.com",
             "Some text abc.cdf.com",
         ],
     ),
     RegexRule(
+        name="integer_number",
+        description="Integer Number",
+        definition=r"^-?\d+$",
+        match_example=["123", "-123", "0"],
+        nomatch_example=["", "123.45", "123,45", "123,0", "123.0", "123,456,789", "1$"],
+    ),
+    RegexRule(
         name="ip_v4",
         description="IP address v4",
         definition=r"^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$",
         match_example=["192.1.1.1", "0.0.0.0"],
         nomatch_example=["192"],
     ),
     RegexRule(
@@ -237,41 +239,37 @@
     ),
 ]
 
 localized_rules = {
     "us": [
         RegexRule(
             name="us_mailing_address",
-            type="regex",
             description="US Mailing Address",
             definition=r"^\d+\s[A-z]+\s[A-z]+",
             match_example=["123 Main St", "456 Elm St", "789 Pine St"],
             nomatch_example=["123 Main", "456 Elm", "789 Pine"],
         ),
         RegexRule(
             name="us_phone_number",
-            type="regex",
             description="US Phone Number",
             definition=r"^\+?1?[-. (]*(\d{3})[-. )]*(\d{3})[-. ]*(\d{4})$",
             match_example=["+1 (123) 456-7890", "123-456-7890", "123.456.7890", "1234567890", "(123)456-7890"],
             nomatch_example=["123-45-6789", "987-65-4321"],
         ),
         RegexRule(
             name="us_social_security_number",
-            type="regex",
             description="US Social Security Number",
             definition=r"^(?!000|666|9)\d{3}-(?!00)\d{2}-(?!0000)\d{4}$",
             match_example=["123-45-6789"],
             nomatch_example=["123-45-678", "123-456-7890", "123-45-67890", "123-456-789"],
         ),
         RegexRule(
             name="us_state",
-            type="regex",
             description="US State",
-            definition=r"^(?i)(Alabama|Alaska|American Samoa|Arizona|Arkansas|California|Colorado|Connecticut|Delaware|District of Columbia|Federated States of Micronesia|Florida|Georgia|Guam|Hawaii|Idaho|Illinois|Indiana|Iowa|Kansas|Kentucky|Louisiana|Maine|Marshall Islands|Maryland|Massachusetts|Michigan|Minnesota|Mississippi|Missouri|Montana|Nebraska|Nevada|New Hampshire|New Jersey|New Mexico|New York|North Carolina|North Dakota|Northern Mariana Islands|Ohio|Oklahoma|Oregon|Palau|Pennsylvania|Puerto Rico|Rhode Island|South Carolina|South Dakota|Tennessee|Texas|Utah|Vermont|Virgin Islands|Virginia|Washington|West Virginia|Wisconsin|Wyoming)$",
+            definition=r"(?i)^(Alabama|Alaska|American Samoa|Arizona|Arkansas|California|Colorado|Connecticut|Delaware|District of Columbia|Federated States of Micronesia|Florida|Georgia|Guam|Hawaii|Idaho|Illinois|Indiana|Iowa|Kansas|Kentucky|Louisiana|Maine|Marshall Islands|Maryland|Massachusetts|Michigan|Minnesota|Mississippi|Missouri|Montana|Nebraska|Nevada|New Hampshire|New Jersey|New Mexico|New York|North Carolina|North Dakota|Northern Mariana Islands|Ohio|Oklahoma|Oregon|Palau|Pennsylvania|Puerto Rico|Rhode Island|South Carolina|South Dakota|Tennessee|Texas|Utah|Vermont|Virgin Islands|Virginia|Washington|West Virginia|Wisconsin|Wyoming)$",
             match_example=[
                 "Alabama",
                 "Alaska",
                 "Arizona",
                 "Arkansas",
                 "California",
                 "Colorado",
@@ -380,17 +378,16 @@
                 "WV",
                 "WI",
                 "WY",
             ],
         ),
         RegexRule(
             name="us_state_abbreviation",
-            type="regex",
             description="US State Abbreviation",
-            definition=r"^(?i)(AL|AK|AS|AZ|AR|CA|CO|CT|DE|DC|FM|FL|GA|GU|HI|ID|IL|IN|IA|KS|KY|LA|ME|MH|MD|MA|MI|MN|MS|MO|MT|NE|NV|NH|NJ|NM|NY|NC|ND|MP|OH|OK|OR|PW|PA|PR|RI|SC|SD|TN|TX|UT|VT|VI|VA|WA|WV|WI|WY)$",
+            definition=r"(?i)^(AL|AK|AS|AZ|AR|CA|CO|CT|DE|DC|FM|FL|GA|GU|HI|ID|IL|IN|IA|KS|KY|LA|ME|MH|MD|MA|MI|MN|MS|MO|MT|NE|NV|NH|NJ|NM|NY|NC|ND|MP|OH|OK|OR|PW|PA|PR|RI|SC|SD|TN|TX|UT|VT|VI|VA|WA|WV|WI|WY)$",
             match_example=[
                 "AL",
                 "AK",
                 "AS",
                 "AZ",
                 "AR",
                 "CA",
@@ -500,15 +497,14 @@
                 "West Virginia",
                 "Wisconsin",
                 "Wyoming",
             ],
         ),
         RegexRule(
             name="us_zip_code",
-            type="regex",
             description="US Zip Code",
             definition=r"^\d{5}(?:[-\s]\d{4})?$",
             match_example=["12345", "12345-6789"],
             nomatch_example=["1234", "123456"],
         ),
     ]
 }
```

### Comparing `dbl_discoverx-0.0.3/discoverx/scanner.py` & `dbl_discoverx-0.0.4/discoverx/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,31 +113,38 @@
             self.spark.sql(f"CREATE DATABASE IF NOT EXISTS {catalog + '.' + schema}")
 
         self.spark.sql(
             f"CREATE TABLE IF NOT EXISTS {scan_table_name} (table_catalog string, table_schema string, table_name string, column_name string, class_name string, score double, effective_timestamp timestamp)"
         )
         logger.friendly(f"The scan result table {scan_table_name} has been created.")
 
-    def _get_or_create_result_table_from_delta(self, scan_table_name: str):
+    def _get_or_create_result_table_from_delta(self, scan_table_name: str) -> DeltaTable:
         try:
-            DeltaTable.forName(self.spark, scan_table_name)
+            return DeltaTable.forName(self.spark, scan_table_name)
         except Exception:
             self._create_databes_if_not_exists(scan_table_name)
+            return DeltaTable.forName(self.spark, scan_table_name)
 
     def save(self, scan_table_name: str):
-        self._get_or_create_result_table_from_delta(scan_table_name)
+        scan_delta_table = self._get_or_create_result_table_from_delta(scan_table_name)
 
         scan_result_df = self.spark.createDataFrame(
             self.df,
             "table_catalog: string, table_schema: string, table_name: string, column_name: string, class_name: string, score: double",
         ).withColumn("effective_timestamp", func.current_timestamp())
 
-        logger.friendly(f"Overwrite scan result table {scan_table_name}")
+        logger.friendly(f"Merging results into {scan_table_name}")
 
-        scan_result_df.write.format("delta").mode("overwrite").saveAsTable(scan_table_name)
+        scan_delta_table.alias("scan_delta_table").merge(
+            scan_result_df.alias("scan_result_df"),
+            "scan_delta_table.table_catalog = scan_result_df.table_catalog \
+            and scan_delta_table.table_schema = scan_result_df.table_schema \
+            and scan_delta_table.table_name = scan_result_df.table_name \
+            and scan_delta_table.column_name = scan_result_df.column_name ",
+        ).whenMatchedUpdateAll().whenNotMatchedInsertAll().execute()
 
     def load(self, scan_table_name: str):
         try:
             self.df = DeltaTable.forName(self.spark, scan_table_name).toDF().drop("effective_timestamp").toPandas()
         except Exception as e:
             logger.error(f"Error while reading the scan result table {scan_table_name}: {e}")
             raise e
@@ -223,15 +230,15 @@
     def _resolve_scan_content(self) -> ScanContent:
         table_list = self._get_list_of_tables()
         catalogs = set(map(lambda x: x.catalog, table_list))
         schemas = set(map(lambda x: f"{x.catalog}.{x.schema}", table_list))
 
         return ScanContent(table_list, catalogs, schemas)
 
-    def scan_table(self, table):
+    def scan_table(self, table: TableInfo):
         try:
             if self.what_if:
                 logger.friendly(f"SQL that would be executed for '{table.catalog}.{table.schema}.{table.table}'")
             else:
                 logger.friendly(f"Scanning table '{table.catalog}.{table.schema}.{table.table}'")
 
             # Build rule matching SQL
```

### Comparing `dbl_discoverx-0.0.3/pyproject.toml` & `dbl_discoverx-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbl_discoverx-0.0.3/setup.py` & `dbl_discoverx-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 VERSION_PATTERN = r"^__version__ = ['\"]([^'\"]*)['\"]"
 parsed_version = re.search(VERSION_PATTERN, version_line, re.M)
 if parsed_version:
     version_string = parsed_version.group(1)
 else:
     raise RuntimeError("Unable to find version string in discoverx/version.py")
 
-PACKAGE_REQUIREMENTS = ["pyyaml", "pydantic>=2.0"]
+PACKAGE_REQUIREMENTS = ["pyyaml"]
 
 # packages for local development and unit testing
 # please note that these packages are already available in DBR, there is no need to install them on DBR.
 LOCAL_REQUIREMENTS = [
     "pyspark>=3.3.0",
     "delta-spark>=2.2.0",
     "pandas<2.0.0",  # From 2.0.0 onwards, pandas does not support iteritems() anymore, spark.createDataFrame will fail
```

