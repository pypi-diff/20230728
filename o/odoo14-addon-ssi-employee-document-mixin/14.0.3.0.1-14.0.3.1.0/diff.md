# Comparing `tmp/odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 52969 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1219 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/__init__.py
--rw-r--r--  2.0 unx      548 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/__manifest__.py
--rw-r--r--  2.0 unx      198 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/models/__init__.py
--rw-r--r--  2.0 unx     1898 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Jul-24 06:38 odoo/addons/ssi_employee_document_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     1820 b- defN 23-Jul-24 06:38 odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 06:38 odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 06:38 odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1143 b- defN 23-Jul-24 06:38 odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/RECORD
-10 files, 55437 bytes uncompressed, 50919 bytes compressed:  8.1%
+Zip file size: 53012 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1219 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/__init__.py
+-rw-r--r--  2.0 unx      548 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      198 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py
+-rw-r--r--  2.0 unx    48333 b- defN 23-Jul-28 07:53 odoo/addons/ssi_employee_document_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     1820 b- defN 23-Jul-28 07:53 odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 07:53 odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-28 07:53 odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-Jul-28 07:53 odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/RECORD
+10 files, 55589 bytes uncompressed, 50962 bytes compressed:  8.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py
 Comment: 
 
 Filename: odoo/addons/ssi_employee_document_mixin/static/description/icon.png
 Comment: 
 
-Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/METADATA
+Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/WHEEL
+Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/RECORD
+Filename: odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_employee_document_mixin/__manifest__.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 # pylint: disable=locally-disabled, manifest-required-author
 {
     "name": "Employee Document Mixin",
-    "version": "14.0.3.0.1",
+    "version": "14.0.3.1.0",
     "website": "https://simetri-sinergi.id",
     "author": "PT. Simetri Sinergi Indonesia, OpenSynergy Indonesia",
     "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_hr_employee",
         "ssi_transaction_mixin",
```

## odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py

```diff
@@ -37,14 +37,19 @@
     )
     job_id = fields.Many2one(
         string="Job Position",
         comodel_name="hr.job",
         readonly=True,
         states={"draft": [("readonly", False)]},
     )
+    employee_partner_id = fields.Many2one(
+        string="Employee Partner",
+        related="employee_id.address_home_id",
+        store=False,
+    )
 
     @api.onchange(
         "employee_id",
     )
     def onchange_department_id(self):
         self.department_id = False
         if self.employee_id:
```

## Comparing `odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/METADATA` & `odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-employee-document-mixin
-Version: 14.0.3.0.1
+Version: 14.0.3.1.0
 Summary: Employee Document Mixin
 Home-page: https://simetri-sinergi.id
 Author: PT. Simetri Sinergi Indonesia, OpenSynergy Indonesia
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/RECORD` & `odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/ssi_employee_document_mixin/README.rst,sha256=BAad72fffnn6tyYBDhgLd-p_dulVfSU98PZomKNzdJ0,1219
 odoo/addons/ssi_employee_document_mixin/__init__.py,sha256=X3ayW9k4OH3xqib3X0KEzYY9_pqaAhP2YdhFFVEJSvo,181
-odoo/addons/ssi_employee_document_mixin/__manifest__.py,sha256=xgpNhrmwSjQweWV1Ns3RW9C4DBwiThjDulbsWQl1uJA,548
+odoo/addons/ssi_employee_document_mixin/__manifest__.py,sha256=A9YuSkUrLlUfB8djcUZ_iCae9SZjf3r3cOgGuId0ksw,548
 odoo/addons/ssi_employee_document_mixin/models/__init__.py,sha256=R_CS7Gs6W0rcBTPsxl8Tj1gwaLNa-Q-S8PKzQFxvyNg,198
-odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py,sha256=LRW91fRA7q48vghnGW4eE9Fivbt17HOc2vqjHFCyCxo,1898
+odoo/addons/ssi_employee_document_mixin/models/mixin_employee_document.py,sha256=dg0If0D4K1ipa-WsPZZ23sBByrGluZl8lb9nH5wJEBg,2050
 odoo/addons/ssi_employee_document_mixin/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/METADATA,sha256=2qVJJdU-3JAk24T-BcZmgzclbXwPUSdi045en5UuSmM,1820
-odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_employee_document_mixin-14.0.3.0.1.dist-info/RECORD,,
+odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/METADATA,sha256=hsh19pnd-Z--WBihadfBH6kH5zFAd4HnZptiB3j6MVk,1820
+odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_employee_document_mixin-14.0.3.1.0.dist-info/RECORD,,
```

