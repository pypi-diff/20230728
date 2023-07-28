# Comparing `tmp/pytbai-1.4.2.tar.gz` & `tmp/pytbai-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.4.2.tar", last modified: Thu Jul 27 09:22:18 2023, max compression
+gzip compressed data, was "pytbai-1.4.3.tar", last modified: Fri Jul 28 11:50:13 2023, max compression
```

## Comparing `pytbai-1.4.2.tar` & `pytbai-1.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.330471 pytbai-1.4.2/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2651 2023-07-27 09:22:17.000000 pytbai-1.4.2/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-27 09:22:17.000000 pytbai-1.4.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-27 09:22:17.000000 pytbai-1.4.2/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-27 09:22:17.000000 pytbai-1.4.2/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 09:22:17.000000 pytbai-1.4.2/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 09:22:18.330471 pytbai-1.4.2/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-27 09:22:17.000000 pytbai-1.4.2/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.330471 pytbai-1.4.2/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5086 2023-07-27 09:22:17.000000 pytbai-1.4.2/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.326471 pytbai-1.4.2/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-27 09:22:18.000000 pytbai-1.4.2/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-27 09:22:18.000000 pytbai-1.4.2/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-27 09:22:18.000000 pytbai-1.4.2/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-27 09:22:18.000000 pytbai-1.4.2/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-27 09:22:17.000000 pytbai-1.4.2/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-27 09:22:18.330471 pytbai-1.4.2/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1098 2023-07-27 09:22:17.000000 pytbai-1.4.2/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.330471 pytbai-1.4.2/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.330471 pytbai-1.4.2/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-27 09:22:18.330471 pytbai-1.4.2/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3045 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-27 09:22:17.000000 pytbai-1.4.2/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.549311 pytbai-1.4.3/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2767 2023-07-28 11:50:12.000000 pytbai-1.4.3/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-28 11:50:12.000000 pytbai-1.4.3/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-28 11:50:12.000000 pytbai-1.4.3/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-28 11:50:12.000000 pytbai-1.4.3/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-28 11:50:12.000000 pytbai-1.4.3/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-28 11:50:13.549311 pytbai-1.4.3/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-28 11:50:12.000000 pytbai-1.4.3/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11287 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.549311 pytbai-1.4.3/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2023-07-28 11:50:12.000000 pytbai-1.4.3/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.545311 pytbai-1.4.3/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-28 11:50:13.000000 pytbai-1.4.3/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-28 11:50:13.000000 pytbai-1.4.3/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-28 11:50:13.000000 pytbai-1.4.3/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-28 11:50:13.000000 pytbai-1.4.3/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-28 11:50:12.000000 pytbai-1.4.3/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-28 11:50:13.549311 pytbai-1.4.3/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1098 2023-07-28 11:50:12.000000 pytbai-1.4.3/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.549311 pytbai-1.4.3/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.549311 pytbai-1.4.3/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-28 11:50:13.549311 pytbai-1.4.3/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-28 11:50:12.000000 pytbai-1.4.3/tests/test_basic.py
```

### Comparing `pytbai-1.4.2/CHANGELOG.txt` & `pytbai-1.4.3/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.4.3 (2023-07-28)
+------------------
+
+- get vat breakdown in json [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.4.2 (2023-07-27)
 ------------------
 
 - include templates [Urtzi Odriozola <uodriozola@codesyntax.com>]
 
 - include templates [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.4.2/LICENSE` & `pytbai-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/PKG-INFO` & `pytbai-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.2
+Version: 1.4.3
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.2/README.md` & `pytbai-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/core.py` & `pytbai-1.4.3/pytbai/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,25 +200,29 @@
         for vat_type in L11:
             lines = [
                 line for line in self.get_lines() if line.vat_type == vat_type
             ]
             if lines:
                 line_types = {"type": vat_type, "rates": {}}
                 for line in lines:
-                    if line.vat_rate in line_types["rates"]:
-                        line_types["rates"][line.vat_rate] = {
-                            "base": line_types["rates"][line.vat_rate]["base"]
+                    if str(line.vat_rate) in line_types["rates"]:
+                        line_types["rates"][str(line.vat_rate)] = {
+                            "base": line_types["rates"][str(line.vat_rate)][
+                                "base"
+                            ]
                             + line.vat_base,
-                            "fee": line_types["rates"][line.vat_rate]["fee"]
+                            "fee": line_types["rates"][str(line.vat_rate)][
+                                "fee"
+                            ]
                             + line.vat_fee,
                         }
                     else:
                         line_types["rates"].update(
                             {
-                                line.vat_rate: {
+                                str(line.vat_rate): {
                                     "base": line.vat_base,
                                     "fee": line.vat_fee,
                                 }
                             }
                         )
                 breakdown.append(line_types)
         return breakdown
@@ -251,14 +255,15 @@
     def get_dict(self):
         invoice_json = copy.deepcopy(self.__dict__)
         lines_json = []
         for line in invoice_json["lines"]:
             lines_json.append(line.get_dict())
         invoice_json["lines"] = lines_json
         invoice_json["total_amount"] = self.get_total_amount()
+        invoice_json["vat_breakdown"] = self.get_vat_breakdown()
         return invoice_json
 
 
 class Software:
     def __init__(
         self,
         license,
```

### Comparing `pytbai-1.4.2/pytbai/definitions.py` & `pytbai-1.4.3/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.4.3/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.4.3/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.4.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.4.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/utils/pdf.py` & `pytbai-1.4.3/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/pytbai/utils/xml.py` & `pytbai-1.4.3/pytbai/utils/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
         fp_root = root.find(".//HuellaTBAI")
         p_inv = ET.Element("EncadenamientoFacturaAnterior")
         fp_root.insert(0, p_inv)
         serial_code = ET.SubElement(p_inv, "SerieFacturaAnterior")
         serial_code.text = pre_invoice["serial_code"]
         num = ET.SubElement(p_inv, "NumFacturaAnterior")
         num.text = pre_invoice["num"]
+        expedition_date = ET.SubElement(
+            p_inv, "FechaExpedicionFacturaAnterior"
+        )
+        expedition_date.text = pre_invoice["expedition_date"]
         signature_value = ET.SubElement(
             p_inv, "SignatureValueFirmaFacturaAnterior"
         )
         signature_value.text = pre_invoice["signature_value"]
 
     return root
```

### Comparing `pytbai-1.4.2/pytbai.egg-info/PKG-INFO` & `pytbai-1.4.3/pytbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.2
+Version: 1.4.3
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.2/pytbai.egg-info/SOURCES.txt` & `pytbai-1.4.3/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/setup.py` & `pytbai-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.4.2",
+    version="1.4.3",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.4.2/tests/certs/cert.pem` & `pytbai-1.4.3/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/tests/certs/cert_for_tests.p12` & `pytbai-1.4.3/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/tests/certs/key.pem` & `pytbai-1.4.3/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.2/tests/data/tbai_json.py` & `pytbai-1.4.3/tests/data/tbai_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         "expedition_time": "12:58:17",
         "transaction_date": "2023-07-05",
         "simplified": "N",
         "substitution": "N",
         "vat_regime": "01",
         "lines": [],
         "total_amount": 0,
+        "vat_breakdown": [],
     },
     "software": {
         "license": "TBAIGIPRE00000000501",
         "dev_entity": "P2000000F",
         "soft_name": "FAKTURABAI",
         "soft_version": "1.0",
     },
@@ -91,14 +92,17 @@
                 "vat_fee": 147.0,
                 "vat_type": "S1",
                 "vat_base": 700,
                 "total": 847.0,
             },
         ],
         "total_amount": 1040.6,
+        "vat_breakdown": [
+            {"type": "S1", "rates": {"21": {"base": 860.0, "fee": 180.6}}}
+        ],
     },
     "software": {
         "license": "TBAIGIPRE00000000501",
         "dev_entity": "P2000000F",
         "soft_name": "FAKTURABAI",
         "soft_version": "1.0",
     },
```

### Comparing `pytbai-1.4.2/tests/test_basic.py` & `pytbai-1.4.3/tests/test_basic.py`

 * *Files identical despite different names*

