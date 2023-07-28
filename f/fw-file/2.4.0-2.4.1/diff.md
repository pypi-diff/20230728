# Comparing `tmp/fw_file-2.4.0-py3-none-any.whl.zip` & `tmp/fw_file-2.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 358219 bytes, number of entries: 36
+Zip file size: 358400 bytes, number of entries: 36
 -rw-r--r--  2.0 unx      229 b- defN 80-Jan-01 00:00 fw_file/__init__.py
 -rw-r--r--  2.0 unx     8377 b- defN 80-Jan-01 00:00 fw_file/base.py
 -rw-r--r--  2.0 unx     3184 b- defN 80-Jan-01 00:00 fw_file/bruker.py
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 fw_file/dicom/__init__.py
 -rw-r--r--  2.0 unx     6011 b- defN 80-Jan-01 00:00 fw_file/dicom/config.py
 -rw-r--r--  2.0 unx    44285 b- defN 80-Jan-01 00:00 fw_file/dicom/dcmdict.py
 -rw-r--r--  2.0 unx    17633 b- defN 80-Jan-01 00:00 fw_file/dicom/dicom.py
 -rw-r--r--  2.0 unx    18949 b- defN 80-Jan-01 00:00 fw_file/dicom/fixers.py
--rw-r--r--  2.0 unx    17415 b- defN 80-Jan-01 00:00 fw_file/dicom/reader.py
+-rw-r--r--  2.0 unx    18042 b- defN 80-Jan-01 00:00 fw_file/dicom/reader.py
 -rw-r--r--  2.0 unx    27658 b- defN 80-Jan-01 00:00 fw_file/dicom/series.py
 -rw-r--r--  2.0 unx   421033 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/dict_info.json
 -rw-r--r--  2.0 unx   188832 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/iod_info.json
 -rw-r--r--  2.0 unx   528709 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/module_info.json
 -rw-r--r--  2.0 unx    31221 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/uid_info.json
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023b/json/version
 -rw-r--r--  2.0 unx   422965 b- defN 80-Jan-01 00:00 fw_file/dicom/standard/2023c/json/dict_info.json
@@ -27,12 +27,12 @@
 -rw-r--r--  2.0 unx      778 b- defN 80-Jan-01 00:00 fw_file/jpg.py
 -rw-r--r--  2.0 unx     2186 b- defN 80-Jan-01 00:00 fw_file/json.py
 -rw-r--r--  2.0 unx     1440 b- defN 80-Jan-01 00:00 fw_file/nifti.py
 -rw-r--r--  2.0 unx     5265 b- defN 80-Jan-01 00:00 fw_file/philips.py
 -rw-r--r--  2.0 unx     8385 b- defN 80-Jan-01 00:00 fw_file/png.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_file/py.typed
 -rw-r--r--  2.0 unx    10521 b- defN 80-Jan-01 00:00 fw_file/siemens.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_file-2.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9569 b- defN 80-Jan-01 00:00 fw_file-2.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_file-2.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3031 b- defN 16-Jan-01 00:00 fw_file-2.4.0.dist-info/RECORD
-36 files, 2566589 bytes uncompressed, 353409 bytes compressed:  86.3%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_file-2.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9569 b- defN 80-Jan-01 00:00 fw_file-2.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_file-2.4.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     3031 b- defN 16-Jan-01 00:00 fw_file-2.4.1.dist-info/RECORD
+36 files, 2567216 bytes uncompressed, 353590 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -90,20 +90,20 @@
 
 Filename: fw_file/py.typed
 Comment: 
 
 Filename: fw_file/siemens.py
 Comment: 
 
-Filename: fw_file-2.4.0.dist-info/LICENSE
+Filename: fw_file-2.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: fw_file-2.4.0.dist-info/METADATA
+Filename: fw_file-2.4.1.dist-info/METADATA
 Comment: 
 
-Filename: fw_file-2.4.0.dist-info/WHEEL
+Filename: fw_file-2.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: fw_file-2.4.0.dist-info/RECORD
+Filename: fw_file-2.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_file/dicom/reader.py

```diff
@@ -316,14 +316,19 @@
             with no_fixes():
                 write_data_element(buffer, de)
             self.modified_attrs[tag] = DataElement(tag, VR, val)
         except (ValueError, KeyError):
             log.debug(f"value {raw_val!r} for tag {tag:>08x} invalid, writing to {NAS}")
             # If either tag doesn't have VR or if the value is invalid,
             # write to nonconforming sequence
+            # During non-strict validation, raw_val may have been changed
+            # from bytes to str, and upstream of .add_nonconforming_elem requires
+            # bytes, not str
+            if type(raw_val) == str:
+                raw_val = bytes(raw_val, "utf-8")  # type: ignore
             self.add_nonconforming_elem(tag, raw_val, 0)
 
     def process_tracker(self, required_tags: t.Set[int], dataset: Dataset):
         """Handle tracker events and populate modified attributes as necessary."""
         # First look at tracked elements that have been changed, filter them,
         #   and add them to the modified attribute sequences as necessary.
         self.trim()
@@ -365,17 +370,23 @@
                 # before we bailed out (removed the value) will be lost,
                 # only the original Value from the dicom will be written
                 # back if it can be
                 VR = t.cast(str, elem.VR)
                 # So that validation_mode is set to do as little validation as possible,
                 # it's set to 0 ("IGNORE") here, so that it won't raise if the value
                 # doesn't fit DICOM standards, only if it's unable to be parsed at all.
-                out = DataElement(elem.tag, VR, elem.original.value, validation_mode=0)
-                write_data_element(buffer, out)
-                dataset[out.tag] = out
+                # If a group 2 element gets in the main dataset, the DICOM can't save...
+                if (hasattr(dataset, "file_meta") and elem.tag.group != 0x0002) or (
+                    hasattr(dataset, "file_meta") is False and elem.tag.group == 0x0002
+                ):
+                    out = DataElement(
+                        elem.tag, VR, elem.original.value, validation_mode=0
+                    )
+                    write_data_element(buffer, out)
+                    dataset[out.tag] = out
             except Exception as exc:
                 # Writing will fail but we want to warn the user on all DEs that
                 # fall into this category
                 warnings.warn(
                     (
                         "Could not write original element. Original element "
                         "is required but invalid and cannot be written.\n\n"
```

## Comparing `fw_file-2.4.0.dist-info/LICENSE` & `fw_file-2.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_file-2.4.0.dist-info/METADATA` & `fw_file-2.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-file
-Version: 2.4.0
+Version: 2.4.1
 Summary: Unified data-file interface
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-file
 License: MIT
 Keywords: Flywheel,parse,medical,file,metadata,extract,DICOM,RAW,MR,CT,PET,NIfTI,JPG,JPEG,PNG,Bruker,ParaVision,GE,PFile,Philips,PARREC,Siemens,PTD
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_file-2.4.0.dist-info/RECORD` & `fw_file-2.4.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 fw_file/base.py,sha256=skak6Ex5bfSPwzN48F5dsJvfEz-vcg-Kn84SkfhhHzI,8377
 fw_file/bruker.py,sha256=yM_xq-cdgJ8zPKjhHBBQ8YrJRvj1U3JHmzMj8MR3oUA,3184
 fw_file/dicom/__init__.py,sha256=Dh7WgsG2PoelxuqtM5-_5C0dbAi_CG_TW35_N5aRBxY,1515
 fw_file/dicom/config.py,sha256=LDFuDZGl0Uk0RnIH9WJLR1RdwNZ-bXb-rtFjm5oziDc,6011
 fw_file/dicom/dcmdict.py,sha256=y_NpdECSc-klhPnf69qpYbjwy_TsI2ikXwLckZIDVcA,44285
 fw_file/dicom/dicom.py,sha256=XavmLF1TWEQh4Py6_7v9WNpkF8UJU1iyzC23isVA5Yk,17633
 fw_file/dicom/fixers.py,sha256=SAr-XspzAgblkBMTNuexNQyqoy5QE7qz70hLmdXzjwU,18949
-fw_file/dicom/reader.py,sha256=pM2UMGdiO8xPC51G6Z0Kdx9lwbPCBDnpp7SLAlAPuVQ,17415
+fw_file/dicom/reader.py,sha256=NjypbIYiYvWBLIN3HKVZakkyuVb9MQOVlSfd7oGsBWQ,18042
 fw_file/dicom/series.py,sha256=Fe6_OwInAp8ZU1INnkvRP7yf0BdIbuBNx32jCngY0hI,27658
 fw_file/dicom/standard/2023b/json/dict_info.json,sha256=G57E1IYRQssb6NVgA6hRA-qgrTAk-b_JgP7QUBjym1k,421033
 fw_file/dicom/standard/2023b/json/iod_info.json,sha256=kOR8UWIR7Gyut7WVGHmEXTJymjF8XYty6lqJWsoTwMs,188832
 fw_file/dicom/standard/2023b/json/module_info.json,sha256=juOJ1KQVVhL0J24fzGDl2joL6MtsBf223_PpkSvfwS8,528709
 fw_file/dicom/standard/2023b/json/uid_info.json,sha256=tkQbqwXGQO6_WsPxbNwf4eHQ8tdANM_PisWW8zqc864,31221
 fw_file/dicom/standard/2023b/json/version,sha256=uPt4p7NTFCveH-UkqLcBd1htCl0u6YAhWEHipHmPbBs,5
 fw_file/dicom/standard/2023c/json/dict_info.json,sha256=D9Ddu8tEEBaEGt3deC-UBirNO37E0Z7LCKvCz2Tux88,422965
@@ -26,11 +26,11 @@
 fw_file/jpg.py,sha256=3qLSgZztivZ3so1CYD-CBC-x59kahOZO5Y5PIbVDX10,778
 fw_file/json.py,sha256=ufQ2YnNsyWocsB1yrTFEncHCKmIr7OeiwEUqOm3n3VY,2186
 fw_file/nifti.py,sha256=hKjKGhUUTrqIv6QsPe2qWJqteLbZPHZ52yWPf788iOQ,1440
 fw_file/philips.py,sha256=E9gyia6ZpyTg2RYktYFFDBNaI-plmYSVunhhWgfR_GA,5265
 fw_file/png.py,sha256=dqpSGSPg7Ox_B4JOFcSD2Uy5y0fXhM5O2tZgI-aZ4kU,8385
 fw_file/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_file/siemens.py,sha256=IYUQkiEJs9_25hb50NgdoHM8cw-l5iATlI1V1EdQwpc,10521
-fw_file-2.4.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_file-2.4.0.dist-info/METADATA,sha256=YQAzG13VLrfw-OhDrByAIopw0KR0R675OFkV4vZFT5U,9569
-fw_file-2.4.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-fw_file-2.4.0.dist-info/RECORD,,
+fw_file-2.4.1.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_file-2.4.1.dist-info/METADATA,sha256=a7a0sIltKvcshmmj9rjTXT7M2ykezbAdqpU1mtmFLjs,9569
+fw_file-2.4.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_file-2.4.1.dist-info/RECORD,,
```

