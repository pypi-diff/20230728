# Comparing `tmp/dkimpy-1.1.4.tar.gz` & `tmp/dkimpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkimpy-1.1.4.tar", last modified: Fri May 12 05:18:26 2023, max compression
+gzip compressed data, was "dkimpy-1.1.5.tar", last modified: Fri Jul 28 16:02:28 2023, max compression
```

## Comparing `dkimpy-1.1.4.tar` & `dkimpy-1.1.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.983443 dkimpy-1.1.4/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    14121 2023-05-12 05:17:52.000000 dkimpy-1.1.4/ChangeLog
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.4/LICENSE
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.4/MANIFEST.in
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-05-12 05:18:26.983443 dkimpy-1.1.4/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8122 2023-05-07 18:37:17.000000 dkimpy-1.1.4/README.md
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.975443 dkimpy-1.1.4/dkim/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57999 2023-05-12 05:08:45.000000 dkimpy-1.1.4/dkim/__init__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/__main__.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/arcsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/arcverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/asn1.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-04-30 13:58:34.000000 dkimpy-1.1.4/dkim/asyncsupport.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/dkimsign.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/dkimverify.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4737 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/dknewkey.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3300 2023-05-12 05:07:38.000000 dkimpy-1.1.4/dkim/dnsplug.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.979443 dkimpy-1.1.4/dkim/tests/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/__init__.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.979443 dkimpy-1.1.4/dkim/tests/data/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/1024_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/1024_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/2048_testkey.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/data/2048_testkey_PKCS8.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/2048_testkey_wo_markers.pub.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/badk.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/badversion.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/ed25519test.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/ed25519test.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/ed25519test.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/ed25519test2.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/eximtest.dns
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/message.mbox
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/rfc6376.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/rfc6376.signed.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/rfc6376.signed.rsa.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/data/rfc6376.w1258.msg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/rfc8032_7_1.key
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/data/test.message.baddomain
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test2.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test2.private
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test2.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test_bad.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test_extra.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/data/test_nofrom.message
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/data/test_tlsrpt.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/test_arc.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/test_canonicalization.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/test_crypto.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/test_dkim.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/test_dkim_ed25519.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4476 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/test_dkim_generate.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2023-04-30 14:18:48.000000 dkimpy-1.1.4/dkim/tests/test_dkim_rsavariants.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/test_dkim_tlsrpt.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.4/dkim/tests/test_dnsplug.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/tests/test_util.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.4/dkim/util.py
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.983443 dkimpy-1.1.4/dkimpy.egg-info/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/PKG-INFO
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/SOURCES.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/dependency_links.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/entry_points.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.4/dkimpy.egg-info/not-zip-safe
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/requires.txt
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-05-12 05:18:26.000000 dkimpy-1.1.4/dkimpy.egg-info/top_level.txt
-drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-05-12 05:18:26.983443 dkimpy-1.1.4/man/
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.4/man/arcsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.4/man/arcverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.4/man/dkimsign.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2023-04-30 14:18:48.000000 dkimpy-1.1.4/man/dkimverify.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.4/man/dknewkey.1
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-05-12 05:18:26.983443 dkimpy-1.1.4/setup.cfg
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3387 2023-05-07 18:35:32.000000 dkimpy-1.1.4/setup.py
--rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.4/test.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.864313 dkimpy-1.1.5/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    14298 2023-07-28 15:57:20.000000 dkimpy-1.1.5/ChangeLog
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      979 2020-04-06 04:06:13.000000 dkimpy-1.1.5/LICENSE
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      200 2020-04-06 04:27:45.000000 dkimpy-1.1.5/MANIFEST.in
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-07-28 16:02:28.864313 dkimpy-1.1.5/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8122 2023-07-28 15:59:27.000000 dkimpy-1.1.5/README.md
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.840312 dkimpy-1.1.5/dkim/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    57999 2023-05-12 05:08:45.000000 dkimpy-1.1.5/dkim/__init__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      139 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/__main__.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2570 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/arcsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1774 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/arcverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4300 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/asn1.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4829 2023-04-30 13:58:34.000000 dkimpy-1.1.5/dkim/asyncsupport.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4610 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     8173 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3628 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/dkimsign.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1951 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/dkimverify.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4737 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/dknewkey.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3315 2023-07-28 15:54:58.000000 dkimpy-1.1.5/dkim/dnsplug.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.848312 dkimpy-1.1.5/dkim/tests/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1769 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/__init__.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.860313 dkimpy-1.1.5/dkim/tests/data/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      212 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/1024_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1679 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1704 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      384 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_wo_markers.pub.rsa.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      416 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/2048_testkey_wo_markers.pub.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      251 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/badk.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/badversion.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       58 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      588 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/ed25519test2.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       67 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/eximtest.dns
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4444 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/message.mbox
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      269 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1069 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      708 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.rsa.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      275 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/rfc6376.w1258.msg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       45 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/rfc8032_7_1.key
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      346 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      778 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/data/test.message.baddomain
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1104 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      887 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.private
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      233 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test2.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      240 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_bad.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      219 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_extra.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      164 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/data/test_nofrom.message
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      250 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/data/test_tlsrpt.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     5300 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_arc.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6045 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_canonicalization.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     6786 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_crypto.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    23644 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    12866 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dkim_ed25519.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4476 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim_generate.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2023-04-30 14:18:48.000000 dkimpy-1.1.5/dkim/tests/test_dkim_rsavariants.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11980 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dkim_tlsrpt.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1557 2020-04-06 04:27:45.000000 dkimpy-1.1.5/dkim/tests/test_dnsplug.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3432 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/tests/test_util.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     2501 2020-04-06 04:06:13.000000 dkimpy-1.1.5/dkim/util.py
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.860313 dkimpy-1.1.5/dkimpy.egg-info/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)    11065 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/PKG-INFO
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     1986 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      173 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/entry_points.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        1 2020-04-06 12:14:30.000000 dkimpy-1.1.5/dkimpy.egg-info/not-zip-safe
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       84 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/requires.txt
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)        5 2023-07-28 16:02:28.000000 dkimpy-1.1.5/dkimpy.egg-info/top_level.txt
+drwxr-xr-x   0 kitterma  (1001) kitterma  (1001)        0 2023-07-28 16:02:28.864313 dkimpy-1.1.5/man/
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4392 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/arcsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4152 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/arcverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4957 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/dkimsign.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4273 2023-04-30 14:18:48.000000 dkimpy-1.1.5/man/dkimverify.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     4923 2020-04-06 04:06:13.000000 dkimpy-1.1.5/man/dknewkey.1
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)       38 2023-07-28 16:02:28.864313 dkimpy-1.1.5/setup.cfg
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)     3386 2023-07-28 15:59:47.000000 dkimpy-1.1.5/setup.py
+-rw-r--r--   0 kitterma  (1001) kitterma  (1001)      268 2020-04-06 04:06:13.000000 dkimpy-1.1.5/test.py
```

### Comparing `dkimpy-1.1.4/ChangeLog` & `dkimpy-1.1.5/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-28 Version 1.1.5
+   - Use dns.resolver.resolve instead of dns.resolver.query due to deprecation
+     (LP: 2028783) - Thanks to Pedro Vicente for the report and the fix
+
 2023-05-12 Version 1.1.4
    - Treat dns.resolver.NoNameservers like NXDOMAIN (not an error) (Thanks to
      David for the patch and the report)
    - Confine errors from dnspython to dnsplug and use dkim errors, since
      dkim.__init__.py doesn't import dns and needs dkim errors (LP: #2018646)
 
 2023-04-30 Version 1.1.3
```

### Comparing `dkimpy-1.1.4/LICENSE` & `dkimpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/PKG-INFO` & `dkimpy-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.4.
+        This is dkimpy 1.1.5.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.4/README.md` & `dkimpy-1.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
 signing and verification.  Basic DKIM requirements are defined in RFC 6376:
 
 https://tools.ietf.org/html/rfc6376
 
 # VERSION
 
-This is dkimpy 1.1.4.
+This is dkimpy 1.1.5.
 
 # REQUIREMENTS
 
 Dependencies will be automatically included for normal DKIM usage.  The
 extras_requires feature 'ed25519' will add the dependencies needed for signing
 and verifying using the new DCRUP ed25519-sha256 algorithm.  The
 extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.4/dkim/__init__.py` & `dkimpy-1.1.5/dkim/__init__.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/arcsign.py` & `dkimpy-1.1.5/dkim/arcsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/arcverify.py` & `dkimpy-1.1.5/dkim/arcverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/asn1.py` & `dkimpy-1.1.5/dkim/asn1.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/asyncsupport.py` & `dkimpy-1.1.5/dkim/asyncsupport.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/canonicalization.py` & `dkimpy-1.1.5/dkim/canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/crypto.py` & `dkimpy-1.1.5/dkim/crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/dkimsign.py` & `dkimpy-1.1.5/dkim/dkimsign.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/dkimverify.py` & `dkimpy-1.1.5/dkim/dkimverify.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/dknewkey.py` & `dkimpy-1.1.5/dkim/dknewkey.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/dnsplug.py` & `dkimpy-1.1.5/dkim/dnsplug.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ]
 
 
 def get_txt_dnspython(name, timeout=5):
     """Return a TXT record associated with a DNS name."""
     import dkim
     try:
-      a = dns.resolver.query(name, dns.rdatatype.TXT,raise_on_no_answer=False, lifetime=timeout)
+      a = dns.resolver.resolve(name, dns.rdatatype.TXT,raise_on_no_answer=False, lifetime=timeout, search=True)
       for r in a.response.answer:
           if r.rdtype == dns.rdatatype.TXT:
               return b"".join(list(r.items)[0].strings)
     except dns.resolver.NXDOMAIN: pass
     except dns.resolver.NoNameservers: pass
     except dns.resolver.NoResolverConfiguration as e:
         raise dkim.DnsTimeoutError('dns.resolver.NoResolverConfiguration: {0}'.format(e))
```

### Comparing `dkimpy-1.1.4/dkim/tests/__init__.py` & `dkimpy-1.1.5/dkim/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/1024_testkey.key` & `dkimpy-1.1.5/dkim/tests/data/1024_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/2048_testkey.key` & `dkimpy-1.1.5/dkim/tests/data/2048_testkey.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/2048_testkey_PKCS8.key` & `dkimpy-1.1.5/dkim/tests/data/2048_testkey_PKCS8.key`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/ed25519test2.msg` & `dkimpy-1.1.5/dkim/tests/data/ed25519test2.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/message.mbox` & `dkimpy-1.1.5/dkim/tests/data/message.mbox`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/rfc6376.signed.msg` & `dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/rfc6376.signed.rsa.msg` & `dkimpy-1.1.5/dkim/tests/data/rfc6376.signed.rsa.msg`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/test.message.baddomain` & `dkimpy-1.1.5/dkim/tests/data/test.message.baddomain`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/test.private` & `dkimpy-1.1.5/dkim/tests/data/test.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/test2.message` & `dkimpy-1.1.5/dkim/tests/data/test2.message`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/data/test2.private` & `dkimpy-1.1.5/dkim/tests/data/test2.private`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_arc.py` & `dkimpy-1.1.5/dkim/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_canonicalization.py` & `dkimpy-1.1.5/dkim/tests/test_canonicalization.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_crypto.py` & `dkimpy-1.1.5/dkim/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dkim.py` & `dkimpy-1.1.5/dkim/tests/test_dkim.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dkim_ed25519.py` & `dkimpy-1.1.5/dkim/tests/test_dkim_ed25519.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dkim_generate.py` & `dkimpy-1.1.5/dkim/tests/test_dkim_generate.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dkim_rsavariants.py` & `dkimpy-1.1.5/dkim/tests/test_dkim_rsavariants.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dkim_tlsrpt.py` & `dkimpy-1.1.5/dkim/tests/test_dkim_tlsrpt.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_dnsplug.py` & `dkimpy-1.1.5/dkim/tests/test_dnsplug.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/tests/test_util.py` & `dkimpy-1.1.5/dkim/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkim/util.py` & `dkimpy-1.1.5/dkim/util.py`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/dkimpy.egg-info/PKG-INFO` & `dkimpy-1.1.5/dkimpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkimpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: DKIM (DomainKeys Identified Mail), ARC (Authenticated Receive Chain), and TLSRPT (TLS Report) email signing and verification
 Home-page: https://launchpad.net/dkimpy
 Author: Scott Kitterman
 Author-email: scott@kitterman.com
 License: BSD-like
 Description: dkimpy - DKIM (DomainKeys Identified Mail)
         https://launchpad.net/dkimpy/
@@ -17,15 +17,15 @@
         dkimpy is a library that implements DKIM (DomainKeys Identified Mail) email
         signing and verification.  Basic DKIM requirements are defined in RFC 6376:
         
         https://tools.ietf.org/html/rfc6376
         
         # VERSION
         
-        This is dkimpy 1.1.4.
+        This is dkimpy 1.1.5.
         
         # REQUIREMENTS
         
         Dependencies will be automatically included for normal DKIM usage.  The
         extras_requires feature 'ed25519' will add the dependencies needed for signing
         and verifying using the new DCRUP ed25519-sha256 algorithm.  The
         extras_requires feature 'ARC' will add the extra dependencies needed for ARC.
```

### Comparing `dkimpy-1.1.4/dkimpy.egg-info/SOURCES.txt` & `dkimpy-1.1.5/dkimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/man/arcsign.1` & `dkimpy-1.1.5/man/arcsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/man/arcverify.1` & `dkimpy-1.1.5/man/arcverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/man/dkimsign.1` & `dkimpy-1.1.5/man/dkimsign.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/man/dkimverify.1` & `dkimpy-1.1.5/man/dkimverify.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/man/dknewkey.1` & `dkimpy-1.1.5/man/dknewkey.1`

 * *Files identical despite different names*

### Comparing `dkimpy-1.1.4/setup.py` & `dkimpy-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 # This has been modified from the original software.
 # Copyright (c) 2011,2012,2018 Scott Kitterman <scott@kitterman.com>
 
 from setuptools import setup
 import os
 import sys
 
-version = "1.1.4"
+version = "1.1.5"
 
 kw = {}  # Work-around for lack of 'or' requires in setuptools.
 try:
     import DNS
     kw['install_requires'] = ['Py3DNS']
 except ImportError:  # If PyDNS is not installed, prefer dnspython
-    kw['install_requires'] = ['dnspython>=1.16.0']
+    kw['install_requires'] = ['dnspython>=2.0.0']
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "dkimpy",
     version = version,
```

