# Comparing `tmp/saspy-5.2.2.tar.gz` & `tmp/saspy-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.2.2.tar", last modified: Fri Jul  7 20:04:31 2023, max compression
+gzip compressed data, was "saspy-5.2.3.tar", last modified: Fri Jul 28 19:15:19 2023, max compression
```

## Comparing `saspy-5.2.2.tar` & `saspy-5.2.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.341883 saspy-5.2.2/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-07-07 20:04:15.000000 saspy-5.2.2/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-07-07 20:04:15.000000 saspy-5.2.2/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-07 20:04:31.340883 saspy-5.2.2/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-07-07 20:04:15.000000 saspy-5.2.2/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-07-07 20:04:15.000000 saspy-5.2.2/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.320881 saspy-5.2.2/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.322882 saspy-5.2.2/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.331882 saspy-5.2.2/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.334882 saspy-5.2.2/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.339883 saspy-5.2.2/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   130270 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2418 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37669 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87058 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    87201 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    99770 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.340883 saspy-5.2.2/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-07-07 20:04:15.000000 saspy-5.2.2/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-07 20:04:31.321882 saspy-5.2.2/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-07-07 20:04:31.000000 saspy-5.2.2/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-07-07 20:04:31.341883 saspy-5.2.2/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-07-07 20:04:15.000000 saspy-5.2.2/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.883450 saspy-5.2.3/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2023-07-28 19:15:04.000000 saspy-5.2.3/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2023-07-28 19:15:04.000000 saspy-5.2.3/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-28 19:15:19.883450 saspy-5.2.3/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2023-07-28 19:15:04.000000 saspy-5.2.3/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2023-07-28 19:15:04.000000 saspy-5.2.3/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.853448 saspy-5.2.3/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.855448 saspy-5.2.3/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.869449 saspy-5.2.3/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.874449 saspy-5.2.3/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    17665 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    32061 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18548 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.882450 saspy-5.2.3/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   131141 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10967 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3430 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    35589 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    85134 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    84878 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    97422 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.882450 saspy-5.2.3/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2023-07-28 19:15:04.000000 saspy-5.2.3/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2023-07-28 19:15:19.855448 saspy-5.2.3/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4007 2023-07-28 19:15:19.000000 saspy-5.2.3/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1392 2023-07-28 19:15:19.000000 saspy-5.2.3/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2023-07-28 19:15:19.000000 saspy-5.2.3/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2023-07-28 19:15:19.000000 saspy-5.2.3/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2023-07-28 19:15:19.000000 saspy-5.2.3/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2023-07-28 19:15:19.884450 saspy-5.2.3/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2023-07-28 19:15:04.000000 saspy-5.2.3/setup.py
```

### Comparing `saspy-5.2.2/LICENSE.md` & `saspy-5.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/PKG-INFO` & `saspy-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.2.2
+Version: 5.2.3
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.2.2/README.md` & `saspy-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/SASLogLexer.py` & `saspy-5.2.3/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/__init__.py` & `saspy-5.2.3/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/autocfg.py` & `saspy-5.2.3/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.2.3/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/sas.core.jar` & `saspy-5.2.3/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.2.3/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.2.3/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/pyiom/saspy2j.class` & `saspy-5.2.3/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/pyiom/saspy2j.java` & `saspy-5.2.3/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/saspyiom.jar` & `saspy-5.2.3/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/NOTICE.md` & `saspy-5.2.3/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.2.3/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.2.3/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.2.3/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/libname_gen.sas` & `saspy-5.2.3/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasViyaML.py` & `saspy-5.2.3/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sas_magic.py` & `saspy-5.2.3/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasbase.py` & `saspy-5.2.3/saspy/sasbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1174,15 +1174,30 @@
         """
         lastlog = len(self._io._log)
         opts    = opts if opts is not None else {}
 
         if results == '':
             results = self.results
 
-        self._io.read_csv(file, table, libref, self.nosub, opts)
+        code  = "filename _x "
+
+        if file.lower().startswith("http"):
+           code += "url "
+
+        code += "\""+file+"\";\n"
+        code += "proc import datafile=_x out="
+        if len(libref):
+           code += libref+"."
+        code += "'"+table.strip().replace("'", "''")+"'n dbms=csv replace; "+self._impopts(opts)+" run;"
+        code += "filename _x clear;\n"
+
+        if self.nosub:
+           print(code)
+        else:
+           ll = self._io.submit(code, "text")
 
         if self.exist(table, libref):
             sd = SASdata(self, libref, table, results)
         else:
             sd =None
 
         self._lastlog = self._io._log[lastlog:]
@@ -1226,17 +1241,33 @@
 
                              {'delimiter' : '~',
                               'putnames'  : True
                              }
         :return: SAS log
         """
         dsopts = dsopts if dsopts is not None else {}
-        opts = opts if opts is not None else {}
+        opts   = opts if opts is not None else {}
+
+        code  = "filename _x \""+file+"\";\n"
+        code += "options nosource;\n"
+        code += "proc export data="
+
+        if len(libref):
+           code += libref+"."
+
+        code += "'"+table.strip().replace("'", "''")+"'n "+self._dsopts(dsopts)+" outfile=_x dbms=csv replace;\n"
+        code += self._expopts(opts)+" run;\n"
+        code += "filename _x clear;"
+        code += "options source;\n"
+
+        if self.nosub:
+           print(code)
+        else:
+           log = self._io.submit(code, "text")['LOG']
 
-        log = self._io.write_csv(file, table, libref, self.nosub, dsopts, opts)
         if not self.batch:
             print(log)
         else:
             return log
 
     def upload(self, localfile: str, remotefile: str, overwrite: bool = True, permission: str = '', **kwargs):
         """
```

### Comparing `saspy-5.2.2/saspy/sascfg.py` & `saspy-5.2.3/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasdata.py` & `saspy-5.2.3/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasdecorator.py` & `saspy-5.2.3/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasets.py` & `saspy-5.2.3/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasiocom.py` & `saspy-5.2.3/saspy/sasiocom.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 import datetime
-import csv
 import io
 import numbers
 import os
 import shlex
 import sys
 import warnings
 
@@ -597,65 +596,14 @@
             rows.append([meta[x.Name]['CONVERT'](x.Value) for x in recordset.Fields])
             recordset.MoveNext()
 
         recordset.Close()
 
         return (header, rows, meta)
 
-    def read_csv(self, filepath: str, table: str, libref: str=None, nosub: bool=False, opts: dict=None):
-        """
-        Submit an import job to the SAS workspace.
-        :param filepath [str]: File URI.
-        :param table [str]: Table name.
-        :option libref [str]: Library name.
-        :option nosob [bool]: Return the SAS code instead of executing it.
-        :option opts [dict]: SAS PROC IMPORT options.
-        """
-        opts = opts if opts is not None else {}
-        filepath = 'url ' + filepath if filepath.lower().startswith('http') else filepath
-        tablepath = self._tablepath(table, libref=libref)
-
-        proc_code = """
-            filename csv_file "{}";
-            proc import datafile=csv_file out={} dbms=csv replace;
-                {}
-            run;
-        """.format(filepath.replace('"', '""'), tablepath, self._sb._impopts(opts))
-
-        if nosub is True:
-            return proc_code
-        else:
-            return self.submit(proc_code, 'text')
-
-    def write_csv(self, filepath: str, table: str, libref: str=None, nosub: bool=True, dsopts: dict=None, opts: dict=None):
-        """
-        Submit an export job to the SAS workspace.
-        :param filepath [str]: File URI.
-        :param table [str]: Table name.
-        :option libref [str]: Library name.
-        :option nosob [bool]: Return the SAS code instead of executing it.
-        :option opts [dict]: SAS PROC IMPORT options.
-        :option dsopts [dict]: SAS dataset options.
-        """
-        opts = opts if opts is not None else {}
-        dsopts = dsopts if dsopts is not None else {}
-        tablepath = self._tablepath(table, libref=libref)
-
-        proc_code = """
-            filename csv_file "{}";
-            proc export data={} {} outfile=csv_file dbms=csv replace;
-                {}
-            run;
-        """.format(filepath.replace('"', '""'), tablepath, self._sb._dsopts(dsopts), self._sb._expopts(opts))
-
-        if nosub is True:
-            return proc_code
-        else:
-            return self.submit(proc_code, 'text')['LOG']
-
     def dataframe2sasdata(self, df: '<Pandas Data Frame object>', table: str ='a',
                           libref: str ="", keep_outer_quotes: bool=False,
                                            embedded_newlines: bool=True,
                           LF: str = '\x01', CR: str = '\x02',
                           colsep: str = '\x03', colrep: str = ' ',
                           datetimes: dict={}, outfmts: dict={}, labels: dict={},
                           outdsopts: dict={}, encode_errors = None, char_lengths = None,
```

### Comparing `saspy-5.2.2/saspy/sasiohttp.py` & `saspy-5.2.3/saspy/sasiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,16 +542,16 @@
             if contexts[i].get('name') == self.ctxname:
                self.ctx = contexts[i]
                break
 
          if self.ctx == {}:
             raise SASHTTPconnectionError(msg="No context information returned for context {}\n{}".format(self.ctxname, contexts))
       else:
-         self.ctx = contexts
-         self.ctxname = 'tom'
+         self.ctx     = contexts
+         self.ctxname = self.serverid
 
          return
 
    def _authenticate(self, user, pw, authcode, client_id, client_secret, jwt):
 
       if self.serverid:
          return {'access_token':'tom'}
@@ -600,16 +600,14 @@
          raise SASHTTPauthenticateError(msg)
          #return None
 
       js = json.loads(resp.decode(self.encoding))
       return js
 
    def _get_contexts(self):
-      #import pdb; pdb.set_trace()
-
       # GET Contexts
       conn = self.HTTPConn; conn.connect()
 
       if not self.serverid:
          headers={"Accept":"application/vnd.sas.collection+json",
                   "Accept-Item":"application/vnd.sas.compute.context.summary+json",
                   "Authorization":"Bearer "+self._token}
@@ -707,15 +705,15 @@
          options = (options.rpartition(','))[0]+']'
       else:
          options = '[]'
 
       # POST Session
       uri = None
       for ld in self.sascfg.ctx.get('links'):
-         if ld.get('method') == 'POST':
+         if ld.get('method') == 'POST' and ld.get('rel') == 'createSession':
             uri = ld.get('uri')
             break
 
       if not uri:
          raise SASHTTPconnectionError(msg=
          "POST uri not found in context info. You may not have permission to use this context.\n{}".format(self.sascfg.ctx))
 
@@ -1262,63 +1260,14 @@
          exists = True
       else:
          exists = False
 
       return exists
       """
 
-   def read_csv(self, file: str, table: str, libref: str ="", nosub: bool=False, opts: dict ={}) -> '<SASdata object>':
-      '''
-      This method will import a csv file into a SAS Data Set and return the SASdata object referring to it.
-      file    - eithe the OS filesystem path of the file, or HTTP://... for a url accessible file
-      table   - the name of the SAS Data Set to create
-      libref  - the libref for the SAS Data Set being created. Defaults to WORK, or USER if assigned
-      opts    - a dictionary containing any of the following Proc Import options(datarow, delimiter, getnames, guessingrows)
-      '''
-      code  = "filename x "
-
-      if file.lower().startswith("http"):
-         code += "url "
-
-      code += "\""+file+"\";\n"
-      code += "proc import datafile=x out="
-      if len(libref):
-         code += libref+"."
-      code += "'"+table.strip().replace("'", "''")+"'n dbms=csv replace; "+self._sb._impopts(opts)+" run;"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-
-   def write_csv(self, file: str, table: str, libref: str ="", nosub: bool =False, dsopts: dict ={}, opts: dict ={}) -> 'The LOG showing the results of the step':
-      '''
-      This method will export a SAS Data Set to a file in CCSV format.
-      file    - the OS filesystem path of the file to be created (exported from the SAS Data Set)
-      table   - the name of the SAS Data Set you want to export to a CSV file
-      libref  - the libref for the SAS Data Set.
-      opts    - a dictionary containing any of the following Proc Export options(delimiter, putnames)
-      '''
-      code  = "filename x \""+file+"\";\n"
-      code += "options nosource;\n"
-      code += "proc export data="
-
-      if len(libref):
-         code += libref+"."
-
-      code += "'"+table.strip().replace("'", "''")+"'n "+self._sb._dsopts(dsopts)+" outfile=x dbms=csv replace; "
-      code += self._sb._expopts(opts)+" run\n;"
-      code += "options source;\n"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-         return ll['LOG']
-
    def upload(self, localfile: str, remotefile: str, overwrite: bool = True, permission: str = '', **kwargs):
       """
       This method uploads a local file to the SAS servers file system.
       localfile  - path to the local file to upload
       remotefile - path to remote file to create or overwrite
       overwrite  - overwrite the output file if it exists?
       permission - permissions to set on the new file. See SAS Filename Statement Doc for syntax
@@ -1858,14 +1807,15 @@
       else:
          dts = k_dts
 
       code  = "filename _tomodsx '"+self._sb.workpath+"_tomodsx' lrecl="+str(self.sascfg.lrecl)+" recfm=v  encoding='utf-8';\n"
       code += "proc export data=work.sasdata2dataframe outfile=_tomodsx dbms=csv replace;\n"
       code += self._sb._expopts(opts)+" run;\n"
       code += "proc delete data=work.sasdata2dataframe(memtype=view);run;\n"
+      code += "filename _tomodsx;"
 
       ll = self.submit(code, 'text')
       logf  = ll['LOG']
 
       code = "filename _sp_updn '"+self._sb.workpath+"_tomodsx' recfm=F encoding=binary lrecl=4096;"
 
       ll = self.submit(code, "text")
@@ -1887,15 +1837,17 @@
 
       if k_dts is None:  # don't override these if user provided their own dtypes
          for i in range(nvars):
             if vartype[i] == 'FLOAT':
                if varcat[i] in self._sb.sas_date_fmts + self._sb.sas_time_fmts + self._sb.sas_datetime_fmts:
                   df[dvarlist[i]] = pd.to_datetime(df[dvarlist[i]], errors='coerce')
 
-      ll = self.submit("filename _sp_updn;", 'text')
+      code = "data _null_; fdelete(_sp_updn); run;\nfilename _sp_updn;"
+
+      ll = self.submit(code, 'text')
       logf += ll['LOG']
 
       return df
 
    def sasdata2dataframeDISK(self, table: str, libref: str ='', dsopts: dict = None,
                              rowsep: str = '\x01', colsep: str = '\x02',
                              rowrep: str = ' ',    colrep: str = ' ', **kwargs) -> '<Pandas Data Frame object>':
@@ -2061,15 +2013,15 @@
          if i % 10 == 9:
             code +='\n'
       code += "\nput "
       for i in range(nvars):
          code += " '"+varlist[i]+"'n "
          if i % 10 == 9:
             code +='\n'
-      code += rdelim+";\nrun;"
+      code += rdelim+";\nrun;\nfilename _tomodsx;"
 
       ll = self.submit(code, "text")
 
       if k_dts is None:
          dts = {}
          for i in range(nvars):
             if vartype[i] == 'FLOAT':
@@ -2108,15 +2060,17 @@
 
       if k_dts is None:  # don't override these if user provided their own dtypes
          for i in range(nvars):
             if vartype[i] == 'FLOAT':
                if varcat[i] in self._sb.sas_date_fmts + self._sb.sas_time_fmts + self._sb.sas_datetime_fmts:
                   df[dvarlist[i]] = pd.to_datetime(df[dvarlist[i]], errors='coerce')
 
-      ll = self.submit("filename _sp_updn;", 'text')
+      code = "data _null_; fdelete(_sp_updn); run;\nfilename _sp_updn;"
+
+      ll = self.submit(code, 'text')
       logf += ll['LOG']
 
       return df
 
 class _read_sock(io.StringIO):
    def __init__(self, **kwargs):
       self.req      = kwargs.get('req')
```

### Comparing `saspy-5.2.2/saspy/sasioiom.py` & `saspy-5.2.3/saspy/sasioiom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1183,69 +1183,14 @@
 
       l2 = ll['LOG'].rpartition("TABLE_EXISTS= ")
       l2 = l2[2].partition("\n")
       exists = int(l2[0])
 
       return bool(exists)
 
-   def read_csv(self, file: str, table: str, libref: str ="", nosub: bool =False, opts: dict = None) -> '<SASdata object>':
-      """
-      This method will import a csv file into a SAS Data Set and return the SASdata object referring to it.
-      file    - eithe the OS filesystem path of the file, or HTTP://... for a url accessible file
-      table   - the name of the SAS Data Set to create
-      libref  - the libref for the SAS Data Set being created. Defaults to WORK, or USER if assigned
-      opts    - a dictionary containing any of the following Proc Import options(datarow, delimiter, getnames, guessingrows)
-      """
-      opts = opts if opts is not None else {}
-
-      code  = "filename x "
-
-      if file.lower().startswith("http"):
-         code += "url "
-
-      code += "\""+file+"\";\n"
-      code += "proc import datafile=x out="
-      if len(libref):
-         code += libref+"."
-      code += "'"+table.strip().replace("'", "''")+"'n dbms=csv replace; "+self._sb._impopts(opts)+" run;"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-
-   def write_csv(self, file: str, table: str, libref: str ="", nosub: bool =False, dsopts: dict = None, opts: dict = None) -> 'The LOG showing the results of the step':
-      """
-      This method will export a SAS Data Set to a file in CSV format.
-      file    - the OS filesystem path of the file to be created (exported from the SAS Data Set)
-      table   - the name of the SAS Data Set you want to export to a CSV file
-      libref  - the libref for the SAS Data Set.
-      dsopts  - a dictionary containing any of the following SAS data set options(where, drop, keep, obs, firstobs)
-      opts    - a dictionary containing any of the following Proc Export options(delimiter, putnames)
-      """
-      dsopts = dsopts if dsopts is not None else {}
-      opts = opts if opts is not None else {}
-
-      code  = "filename x \""+file+"\";\n"
-      code += "options nosource;\n"
-      code += "proc export data="
-
-      if len(libref):
-         code += libref+"."
-
-      code += "'"+table.strip().replace("'", "''")+"'n "+self._sb._dsopts(dsopts)+" outfile=x dbms=csv replace; "
-      code += self._sb._expopts(opts)+" run\n;"
-      code += "options source;\n"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-         return ll['LOG']
-
    def upload_slow(self, localfile: str, remotefile: str, overwrite: bool = True, permission: str = '', **kwargs):
       """
       This method uploads a local file to the SAS servers file system.
       localfile  - path to the local file to upload
       remotefile - path to remote file to create or overwrite
       overwrite  - overwrite the output file if it exists?
       permission - permissions to set on the new file. See SAS Filename Statement Doc for syntax
@@ -1890,14 +1835,16 @@
          local   = False
          outname = self._tomods1.decode()
          code    = ''
 
       code += "proc export data=work.sasdata2dataframe outfile="+outname+" dbms=csv replace;\n"
       code += self._sb._expopts(opts)+" run;\n"
       code += "proc delete data=work.sasdata2dataframe(memtype=view);run;\n"
+      if local:
+         code += "filename _tomodsx;"
 
       ll = self._asubmit(code, 'text')
 
       self.stdin[0].send(b'\ntom says EOL='+logcodeo.encode())
       #self.stdin[0].send(b'\n'+logcodei.encode()+b'\n'+b'tom says EOL='+logcodeo.encode())
 
       done  = False
```

### Comparing `saspy-5.2.2/saspy/sasiostdio.py` & `saspy-5.2.3/saspy/sasiostdio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1266,69 +1266,14 @@
 
       ll = self.submit(code, "text")
 
       exists = int(ll['LOG'].rpartition("TABLE_EXISTS=")[2].rpartition(" TAB_EXTEND=")[0])
 
       return bool(exists)
 
-   def read_csv(self, file: str, table: str, libref: str ="", nosub: bool =False, opts: dict = None) -> '<SASdata object>':
-      """
-      This method will import a csv file into a SAS Data Set and return the SASdata object referring to it.
-      file    - eithe the OS filesystem path of the file, or HTTP://... for a url accessible file
-      table   - the name of the SAS Data Set to create
-      libref  - the libref for the SAS Data Set being created. Defaults to WORK, or USER if assigned
-      opts    - a dictionary containing any of the following Proc Import options(datarow, delimiter, getnames, guessingrows)
-      """
-      opts = opts if opts is not None else {}
-      code  = "filename x "
-
-      if file.lower().startswith("http"):
-         code += "url "
-
-      code += "\""+file+"\";\n"
-      code += "proc import datafile=x out="
-      if len(libref):
-         code += libref+"."
-
-      code += "'"+table.strip().replace("'", "''")+"'n dbms=csv replace; "+self._sb._impopts(opts)+" run;"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-
-   def write_csv(self, file: str, table: str, libref: str ="", nosub: bool =False, dsopts: dict = None, opts: dict = None) -> 'The LOG showing the results of the step':
-      """
-      This method will export a SAS Data Set to a file in CSV format.
-      file    - the OS filesystem path of the file to be created (exported from the SAS Data Set)
-      table   - the name of the SAS Data Set you want to export to a CSV file
-      libref  - the libref for the SAS Data Set.
-      dsopts  - a dictionary containing any of the following SAS data set options(where, drop, keep, obs, firstobs)
-      opts    - a dictionary containing any of the following Proc Export options(delimiter, putnames)
-      """
-      dsopts = dsopts if dsopts is not None else {}
-      opts = opts if opts is not None else {}
-
-      code  = "filename x \""+file+"\";\n"
-      code += "options nosource;\n"
-      code += "proc export data="
-
-      if len(libref):
-         code += libref+"."
-
-      code += "'"+table.strip().replace("'", "''")+"'n "+self._sb._dsopts(dsopts)+" outfile=x dbms=csv replace;\n"
-      code += self._sb._expopts(opts)+" run;\n"
-      code += "options source;\n"
-
-      if nosub:
-         print(code)
-      else:
-         ll = self.submit(code, "text")
-         return ll['LOG']
-
    def upload_slow(self, localfile: str, remotefile: str, overwrite: bool = True, permission: str = '', **kwargs):
       """
       This method uploads a local file to the SAS servers file system.
       localfile  - path to the local file to upload
       remotefile - path to remote file to create or overwrite
       overwrite  - overwrite the output file if it exists?
       permission - permissions to set on the new file. See SAS Filename Statement Doc for syntax
@@ -1428,25 +1373,25 @@
       try:
          fd = open(localfile, 'rb')
       except OSError as e:
          return {'Success' : False,
                  'LOG'     : "File "+str(localfile)+" could not be opened. Error was: "+str(e)}
 
       code = """
-         filename saspydir '"""+remf+"""' recfm=F encoding=binary lrecl=1 permission='"""+permission+"""';
+         filename _sp_updn '"""+remf+"""' recfm=F encoding=binary lrecl=1 permission='"""+permission+"""';
          filename sock socket ':"""+str(port)+"""' server reconn=0 recfm=S lrecl=4096;
 
          data _null_; nb = -1;
          infile sock nbyte=nb;
-         file saspydir;
+         file _sp_updn;
          input;
          put _infile_;
          run;
 
-         filename saspydir;
+         filename _sp_updn;
          filename sock;\n"""
 
       self._asubmit(code, "text")
 
       sock = socks.socket()
       sock.connect((host, port))
 
@@ -1543,26 +1488,26 @@
             sock.bind(('', port))
          port = sock.getsockname()[1]
       except OSError:
          return {'Success' : False,
                  'LOG'     : "Error try to open a socket in the upload method. Call failed."}
 
       code = """
-         filename saspydir '"""+remf+"""' recfm=F encoding=binary lrecl=1 permission='"""+permission+"""';
+         filename _sp_updn '"""+remf+"""' recfm=F encoding=binary lrecl=1 permission='"""+permission+"""';
          filename sock socket '"""+host+""":"""+str(port)+"""' recfm=S lrecl=4096;
          /* filename sock socket '"""+host+""":"""+str(port)+"""' recfm=S encoding=binary lrecl=4096; */
 
          data _null_; nb = -1;
          infile sock nbyte=nb;
-         file saspydir;
+         file _sp_updn;
          input;
          put _infile_;
          run;
 
-         filename saspydir;
+         filename _sp_updn;
          filename sock;\n"""
 
       sock.listen(1)
       self._asubmit(code, 'text')
 
       if sel.select([sock],[],[],10)[0] == []:
          logger.error("error occured in SAS during upload. Check the returned LOG for issues.")
@@ -1664,20 +1609,20 @@
             host = self.sascfg.hostip #socks.gethostname()
          else:
             host = 'localhost'
       else:
          host = ''
 
       code = """
-         filename saspydir '"""+remotefile+"""' recfm=F encoding=binary lrecl=4096;
+         filename _sp_updn '"""+remotefile+"""' recfm=F encoding=binary lrecl=4096;
          filename sock socket '"""+host+""":"""+str(port)+"""' recfm=S lrecl=4096;
          /* filename sock socket '"""+host+""":"""+str(port)+"""' recfm=S encoding=binary; */
          data _null_;
          file sock;
-         infile saspydir;
+         infile _sp_updn;
          input;
          put _infile_;
          run;\n"""
 
       sock.listen(1)
       self._asubmit(code, 'text')
 
@@ -1714,29 +1659,29 @@
                   pass
                newsock[0].shutdown(socks.SHUT_RDWR)
                newsock[0].close()
          except:
             pass
          sock.close()
          fd.close()
-         ll = self.submit("filename saspydir;", 'text')
+         ll = self.submit("filename _sp_updn;", 'text')
          return {'Success' : False,
                  'LOG'     : "Download was interrupted. Returning the SAS log:\n\n"+str(e)+"\n\n"+ll['LOG']}
 
       try: # Mac OS Python has bugs with this call
          newsock[0].shutdown(socks.SHUT_RDWR)
       except:
          pass
       newsock[0].close()
       sock.close()
 
       fd.flush()
       fd.close()
 
-      ll = self.submit("filename saspydir;", 'text')
+      ll = self.submit("filename _sp_updn;", 'text')
       return {'Success' : True,
               'LOG'     : ll['LOG']}
 
    def _getbytelenF(self, x):
       return len(x.encode(self.sascfg.encoding))
 
    def _getbytelenR(self, x):
@@ -2319,18 +2264,18 @@
                else:
                   dts[dvarlist[i]] = 'str'
             else:
                dts[dvarlist[i]] = 'str'
       else:
          dts = k_dts
 
-      code  = ''
       code  = "proc export data=work.sasdata2dataframe outfile=sock dbms=csv replace;\n"
       code += self._sb._expopts(opts)+" run;\n"
       code += "proc delete data=work.sasdata2dataframe(memtype=view);run;\n"
+      code += "filename sock;"
 
       sock.listen(1)
       self._asubmit(code, 'text')
 
       if wait > 0 and sel.select([sock],[],[],wait)[0] == []:
          logger.error("error occured in SAS during sasdata2dataframe. Trying to return the saslog instead of a data frame.")
          sock.close()
@@ -2546,15 +2491,15 @@
          if i % 10 == 9:
             code +='\n'
       code += "\nput "
       for i in range(nvars):
          code += " '"+varlist[i]+"'n "
          if i % 10 == 9:
             code +='\n'
-      code += rdelim+";\nrun;"
+      code += rdelim+";\nrun;\nfilename sock;"
 
       if k_dts is None:
          dts = {}
          for i in range(nvars):
             if vartype[i] == 'N':
                if varcat[i] not in self._sb.sas_date_fmts + self._sb.sas_time_fmts + self._sb.sas_datetime_fmts:
                   dts[dvarlist[i]] = 'float'
```

### Comparing `saspy-5.2.2/saspy/sasml.py` & `saspy-5.2.3/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasproccommons.py` & `saspy-5.2.3/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasqc.py` & `saspy-5.2.3/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasresults.py` & `saspy-5.2.3/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasstat.py` & `saspy-5.2.3/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sastabulate.py` & `saspy-5.2.3/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/sasutil.py` & `saspy-5.2.3/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy/scripts/run_sas.py` & `saspy-5.2.3/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/saspy.egg-info/PKG-INFO` & `saspy-5.2.3/saspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.2.2
+Version: 5.2.3
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.2.2/saspy.egg-info/SOURCES.txt` & `saspy-5.2.3/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.2.2/setup.py` & `saspy-5.2.3/setup.py`

 * *Files identical despite different names*

