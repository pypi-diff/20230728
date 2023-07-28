# Comparing `tmp/odxtools-4.0.5.tar.gz` & `tmp/odxtools-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odxtools-4.0.5.tar", last modified: Tue Jul 11 10:04:37 2023, max compression
+gzip compressed data, was "odxtools-4.1.0.tar", last modified: Fri Jul 28 15:24:44 2023, max compression
```

## Comparing `odxtools-4.0.5.tar` & `odxtools-4.1.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.840000 odxtools-4.0.5/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.5/LICENSE
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-11 10:04:37.836000 odxtools-4.0.5/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.5/README.md
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.795999 odxtools-4.0.5/examples/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/__init__.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.5/examples/isotp_send.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/mksomersaultpdx.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/pdxcopy.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    81924 2023-07-02 11:28:36.000000 odxtools-4.0.5/examples/somersaultecu.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/somersaultlazy.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.815999 odxtools-4.0.5/odxtools/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.5/odxtools/__main__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/admindata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/audience.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.820000 odxtools-4.0.5/odxtools/cli/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.5/odxtools/cli/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/_parser_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/cli/_print_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/browse.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/dummy_sub_parser.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/find.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7337 2023-07-04 15:58:15.000000 odxtools-4.0.5/odxtools/cli/list.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/main.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/snoop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/communicationparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/companydata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/comparam_subset.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.824000 odxtools-4.0.5/odxtools/compumethods/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compumethodbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compurationalcoeffs.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compuscale.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7662 2023-07-02 11:28:36.000000 odxtools-4.0.5/odxtools/compumethods/createanycompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/identicalcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/limit.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/linearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/scalelinearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/tabintpcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/texttablecompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/database.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/dataobjectproperty.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/decodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diagcodedtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diagdatadictionaryspec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39660 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/diaglayer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diaglayercontainer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11412 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools/diaglayerraw.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diaglayertype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6969 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/ecu_variant_matcher.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/encodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7307 2023-07-07 06:40:10.000000 odxtools-4.0.5/odxtools/endofpdufield.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/envdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/envdatadesc.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/exceptions.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/functionalclass.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/globals.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/isotp_state_machine.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_odx_d_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_pdx_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/message.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/multiplexer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/nameditemlist.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/obd.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/odxlink.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameter_info.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.832000 odxtools-4.0.5/odxtools/parameters/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/codedconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/createanyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/dynamicparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/lengthkeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/parameters/matchingrequestparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/nrcconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/parameters/parameterbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4108 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/parameters/parameterwithdop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/physicalconstantparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/reservedparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/systemparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/tableentryparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2484 2023-07-02 11:28:36.000000 odxtools-4.0.5/odxtools/parameters/tablekeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/tablestructparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/valueparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/parentref.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/physicaltype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13655 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/service.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/specialdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/state.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/statechart.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/statetransition.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/structures.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/table.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/uds.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/units.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools/version.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/write_pdx_file.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.815999 odxtools-4.0.5/odxtools.egg-info/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/SOURCES.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/dependency_links.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/entry_points.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/requires.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/top_level.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.5/pyproject.toml
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-07-11 10:04:37.840000 odxtools-4.0.5/setup.cfg
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.5/setup.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.836000 odxtools-4.0.5/tests/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14195 2023-07-02 11:28:36.000000 odxtools-4.0.5/tests/test_compu_methods.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.0.5/tests/test_decoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_diag_coded_types.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_diag_data_dictionary_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_ecu_variant_matching.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.5/tests/test_ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_encoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_odxtools.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_readparameters.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11866 2023-06-28 12:35:57.000000 odxtools-4.0.5/tests/test_somersault.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_unit_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.5/tests/test_utils.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.638891 odxtools-4.1.0/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.1.0/LICENSE
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-28 15:24:44.635557 odxtools-4.1.0/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.1.0/README.md
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.602223 odxtools-4.1.0/examples/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.1.0/examples/__init__.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.1.0/examples/isotp_send.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.1.0/examples/mksomersaultpdx.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.1.0/examples/pdxcopy.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    86965 2023-07-28 15:24:44.000000 odxtools-4.1.0/examples/somersaultecu.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    18944 2023-07-28 15:24:44.000000 odxtools-4.1.0/examples/somersaultlazy.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.615557 odxtools-4.1.0/odxtools/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.1.0/odxtools/__main__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/admindata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/audience.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.622223 odxtools-4.1.0/odxtools/cli/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.1.0/odxtools/cli/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/_parser_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/cli/_print_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/browse.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/dummy_sub_parser.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/find.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7337 2023-07-04 15:58:15.000000 odxtools-4.1.0/odxtools/cli/list.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/main.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/cli/snoop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/communicationparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.1.0/odxtools/companydata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/comparam_subset.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.625557 odxtools-4.1.0/odxtools/compumethods/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/compumethodbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/compurationalcoeffs.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1511 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/compumethods/compuscale.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7662 2023-07-02 11:28:36.000000 odxtools-4.1.0/odxtools/compumethods/createanycompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/identicalcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2527 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/compumethods/limit.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/linearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/scalelinearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/tabintpcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/compumethods/texttablecompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/database.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16105 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/dataobjectproperty.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      662 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/decodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27793 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/diagcodedtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6667 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/diagdatadictionaryspec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39508 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/diaglayer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/diaglayercontainer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11412 2023-07-11 10:04:37.000000 odxtools-4.1.0/odxtools/diaglayerraw.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/diaglayertype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6965 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/ecu_variant_matcher.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1227 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/encodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7296 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/endofpdufield.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/envdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/envdatadesc.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/exceptions.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/functionalclass.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/globals.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/isotp_state_machine.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/load_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/load_odx_d_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/load_pdx_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      915 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/message.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12894 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/multiplexer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4518 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/nameditemlist.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/obd.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8825 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/odxlink.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4447 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3515 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameter_info.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.628890 odxtools-4.1.0/odxtools/parameters/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4798 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/codedconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/createanyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/dynamicparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2121 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/lengthkeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.1.0/odxtools/parameters/matchingrequestparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5347 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/nrcconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7314 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/parameterbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4175 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/parameterwithdop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/physicalconstantparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/reservedparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/systemparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/tableentryparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6803 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/tablekeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6894 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/parameters/tablestructparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/parameters/valueparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/parentref.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/physicaltype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13637 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/service.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16356 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/specialdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/state.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/statechart.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/statetransition.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23313 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/structures.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4528 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/table.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5938 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/tablerow.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4392 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/uds.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/units.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.1.0/odxtools/utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools/version.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.1.0/odxtools/write_pdx_file.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.618890 odxtools-4.1.0/odxtools.egg-info/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3363 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/entry_points.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/requires.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-07-28 15:24:44.000000 odxtools-4.1.0/odxtools.egg-info/top_level.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.1.0/pyproject.toml
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-07-28 15:24:44.638891 odxtools-4.1.0/setup.cfg
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.1.0/setup.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-28 15:24:44.635557 odxtools-4.1.0/tests/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14195 2023-07-02 11:28:36.000000 odxtools-4.1.0/tests/test_compu_methods.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.1.0/tests/test_decoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36769 2023-07-28 15:24:44.000000 odxtools-4.1.0/tests/test_diag_coded_types.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10951 2023-07-28 15:24:44.000000 odxtools-4.1.0/tests/test_diag_data_dictionary_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14047 2023-07-28 15:24:44.000000 odxtools-4.1.0/tests/test_ecu_variant_matching.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.1.0/tests/test_ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.1.0/tests/test_encoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.1.0/tests/test_odxtools.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.1.0/tests/test_odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.1.0/tests/test_readparameters.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.1.0/tests/test_singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15420 2023-07-28 15:24:44.000000 odxtools-4.1.0/tests/test_somersault.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.1.0/tests/test_unit_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.1.0/tests/test_utils.py
```

### Comparing `odxtools-4.0.5/LICENSE` & `odxtools-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/PKG-INFO` & `odxtools-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.5
+Version: 4.1.0
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.5/README.md` & `odxtools-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/examples/isotp_send.py` & `odxtools-4.1.0/examples/isotp_send.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/examples/mksomersaultpdx.py` & `odxtools-4.1.0/examples/mksomersaultpdx.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/examples/pdxcopy.py` & `odxtools-4.1.0/examples/pdxcopy.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/examples/somersaultecu.py` & `odxtools-4.1.0/examples/somersaultecu.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from odxtools.globals import logger
 from odxtools.multiplexer import (Multiplexer, MultiplexerCase, MultiplexerDefaultCase,
                                   MultiplexerSwitchKey)
 from odxtools.nameditemlist import NamedItemList
 from odxtools.odxlink import OdxDocFragment, OdxLinkId, OdxLinkRef
 from odxtools.odxtypes import DataType
 from odxtools.parameters import (CodedConstParameter, MatchingRequestParameter, NrcConstParameter,
-                                 ValueParameter)
+                                 TableKeyParameter, TableStructParameter, ValueParameter)
 from odxtools.parentref import ParentRef
 from odxtools.physicaltype import PhysicalType
 from odxtools.service import DiagService
 from odxtools.singleecujob import ProgCode, SingleEcuJob
 from odxtools.structures import Request, Response
 from odxtools.table import Table, TableRow
 from odxtools.units import PhysicalDimension, Unit, UnitGroup, UnitSpec
@@ -288,14 +288,23 @@
             base_data_type="A_UINT32",
             bit_length=16,
             bit_mask=None,
             base_type_encoding=None,
             is_condensed_raw=None,
             is_highlow_byte_order_raw=None,
         ),
+    "float32":
+        StandardLengthType(
+            base_data_type="A_FLOAT32",
+            bit_length=32,
+            bit_mask=None,
+            is_condensed_raw=None,
+            is_highlow_byte_order_raw=None,
+            base_type_encoding=None,
+        ),
 }
 
 somersault_physical_dimensions = {
     "time":
         PhysicalDimension(
             odx_id=OdxLinkId("somersault.PD.time", doc_frags),
             short_name="time",
@@ -384,14 +393,16 @@
         ),
 }
 
 # computation methods
 somersault_compumethods = {
     "uint_passthrough":
         IdenticalCompuMethod(internal_type="A_UINT32", physical_type="A_UINT32"),
+    "float_passthrough":
+        IdenticalCompuMethod(internal_type="A_FLOAT32", physical_type="A_FLOAT32"),
     "boolean":
         TexttableCompuMethod(
             internal_type="A_UINT32",
             internal_to_phys=[
                 CompuScale(compu_const="false", lower_limit=Limit(0), upper_limit=Limit(0)),
                 CompuScale(compu_const="true", lower_limit=Limit(1), upper_limit=Limit(1)),
             ],
@@ -501,16 +512,45 @@
             physical_type=PhysicalType(
                 DataType.A_UNICODE2STRING, display_radix=None, precision=None),
             compu_method=somersault_compumethods["boolean"],
             unit_ref=None,
             is_visible_raw=None,
             sdgs=[],
         ),
+    "uint8":
+        DataObjectProperty(
+            odx_id=OdxLinkId("somersault.DOP.uint8", doc_frags),
+            short_name="uint8",
+            long_name=None,
+            description=None,
+            diag_coded_type=somersault_diagcodedtypes["uint8"],
+            physical_type=PhysicalType(DataType.A_UINT32, display_radix=None, precision=None),
+            compu_method=somersault_compumethods["uint_passthrough"],
+            unit_ref=None,
+            is_visible_raw=None,
+            sdgs=[],
+        ),
+    "float":
+        DataObjectProperty(
+            odx_id=OdxLinkId("somersault.DOP.float", doc_frags),
+            short_name="float",
+            long_name=None,
+            description=None,
+            diag_coded_type=somersault_diagcodedtypes["float32"],
+            physical_type=PhysicalType(DataType.A_FLOAT32, display_radix=None, precision=None),
+            compu_method=somersault_compumethods["float_passthrough"],
+            unit_ref=None,
+            is_visible_raw=None,
+            sdgs=[],
+        ),
 }
 
+last_flip_details_table_id = OdxLinkId("somersault.table.last_flip_details", doc_frags)
+last_flip_details_table_ref = OdxLinkRef.from_id(last_flip_details_table_id)
+
 # positive responses
 somersault_positive_responses = {
     "session":
         Response(
             odx_id=OdxLinkId("somersault.PR.session_start", doc_frags),
             short_name="session",
             long_name=None,
@@ -698,23 +738,35 @@
                         diag_coded_type=somersault_diagcodedtypes["uint8"],
                         byte_position=0,
                         coded_value=uds.positive_response_id(
                             SID.BackwardFlip.value),  # type: ignore
                         bit_position=None,
                         sdgs=[],
                     ),
-                    # TODO (?): non-byte aligned MatchingRequestParameters
-                    MatchingRequestParameter(
+                    ValueParameter(
                         short_name="num_flips_done",
                         long_name=None,
                         semantic=None,
                         description=None,
-                        request_byte_position=3,
-                        byte_position=1,
-                        byte_length=1,
+                        physical_default_value_raw=None,
+                        dop_ref=OdxLinkRef("somersault.DOP.uint8", doc_frags),
+                        dop_snref=None,
+                        byte_position=None,
+                        bit_position=None,
+                        sdgs=[],
+                    ),
+                    ValueParameter(
+                        short_name="grumpiness_level",
+                        long_name=None,
+                        semantic=None,
+                        description=None,
+                        physical_default_value_raw=None,
+                        dop_ref=OdxLinkRef("somersault.DOP.uint8", doc_frags),
+                        dop_snref=None,
+                        byte_position=None,
                         bit_position=None,
                         sdgs=[],
                     ),
                 ],
             ),
             byte_size=None,
         ),
@@ -763,14 +815,41 @@
                         physical_default_value_raw=None,
                         byte_position=2,
                         dop_ref=OdxLinkRef("somersault.DOP.happiness_level", doc_frags),
                         dop_snref=None,
                         bit_position=None,
                         sdgs=[],
                     ),
+                    TableKeyParameter(
+                        odx_id=OdxLinkId("somersault.PR.report_status.last_pos_response_key",
+                                         doc_frags),
+                        short_name="last_pos_response_key",
+                        long_name=None,
+                        semantic=None,
+                        description=None,
+                        table_ref=last_flip_details_table_ref,
+                        table_snref=None,
+                        table_row_ref=None,
+                        table_row_snref=None,
+                        byte_position=3,
+                        bit_position=None,
+                        sdgs=[],
+                    ),
+                    TableStructParameter(
+                        short_name="last_pos_response",
+                        long_name=None,
+                        semantic=None,
+                        description=None,
+                        table_key_ref=OdxLinkRef(
+                            "somersault.PR.report_status.last_pos_response_key", doc_frags),
+                        table_key_snref=None,
+                        byte_position=None,
+                        bit_position=None,
+                        sdgs=[],
+                    ),
                 ],
             ),
             byte_size=None,
         ),
     "set_operation_params":
         Response(
             odx_id=OdxLinkId("somersault.PR.set_operation_params", doc_frags),
@@ -1022,59 +1101,90 @@
                 ],
             ),
             byte_size=None,
         )
 }
 
 # tables
+flip_quality_table_id = OdxLinkId("somersault.table.flip_quality", doc_frags)
+flip_quality_table_ref = OdxLinkRef.from_id(flip_quality_table_id)
 somersault_tables = {
-    "flip_quality":
+    "last_flip_details":
         Table(
-            odx_id=OdxLinkId("somersault.table.flip_quality", doc_frags),
-            short_name="flip_quality",
-            long_name="Flip Quality",
-            description="<p>The quality the flip (average, good or best)</p>",
-            semantic="QUALITY",
-            key_dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-            table_rows=[
+            odx_id=last_flip_details_table_id,
+            short_name="last_flip_details",
+            long_name="Flip Details",
+            description="<p>The details the last successfully executed request</p>",
+            semantic="DETAILS",
+            admin_data=None,
+            key_label="key",
+            struct_label="response",
+            key_dop_ref=OdxLinkRef.from_id(somersault_dops["uint8"].odx_id),
+            table_rows_raw=[
                 TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.average", doc_frags),
-                    short_name="average",
-                    long_name="Average",
-                    key=3,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
-                    description="<p>The quality of the flip is average</p>",
-                    semantic="QUALITY-KEY",
+                    table_ref=last_flip_details_table_ref,
+                    odx_id=OdxLinkId("somersault.table.last_flip_details.none", doc_frags),
+                    short_name="none",
+                    long_name="No Flips Done Yet",
+                    key_raw="0",
+                    structure_ref=None,
+                    structure_snref=None,
+                    description="<p>We have not done any flips yet!</p>",
+                    semantic="DETAILS-KEY",
+                    dop_ref=OdxLinkRef.from_id(somersault_dops["soberness_check"].odx_id),
+                    dop_snref=None,
+                    sdgs=[],
+                ),
+                TableRow(
+                    table_ref=last_flip_details_table_ref,
+                    odx_id=OdxLinkId("somersault.table.last_flip_details.forward_grudging",
+                                     doc_frags),
+                    short_name="forward_grudging",
+                    long_name="Forward Flips Grudgingly Done",
+                    key_raw="3",
+                    structure_ref=OdxLinkRef.from_id(
+                        somersault_positive_responses["forward_flips_grudgingly_done"].odx_id),
+                    structure_snref=None,
+                    description="<p>The the last forward flip was grudgingly done</p>",
+                    semantic="DETAILS-KEY",
                     dop_ref=None,
+                    dop_snref=None,
                     sdgs=[],
                 ),
                 TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.good", doc_frags),
-                    short_name="good",
-                    long_name="Good",
+                    table_ref=last_flip_details_table_ref,
+                    odx_id=OdxLinkId("somersault.table.last_flip_details.forward_happy", doc_frags),
+                    short_name="forward_happily",
+                    long_name="Forward Flips Happily Done",
                     description=None,
                     semantic=None,
-                    key=5,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    key_raw="5",
+                    structure_ref=OdxLinkRef.from_id(
+                        somersault_positive_responses["forward_flips_happily_done"].odx_id),
+                    structure_snref=None,
                     dop_ref=None,
+                    dop_snref=None,
                     sdgs=[],
                 ),
                 TableRow(
-                    odx_id=OdxLinkId("somersault.table.flip_quality.best", doc_frags),
-                    short_name="best",
-                    long_name="Best",
+                    table_ref=last_flip_details_table_ref,
+                    odx_id=OdxLinkId("somersault.table.last_flip_details.backward", doc_frags),
+                    short_name="backward_grudging",
+                    long_name="Backward Flips",
                     description=None,
                     semantic=None,
-                    key=10,
-                    structure_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
+                    key_raw="10",
+                    structure_ref=OdxLinkRef.from_id(
+                        somersault_positive_responses["backward_flips_grudgingly_done"].odx_id),
+                    structure_snref=None,
                     dop_ref=None,
+                    dop_snref=None,
                     sdgs=[],
                 ),
             ],
-            table_row_refs=[],
             sdgs=[],
         )
 }
 
 # muxs
 somersault_muxs = {
     "flip_preference":
@@ -1192,15 +1302,15 @@
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=0,
                     coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
                     bit_position=None,
                     sdgs=[],
                 ),
                 CodedConstParameter(
-                    short_name="odx_id",
+                    short_name="id",
                     long_name=None,
                     semantic=None,
                     description=None,
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=1,
                     coded_value=0x0,
                     bit_position=None,
@@ -1226,15 +1336,15 @@
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=0,
                     coded_value=SID.DiagnosticSessionControl.value,  # type: ignore
                     bit_position=None,
                     sdgs=[],
                 ),
                 CodedConstParameter(
-                    short_name="odx_id",
+                    short_name="id",
                     long_name=None,
                     semantic=None,
                     description=None,
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=1,
                     coded_value=0x1,
                     bit_position=None,
@@ -1260,15 +1370,15 @@
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=0,
                     coded_value=SID.TesterPresent.value,  # type: ignore
                     bit_position=None,
                     sdgs=[],
                 ),
                 CodedConstParameter(
-                    short_name="odx_id",
+                    short_name="id",
                     long_name=None,
                     semantic=None,
                     description=None,
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=1,
                     coded_value=0x0,
                     bit_position=None,
@@ -1426,15 +1536,15 @@
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=0,
                     coded_value=SID.ReadDataByIdentifier.value,  # type: ignore
                     bit_position=None,
                     sdgs=[],
                 ),
                 CodedConstParameter(
-                    short_name="odx_id",
+                    short_name="id",
                     long_name=None,
                     semantic=None,
                     description=None,
                     diag_coded_type=somersault_diagcodedtypes["uint8"],
                     byte_position=1,
                     coded_value=0x0,
                     bit_position=None,
```

### Comparing `odxtools-4.0.5/examples/somersaultlazy.py` & `odxtools-4.1.0/examples/somersaultlazy.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,46 +154,32 @@
         self._diag_session_open = False
         self._data_receive_event = asyncio.Event()
         self.dizziness_level = 0
         self.max_dizziness_level = 10
 
         self.isotp_socket = create_isotp_socket(
             can_channel,
-            rxid=somersault_lazy_diag_layer.get_receive_id(),
-            txid=somersault_lazy_diag_layer.get_send_id(),
+            rxid=somersault_lazy_diag_layer.get_can_receive_id(),
+            txid=somersault_lazy_diag_layer.get_can_send_id(),
         )
 
         ##############
         # extract the tester present parameters from the ECU's
         # communication parameters.
-        #
-        # TODO: move this into the DiagLayer analogous to
-        # get_receive_id() plus deal with more parameters.
         ##############
 
-        # the timeout on inactivity [s]
-        cps = [
-            x for x in somersault_lazy_diag_layer.communication_parameters
-            if x.id_ref == "ISO_14230_3.CP_TesterPresentTime"
-        ]
-
-        if len(cps):
-            assert len(cps) == 1
-            self._idle_timeout = int(cps[0].value) / 1e6
-        else:
+        # determine the timeout on inactivity [s]
+        self._idle_timeout = somersault_lazy_diag_layer.get_tester_present_time()
+        if self._idle_timeout is None:
             self._idle_timeout = 3.0  # default specified by the standard
 
         # we send a response to tester present messages. make sure
         # that this is specified
-        cps = [
-            x for x in somersault_lazy_diag_layer.communication_parameters
-            if x.id_ref == "ISO_15765_3.CP_TesterPresentReqRsp"
-        ]
-        assert len(cps) == 1
-        assert cps[0].value == "Response expected" or cps[0].value == "1"
+        cp = somersault_lazy_diag_layer.get_communication_parameter("CP_TesterPresentReqRsp")
+        assert cp.value == "Response expected" or cp.value == "1"
 
     async def _handle_requests_task(self):
         loop = asyncio.get_running_loop()
 
         while True:
             data = await ecu_recv(self.isotp_socket)
 
@@ -284,57 +270,52 @@
         service = message.service
         # TODO: the need for .param_dict is quite ugly IMO,
         # i.e. provide a __getitem__() method for the Message class() (?)
         soberness_check = message.param_dict["forward_soberness_check"]
         num_flips = message.param_dict["num_flips"]
 
         if soberness_check != 0x12:
-            response = [x for x in service.negative_responses if x.short_name == "flips_not_done"
-                       ][0]
+            response = service.negative_responses.flips_not_done
             response_data = response.encode(
                 coded_request=message.coded_message,
                 reason=0,  # -> not sober
                 flips_successfully_done=0,
             )
             await ecu_send(self.isotp_socket, response_data)
             return
 
         # we cannot do all flips because we are too dizzy
         if self.dizziness_level + num_flips > self.max_dizziness_level:
 
-            response = [
-                x for x in service.positive_responses if x.short_name == "grudging_forward"
-            ][0]
+            response = service.positive_responses.grudging_forward
             response_data = response.encode(
                 coded_request=message.coded_message,
                 reason=1,  # -> too dizzy
                 flips_successfully_done=self.max_dizziness_level - self.dizziness_level,
             )
             await ecu_send(self.isotp_socket, response_data)
             self.dizziness_level = self.max_dizziness_level
             return
 
         # do the flips, but be aware that 1% of our attempts fail
         # because we stumble
         for i in range(0, num_flips):
             if random.randrange(0, 10000) < 100:
-                response = [
-                    x for x in service.negative_responses if x.short_name == "flips_not_done"
-                ]
+                response = service.negative_responses.flips_not_done
                 response_data = response.encode(
                     coded_request=message.coded_message,
                     reason=2,  # -> stumbled
                     flips_successfully_done=i,
                 )
                 await ecu_send(self.isotp_socket, response_data)
                 return
 
             self.dizziness_level += 1
 
-        response = [x for x in service.positive_responses if x.short_name == "grudging_forward"][0]
+        response = service.positive_responses.grudging_forward
         response_data = response.encode(coded_request=message.coded_message)
         await ecu_send(self.isotp_socket, response_data)
 
     def close_diag_session(self):
         if not self._diag_session_open:
             return
 
@@ -424,16 +405,16 @@
     tester_logger.info("running diagnostic tester")
 
     # note that ODX specifies the CAN IDs from the ECU's point of
     # view, i.e., from the tester's (our) perspective, they are
     # reversed.
     isotp_socket = create_isotp_socket(
         can_channel,
-        txid=somersault_lazy_diag_layer.get_receive_id(),
-        rxid=somersault_lazy_diag_layer.get_send_id(),
+        txid=somersault_lazy_diag_layer.get_can_receive_id(),
+        rxid=somersault_lazy_diag_layer.get_can_send_id(),
     )
 
     # try to to do a single forward flip without having an active session (ought to fail)
     tester_logger.debug(f"attempting a sessionless forward flip")
     raw_message = somersault_lazy_diag_layer.services.do_forward_flips(
         forward_soberness_check=0x12, num_flips=1)
     await tester_send(isotp_socket, raw_message)
@@ -503,17 +484,14 @@
     if args.mode == "server":
         await server_task
     elif args.mode == "tester":
         await tester_task
     else:
         assert args.mode == "unittest"
 
-        logging.basicConfig(level=logging.DEBUG)
-        logging.getLogger("odxtools").setLevel(logging.WARNING)
-
         # run both tasks in parallel. Since the server task does not
         # complete, we need to wait until the first task is completed
         # and then manually that this was the server task
         done, pending = await asyncio.wait([tester_task, server_task],
                                            return_when=asyncio.FIRST_COMPLETED)
 
         if tester_task in pending:
@@ -546,10 +524,15 @@
     default="unittest",
     required=False,
     help="Specify whether to start the ECU side ('server'), the tester side ('tester') or both ('unittest')",
 )
 
 args = parser.parse_args()  # deals with the help message handling
 
+# set the verbosity of the log output
+logging.basicConfig(level=logging.DEBUG)  # log messages from the ECU itself
+logging.getLogger("odxtools").setLevel(
+    logging.WARNING)  # log messages stemming from the odxtools library
+
 can_channel = args.channel
 
 asyncio.run(main(args))
```

### Comparing `odxtools-4.0.5/odxtools/__init__.py` & `odxtools-4.1.0/odxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/admindata.py` & `odxtools-4.1.0/odxtools/admindata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/audience.py` & `odxtools-4.1.0/odxtools/audience.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/_parser_utils.py` & `odxtools-4.1.0/odxtools/cli/_parser_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/_print_utils.py` & `odxtools-4.1.0/odxtools/cli/_print_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/browse.py` & `odxtools-4.1.0/odxtools/cli/browse.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/dummy_sub_parser.py` & `odxtools-4.1.0/odxtools/cli/dummy_sub_parser.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/find.py` & `odxtools-4.1.0/odxtools/cli/find.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/list.py` & `odxtools-4.1.0/odxtools/cli/list.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/main.py` & `odxtools-4.1.0/odxtools/cli/main.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/cli/snoop.py` & `odxtools-4.1.0/odxtools/cli/snoop.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/communicationparameter.py` & `odxtools-4.1.0/odxtools/communicationparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/companydata.py` & `odxtools-4.1.0/odxtools/companydata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/comparam_subset.py` & `odxtools-4.1.0/odxtools/comparam_subset.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/__init__.py` & `odxtools-4.1.0/odxtools/compumethods/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/compumethodbase.py` & `odxtools-4.1.0/odxtools/compumethods/compumethodbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/compuscale.py` & `odxtools-4.1.0/odxtools/compumethods/compuscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from typing import NamedTuple, Optional, Union
 
+from ..odxtypes import AtomicOdxType
 from .compurationalcoeffs import CompuRationalCoeffs
 from .limit import Limit
 
 
 class CompuScale(NamedTuple):
     """A COMPU-SCALE represents one value range of a COMPU-METHOD.
 
@@ -29,10 +30,10 @@
     Either `compu_const` or `compu_rational_coeffs` must be defined but never both.
     """
 
     short_label: Optional[str] = None
     description: Optional[str] = None
     lower_limit: Optional[Limit] = None
     upper_limit: Optional[Limit] = None
-    compu_inverse_value: Optional[Union[float, str, bytearray]] = None
+    compu_inverse_value: Optional[AtomicOdxType] = None
     compu_const: Optional[Union[float, str]] = None
     compu_rational_coeffs: Optional[CompuRationalCoeffs] = None
```

### Comparing `odxtools-4.0.5/odxtools/compumethods/createanycompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/createanycompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/identicalcompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/identicalcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/limit.py` & `odxtools-4.1.0/odxtools/compumethods/limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             else:
                 assert et_element.tag == "UPPER-LIMIT"
                 return Limit(float("inf"), interval_type)
         elif internal_type == DataType.A_BYTEFIELD:
             hex_text = et_element.text
             if len(hex_text) % 2 == 1:
                 hex_text = "0" + hex_text
-            return Limit(bytearray.fromhex(hex_text), interval_type)
+            return Limit(bytes.fromhex(hex_text), interval_type)
         else:
             return Limit(internal_type.from_string(et_element.text), interval_type)
 
     def complies_to_upper(self, value):
         """Checks if the value is in the range w.r.t. the upper limit.
 
         * If the interval type is closed, return `value <= limit.value`.
```

### Comparing `odxtools-4.0.5/odxtools/compumethods/linearcompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/linearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/scalelinearcompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/scalelinearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/tabintpcompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/tabintpcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/compumethods/texttablecompumethod.py` & `odxtools-4.1.0/odxtools/compumethods/texttablecompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/database.py` & `odxtools-4.1.0/odxtools/database.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/dataobjectproperty.py` & `odxtools-4.1.0/odxtools/dataobjectproperty.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 from .compumethods import CompuMethod, create_any_compu_method_from_et
 from .decodestate import DecodeState
 from .diagcodedtypes import DiagCodedType, StandardLengthType, create_any_diag_coded_type_from_et
 from .encodestate import EncodeState
 from .exceptions import DecodeError, EncodeError
 from .globals import logger
@@ -38,16 +38,14 @@
     def __hash__(self) -> int:
         result = 0
 
         result += hash(self.short_name)
         result += hash(self.long_name)
         result += hash(self.description)
         result += hash(self.is_visible_raw)
-        for sdg in self.sdgs:
-            result += hash(sdg)
 
         return result
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         result = {self.odx_id: self}
 
         for sdg in self.sdgs:
@@ -162,60 +160,80 @@
                 linked_dtc_dop_refs=linked_dtc_dop_refs,
                 is_visible_raw=is_visible_raw,
                 sdgs=sdgs,
             )
         return dop
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        return super()._build_odxlinks()
+        result = super()._build_odxlinks()
+        result.update(self.diag_coded_type._build_odxlinks())
+        return result
 
     def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
         """Resolves the reference to the unit"""
         super()._resolve_odxlinks(odxlinks)
 
+        self.diag_coded_type._resolve_odxlinks(odxlinks)
+
         self._unit: Optional[Unit] = None
         if self.unit_ref:
             self._unit = odxlinks.resolve(self.unit_ref, Unit)
 
     def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         super()._resolve_snrefs(diag_layer)
 
+        self.diag_coded_type._resolve_snrefs(diag_layer)
+
     @property
     def unit(self) -> Optional[Unit]:
         return self._unit
 
     @property
     def bit_length(self):
         # TODO: The DiagCodedTypes except StandardLengthType don't have a bit length.
         #       Should we remove this bit_length property from DOP or return None?
         if isinstance(self.diag_coded_type, StandardLengthType):
             return self.diag_coded_type.bit_length
         else:
             return None
 
-    def convert_physical_to_internal(self, physical_value):
+    def convert_physical_to_internal(self, physical_value: Any) -> Any:
+        """
+        Convert a physical representation of a parameter to its internal counterpart
+        """
         assert self.physical_type.base_data_type.isinstance(
             physical_value
         ), f"Expected {self.physical_type.base_data_type.value}, got {type(physical_value)}"
 
         return self.compu_method.convert_physical_to_internal(physical_value)
 
-    def convert_physical_to_bytes(self, physical_value, encode_state, bit_position):
+    def convert_physical_to_bytes(self, physical_value: Any, encode_state: EncodeState,
+                                  bit_position: int) -> bytes:
+        """
+        Convert a physical representation of a parameter to a string bytes that can be send over the wire
+        """
         if not self.is_valid_physical_value(physical_value):
             raise EncodeError(f"The value {repr(physical_value)} of type {type(physical_value)}"
                               f" is not a valid." +
                               (f" Valid values are {self.compu_method.get_valid_physical_values()}"
                                if self.compu_method.get_valid_physical_values(
                                ) else f" Expected type {self.physical_type.base_data_type.value}."))
 
         internal_val = self.convert_physical_to_internal(physical_value)
         return self.diag_coded_type.convert_internal_to_bytes(
             internal_val, encode_state, bit_position=bit_position)
 
-    def convert_bytes_to_physical(self, decode_state, bit_position: int = 0):
+    def convert_bytes_to_physical(self,
+                                  decode_state: DecodeState,
+                                  bit_position: int = 0) -> Tuple[Any, int]:
+        """
+        Convert the internal representation of a value into its physical value.
+
+        Returns a (physical_value, start_position_of_next_parameter) tuple.
+        """
         assert 0 <= bit_position and bit_position < 8
 
         internal, next_byte_position = self.diag_coded_type.convert_bytes_to_internal(
             decode_state, bit_position=bit_position)
 
         if self.compu_method.is_valid_internal_value(internal):
             return self.compu_method.convert_internal_to_physical(internal), next_byte_position
@@ -251,15 +269,15 @@
 @dataclass
 class DiagnosticTroubleCode:
     trouble_code: int
     odx_id: Optional[OdxLinkId]
     short_name: Optional[str]
     text: Optional[str]
     display_trouble_code: Optional[str]
-    level: Union[bytes, bytearray, None]
+    level: Union[bytes, None]
     is_temporary_raw: Optional[bool]
     sdgs: List[SpecialDataGroup]
 
     @property
     def is_temporary(self) -> bool:
         return self.is_temporary_raw == True
```

### Comparing `odxtools-4.0.5/odxtools/diagcodedtypes.py` & `odxtools-4.1.0/odxtools/diagcodedtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import abc
-import math
-from typing import Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 import bitstruct
 
 from .decodestate import DecodeState
 from .encodestate import EncodeState
 from .exceptions import DecodeError, EncodeError
 from .globals import logger, xsi
-from .odxlink import OdxDocFragment, OdxLinkId
+from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import DataType, odxstr_to_bool
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+    from .parameters.lengthkeyparameter import LengthKeyParameter
+
 ODX_TYPE_TO_FORMAT_LETTER = {
     DataType.A_INT32: "s",
     DataType.A_UINT32: "u",
     DataType.A_FLOAT32: "f",
     DataType.A_FLOAT64: "f",
     DataType.A_BYTEFIELD: "r",
     DataType.A_UNICODE2STRING: "r",  # UTF-16 strings must be converted explicitly
@@ -36,14 +39,25 @@
         is_highlow_byte_order_raw: Optional[bool],
     ):
         self.base_data_type = DataType(base_data_type)
         self.dct_type = dct_type
         self.base_type_encoding = base_type_encoding
         self.is_highlow_byte_order_raw = is_highlow_byte_order_raw
 
+    def _build_odxlinks(self):
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        """Recursively resolve any odxlinks references"""
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        """Recursively resolve any short-name references"""
+        pass
+
     @property
     def is_highlow_byte_order(self) -> bool:
         return self.is_highlow_byte_order_raw in [None, True]
 
     def _extract_internal(
         self,
         coded_message: bytes,
@@ -173,15 +187,15 @@
             byte_length = len(bytes(internal_value, "utf-16-le"))
             assert byte_length % 2 == 0, (f"The bit length of A_UNICODE2STRING must"
                                           f" be a multiple of 16 but is {8*byte_length}")
         return byte_length
 
     @abc.abstractmethod
     def convert_internal_to_bytes(self, internal_value: Any, encode_state: EncodeState,
-                                  bit_position: int) -> Union[bytes, bytearray]:
+                                  bit_position: int) -> bytes:
         """Encode the internal value.
 
         Parameters
         ----------
         internal_value : python type corresponding to self.base_data_type
             the value to be encoded
         bit_position : int
@@ -199,15 +213,15 @@
         Parameters
         ----------
         decode_state : DecodeState
             The decoding state
 
         Returns
         -------
-        str or int or bytes or bytearray or dict
+        str or int or bytes or dict
             the decoded parameter value
         int
             the next byte position after the extracted parameter
         """
         pass
 
 
@@ -234,15 +248,15 @@
             DataType.A_BYTEFIELD,
             DataType.A_ASCIISTRING,
             DataType.A_UNICODE2STRING,
             DataType.A_UTF8STRING,
         ], f"A leading length info type cannot have the base data type {self.base_data_type}."
 
     def convert_internal_to_bytes(self, internal_value: Any, encode_state: EncodeState,
-                                  bit_position: int) -> Union[bytes, bytearray]:
+                                  bit_position: int) -> bytes:
 
         byte_length = self._minimal_byte_length_of(internal_value)
 
         length_byte = self._to_bytes(
             byte_length,
             bit_position=bit_position,
             bit_length=self.bit_length,
@@ -464,29 +478,46 @@
 
 class ParamLengthInfoType(DiagCodedType):
 
     def __init__(
         self,
         *,
         base_data_type: Union[str, DataType],
-        length_key_id: OdxLinkId,
+        length_key_ref: OdxLinkRef,
         base_type_encoding: Optional[str],
         is_highlow_byte_order_raw: Optional[bool],
     ):
         super().__init__(
             base_data_type=base_data_type,
             dct_type="PARAM-LENGTH-INFO-TYPE",
             base_type_encoding=base_type_encoding,
             is_highlow_byte_order_raw=is_highlow_byte_order_raw,
         )
-        self.length_key_id = length_key_id
+        self.length_key_ref = length_key_ref
+
+    def _build_odxlinks(self):
+        return super()._build_odxlinks()
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        """Recursively resolve any odxlinks references"""
+        super()._resolve_odxlinks(odxlinks)
+
+        self._length_key = odxlinks.resolve(self.length_key_ref)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        """Recursively resolve any short-name references"""
+        super()._resolve_snrefs(diag_layer)
+
+    @property
+    def length_key(self) -> "LengthKeyParameter":
+        return self._length_key
 
     def convert_internal_to_bytes(self, internal_value, encode_state: EncodeState,
                                   bit_position: int) -> bytes:
-        bit_length = encode_state.length_keys.get(self.length_key_id, None)
+        bit_length = encode_state.parameter_values.get(self.length_key.short_name, None)
 
         if bit_length is None:
             if self.base_data_type in [
                     DataType.A_BYTEFIELD,
                     DataType.A_ASCIISTRING,
                     DataType.A_UTF8STRING,
             ]:
@@ -495,55 +526,52 @@
                 bit_length = 16 * len(internal_value)
 
             if self.base_data_type in [DataType.A_INT32, DataType.A_UINT32]:
                 bit_length = int(internal_value).bit_length()
                 if self.base_data_type == DataType.A_INT32:
                     bit_length += 1
                 # Round up
-                bit_length = math.ceil(bit_length / 8.0) * 8
+                bit_length = ((bit_length + 7) // 8) * 8
+
+            encode_state.parameter_values[self.length_key.short_name] = bit_length
 
         assert bit_length is not None
-        encode_state.length_keys[self.length_key_id] = bit_length
 
         return self._to_bytes(
             internal_value,
             bit_position=bit_position,
             bit_length=bit_length,
             base_data_type=self.base_data_type,
             is_highlow_byte_order=self.is_highlow_byte_order,
         )
 
     def convert_bytes_to_internal(self, decode_state: DecodeState, bit_position: int = 0):
         # Find length key with matching ID.
         bit_length = 0
-        for parameter, value in decode_state.parameter_value_pairs:
-            # if isinstance(param_value.parameter, LengthKeyParameter) would be prettier,
-            # but leads to cyclic import...
-            if (parameter.parameter_type == "LENGTH-KEY" and
-                    parameter.odx_id == self.length_key_id  # type: ignore
-               ):
+        for parameter_name, value in decode_state.parameter_values.items():
+            if parameter_name == self.length_key.short_name:
                 # The bit length of the parameter to be extracted is given by the length key.
                 assert isinstance(value, int)
                 bit_length = value
                 break
 
-        assert bit_length is not None, f"Did not find any length key with ID {self.length_key_id}"
+        assert bit_length is not None, f"Did not find any length key with short name {self.length_key.short_name}"
 
         # Extract the internal value and return.
         return self._extract_internal(
             decode_state.coded_message,
             decode_state.next_byte_position,
             bit_position,
             bit_length,
             self.base_data_type,
             self.is_highlow_byte_order,
         )
 
     def __repr__(self) -> str:
-        repr_str = f"ParamLengthInfoType(base_data_type='{self.base_data_type}', length_key_id={self.length_key_id}"
+        repr_str = f"ParamLengthInfoType(base_data_type='{self.base_data_type}', length_key={self.length_key.short_name}"
         if self.base_type_encoding is not None:
             repr_str += f", base_type_encoding={self.base_type_encoding}"
         if not self.is_highlow_byte_order:
             repr_str += f", is_highlow_byte_order={self.is_highlow_byte_order}"
         return repr_str + ")"
 
     def __str__(self) -> str:
@@ -650,27 +678,19 @@
             min_length=min_length,
             max_length=max_length,
             termination=termination,
             base_type_encoding=base_type_encoding,
             is_highlow_byte_order_raw=is_highlow_byte_order_raw,
         )
     elif dct_type == "PARAM-LENGTH-INFO-TYPE":
-        # TODO: This is a bit hacky: we make an ID where the data
-        # specifies a reference. The reason is that we need to store
-        # the result in an associative array which is not possible
-        # with references. Note that we currently ignore the DOCREF
-        # attribute of the reference, so if there are any ID conflicts
-        # between document fragments, the encoding process will go
-        # wrong...
-        length_key_elem = et_element.find("LENGTH-KEY-REF")
-        length_key_id = OdxLinkId(length_key_elem.attrib["ID-REF"], doc_frags)
+        length_key_ref = OdxLinkRef.from_et(et_element.find("LENGTH-KEY-REF"), doc_frags)
 
         return ParamLengthInfoType(
             base_data_type=base_data_type,
-            length_key_id=length_key_id,
+            length_key_ref=length_key_ref,
             base_type_encoding=base_type_encoding,
             is_highlow_byte_order_raw=is_highlow_byte_order_raw,
         )
     elif dct_type == "STANDARD-LENGTH-TYPE":
         bit_length = int(et_element.findtext("BIT-LENGTH"))
         bit_mask = None
         if et_element.find("BIT-MASK"):
```

### Comparing `odxtools-4.0.5/odxtools/diagdatadictionaryspec.py` & `odxtools-4.1.0/odxtools/diagdatadictionaryspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,22 +155,22 @@
     def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
 
         for obj in chain(self.data_object_props, self.dtc_dops, self.end_of_pdu_fields,
                          self.env_data_descs, self.env_datas, self.muxs, self.sdgs, self.structures,
                          self.tables):
             obj._resolve_odxlinks(odxlinks)
 
-        if self.unit_spec:
+        if self.unit_spec is not None:
             self.unit_spec._resolve_odxlinks(odxlinks)
 
     def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         for obj in chain(self.data_object_props, self.dtc_dops, self.end_of_pdu_fields,
                          self.env_data_descs, self.env_datas, self.muxs, self.sdgs, self.structures,
                          self.tables):
             obj._resolve_snrefs(diag_layer)
 
-        if self.unit_spec:
+        if self.unit_spec is not None:
             self.unit_spec._resolve_snrefs(diag_layer)
 
     @property
     def all_data_object_properties(self):
         return self._all_data_object_properties
```

### Comparing `odxtools-4.0.5/odxtools/diaglayer.py` & `odxtools-4.1.0/odxtools/diaglayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,17 +105,14 @@
         single_ecu_jobs = [dc for dc in diag_comms if isinstance(dc, SingleEcuJob)]
         self._services = NamedItemList(short_name_as_id, services)
         self._single_ecu_jobs = NamedItemList(short_name_as_id, single_ecu_jobs)
 
         global_negative_responses = self._compute_available_global_neg_responses(odxlinks)
         self._global_negative_responses = NamedItemList(short_name_as_id, global_negative_responses)
 
-        tables = self._compute_available_tables()
-        self._tables = NamedItemList(short_name_as_id, tables)
-
         functional_classes = self._compute_available_functional_classes()
         self._functional_classes = NamedItemList(short_name_as_id, functional_classes)
 
         additional_audiences = self._compute_available_additional_audiences()
         self._additional_audiences = NamedItemList(short_name_as_id, additional_audiences)
 
         state_charts = self._compute_available_state_charts()
@@ -153,14 +150,15 @@
                 unit_groups=NamedItemList(short_name_as_id, unit_groups),
                 units=local_unit_spec.units,
                 physical_dimensions=local_unit_spec.physical_dimensions,
                 sdgs=[])
         ############
 
         dops = NamedItemList(short_name_as_id, self._compute_available_data_object_props())
+        tables = NamedItemList(short_name_as_id, self._compute_available_tables())
         dtc_dops: NamedItemList[DtcDop]
         structures: NamedItemList[BasicStructure]
         end_of_pdu_fields: NamedItemList[EndOfPduField]
         env_data_descs: NamedItemList[EnvironmentDataDescription]
         env_datas: NamedItemList[EnvironmentData]
         muxs: NamedItemList[Multiplexer]
         ddds_sdgs: List[SpecialDataGroup]
@@ -186,15 +184,15 @@
         # hey, it's described like this in the standard.
         self._diag_data_dictionary_spec = \
             DiagDataDictionarySpec(
                 data_object_props=dops,
                 dtc_dops=dtc_dops,
                 structures=structures,
                 end_of_pdu_fields=end_of_pdu_fields,
-                tables=NamedItemList(short_name_as_id, tables),
+                tables=tables,
                 env_data_descs=env_data_descs,
                 env_datas=env_datas,
                 muxs=muxs,
                 unit_spec=unit_spec,
                 sdgs=ddds_sdgs)
 
         #####
@@ -310,17 +308,17 @@
 
     @property
     def global_negative_responses(self) -> NamedItemList[Response]:
         """All global negative responses applicable to this DiagLayer"""
         return self._global_negative_responses
 
     @property
+    @deprecated(details="use diag_data_dictionary_spec.tables")
     def tables(self) -> NamedItemList[Table]:
-        """All tables applicable to this DiagLayer"""
-        return self._tables
+        return self.diag_data_dictionary_spec.tables
 
     @property
     def functional_classes(self) -> NamedItemList[FunctionalClass]:
         """All functional classes applicable to this DiagLayer"""
         return self._functional_classes
 
     @property
@@ -888,31 +886,30 @@
         # assigning the list of possible objects to the key -1 of the
         # dictionary (this is quite hacky...)
         if sub_tree.get(-1) is None:
             sub_tree[-1] = [service]
         else:
             cast(List[DiagService], sub_tree[-1]).append(service)
 
-    def _find_services_for_uds(self, message: Union[bytes, bytearray]) -> List[DiagService]:
+    def _find_services_for_uds(self, message: bytes) -> List[DiagService]:
         prefix_tree = self._prefix_tree
 
         # Find matching service(s) in prefix tree
         possible_services: List[DiagService] = []
         for b in message:
             if b in prefix_tree:
                 assert isinstance(prefix_tree[b], dict)
                 prefix_tree = cast(PrefixTree, prefix_tree[b])
             else:
                 break
             if -1 in prefix_tree:
                 possible_services += cast(List[DiagService], prefix_tree[-1])
         return possible_services
 
-    def _decode(self, message: Union[bytes, bytearray],
-                candidate_services: Iterable[DiagService]) -> List[Message]:
+    def _decode(self, message: bytes, candidate_services: Iterable[DiagService]) -> List[Message]:
         decoded_messages: List[Message] = []
 
         for service in candidate_services:
             try:
                 decoded_messages.append(service.decode_message(message))
             except DecodeError as e:
                 # check if the message can be decoded as a global
@@ -931,21 +928,20 @@
 
         if len(decoded_messages) == 0:
             raise DecodeError(
                 f"None of the services {candidate_services} could parse {message.hex()}.")
 
         return decoded_messages
 
-    def decode(self, message: Union[bytes, bytearray]) -> List[Message]:
+    def decode(self, message: bytes) -> List[Message]:
         candidate_services = self._find_services_for_uds(message)
 
         return self._decode(message, candidate_services)
 
-    def decode_response(self, response: Union[bytes, bytearray],
-                        request: Union[bytes, bytearray, Message]) -> Iterable[Message]:
+    def decode_response(self, response: bytes, request: Union[bytes, Message]) -> Iterable[Message]:
         if isinstance(request, Message):
             candidate_services = [request.service]
         else:
             if not isinstance(request, (bytes, bytearray)):
                 raise TypeError(f"Request parameter must have type "
                                 f"Message, bytes or bytearray but was {type(request)}")
             candidate_services = self._find_services_for_uds(request)
```

### Comparing `odxtools-4.0.5/odxtools/diaglayercontainer.py` & `odxtools-4.1.0/odxtools/diaglayercontainer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/diaglayerraw.py` & `odxtools-4.1.0/odxtools/diaglayerraw.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/diaglayertype.py` & `odxtools-4.1.0/odxtools/diaglayertype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/ecu_variant_matcher.py` & `odxtools-4.1.0/odxtools/ecu_variant_matcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2023 MBition GmbH
 
 from enum import Enum
-from typing import ByteString, Dict, Generator, List, Optional, Union
+from typing import Dict, Generator, List, Optional, Union
 
-from odxtools.diaglayer import DiagLayer
-from odxtools.diaglayertype import DiagLayerType
-from odxtools.ecu_variant_patterns import MatchingParameter
-from odxtools.exceptions import OdxError
-from odxtools.service import DiagService
-from odxtools.structures import Response
+from .diaglayer import DiagLayer
+from .diaglayertype import DiagLayerType
+from .ecu_variant_patterns import MatchingParameter
+from .exceptions import OdxError
+from .odxtypes import ParameterValue
+from .service import DiagService
+from .structures import Response
 
 
 class EcuVariantMatcher:
     """EcuVariantMatcher implements the matching algorithm of ecu variants according to their
     ECU-VARIANT-PATTERN according to ISO 22901-1.
 
     Usage (example):
@@ -54,15 +55,15 @@
         service = EcuVariantMatcher.get_ident_service(diag_layer, matching_param)
         return bytes(service.encode_request())
 
     @staticmethod
     def decode_ident_response(
         diag_layer: DiagLayer,
         matching_param: MatchingParameter,
-        response_bytes: Union[bytes, bytearray],
+        response_bytes: bytes,
     ) -> str:
         """Decode a binary response and extract the identification string according
         to the snref or snpathref of the matching_param.
         """
         service = EcuVariantMatcher.get_ident_service(diag_layer, matching_param)
 
         # ISO 22901 requires that snref or snpathref is resolvable in at least one
@@ -70,19 +71,19 @@
         pos_neg_responses: List[Response] = []
         if service.positive_responses is not None:
             pos_neg_responses.extend(service.positive_responses)
         if service.negative_responses is not None:
             pos_neg_responses.extend(service.negative_responses)
 
         for any_response in pos_neg_responses:
-            decoded_val = any_response.decode(response_bytes)
+            decoded_val: Optional[ParameterValue] = any_response.decode(response_bytes)
             # disassemble snref / snpathref
             path_ref = matching_param.out_param_if.split(".")
             for ref in path_ref:
-                if ref in decoded_val:
+                if isinstance(decoded_val, dict) and ref in decoded_val:
                     decoded_val = decoded_val[ref]
                 else:
                     decoded_val = None
                     break
 
             if decoded_val is not None:
                 if isinstance(decoded_val, str) or isinstance(decoded_val, int):
@@ -94,15 +95,15 @@
     def __init__(self, ecu_variant_candidates: List[DiagLayer], use_cache: bool = True):
 
         self.ecus = ecu_variant_candidates
         for ecu in self.ecus:
             assert ecu.variant_type == DiagLayerType.ECU_VARIANT
 
         self.use_cache = use_cache
-        self.req_resp_cache: Dict[ByteString, bytes] = {}
+        self.req_resp_cache: Dict[bytes, bytes] = {}
         self._recent_ident_response: Optional[bytes] = None
 
         self._state = EcuVariantMatcher.State.PENDING
 
     def request_loop(self) -> Generator[bytes, None, None]:
         """The request loop yields byte sequences of requests, which shall be executed within the
         loop body. It is required to pass the response back to the matcher using the evaluate method.
@@ -132,15 +133,15 @@
                 self._state = EcuVariantMatcher.State.MATCH
                 self._match = ecu
                 break
         if self.is_pending():
             # no pattern has matched for any ecu variant
             self._state = EcuVariantMatcher.State.NO_MATCH
 
-    def evaluate(self, resp_bytes: Union[bytes, bytearray]) -> None:
+    def evaluate(self, resp_bytes: bytes) -> None:
         """Update the matcher with the response to a requst.
 
         Warning: Use this method EXACTLY once within the loop body of the request loop.
         """
         self._recent_ident_response = bytes(resp_bytes)
 
     def is_pending(self) -> bool:
```

### Comparing `odxtools-4.0.5/odxtools/ecu_variant_patterns.py` & `odxtools-4.1.0/odxtools/ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/encodestate.py` & `odxtools-4.1.0/odxtools/encodestate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
-from typing import Any, Dict, NamedTuple, Optional, Union
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any, Dict, NamedTuple, Optional, Union
 
 from .odxlink import OdxLinkId
+from .odxtypes import AtomicOdxType
 
+if TYPE_CHECKING:
+    from .table import TableRow
 
-class EncodeState(NamedTuple):
-    """Utility class to be used while encoding a message.
-
-    While encoding parameters may update the dicts with new keys
-    but this is the only allowed change.
-    In particular the coded_message is not updated in-place.
-    Instead the new encode state can be constructed with::
-
-        for p in self.parameters:
-            prefix = p.encode_into_pdu(encode_state)
-            encode_state = encode_state._replace(coded_message=prefix)
 
+@dataclass
+class EncodeState:
+    """Utility class to holding the state variables needed for encoding a message.
     """
 
+    #: payload that is constructed so far
     coded_message: bytes
-    """payload that is constructed so far"""
+
+    #: a mapping from short name to value for each parameter
     parameter_values: Dict[str, Any]
-    """a mapping from short name to value for each parameter"""
-    triggering_request: Optional[Union[bytes, bytearray]] = None
-    """If encoding a response: request that triggered the response"""
-    length_keys: Dict[OdxLinkId, int] = {}
-    """Mapping from IDs to bit lengths (specified by LengthKeyParameters)"""
+
+    #: If encoding a response: request that triggered the response
+    triggering_request: Optional[bytes] = None
+
+    #: Mapping from the short name of a length-key parameter to bit
+    #: lengths (specified by LengthKeyParameter)
+    length_keys: Dict[str, int] = field(default_factory=dict)
+
+    #: Mapping from the short name of a table-key parameter to the
+    #: corresponding row of the table (specified by TableKeyParameter)
+    table_keys: Dict[str, "TableRow"] = field(default_factory=dict)
+
+    #: Flag whether we are currently the last parameter of the PDU
+    #: (needed for MinMaxLengthType)
     is_end_of_pdu: bool = False
-    """Flag whether the parameter is the last on the PDU (needed for MinMaxLengthType)"""
```

### Comparing `odxtools-4.0.5/odxtools/endofpdufield.py` & `odxtools-4.1.0/odxtools/endofpdufield.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
+from copy import copy
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from .dataobjectproperty import DopBase
 from .decodestate import DecodeState
 from .encodestate import EncodeState
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
-from .odxtypes import odxstr_to_bool
+from .odxtypes import ParameterValueDict, odxstr_to_bool
 from .specialdata import create_sdgs_from_et
 from .structures import BasicStructure
 from .utils import create_description_from_et
 
 if TYPE_CHECKING:
     from .diaglayer import DiagLayer
 
@@ -104,47 +105,47 @@
         return self.structure.bit_length
 
     def convert_physical_to_internal(self, physical_value):
         return self.structure.convert_physical_to_internal(physical_value)
 
     def convert_physical_to_bytes(
         self,
-        physical_value: Union[dict, List[dict]],
+        physical_value: ParameterValueDict,
         encode_state: EncodeState,
         bit_position: int = 0,
-    ):
+    ) -> bytes:
         assert (bit_position == 0
                ), "End of PDU field must be byte aligned. Is there an error in reading the .odx?"
         if isinstance(physical_value, dict):
             # If the value is given as a dict, the End of PDU field behaves like the underlying structure.
             return self.structure.convert_physical_to_bytes(physical_value, encode_state)
         else:
             assert isinstance(physical_value,
                               list), "The value of an End-of-PDU-field must be a list or a dict."
             # If the value is given as a list, each list element is a encoded seperately using the structure.
             coded_rpc = bytes()
             for value in physical_value:
-                encode_state = encode_state._replace(coded_message=bytes())
                 coded_rpc += self.structure.convert_physical_to_bytes(value, encode_state)
             return coded_rpc
 
     def convert_bytes_to_physical(self, decode_state: DecodeState, bit_position: int = 0):
+        decode_state = copy(decode_state)
         next_byte_position = decode_state.next_byte_position
         byte_code = decode_state.coded_message
 
         value = []
         while len(byte_code) > next_byte_position:
             # ATTENTION: the ODX specification is very misleading
             # here: it says that the item is repeated until the end of
             # the PDU, but it means that DOP of the items that are
             # repeated are identical, not their values
             new_value, next_byte_position = self.structure.convert_bytes_to_physical(
                 decode_state, bit_position=bit_position)
             # Update next byte_position
-            decode_state = decode_state._replace(next_byte_position=next_byte_position)
+            decode_state.next_byte_position = next_byte_position
             value.append(new_value)
 
         return value, next_byte_position
 
     def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         """Recursively resolve any odxlinks references"""
         if self.structure_ref is not None:
```

### Comparing `odxtools-4.0.5/odxtools/envdata.py` & `odxtools-4.1.0/odxtools/envdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/envdatadesc.py` & `odxtools-4.1.0/odxtools/envdatadesc.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/exceptions.py` & `odxtools-4.1.0/odxtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/functionalclass.py` & `odxtools-4.1.0/odxtools/functionalclass.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/isotp_state_machine.py` & `odxtools-4.1.0/odxtools/isotp_state_machine.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/message.py` & `odxtools-4.1.0/odxtools/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 # Copyright (c) 2022 MBition GmbH
 from typing import Union
 
 
 class Message:
     """A CAN message with its interpretation."""
 
-    def __init__(self, *, coded_message: Union[bytes, bytearray], service, structure,
-                 param_dict: dict):
+    def __init__(self, *, coded_message: bytes, service, structure, param_dict: dict):
         """
         Parameters
         ----------
-        coded_message : bytes or bytearray
+        coded_message : bytes
         service : DiagService
         structure : Request or Response
         param_dict : dict
         """
         self.coded_message = coded_message
         self.service = service
         self.structure = structure
```

### Comparing `odxtools-4.0.5/odxtools/multiplexer.py` & `odxtools-4.1.0/odxtools/multiplexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,25 +259,25 @@
 
         if bit_position != 0:
             raise DecodeError("Multiplexer must be aligned, i.e. bit_position=0, but "
                               f"{self.short_name} was passed the bit position {bit_position}")
         byte_code = decode_state.coded_message[decode_state.next_byte_position:]
         key_decode_state = DecodeState(
             coded_message=byte_code[self.switch_key.byte_position:],
-            parameter_value_pairs=[],
+            parameter_values=dict(),
             next_byte_position=0,
         )
         bit_position_int = (
             self.switch_key.bit_position if self.switch_key.bit_position is not None else 0)
         key_value, key_next_byte = self.switch_key._dop.convert_bytes_to_physical(
             key_decode_state, bit_position=bit_position_int)
 
         case_decode_state = DecodeState(
             coded_message=byte_code[self.byte_position:],
-            parameter_value_pairs=[],
+            parameter_values=dict(),
             next_byte_position=0,
         )
         case_found = False
         case_next_byte = 0
         case_value = None
         for case in self.cases or []:
             lower, upper = self._get_case_limits(case)
```

### Comparing `odxtools-4.0.5/odxtools/nameditemlist.py` & `odxtools-4.1.0/odxtools/nameditemlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import warnings
+from keyword import iskeyword
 from typing import Callable, Dict, Generic, Iterable, List, Optional, TypeVar, Union
 
 T = TypeVar("T")
 
 
 class NamedItemList(Generic[T]):
     """A list that provides direct access to its items as named attributes.
@@ -45,24 +46,32 @@
 
         if not item_name.isidentifier():
             warnings.warn(f"For NamedItemList objects to work properly, all "
                           f"item names must be valid python identifiers."
                           f"Encountered name '{item_name}' which is not an "
                           f"identifier!")
 
+        # make sure that the name of the item in question is not a
+        # python keyword (this would lead to syntax errors)
+        if iskeyword(item_name):
+            item_name = f"{item_name}_"
+
         i = 1
         tmp = item_name
         while True:
             if tmp not in self.__dict__:
                 self.__dict__[tmp] = item
                 self._typed_dict[tmp] = item
                 return tmp
 
             i += 1
-            tmp = f"{item_name}_{i}"
+            if item_name.endswith("_"):
+                tmp = f"{item_name}{i}"
+            else:
+                tmp = f"{item_name}_{i}"
 
     def sort(self, key=None, reverse=False):
         return self._list.sort(key=key, reverse=reverse)
 
     def __contains__(self, x) -> bool:
         return x in self._list
```

### Comparing `odxtools-4.0.5/odxtools/obd.py` & `odxtools-4.1.0/odxtools/obd.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/odxlink.py` & `odxtools-4.1.0/odxtools/odxlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,22 +200,31 @@
                 )
                 continue
 
             obj = doc_frag_db.get(odx_id)
             if obj is not None:
                 if expected_type is not None:
                     assert isinstance(obj, expected_type)
-                    return obj
 
                 return obj
 
         raise KeyError(f"ODXLINK reference {ref} could not be resolved for any "
                        f"of the document fragments {ref.ref_docs}")
 
-    def resolve_lenient(self, ref: OdxLinkRef) -> Optional[Any]:
+    @overload
+    def resolve_lenient(self, ref: OdxLinkRef, expected_type: None = None) -> Any:
+        ...
+
+    @overload
+    def resolve_lenient(self, ref: OdxLinkRef, expected_type: Type[T]) -> Optional[T]:
+        ...
+
+    def resolve_lenient(self,
+                        ref: OdxLinkRef,
+                        expected_type: Optional[Type[T]] = None) -> Optional[Any]:
         """
         Resolve a reference to an object
 
         If the database does not contain any object which is referred to, None
         is returned.
         """
         assert isinstance(ref, OdxLinkRef)
@@ -232,14 +241,17 @@
                     f"when resolving reference {ref}",
                     OdxWarning,
                 )
                 continue
 
             obj = doc_frag_db.get(odx_id)
             if obj is not None:
+                if expected_type is not None:
+                    assert isinstance(obj, expected_type)
+
                 return obj
 
         return None
 
     def update(self, new_entries: Dict[OdxLinkId, Any]) -> None:
         """
         Add a bunch of new objects to the ODXLINK database.
```

### Comparing `odxtools-4.0.5/odxtools/parameter_info.py` & `odxtools-4.1.0/odxtools/parameter_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) 2022 MBition GmbH
 import re
 from typing import Iterable, Union
 
 from .compumethods import (IdenticalCompuMethod, IntervalType, Limit, LinearCompuMethod,
                            TexttableCompuMethod)
 from .dataobjectproperty import DataObjectProperty
+from .diagcodedtypes import ParamLengthInfoType
 from .endofpdufield import EndOfPduField
 from .parameters import (CodedConstParameter, MatchingRequestParameter, Parameter, ParameterWithDOP,
                          ReservedParameter)
 
 
 def parameter_info(param_list: Iterable[Union[Parameter, EndOfPduField]]) -> str:
     result = ""
```

### Comparing `odxtools-4.0.5/odxtools/parameters/__init__.py` & `odxtools-4.1.0/odxtools/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/codedconstparameter.py` & `odxtools-4.1.0/odxtools/parameters/codedconstparameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import warnings
-from typing import ByteString, Union
+from copy import copy
+from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from ..decodestate import DecodeState
 from ..diagcodedtypes import DiagCodedType
 from ..encodestate import EncodeState
 from ..exceptions import DecodeError
+from ..odxlink import OdxLinkDatabase, OdxLinkId
 from ..odxtypes import DataType
 from .parameterbase import Parameter
 
+if TYPE_CHECKING:
+    from ..diaglayer import DiagLayer
+
 
 class CodedConstParameter(Parameter):
 
-    def __init__(self, *, diag_coded_type: DiagCodedType, coded_value: Union[int, ByteString],
-                 **kwargs):
+    def __init__(self, *, diag_coded_type: DiagCodedType, coded_value: Union[int, bytes], **kwargs):
         super().__init__(parameter_type="CODED-CONST", **kwargs)
 
-        self._diag_coded_type = diag_coded_type
+        self.diag_coded_type = diag_coded_type
         assert isinstance(coded_value, (int, bytes, bytearray))
         self.coded_value = coded_value
 
-    @property
-    def diag_coded_type(self):
-        return self._diag_coded_type
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = super()._build_odxlinks()
+
+        result.update(self.diag_coded_type._build_odxlinks())
+
+        return result
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
 
     @property
     def bit_length(self):
         return self.diag_coded_type.bit_length
 
     @property
     def internal_data_type(self) -> DataType:
@@ -48,17 +61,18 @@
             raise TypeError(f"The parameter '{self.short_name}' is constant {self._coded_value_str}"
                             " and thus can not be changed.")
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         return self.diag_coded_type.convert_internal_to_bytes(
             self.coded_value, encode_state=encode_state, bit_position=bit_position_int)
 
     def decode_from_pdu(self, decode_state: DecodeState):
+        decode_state = copy(decode_state)
         if self.byte_position is not None and self.byte_position != decode_state.next_byte_position:
             # Update byte position
-            decode_state = decode_state._replace(next_byte_position=self.byte_position)
+            decode_state.next_byte_position = self.byte_position
 
         # Extract coded values
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         coded_val, next_byte_position = self.diag_coded_type.convert_bytes_to_internal(
             decode_state, bit_position=bit_position_int)
 
         # Check if the coded value in the message is correct.
```

### Comparing `odxtools-4.0.5/odxtools/parameters/createanyparameter.py` & `odxtools-4.1.0/odxtools/parameters/createanyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/dynamicparameter.py` & `odxtools-4.1.0/odxtools/parameters/dynamicparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/matchingrequestparameter.py` & `odxtools-4.1.0/odxtools/parameters/matchingrequestparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/nrcconstparameter.py` & `odxtools-4.1.0/odxtools/parameters/nrcconstparameter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import warnings
-from typing import List
+from copy import copy
+from typing import TYPE_CHECKING, Any, Dict, List
 
 from ..decodestate import DecodeState
 from ..diagcodedtypes import DiagCodedType
 from ..encodestate import EncodeState
 from ..exceptions import DecodeError, EncodeError
+from ..odxlink import OdxLinkDatabase, OdxLinkId
 from ..odxtypes import DataType
 from .parameterbase import Parameter
 
+if TYPE_CHECKING:
+    from ..diaglayer import DiagLayer
+
 
 class NrcConstParameter(Parameter):
     """A param of type NRC-CONST defines a set of values to be matched.
 
     An NRC-CONST can only be used in a negative response.
     Its encoding behaviour is similar to a VALUE parameter with a TEXTTABLE.
     However, an NRC-CONST is used for matching a response (similar to a CODED-CONST).
 
     See ASAM MCD-2 D (ODX), p. 77-79.
     """
 
     def __init__(self, *, diag_coded_type: DiagCodedType, coded_values: List[int], **kwargs):
         super().__init__(parameter_type="NRC-CONST", **kwargs)
 
-        self._diag_coded_type = diag_coded_type
+        self.diag_coded_type = diag_coded_type
         # TODO: Does it have to be an integer or is that just common practice?
         assert all(isinstance(coded_value, int) for coded_value in coded_values)
         self.coded_values = coded_values
 
-    @property
-    def diag_coded_type(self):
-        return self._diag_coded_type
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = super()._build_odxlinks()
+
+        result.update(self.diag_coded_type._build_odxlinks())
+
+        return result
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
 
     @property
     def bit_length(self):
         return self.diag_coded_type.bit_length
 
     @property
     def internal_data_type(self) -> DataType:
@@ -63,17 +77,18 @@
             coded_value = self.coded_values[0]
 
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         return self.diag_coded_type.convert_internal_to_bytes(
             coded_value, encode_state, bit_position=bit_position_int)
 
     def decode_from_pdu(self, decode_state: DecodeState):
+        decode_state = copy(decode_state)
         if self.byte_position is not None and self.byte_position != decode_state.next_byte_position:
             # Update byte position
-            decode_state = decode_state._replace(next_byte_position=self.byte_position)
+            decode_state.next_byte_position = self.byte_position
 
         # Extract coded values
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         coded_value, next_byte_position = self.diag_coded_type.convert_bytes_to_internal(
             decode_state, bit_position=bit_position_int)
 
         # Check if the coded value in the message is correct.
```

### Comparing `odxtools-4.0.5/odxtools/parameters/parameterbase.py` & `odxtools-4.1.0/odxtools/parameters/parameterbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import abc
 import warnings
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from ..decodestate import DecodeState
 from ..encodestate import EncodeState
 from ..exceptions import OdxWarning
 from ..globals import logger
 from ..odxlink import OdxLinkDatabase, OdxLinkId
 from ..specialdata import SpecialDataGroup
@@ -74,18 +74,18 @@
     def get_coded_value_as_bytes(self, encode_state: EncodeState) -> bytes:
         """Get the coded value of the parameter given the encode state.
         Note that this method is called by `encode_into_pdu`.
         """
         pass
 
     @abc.abstractmethod
-    def decode_from_pdu(self, decode_state: DecodeState):
+    def decode_from_pdu(self, decode_state: DecodeState) -> Tuple[Any, int]:
         """Decode the parameter value from the coded message.
 
-        If the paramter does have a byte position property, the coded bytes the parameter covers are extracted
+        If the parameter does have a byte position property, the coded bytes the parameter covers are extracted
         at this byte position and the function parameter `default_byte_position` is ignored.
 
         If the parameter does not have a byte position and a byte position is passed,
         the bytes are extracted at the byte position given by the argument `default_byte_position`.
 
         If the parameter does not have a byte position and the argument `default_byte_position` is None,
         this function throws a `DecodeError`.
@@ -103,64 +103,70 @@
         ParameterValuePair | List[ParameterValuePair]
             the decoded parameter value (the type is defined by the DOP)
         int
             the next byte position after the extracted parameter
         """
         pass
 
-    def encode_into_pdu(self, encode_state: EncodeState) -> bytearray:
-        """Insert the encoded value of a parameter into the coded RPC.
+    def encode_into_pdu(self, encode_state: EncodeState) -> bytes:
+        """Encode the value of a parameter into a binary blob and return it
 
         If the byte position of the parameter is not defined,
-        the byte code is appended to the coded RPC.
+        the byte code is appended to the blob.
 
-        Technical note for subclasses:
-        The default implementation tries to compute the coded value
-        via `self.get_coded_value_as_bytes(encoded_state)` and inserts it into
-        the PDU. Thus it suffices to overwrite `get_coded_value_as_bytes()`.
+        Technical note for subclasses: The default implementation
+        tries to compute the coded value via
+        `self.get_coded_value_as_bytes(encoded_state)` and inserts it
+        into the PDU. Thus it usually suffices to overwrite
+        `get_coded_value_as_bytes()` instead of `encode_into_pdu()`.
 
         Parameters:
         ----------
         encode_state: EncodeState, i.e. a named tuple with attributes
             * coded_message: bytes, the message encoded so far
             * parameter_values: List[ParameterValuePairs]
             * triggering_coded_request: bytes
 
         Returns:
         -------
-        bytearray
-            the updated, coded message after encoding the parameter into it
-        """
-        byte_value = self.get_coded_value_as_bytes(encode_state)
+        bytes
+            the message's blob after adding the encoded parameter into it
 
-        old_rpc = encode_state.coded_message
-        new_rpc = bytearray(old_rpc)
+        """
+        msg_blob = encode_state.coded_message
+        param_blob = self.get_coded_value_as_bytes(encode_state)
 
         if self.byte_position is not None:
             byte_position = self.byte_position
         else:
-            byte_position = len(old_rpc)
+            byte_position = len(msg_blob)
+
+        return self._encode_into_blob(msg_blob, param_blob, byte_position)
+
+    def _encode_into_blob(self, blob: bytes, new_data: bytes, pos: Optional[int] = None) -> bytes:
+        if pos is None:
+            pos = len(blob)
+
+        # Make blob longer if necessary
+        min_length = pos + len(new_data)
+
+        result_blob = bytearray(blob)
+        if len(blob) < min_length:
+            result_blob.extend([0] * (min_length - len(blob)))
 
-        min_length = byte_position + len(byte_value)
-        if len(old_rpc) < min_length:
-            # Make byte code longer if necessary
-            new_rpc += bytearray([0] * (min_length - len(old_rpc)))
-        for byte_idx_val, byte_idx_rpc in enumerate(
-                range(byte_position, byte_position + len(byte_value))):
+        for byte_idx_val, byte_idx_rpc in enumerate(range(pos, pos + len(new_data))):
             # insert byte value
-            if new_rpc[byte_idx_rpc] & byte_value[byte_idx_val] != 0:
+            if result_blob[byte_idx_rpc] & new_data[byte_idx_val] != 0:
                 warnings.warn(
                     f"Parameter {self.short_name} overlaps with another parameter (bytes are already set)",
                     OdxWarning,
                 )
-            new_rpc[byte_idx_rpc] |= byte_value[byte_idx_val]
+            result_blob[byte_idx_rpc] |= new_data[byte_idx_val]
 
-        logger.debug(f"Param {self.short_name} inserts"
-                     f" 0x{byte_value.hex()} at byte pos {byte_position}")
-        return new_rpc
+        return result_blob
 
     def _as_dict(self):
         """
         Mostly for pretty printing purposes (specifically not for reconstructing the object)
         """
         d = {"short_name": self.short_name, "type": self.parameter_type, "semantic": self.semantic}
         if self.byte_position is not None:
```

### Comparing `odxtools-4.0.5/odxtools/parameters/parameterwithdop.py` & `odxtools-4.1.0/odxtools/parameters/parameterwithdop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from copy import copy
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
 
 from ..dataobjectproperty import DataObjectProperty, DopBase, DtcDop
 from ..decodestate import DecodeState
 from ..encodestate import EncodeState
 from ..globals import logger
 from ..odxlink import OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from ..physicaltype import PhysicalType
@@ -79,18 +80,19 @@
     def get_coded_value_as_bytes(self, encode_state: EncodeState):
         assert self.dop is not None, "Reference to DOP is not resolved"
         physical_value = encode_state.parameter_values[self.short_name]
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         return self.dop.convert_physical_to_bytes(
             physical_value, encode_state, bit_position=bit_position_int)
 
-    def decode_from_pdu(self, decode_state: DecodeState):
+    def decode_from_pdu(self, decode_state: DecodeState) -> Tuple[Any, int]:
         assert self.dop is not None, "Reference to DOP is not resolved"
+        decode_state = copy(decode_state)
         if self.byte_position is not None and self.byte_position != decode_state.next_byte_position:
-            decode_state = decode_state._replace(next_byte_position=self.byte_position)
+            decode_state.next_byte_position = self.byte_position
 
         # Use DOP to decode
         bit_position_int = self.bit_position if self.bit_position is not None else 0
         phys_val, next_byte_position = self.dop.convert_bytes_to_physical(
             decode_state, bit_position=bit_position_int)
 
         return phys_val, next_byte_position
```

### Comparing `odxtools-4.0.5/odxtools/parameters/physicalconstantparameter.py` & `odxtools-4.1.0/odxtools/parameters/physicalconstantparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/reservedparameter.py` & `odxtools-4.1.0/odxtools/parameters/reservedparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/systemparameter.py` & `odxtools-4.1.0/odxtools/parameters/systemparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/tableentryparameter.py` & `odxtools-4.1.0/odxtools/parameters/tableentryparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parameters/valueparameter.py` & `odxtools-4.1.0/odxtools/parameters/valueparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/parentref.py` & `odxtools-4.1.0/odxtools/parentref.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/physicaltype.py` & `odxtools-4.1.0/odxtools/physicaltype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/service.py` & `odxtools-4.1.0/odxtools/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
         if self.audience:
             self.audience._resolve_snrefs(diag_layer)
 
         for sdg in self.sdgs:
             sdg._resolve_snrefs(diag_layer)
 
-    def decode_message(self, message: Union[bytes, bytearray]) -> Message:
+    def decode_message(self, message: bytes) -> Message:
 
         # Check if message is a request or positive or negative response
         interpretable_message_types = []
 
         if (self.request is None or self.positive_responses is None or
                 self.negative_responses is None):
             raise RuntimeError("References couldn't be resolved or have not been resolved yet."
```

### Comparing `odxtools-4.0.5/odxtools/singleecujob.py` & `odxtools-4.1.0/odxtools/singleecujob.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,15 @@
         if self.admin_data:
             self.admin_data._resolve_snrefs(diag_layer)
 
         # Resolve references of audience
         if self.audience:
             self.audience._resolve_snrefs(diag_layer)
 
-    def decode_message(self, message: Union[bytes, bytearray]) -> Message:
+    def decode_message(self, message: bytes) -> Message:
         """This function's signature matches `DiagService.decode_message`
         and only raises an informative error.
         """
         raise DecodeError(
             f"Single ECU jobs are completely executed on the tester and thus cannot be decoded."
             f" You tried to decode a response for the job {self.odx_id}.")
```

### Comparing `odxtools-4.0.5/odxtools/specialdata.py` & `odxtools-4.1.0/odxtools/specialdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/state.py` & `odxtools-4.1.0/odxtools/state.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/statechart.py` & `odxtools-4.1.0/odxtools/statechart.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/statetransition.py` & `odxtools-4.1.0/odxtools/statetransition.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/structures.py` & `odxtools-4.1.0/odxtools/structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import math
 import warnings
-from typing import (TYPE_CHECKING, Any, ByteString, Dict, Iterable, List, Optional, OrderedDict,
-                    Tuple, Union)
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, OrderedDict, Tuple, Union
 
 from .dataobjectproperty import DataObjectProperty, DopBase
-from .decodestate import DecodeState, ParameterValuePair
+from .decodestate import DecodeState
 from .encodestate import EncodeState
-from .exceptions import DecodeError, EncodeError, OdxWarning
+from .exceptions import DecodeError, EncodeError, OdxError, OdxWarning
 from .globals import logger
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId
-from .odxtypes import odxstr_to_bool
+from .odxtypes import ParameterDict, ParameterValueDict, odxstr_to_bool
 from .parameters import (CodedConstParameter, MatchingRequestParameter, Parameter, ParameterWithDOP,
                          ValueParameter, create_any_parameter_from_et)
 from .parameters.lengthkeyparameter import LengthKeyParameter
 from .parameters.tablekeyparameter import TableKeyParameter
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et, short_name_as_id
 
 if TYPE_CHECKING:
     from .diaglayer import DiagLayer
     from .endofpdufield import EndOfPduField
 
-ParameterDict = Dict[str, Union[Parameter, "ParameterDict"]]
-
 
 class BasicStructure(DopBase):
 
     def __init__(
         self,
         *,
         parameters: Iterable[Union[Parameter, "EndOfPduField"]],
@@ -38,15 +35,15 @@
     ):
         super().__init__(**kwargs)
         self.parameters: NamedItemList[Union[Parameter, "EndOfPduField"]] = NamedItemList(
             short_name_as_id, parameters)
         self.byte_size = byte_size
 
     @property
-    def bit_length(self):
+    def bit_length(self) -> Optional[int]:
         # Explicit size was specified
         if self.byte_size:
             return 8 * self.byte_size
 
         if all(p.bit_length is not None for p in self.parameters):
             offset = 0
             length = 0
@@ -68,27 +65,25 @@
 
             # Round up to account for padding bits
             return math.ceil(length / 8) * 8
 
         # We were not able to calculate a static bit length
         return None
 
-    def coded_const_prefix(self, request_prefix: Union[bytes, bytearray] = bytes()):
-        prefix = bytearray()
+    def coded_const_prefix(self, request_prefix: bytes = bytes()) -> bytes:
+        prefix = bytes()
         encode_state = EncodeState(prefix, parameter_values={}, triggering_request=request_prefix)
         for p in self.parameters:
             if isinstance(p, CodedConstParameter) and p.bit_length % 8 == 0:
-                prefix = p.encode_into_pdu(encode_state)
-                encode_state = EncodeState(prefix, *encode_state[1:])
+                encode_state.coded_message = p.encode_into_pdu(encode_state)
             elif isinstance(p, MatchingRequestParameter):
-                prefix = p.encode_into_pdu(encode_state)
-                encode_state = EncodeState(prefix, *encode_state[1:])
+                encode_state.coded_message = p.encode_into_pdu(encode_state)
             else:
                 break
-        return prefix
+        return encode_state.coded_message
 
     @property
     def required_parameters(self) -> List[Parameter]:
         """Return the list of parameters which are required for
         encoding the structure."""
         return [p for p in self.parameters if p.is_required()]
 
@@ -123,168 +118,150 @@
         free parameters.
         """
         from .parameter_info import parameter_info
 
         print(parameter_info(self.free_parameters), end="")
 
     def convert_physical_to_internal(self,
-                                     param_values: dict,
-                                     triggering_coded_request,
-                                     is_end_of_pdu=True):
-        logger.debug(f"{self.short_name} encode RPC"
-                     f" with params={param_values}")
+                                     param_values: ParameterValueDict,
+                                     triggering_coded_request: Optional[bytes],
+                                     is_end_of_pdu: bool = True) -> bytes:
 
-        coded_rpc = bytearray()
         encode_state = EncodeState(
-            coded_rpc,
+            bytes(),
             dict(param_values),
             triggering_request=triggering_coded_request,
             is_end_of_pdu=False,
         )
 
-        length_encodings: List[Tuple[LengthKeyParameter, EncodeState]] = []
         for param in self.parameters:
             if param == self.parameters[-1]:
-                # The last parameter is at the end of the PDU if the structure itself is at the end of the PDU
-                encode_state = encode_state._replace(is_end_of_pdu=is_end_of_pdu)
+                # The last parameter is at the end of the PDU if the
+                # structure itself is at the end of the PDU. TODO:
+                # This assumes that the last parameter specified in
+                # the ODX is located last in the PDU...
+                encode_state.is_end_of_pdu = is_end_of_pdu
 
-            implicit_length_encoding = (
-                isinstance(param, LengthKeyParameter) and param.short_name not in param_values)
-            if implicit_length_encoding:
-                # Mark this parameter since we need to re-encode it later on
-                length_encodings.append((param, encode_state))
-                # Give it a default value for now
-                encode_state.parameter_values[param.short_name] = 0
-
-            coded_rpc = param.encode_into_pdu(encode_state)
-            encode_state = encode_state._replace(coded_message=coded_rpc)
-
-            if implicit_length_encoding:
-                # Undo length_keys changes
-                encode_state.length_keys.pop(param.odx_id)
+            encode_state.coded_message = param.encode_into_pdu(encode_state)
 
-        if self.byte_size is not None and len(coded_rpc) < self.byte_size:
+        if self.byte_size is not None and len(encode_state.coded_message) < self.byte_size:
             # Padding bytes needed
-            coded_rpc = coded_rpc.ljust(self.byte_size, b"\0")
+            encode_state.coded_message = encode_state.coded_message.ljust(self.byte_size, b"\0")
 
-        for (param, encode_state) in length_encodings:
-            # Same as previous, but all bytes as 0.
-            param_value = encode_state.length_keys[param.odx_id]
-            state = encode_state._replace(
-                coded_message=bytearray(len(encode_state.coded_message)),
-                parameter_values={param.short_name: param_value},
-            )
-            # Encode the length into the zeros coded message
-            param_bytes = param.encode_into_pdu(state)
-            # Bits that changed value needs to be updated in coded_rpc
-            for i, b in enumerate(param_bytes):
-                coded_rpc[i] |= b
+        # encode the length- and table keys. This cannot be done above
+        # because we allow these to be defined implicitly (i.e. they
+        # are defined by their respective users)
+        for param in self.parameters:
+            if not isinstance(param, (LengthKeyParameter, TableKeyParameter)):
+                # the current parameter is neither a length- nor a table key
+                continue
+
+            # Encode the key parameter into the message
+            encode_state.coded_message = param.encode_into_pdu(encode_state)
 
         # Assert that length is as expected
-        self._validate_coded_rpc(coded_rpc)
+        self._validate_coded_message(encode_state.coded_message)
 
-        return bytearray(coded_rpc)
+        return bytearray(encode_state.coded_message)
 
-    def _validate_coded_rpc(self, coded_rpc: bytearray):
+    def _validate_coded_message(self, coded_message: bytes) -> None:
 
         if self.byte_size is not None:
             # We definitely broke something if we didn't respect the explicit byte_size
-            assert len(coded_rpc) == self.byte_size, self._get_encode_error_str(
-                "was", coded_rpc, self.byte_size * 8)
+            assert len(coded_message) == self.byte_size, self._get_encode_error_str(
+                "was", coded_message, self.byte_size * 8)
             # No need to check further
             return
 
         bit_length = self.bit_length
 
         if bit_length is None:
             # Nothing to check
             return
 
-        if len(coded_rpc) * 8 != bit_length:
+        if len(coded_message) * 8 != bit_length:
             # We may have broke something
             # but it could be that bit_length was mis calculated and not the actual bytes are wrong
             # Could happen with overlapping parameters and parameters with gaps
             warnings.warn(
-                self._get_encode_error_str("may have been", coded_rpc, bit_length), OdxWarning)
-
-    def _get_encode_error_str(self, verb: str, coded_rpc: bytearray, bit_length: int):
+                self._get_encode_error_str("may have been", coded_message, bit_length), OdxWarning)
 
-        return str(f"Structure {self.short_name} {verb} encoded uncorrectly:" +
-                   f" actual length is {len(coded_rpc)}," +
+    def _get_encode_error_str(self, verb: str, coded_message: bytes, bit_length: int) -> str:
+        return str(f"Structure {self.short_name} {verb} encoded incorrectly:" +
+                   f" actual length is {len(coded_message)}," +
                    f" computed byte length is {bit_length // 8}," +
-                   f" computed_rpc is {coded_rpc.hex()}\n" +
+                   f" computed_rpc is {coded_message.hex()}\n" +
                    "\n".join(self.__message_format_lines()))
 
     def convert_physical_to_bytes(self,
-                                  param_values: dict,
+                                  param_values: ParameterValueDict,
                                   encode_state: EncodeState,
-                                  bit_position: int = 0):
+                                  bit_position: int = 0) -> bytes:
         if bit_position != 0:
             raise EncodeError("Structures must be aligned, i.e. bit_position=0, but "
                               f"{self.short_name} was passed the bit position {bit_position}")
         return self.convert_physical_to_internal(
             param_values,
             triggering_coded_request=encode_state.triggering_request,
             is_end_of_pdu=encode_state.is_end_of_pdu,
         )
 
-    def convert_bytes_to_physical(self, decode_state: DecodeState, bit_position: int = 0):
+    def convert_bytes_to_physical(self,
+                                  decode_state: DecodeState,
+                                  bit_position: int = 0) -> Tuple[ParameterValueDict, int]:
         if bit_position != 0:
             raise DecodeError("Structures must be aligned, i.e. bit_position=0, but "
                               f"{self.short_name} was passed the bit position {bit_position}")
         byte_code = decode_state.coded_message[decode_state.next_byte_position:]
         inner_decode_state = DecodeState(
-            coded_message=byte_code, parameter_value_pairs=[], next_byte_position=0)
+            coded_message=byte_code, parameter_values={}, next_byte_position=0)
 
         for parameter in self.parameters:
             value, next_byte_position = parameter.decode_from_pdu(inner_decode_state)
 
-            inner_decode_state.parameter_value_pairs.append(ParameterValuePair(parameter, value))
+            inner_decode_state.parameter_values[parameter.short_name] = value
             inner_decode_state = DecodeState(
                 coded_message=byte_code,
-                parameter_value_pairs=inner_decode_state.parameter_value_pairs,
+                parameter_values=inner_decode_state.parameter_values,
                 next_byte_position=max(inner_decode_state.next_byte_position, next_byte_position),
             )
-        # Construct the param dict.
-        # TODO: Wouldn't it be prettier if we kept the information of each parameter
-        #       instead of just using the short_name as the key and "forgetting" everything else?
-        param_dict = OrderedDict(
-            (pv.parameter.short_name, pv.value) for pv in inner_decode_state.parameter_value_pairs)
 
-        return param_dict, decode_state.next_byte_position + inner_decode_state.next_byte_position
+        return inner_decode_state.parameter_values, decode_state.next_byte_position + inner_decode_state.next_byte_position
 
-    def encode(self, coded_request: Optional[ByteString] = None, **params) -> ByteString:
+    def encode(self, coded_request: Optional[bytes] = None, **params) -> bytes:
         """
         Composes an UDS message as bytes for this service.
         Parameters:
         ----------
         coded_request: bytes
             coded request (only needed when encoding a response)
         params: dict
             Parameters of the RPC as mapping from SHORT-NAME of the parameter to the value
         """
         return self.convert_physical_to_internal(
-            params, triggering_coded_request=coded_request, is_end_of_pdu=True)
+            params,  # type: ignore[arg-type]
+            triggering_coded_request=coded_request,
+            is_end_of_pdu=True)
 
-    def decode(self, message: Union[bytes, bytearray]):
+    def decode(self, message: bytes) -> ParameterValueDict:
         # dummy decode state to be passed to convert_bytes_to_physical
-        decode_state = DecodeState(
-            coded_message=message, parameter_value_pairs=[], next_byte_position=0)
+        decode_state = DecodeState(parameter_values={}, coded_message=message, next_byte_position=0)
         param_values, next_byte_position = self.convert_bytes_to_physical(decode_state)
         if len(message) != next_byte_position:
             warnings.warn(
                 f"The message {message.hex()} is longer than could be parsed."
                 f" Expected {next_byte_position} but got {len(message)}.",
                 DecodeError,
             )
         return param_values
 
     def parameter_dict(self) -> ParameterDict:
         """
-        Returns a dict with parameter short names as keys.
+        Returns a dictionary with all parameter short names as keys.
+
         The values are parameters for simple types or a nested dict for structures.
         """
         assert all(not isinstance(p, ParameterWithDOP) or isinstance(p.dop, DataObjectProperty) or
                    isinstance(p.dop, Structure) for p in self.parameters)
         param_dict: ParameterDict = {
             p.short_name: p
             for p in self.parameters
@@ -502,15 +479,15 @@
 class Response(BasicStructure):
 
     def __init__(self, *, response_type: str, **kwargs):  # "POS-RESPONSE" or "NEG-RESPONSE"
         super().__init__(**kwargs)
 
         self.response_type = response_type
 
-    def encode(self, coded_request: Optional[ByteString] = None, **params) -> ByteString:
+    def encode(self, coded_request: Optional[bytes] = None, **params) -> bytes:
         if coded_request is not None:
             logger.info(f"Compose response message to the request {coded_request.hex()}")
             # Extract MATCHING-REQUEST-PARAMs from the coded request
             for param in self.parameters:
                 if param.parameter_type == "MATCHING-REQUEST-PARAM":
                     logger.info(f"set matching request param value {param.short_name}")
                     byte_pos = param.request_byte_position
```

### Comparing `odxtools-4.0.5/odxtools/uds.py` & `odxtools-4.1.0/odxtools/uds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from enum import IntEnum
 from itertools import chain
-from typing import ByteString, Optional, Union
+from typing import Optional, Union
 
 import odxtools.obd as obd
 
 
 class UDSSID(IntEnum):
     """The service IDs standardized by UDS.
 
@@ -98,15 +98,15 @@
 
 def negative_response_id(service_id: int) -> int:
     """Given a service ID of a request, return the corresponding SID for a negative response"""
     assert service_id != 0x7F - 0x40  # TODO: What is this assert supposed to do?
     return NegativeResponseId
 
 
-def is_reponse_pending(telegram_payload: ByteString, request_sid: Optional[int] = None) -> bool:
+def is_reponse_pending(telegram_payload: bytes, request_sid: Optional[int] = None) -> bool:
     # "response pending" responses exhibit at least three bytes
     if len(telegram_payload) < 3:
         return False
 
     sid = telegram_payload[0]
     rq_sid = telegram_payload[1]
     resp_code = telegram_payload[2]
```

### Comparing `odxtools-4.0.5/odxtools/units.py` & `odxtools-4.1.0/odxtools/units.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/utils.py` & `odxtools-4.1.0/odxtools/utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools/write_pdx_file.py` & `odxtools-4.1.0/odxtools/write_pdx_file.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/odxtools.egg-info/PKG-INFO` & `odxtools-4.1.0/odxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.5
+Version: 4.1.0
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.5/odxtools.egg-info/SOURCES.txt` & `odxtools-4.1.0/odxtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 odxtools/singleecujob.py
 odxtools/specialdata.py
 odxtools/state.py
 odxtools/statechart.py
 odxtools/statetransition.py
 odxtools/structures.py
 odxtools/table.py
+odxtools/tablerow.py
 odxtools/uds.py
 odxtools/units.py
 odxtools/utils.py
 odxtools/version.py
 odxtools/write_pdx_file.py
 odxtools.egg-info/PKG-INFO
 odxtools.egg-info/SOURCES.txt
```

### Comparing `odxtools-4.0.5/setup.py` & `odxtools-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_compu_methods.py` & `odxtools-4.1.0/tests/test_compu_methods.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_decoding.py` & `odxtools-4.1.0/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_diag_coded_types.py` & `odxtools-4.1.0/tests/test_diag_coded_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (c) 2022 MBition GmbH
 import unittest
 from xml.etree import ElementTree
 
 import odxtools.uds as uds
 from odxtools.compumethods import IdenticalCompuMethod, LinearCompuMethod
 from odxtools.dataobjectproperty import DataObjectProperty
-from odxtools.decodestate import ParameterValuePair
 from odxtools.diagcodedtypes import *
 from odxtools.diagdatadictionaryspec import DiagDataDictionarySpec
 from odxtools.diaglayer import DiagLayer
 from odxtools.diaglayerraw import DiagLayerRaw
 from odxtools.diaglayertype import DiagLayerType
 from odxtools.nameditemlist import NamedItemList
 from odxtools.odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
@@ -329,56 +328,72 @@
         self.assertEqual(next_byte, 3)
 
 
 class TestParamLengthInfoType(unittest.TestCase):
 
     def test_decode_param_info_length_type_uint(self):
         length_key_id = OdxLinkId("param.length_key", doc_frags)
+        length_key_ref = OdxLinkRef.from_id(length_key_id)
+        length_key = LengthKeyParameter(
+            odx_id=length_key_id,
+            short_name="length_key",
+            long_name=None,
+            description=None,
+            semantic=None,
+            sdgs=[],
+            dop_ref=OdxLinkRef("DOP.uint8", doc_frags),
+            dop_snref=None,
+            byte_position=1,
+            bit_position=None,
+        )
         dct = ParamLengthInfoType(
             base_data_type="A_UINT32",
             base_type_encoding=None,
-            length_key_id=length_key_id,
+            length_key_ref=length_key_ref,
             is_highlow_byte_order_raw=None,
         )
+        odxlinks = OdxLinkDatabase()
+        odxlinks.update({length_key_id: length_key})
+        dct._resolve_odxlinks(odxlinks)
         state = DecodeState(
-            bytes([0x10, 0x12, 0x34, 0x56]),
-            [
-                ParameterValuePair(
-                    parameter=LengthKeyParameter(
-                        short_name="length_key",
-                        long_name=None,
-                        description=None,
-                        semantic=None,
-                        odx_id=length_key_id,
-                        dop_ref=OdxLinkRef("some_dop", doc_frags),
-                        dop_snref=None,
-                        byte_position=None,
-                        bit_position=None,
-                        sdgs=[],
-                    ),
-                    value=16,
-                )
-            ],
+            coded_message=bytes([0x10, 0x12, 0x34, 0x56]),
+            parameter_values={length_key.short_name: 16},
             next_byte_position=1,
         )
         internal, next_byte = dct.convert_bytes_to_internal(state, bit_position=0)
         self.assertEqual(internal, 0x1234)
         self.assertEqual(next_byte, 3)
 
     def test_encode_param_info_length_type_uint(self):
         length_key_id = OdxLinkId("param.length_key", doc_frags)
+        length_key = LengthKeyParameter(
+            odx_id=length_key_id,
+            short_name="length_key",
+            long_name=None,
+            description=None,
+            semantic=None,
+            sdgs=[],
+            dop_ref=OdxLinkRef("DOP.uint8", doc_frags),
+            dop_snref=None,
+            byte_position=1,
+            bit_position=None,
+        )
+        length_key_ref = OdxLinkRef.from_id(length_key_id)
         dct = ParamLengthInfoType(
             base_data_type="A_UINT32",
             base_type_encoding=None,
-            length_key_id=length_key_id,
+            length_key_ref=OdxLinkRef.from_id(length_key_id),
             is_highlow_byte_order_raw=None,
         )
-        state = EncodeState(bytes([0x10]), {}, length_keys={length_key_id: 40})
+        odxlinks = OdxLinkDatabase()
+        odxlinks.update({length_key_id: length_key})
+        dct._resolve_odxlinks(odxlinks)
+        state = EncodeState(bytes([0x10]), {length_key.short_name: 40})
         byte_val = dct.convert_internal_to_bytes(0x12345, state, bit_position=0)
-        self.assertEqual(byte_val, bytes([0x0, 0x0, 0x1, 0x23, 0x45]))
+        self.assertEqual(byte_val.hex(), "0000012345")
 
     def test_end_to_end(self):
         # diag coded types
         diagcodedtypes = {
             "uint8":
                 StandardLengthType(
                     base_data_type="A_UINT32",
@@ -388,16 +403,15 @@
                     is_condensed_raw=None,
                     is_highlow_byte_order_raw=None,
                 ),
             "length_key_id_to_lengthOfCertificateClient":
                 ParamLengthInfoType(
                     base_data_type="A_UINT32",
                     base_type_encoding=None,
-                    length_key_id=OdxLinkId(
-                        "BV.dummy_DL.RQ.sendCertificate.lengthOfCertificateClient", doc_frags),
+                    length_key_ref=OdxLinkRef("param.dummy_length_key", doc_frags),
                     is_highlow_byte_order_raw=None,
                 ),
         }
 
         # computation methods
         compumethods = {
             "uint_passthrough":
@@ -466,16 +480,15 @@
                 ),
                 LengthKeyParameter(
                     short_name="lengthOfCertificateClient",
                     long_name=None,
                     description="Length parameter for certificateClient.",
                     semantic=None,
                     # LengthKeyParams have an ID to be referenced by a ParamLengthInfoType (which is a diag coded type)
-                    odx_id=diagcodedtypes["length_key_id_to_lengthOfCertificateClient"]
-                    .length_key_id,
+                    odx_id=OdxLinkId("param.dummy_length_key", doc_frags),
                     byte_position=1,
                     bit_position=None,
                     # The DOP multiplies the coded value by 8, since the length key ref expects the number of bits.
                     dop_ref=OdxLinkRef.from_id(dops["uint8_times_8"].odx_id),
                     dop_snref=None,
                     sdgs=[],
                 ),
```

### Comparing `odxtools-4.0.5/tests/test_diag_data_dictionary_spec.py` & `odxtools-4.1.0/tests/test_diag_data_dictionary_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import unittest
 
-from odxtools import PhysicalConstantParameter, ValueParameter
+from examples import somersaultecu
+from odxtools import PhysicalConstantParameter, TableKeyParameter, ValueParameter
 from odxtools.compumethods import IdenticalCompuMethod
 from odxtools.dataobjectproperty import DataObjectProperty, DiagnosticTroubleCode, DtcDop
 from odxtools.diagcodedtypes import StandardLengthType
 from odxtools.diagdatadictionaryspec import DiagDataDictionarySpec
 from odxtools.envdata import EnvironmentData
 from odxtools.envdatadesc import EnvironmentDataDescription
 from odxtools.multiplexer import (Multiplexer, MultiplexerCase, MultiplexerDefaultCase,
                                   MultiplexerSwitchKey)
 from odxtools.nameditemlist import NamedItemList
-from odxtools.odxlink import OdxDocFragment, OdxLinkId, OdxLinkRef
+from odxtools.odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from odxtools.physicaltype import PhysicalType
 from odxtools.table import Table, TableRow
 from odxtools.utils import short_name_as_id
 
 # the document fragment which is used throughout the test
 doc_frags = [OdxDocFragment("UnitTest", "unit_test_doc")]
 
@@ -83,58 +84,71 @@
             diag_coded_type=uint_type,
             physical_type=PhysicalType("A_UINT32", display_radix=None, precision=None),
             compu_method=ident_compu_method,
             unit_ref=None,
             sdgs=[],
         )
 
+        flip_quality_id = OdxLinkId("somersault.table.flip_quality", doc_frags)
+        flip_quality_ref = OdxLinkRef.from_id(flip_quality_id)
         table = Table(
-            odx_id=OdxLinkId("somersault.table.flip_quality", doc_frags),
+            odx_id=flip_quality_id,
             short_name="flip_quality",
             long_name="Flip Quality",
             description=None,
-            key_dop_ref="",
+            key_label=None,
+            struct_label=None,
+            admin_data=None,
+            key_dop_ref=None,
             semantic=None,
-            table_rows=[
+            table_rows_raw=[
                 TableRow(
                     odx_id=OdxLinkId("somersault.table.flip_quality.average", doc_frags),
+                    table_ref=flip_quality_ref,
                     short_name="average",
                     long_name="Average",
                     description=None,
                     semantic=None,
                     dop_ref=None,
-                    key=3,
+                    dop_snref=None,
+                    key_raw="3",
                     structure_ref=None,
+                    structure_snref=None,
                     sdgs=[],
                 ),
                 TableRow(
                     odx_id=OdxLinkId("somersault.table.flip_quality.good", doc_frags),
+                    table_ref=flip_quality_ref,
                     short_name="good",
                     long_name="Good",
                     description=None,
                     semantic=None,
                     dop_ref=None,
-                    key=5,
+                    dop_snref=None,
+                    key_raw="5",
                     structure_ref=None,
+                    structure_snref=None,
                     sdgs=[],
                 ),
                 TableRow(
                     odx_id=OdxLinkId("somersault.table.flip_quality.best", doc_frags),
+                    table_ref=flip_quality_ref,
                     short_name="best",
                     long_name="Best",
                     description=None,
                     semantic=None,
                     dop_ref=None,
-                    key=10,
+                    dop_snref=None,
+                    key_raw="10",
                     structure_ref=None,
+                    structure_snref=None,
                     sdgs=[],
                 ),
             ],
-            table_row_refs=[],
-            sdgs=None,
+            sdgs=[],
         )
 
         env_data = EnvironmentData(
             odx_id=OdxLinkId("somersault.env_data.flip_env_data", doc_frags),
             short_name="flip_env_data",
             long_name="Flip Env Data",
             description=None,
@@ -143,32 +157,46 @@
             parameters=[
                 ValueParameter(
                     short_name="flip_speed",
                     long_name="Flip Speed",
                     description=None,
                     semantic="DATA",
                     byte_position=0,
-                    dop_ref="dop-ref",
+                    dop_ref=OdxLinkRef("somersault.DOP.float", doc_frags),
                     dop_snref=None,
                     physical_default_value_raw=None,
                     bit_position=None,
                     sdgs=[],
                 ),
                 PhysicalConstantParameter(
                     short_name="flip_direction",
                     long_name="Flip Direction",
                     description=None,
                     semantic="DATA",
                     byte_position=1,
                     physical_constant_value=1,
-                    dop_ref="dop-ref",
+                    dop_ref=OdxLinkRef("somersault.DOP.boolean", doc_frags),
                     dop_snref=None,
                     bit_position=None,
                     sdgs=[],
                 ),
+                TableKeyParameter(
+                    short_name="flip_quality",
+                    long_name=None,
+                    description=None,
+                    sdgs=[],
+                    semantic="DATA",
+                    byte_position=2,
+                    bit_position=None,
+                    odx_id=OdxLinkId("somersault.env_data.flip_quality", doc_frags),
+                    table_ref=None,
+                    table_row_ref=None,
+                    table_snref="flip_quality",  # cf. somersaultecu
+                    table_row_snref="good",
+                ),
             ],
             byte_size=None,
             dtc_values=[],
         )
 
         env_data_desc = EnvironmentDataDescription(
             odx_id=OdxLinkId("somersault.env_data_desc.flip_env_data_desc", doc_frags),
@@ -190,15 +218,15 @@
             description=None,
             sdgs=[],
             is_visible_raw=None,
             byte_position=0,
             switch_key=MultiplexerSwitchKey(
                 byte_position=0,
                 bit_position=0,
-                dop_ref="dop-ref",
+                dop_ref=OdxLinkRef("somersault.DOP.boolean", doc_frags),
             ),
             default_case=MultiplexerDefaultCase(
                 short_name="default_case",
                 long_name="Default Case",
                 structure_ref="structure_ref",
             ),
             cases=[
@@ -228,23 +256,33 @@
             muxs=NamedItemList(short_name_as_id, [mux]),
             structures=NamedItemList(short_name_as_id),
             end_of_pdu_fields=NamedItemList(short_name_as_id),
             unit_spec=None,
             sdgs=[],
         )
 
+        # test the short name resolution of TableKeyParameter.
+        odxlinks = OdxLinkDatabase()
+        ecu = somersaultecu.database.ecus.somersault_lazy
+        ecu.diag_layer_raw.diag_data_dictionary_spec = ddds
+        odxlinks.update(ecu._build_odxlinks())
+        table._resolve_odxlinks(odxlinks)
+
         self.assertEqual(ddds.dtc_dops[0], dtc_dop)
         self.assertEqual(ddds.data_object_props[0], dop_1)
         self.assertEqual(ddds.data_object_props.another_dop, dop_2)
         self.assertEqual(ddds.tables[0], table)
         self.assertEqual(ddds.env_data_descs[0], env_data_desc)
         self.assertEqual(ddds.env_datas[0], env_data)
         self.assertEqual(ddds.muxs[0], mux)
 
         self.assertEqual(len(ddds.structures), 0)
         self.assertEqual(len(ddds.end_of_pdu_fields), 0)
 
-        self.assertEqual(set(ddds.all_data_object_properties), set([dtc_dop, dop_1, dop_2, table]))
+        self.assertEqual({x.short_name
+                          for x in ddds.all_data_object_properties},
+                         {x.short_name
+                          for x in (dtc_dop, dop_1, dop_2, table)})
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `odxtools-4.0.5/tests/test_ecu_variant_matching.py` & `odxtools-4.1.0/tests/test_ecu_variant_matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         is_visible_raw=None,
         parameters=[],
         response_type="POS-RESPONSE",
         byte_size=None,
     )
     odxlinks.update({resp.odx_id: resp})
 
-    def decode(message: Union[bytes, bytearray]):
+    def decode(message: bytes):
         msg_str = message.decode(encoding="utf-8")
         msg_dict = json.loads(msg_str)
         return msg_dict
 
     monkeypatch.setattr(resp, "decode", decode)
     return resp
```

### Comparing `odxtools-4.0.5/tests/test_ecu_variant_patterns.py` & `odxtools-4.1.0/tests/test_ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_encoding.py` & `odxtools-4.1.0/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_odxtools.py` & `odxtools-4.1.0/tests/test_odxtools.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_odxtypes.py` & `odxtools-4.1.0/tests/test_odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_readparameters.py` & `odxtools-4.1.0/tests/test_readparameters.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_singleecujob.py` & `odxtools-4.1.0/tests/test_singleecujob.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_unit_spec.py` & `odxtools-4.1.0/tests/test_unit_spec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.5/tests/test_utils.py` & `odxtools-4.1.0/tests/test_utils.py`

 * *Files identical despite different names*

