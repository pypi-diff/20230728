# Comparing `tmp/mds_csv_reader-1.0.4.tar.gz` & `tmp/mds_csv_reader-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mds_csv_reader-1.0.4.tar", last modified: Thu Jan  9 14:51:17 2020, max compression
+gzip compressed data, was "mds_csv_reader-1.0.5.tar", last modified: Fri Jul 28 07:21:42 2023, max compression
```

## Comparing `mds_csv_reader-1.0.4.tar` & `mds_csv_reader-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/csv_reader/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       88 2020-01-09 14:49:18.000000 mds_csv_reader-1.0.4/csv_reader/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8943 2020-01-09 12:08:00.000000 mds_csv_reader-1.0.4/csv_reader/libcsvread.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1523 2019-12-17 10:45:40.000000 mds_csv_reader-1.0.4/setup.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3081 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/PKG-INFO
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3081 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       11 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      256 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2019-12-17 10:45:47.000000 mds_csv_reader-1.0.4/mds_csv_reader.egg-info/not-zip-safe
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1685 2020-01-09 14:50:06.000000 mds_csv_reader-1.0.4/README.rst
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2020-01-09 14:51:17.000000 mds_csv_reader-1.0.4/setup.cfg
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-28 07:21:42.484582 mds_csv_reader-1.0.5/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3253 2023-07-28 07:21:42.484582 mds_csv_reader-1.0.5/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1725 2023-07-28 07:21:17.000000 mds_csv_reader-1.0.5/README.rst
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-28 07:21:42.464582 mds_csv_reader-1.0.5/csv_reader/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)       89 2023-07-28 07:20:42.000000 mds_csv_reader-1.0.5/csv_reader/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9409 2023-07-28 07:20:46.000000 mds_csv_reader-1.0.5/csv_reader/libcsvread.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-28 07:21:42.480582 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3253 2023-07-28 07:21:41.000000 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      256 2023-07-28 07:21:42.000000 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-28 07:21:41.000000 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2019-12-17 10:45:47.000000 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       11 2023-07-28 07:21:41.000000 mds_csv_reader-1.0.5/mds_csv_reader.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-28 07:21:42.484582 mds_csv_reader-1.0.5/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1624 2023-07-28 07:20:46.000000 mds_csv_reader-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mds_csv_reader-1.0.4/csv_reader/libcsvread.py` & `mds_csv_reader-1.0.5/csv_reader/libcsvread.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,158 +1,180 @@
 # -*- coding: utf-8 -*-
 
 
 import csv
-from io import StringIO, IOBase, BytesIO
+from io import StringIO, IOBase
 from decimal import Decimal
 from datetime import date, datetime, time
 
 
 def get_datetime_format(columnname):
     """ extract format from column-name, return: list of format strings
     """
     # select datetime format
     k2 = columnname.split(',')
-    
+
     if len(k2) == 3:
         dt_fmt = k2[2]
         dt_typ = k2[1]
         # check format - find a valid format string
-        f1 = ['y','Y','m','d','H','M','S']
+        f1 = ['y', 'Y', 'm', 'd', 'H', 'M', 'S']
         fnd1 = False
         for i in f1:
             if '%%%s' % i in dt_fmt:
                 fnd1 = True
                 break
-        if fnd1 == False:
-            raise ValueError('no format string found in column name, expected %%Y %%y %%m %%d %%H %%M %%S (was: %s)' % columnname)
+        if fnd1 is False:
+            raise ValueError(
+                'no format string found in column name, ' +
+                'expected %%Y %%y %%m %%d %%H %%M %%S (was: %s)' % columnname)
         dt_fmt = [dt_fmt]
     elif len(k2) == 2:
         if k2[1].lower() == 'd':
-            dt_fmt = ['%Y-%m-%d', '%d.%m.%Y', '%d-%m-%Y', '%Y/%m/%d', '%d/%m/%Y','%m/%d/%Y', '%Y%m%d']
+            dt_fmt = [
+                '%Y-%m-%d', '%d.%m.%Y', '%d-%m-%Y', '%Y/%m/%d',
+                '%d/%m/%Y', '%m/%d/%Y', '%Y%m%d']
             dt_typ = 'd'
         elif k2[1].lower() == 't':
             dt_fmt = ['%H:%M', '%H:%M:%S']
             dt_typ = 't'
         elif k2[1].lower() == 'dt':
-            dt_fmt = ['%Y-%m-%d %H:%M:%S', '%Y/%m/%d %H:%M:%S', '%d.%m.%Y %H:%M']
+            dt_fmt = [
+                '%Y-%m-%d %H:%M:%S', '%Y/%m/%d %H:%M:%S',
+                '%d.%m.%Y %H:%M']
             dt_typ = 'dt'
-    else :
-        raise ValueError('invalid column-name: datetime/date/time --> DT|D|T[,<format string>] (was: "%s")' % columnname)
+    else:
+        raise ValueError(
+            'invalid column-name: datetime/date/time --> ' +
+            'DT|D|T[,<format string>] (was: "%s")' % columnname)
     return (dt_fmt, dt_typ)
 # end get_datetime_format
 
 
 def detect_field_type(feldlst):
     """ detects type by dbase-fieldname,
-        C = Char, L = Boolean, D = Date, 
+        C = Char, L = Boolean, D = Date,
         N = Numeric (N,10,2 = Decimal(10,2) , N,10,0 = Integer),
         e.g.: 'AMOUNT,N,10,2' --> Numeric(digits=(16, 2)) --> 0.00
             'TEMPERATURE,N,3,0' --> Int
     """
     deci_lst = []
     int_lst = []
     text_lst = []
     bool_lst = []
     datum_lst = []
     ren_dict = {}   # rename fields
     infotxt = ''
-    
+
     for i in feldlst:
         l1 = i.split(',')
-        
+
         # name of fields in first part
         fname = l1[0]
         ren_dict[i] = fname
-        
+
         if len(l1) > 1:
             if l1[1].lower() == 'c':
                 text_lst.append(fname)
             elif l1[1].lower() == 'l':
                 bool_lst.append(fname)
             elif l1[1].lower() in ['d', 't', 'dt']:
                 (dt_fmt, dt_typ) = get_datetime_format(i)
                 datum_lst.append((fname, dt_fmt, dt_typ))
             elif l1[1].lower() == 'n':
                 if len(l1) == 4:
                     if l1[3] == '0':
                         int_lst.append(fname)
-                    else :
+                    else:
                         deci_lst.append(fname)
-                else :
-                    infotxt += u"detect_field_type: invalid numeric-fieldname '%s'\n" % l1
-            else :
-                infotxt += u"detect_field_type: undefined fieldtype '%s'\n" % l1[1]
-        else :
-            infotxt += u"detect_field_type: Error - invalid Fieldname '%s'\n" % l1
+                else:
+                    infotxt += u"detect_field_type: " + \
+                        u"invalid numeric-fieldname '%s'\n" % l1
+            else:
+                infotxt += u"detect_field_type: undefined " + \
+                    u"fieldtype '%s'\n" % l1[1]
+        else:
+            infotxt += u"detect_field_type: Error - " + \
+                u"invalid Fieldname '%s'\n" % l1
             continue
-    return (deci_lst, int_lst, text_lst, bool_lst, datum_lst, ren_dict, infotxt)
+    return (
+        deci_lst, int_lst, text_lst, bool_lst, datum_lst,
+        ren_dict, infotxt)
+
 # end detect_field_type
 
 
-def import_csv_file(csvfile, firstline=True, decimalremove=['€', 'EUR', '.'], 
+def import_csv_file(
+        csvfile, firstline=True, decimalremove=['€', 'EUR', '.'],
         ignline=[], ignore_leer=[], encod='utf-8'):
     """ read csf-file,
         csvfile = File or String,
         firstline: first line contains column names,
           column names must contain field type info:
-            NAME1,C --> type String, 
-            CREATEDATE,D[,<date format>, %Y-%m-%d, %d/%m/%Y, ...] --> type Date, 
+            NAME1,C --> type String,
+            CREATEDATE,D[,<date format>, %Y-%m-%d, %d/%m/%Y, ...]
+                --> type Date,
             DATETIME,DT[,<date time format>, %Y-%m-%d %H:%M] --> type DateTime,
             CREATETIME,T[,<time format>, %H:%M] --> type Time,
             NUMSTEP,N,10,0 --> type Numeric (no decimals) --> Integer,
             AMOUNT,N,16,2 --> type Numeric (two decimals) --> Decimal,
-            ISENABLED,L --> Boolean (allowed: true, false, t, f, wahr, falsch, 1, 0),
+            ISENABLED,L --> Boolean
+                (allowed: true, false, t, f, wahr, falsch, 1, 0),
           default-type: String, (if convert to requested type fails),
-        decimalremove: list of strings to remove from decimal-columns (to remove currency-symbols eg.),
+        decimalremove: list of strings to remove from decimal-columns
+            (to remove currency-symbols eg.),
         ignline: list of line-numbers to skip
         ignore_leer: list of field for which are ignored if empty,
         encod: encoding for byte-type,
-        return: ([{<converted line as dictionary>}, ...], [<field name>, ...], '<info text>')
+        return: ([{<converted line as dictionary>}, ...],
+            [<field name>, ...], '<info text>')
     """
     # get string
     if isinstance(csvfile, type(b'')):
         csvtext = csvfile.decode(encod)
     elif isinstance(csvfile, IOBase):
         csvtext = csvfile.read()
     elif isinstance(csvfile, type('')):
         csvtext = csvfile
-    else :
-        raise ValueError("'csvfile' must be String, Bytes or File-like, was: %s" % str(type(csvfile)))
+    else:
+        raise ValueError(
+            "'csvfile' must be String, " +
+            "Bytes or File-like, was: %s" % str(type(csvfile)))
 
     # detect csv-dialect
     csvdialect = csv.Sniffer().sniff(csvtext[:1024])
-    
+
     # read csv-file
     fhdl_mem = StringIO(csvtext)
     csv_rd = csv.DictReader(fhdl_mem, dialect=csvdialect)
-    
+
     cnt1 = 0
     erg_lst = []
     deci_lst = []
     int_lst = []
     text_lst = []
     bool_lst = []
     datum_lst = []
     ren_dict = {}
     infotxt = u''
 
     for i in csv_rd:
         cnt1 += 1
-        if (cnt1 == 1) and (firstline == True):
+        if (cnt1 == 1) and (firstline is True):
             # first line contains names of rows
             # detect columntypes
-            (deci_lst, int_lst, text_lst, bool_lst, datum_lst, ren_dict, infotxt) = detect_field_type(i.keys())
+            (deci_lst, int_lst, text_lst, bool_lst,
+                datum_lst, ren_dict, infotxt) = detect_field_type(i.keys())
 
         ign_line = cnt1 + 1
         if ign_line in ignline:
             continue
 
         r1 = {}
-        
+
         # 1: convert all columns to string
         for k in i.keys():
             r1[k] = u''
             if isinstance(i[k], type(None)):
                 continue
             if len(i[k]) > 0:
                 r1[k] = i[k].strip()
@@ -165,91 +187,100 @@
             r1[ren_dict[k]] = r1[k]
             del r1[k]
 
         # convert date fields
         for k in datum_lst:
             (fieldname, fieldfmtlst, fieldtype) = k
             t1 = r1.get(fieldname, u'')
-            
+
             # ignore empty fields
             if (fieldname in ignore_leer) and (len(t1) == 0):
                 r1[fieldname] = None
                 continue
-                
-            err_txt = u'import_csv_file: Error while convert date/time: %s, Line=%s, %s="%s"\n'
+
+            err_txt = u'import_csv_file: Error while convert ' + \
+                u'date/time: %s, Line=%s, %s="%s"\n'
             # run through all formats
-            for l in fieldfmtlst:
-                try :
-                    r1[fieldname] = datetime.strptime(t1, l)
+            for x in fieldfmtlst:
+                try:
+                    r1[fieldname] = datetime.strptime(t1, x)
                     # accept first valid value
                     break
                 except UnicodeDecodeError as ex1:
                     infotxt += err_txt % (ex1.reason, cnt1, fieldname, t1)
                     continue
-                except:
+                except Exception:
                     pass
             if isinstance(r1[fieldname], type(datetime(2000, 1, 1, 0, 0, 0))):
                 if fieldtype.lower() == 'd':
-                    r1[fieldname] = date(r1[fieldname].year, r1[fieldname].month, r1[fieldname].day)
+                    r1[fieldname] = date(
+                        r1[fieldname].year, r1[fieldname].month,
+                        r1[fieldname].day)
                 elif fieldtype.lower() == 't':
-                    r1[fieldname] = time(r1[fieldname].hour, r1[fieldname].minute, r1[fieldname].second)
+                    r1[fieldname] = time(
+                        r1[fieldname].hour, r1[fieldname].minute,
+                        r1[fieldname].second)
 
         # convert decimal
         for k in deci_lst:
             t1 = r1.get(k, u'0.0')
-            
+
             # delete some strings
-            for l in decimalremove:
-                t1 = t1.replace(l, u'')
+            for x in decimalremove:
+                t1 = t1.replace(x, u'')
             t1 = t1.strip()
-            
+
             if len(t1) == 0:
                 r1[k] = None
                 continue
-            
-            err_txt = u'import_csv_file: Error while convert decimal: %s, Line=%s, %s="%s"\n'
-            try :
+
+            err_txt = u'import_csv_file: Error while convert ' + \
+                u'decimal: %s, Line=%s, %s="%s"\n'
+            try:
                 r1[k] = Decimal(t1.replace(',', '.'))
             except UnicodeDecodeError as ex1:
                 infotxt += err_txt % (ex1.reason, cnt1, k, t1)
                 r1[k] = None
-            except :
-                infotxt += err_txt % (cnt1, k, t1)
+            except Exception:
+                infotxt += err_txt % ('exception', cnt1, k, t1)
                 r1[k] = None
 
         # bool-bool
         for k in bool_lst:
             t1 = r1.get(k, None)
-            if t1.lower() in ['falsch', 'false', 'no', 'nein','0', 'f', 'n']:
+            if t1.lower() in [
+                    'falsch', 'false', 'no', 'nein', '0', 'f', 'n']:
                 r1[k] = False
-            elif t1.lower() in ['wahr', 'true', 'yes', 'ja', '1', 't', 'j', 'w']:
+            elif t1.lower() in [
+                    'wahr', 'true', 'yes', 'ja', '1', 't', 'j', 'w']:
                 r1[k] = True
-            else :
+            else:
                 r1[k] = None
-                
+
         # convert int
-        err_txt = u'import_csv_file: Error while convert integer: %s, Line=%s, %s="%s"\n'
+        err_txt = u'import_csv_file: Error while convert ' + \
+            u'integer: %s, Line=%s, %s="%s"\n'
         for k in int_lst:
             t1 = r1.get(k, u'0')
 
             if len(t1) == 0:
                 r1[k] = None
                 continue
-            try :
+            try:
                 r1[k] = int(t1)
             except UnicodeDecodeError as ex1:
                 infotxt += err_txt % (ex1.reason, cnt1, k, t1)
                 r1[k] = None
-            except :
-                infotxt += err_txt % (cnt1, k, t1)
+            except Exception:
+                infotxt += err_txt % ('exception', cnt1, k, t1)
                 r1[k] = None
 
         erg_lst.append(r1)
-    
+
     fieldnames = csv_rd.fieldnames
     # cleanup
     del csv_rd
-    
+
     fhdl_mem.close()
     del fhdl_mem
     return (erg_lst, fieldnames, infotxt)
 # end import_csv_file
```

### Comparing `mds_csv_reader-1.0.4/setup.py` & `mds_csv_reader-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """ convert csf-file to list of dictionaries
-""" 
+"""
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 import re
 
 here = path.abspath(path.dirname(__file__))
 MODULE = 'csv_reader'
 PREFIX = 'mds'
 
+
 def read(fname):
     return open(path.join(here, fname), 'r', 'utf-8').read()
 
+
 def get_version():
     init = read(path.join(MODULE, '__init__.py'))
     return re.search("__version__ = '([0-9.]*)'", init).group(1)
 
+
 # Get the long description from the README file
 long_description = read('README.rst')
-    
+
 requires = []
 
-setup(name='mds_csv_reader',
+setup(
+    name='mds_csv_reader',
     version=get_version(),
     description='Convert csv-file to list of dictinaries',
     long_description=long_description,
     author='martin-data services',
     author_email='service@m-ds.de',
     url='https://www.m-ds.de/',
     install_requires=requires,
@@ -39,12 +43,14 @@
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Libraries :: Python Modules',
         ],
     license='GPL-3',
     keywords='csv convert',
 )
```

### Comparing `mds_csv_reader-1.0.4/PKG-INFO` & `mds_csv_reader-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds_csv_reader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Convert csv-file to list of dictinaries
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-csv-reader
         ==============
@@ -63,14 +63,18 @@
         default-type: String
          if convert to requested type fails
         
         
         Changes
         =======
         
+        *1.0.5 - 28.07.2023*
+        
+        - code optimized
+        
         *1.0.4 - 09.01.2020*
         
         - fix: detection of boolean, import of csv-text-data
         
         *1.0.2 - 20.12.2019*
         
         - exteded detection of date and time formats
@@ -90,8 +94,10 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mds_csv_reader-1.0.4/mds_csv_reader.egg-info/PKG-INFO` & `mds_csv_reader-1.0.5/mds_csv_reader.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mds-csv-reader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Convert csv-file to list of dictinaries
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-csv-reader
         ==============
@@ -63,14 +63,18 @@
         default-type: String
          if convert to requested type fails
         
         
         Changes
         =======
         
+        *1.0.5 - 28.07.2023*
+        
+        - code optimized
+        
         *1.0.4 - 09.01.2020*
         
         - fix: detection of boolean, import of csv-text-data
         
         *1.0.2 - 20.12.2019*
         
         - exteded detection of date and time formats
@@ -90,8 +94,10 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mds_csv_reader-1.0.4/README.rst` & `mds_csv_reader-1.0.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 default-type: String
  if convert to requested type fails
 
 
 Changes
 =======
 
+*1.0.5 - 28.07.2023*
+
+- code optimized
+
 *1.0.4 - 09.01.2020*
 
 - fix: detection of boolean, import of csv-text-data
 
 *1.0.2 - 20.12.2019*
 
 - exteded detection of date and time formats
```

