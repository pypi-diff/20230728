# Comparing `tmp/excitingtools-1.4.0.tar.gz` & `tmp/excitingtools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excitingtools-1.4.0.tar", last modified: Fri Jul 28 14:10:52 2023, max compression
+gzip compressed data, was "excitingtools-1.5.0.tar", last modified: Fri Jul 28 14:05:01 2023, max compression
```

## Comparing `excitingtools-1.4.0.tar` & `excitingtools-1.5.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.676072 excitingtools-1.4.0/
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.656816 excitingtools-1.4.0/.github/
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.660946 excitingtools-1.4.0/.github/workflows/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      602 2023-07-28 14:10:03.000000 excitingtools-1.4.0/.github/workflows/actions.yml
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      647 2023-07-28 14:10:03.000000 excitingtools-1.4.0/.github/workflows/joss.yml
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    21948 2023-07-28 14:10:03.000000 excitingtools-1.4.0/.pylintrc
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     8901 2023-07-28 14:10:03.000000 excitingtools-1.4.0/.style.yapf
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1916 2023-07-28 14:10:03.000000 excitingtools-1.4.0/CITATION.cff
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5375 2023-07-28 14:10:03.000000 excitingtools-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     7650 2023-07-28 14:10:03.000000 excitingtools-1.4.0/COPYING.LESSER
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    34915 2023-07-28 14:10:03.000000 excitingtools-1.4.0/COPYING.md
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    55195 2023-07-28 14:10:52.675889 excitingtools-1.4.0/PKG-INFO
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    14393 2023-07-28 14:10:03.000000 excitingtools-1.4.0/README.md
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.661107 excitingtools-1.4.0/excitingtools/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      651 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/__init__.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.661872 excitingtools-1.4.0/excitingtools/constants/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1567 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/constants/units.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.662606 excitingtools-1.4.0/excitingtools/dataclasses/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      123 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/dataclasses/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5366 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/dataclasses/band_structure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      807 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/dataclasses/data_structs.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      145 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/dataclasses/density_of_states.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     6662 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/dataclasses/eigenvalues.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.662745 excitingtools-1.4.0/excitingtools/eigenstates/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1111 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/eigenstates/eigenstates.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.664466 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4714 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4020 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/bse_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    13634 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/groundstate_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     6829 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3880 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    16723 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_info_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3292 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5917 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/input_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     9945 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/parser_factory.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    24457 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/properties_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4160 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_dict_parsers/species_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.665168 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      219 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1448 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4331 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      638 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/input_xml.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1230 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/exciting_obj_parsers/ks_band_structure.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.666078 excitingtools-1.4.0/excitingtools/input/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      234 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2597 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/bandstructure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     9050 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/base_class.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4581 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/dynamic_class.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5267 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/input_classes.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    11383 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/structure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5229 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/input/xml_utils.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.666293 excitingtools-1.4.0/excitingtools/math/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/math/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      576 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/math/math_utils.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.667214 excitingtools-1.4.0/excitingtools/parser_utils/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       78 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       46 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/erroneous_file_error.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      960 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/grep_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2505 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/parser_decorators.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2666 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/parser_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2227 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/regex_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1668 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/parser_utils/simple_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.667424 excitingtools-1.4.0/excitingtools/runner/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/runner/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     6165 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/runner/runner.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.667806 excitingtools-1.4.0/excitingtools/structure/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      878 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/structure/ase_utilities.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4137 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/structure/lattice.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1532 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/structure/pymatgen_utilities.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.668669 excitingtools-1.4.0/excitingtools/utils/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5853 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/dict_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      500 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/jobflow_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     9505 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/schema_parsing.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      622 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/test_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2298 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    17412 2023-07-28 14:10:03.000000 excitingtools-1.4.0/excitingtools/utils/valid_attributes.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.661749 excitingtools-1.4.0/excitingtools.egg-info/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    55195 2023-07-28 14:10:52.000000 excitingtools-1.4.0/excitingtools.egg-info/PKG-INFO
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4524 2023-07-28 14:10:52.000000 excitingtools-1.4.0/excitingtools.egg-info/SOURCES.txt
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        1 2023-07-28 14:10:52.000000 excitingtools-1.4.0/excitingtools.egg-info/dependency_links.txt
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       58 2023-07-28 14:10:52.000000 excitingtools-1.4.0/excitingtools.egg-info/requires.txt
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       14 2023-07-28 14:10:52.000000 excitingtools-1.4.0/excitingtools.egg-info/top_level.txt
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      243 2023-07-28 14:10:03.000000 excitingtools-1.4.0/git-blame-ignore-revs
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.669230 excitingtools-1.4.0/paper/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    10387 2023-07-28 14:10:03.000000 excitingtools-1.4.0/paper/joss_latex.template
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    14039 2023-07-28 14:10:03.000000 excitingtools-1.4.0/paper/latex.template
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5301 2023-07-28 14:10:03.000000 excitingtools-1.4.0/paper/paper.bib
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     8645 2023-07-28 14:10:03.000000 excitingtools-1.4.0/paper/paper.md
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      808 2023-07-28 14:10:03.000000 excitingtools-1.4.0/pyproject.toml
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       81 2023-07-28 14:10:03.000000 excitingtools-1.4.0/pytest.ini
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       33 2023-07-28 14:10:03.000000 excitingtools-1.4.0/requirements.txt
--rw-r--r--   0 fabianpeschel   (501) staff       (20)       38 2023-07-28 14:10:52.676115 excitingtools-1.4.0/setup.cfg
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.669442 excitingtools-1.4.0/tests/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      416 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/conftest.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.669797 excitingtools-1.4.0/tests/dataclasses/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dataclasses/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3774 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dataclasses/test_band_structure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5438 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dataclasses/test_eigenvalues.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.670692 excitingtools-1.4.0/tests/dict_parsers/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    13221 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_bse_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    42033 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_groundstate_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.671633 excitingtools-1.4.0/tests/dict_parsers/test_gw/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    17883 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/mock_gw_info_out.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1874 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    16110 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4445 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    14356 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_info_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4471 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     6473 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_input_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     8348 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_ks_band_structure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1618 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_properties_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    11166 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/dict_parsers/test_species_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.671847 excitingtools-1.4.0/tests/eigenstates/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/eigenstates/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      954 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/eigenstates/test_eigenstates.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.672997 excitingtools-1.4.0/tests/input/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1431 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_base_class.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1658 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_dynamic_class.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     8196 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_ground_state.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     8886 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_input_xml.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     5352 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_properties.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)    19217 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_structure.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3216 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_xml_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     7670 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/input/test_xs.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.673220 excitingtools-1.4.0/tests/math/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/math/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      340 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/math/test_math_utils.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.673803 excitingtools-1.4.0/tests/obj_parsers/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/obj_parsers/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3508 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/obj_parsers/test_eigenvalue_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1861 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/obj_parsers/test_gw_dos.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     9190 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/obj_parsers/test_gw_eigenvalues.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1611 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/obj_parsers/test_input_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.674275 excitingtools-1.4.0/tests/parser_utils/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/parser_utils/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1529 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/parser_utils/test_parser_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     3176 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/parser_utils/test_regex_parser.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2122 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/parser_utils/test_simple_parser.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.674404 excitingtools-1.4.0/tests/runner/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     4605 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/runner/test_runner.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.674987 excitingtools-1.4.0/tests/structure/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/structure/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)      430 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/structure/test_ase_utilities.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2280 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/structure/test_lattice.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     2254 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/structure/test_pymatgen_utilities.py
-drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:52.675511 excitingtools-1.4.0/tests/utils/
--rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/utils/__init__.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     6021 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/utils/test_dict_utils.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1255 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/utils/test_schema_parsing.py
--rw-r--r--   0 fabianpeschel   (501) staff       (20)     1428 2023-07-28 14:10:03.000000 excitingtools-1.4.0/tests/utils/test_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.610550 excitingtools-1.5.0/
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.591223 excitingtools-1.5.0/.github/
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.595478 excitingtools-1.5.0/.github/workflows/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      602 2023-07-28 14:03:41.000000 excitingtools-1.5.0/.github/workflows/actions.yml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      647 2023-07-28 14:03:41.000000 excitingtools-1.5.0/.github/workflows/joss.yml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    21948 2023-07-28 14:03:41.000000 excitingtools-1.5.0/.pylintrc
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8901 2023-07-28 14:03:41.000000 excitingtools-1.5.0/.style.yapf
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1916 2023-07-28 14:03:41.000000 excitingtools-1.5.0/CITATION.cff
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5375 2023-07-28 14:03:41.000000 excitingtools-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7650 2023-07-28 14:03:41.000000 excitingtools-1.5.0/COPYING.LESSER
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    34915 2023-07-28 14:03:41.000000 excitingtools-1.5.0/COPYING.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    55193 2023-07-28 14:05:01.610368 excitingtools-1.5.0/PKG-INFO
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14391 2023-07-28 14:03:53.000000 excitingtools-1.5.0/README.md
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.595628 excitingtools-1.5.0/excitingtools/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      702 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/__init__.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.596315 excitingtools-1.5.0/excitingtools/constants/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1727 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/constants/units.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.596983 excitingtools-1.5.0/excitingtools/dataclasses/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      123 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/dataclasses/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5366 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/dataclasses/band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      807 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/dataclasses/data_structs.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      145 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/dataclasses/density_of_states.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6662 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/dataclasses/eigenvalues.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.597123 excitingtools-1.5.0/excitingtools/eigenstates/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1111 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/eigenstates/eigenstates.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.598685 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5941 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4020 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/bse_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    15919 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/groundstate_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6829 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3880 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    16723 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_info_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3292 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5917 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/input_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    10450 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/parser_factory.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    24457 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/properties_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4160 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_dict_parsers/species_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.599345 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      219 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1448 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4331 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      638 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/input_xml.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1230 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/exciting_obj_parsers/ks_band_structure.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.600251 excitingtools-1.5.0/excitingtools/input/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      234 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/input/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2597 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/input/bandstructure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     9050 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/input/base_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4581 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/input/dynamic_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4986 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/input/input_classes.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    11383 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/input/structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4617 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/input/xml_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.600435 excitingtools-1.5.0/excitingtools/math/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/math/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      576 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/math/math_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.601342 excitingtools-1.5.0/excitingtools/parser_utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       78 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       46 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/erroneous_file_error.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      960 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/grep_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2505 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/parser_decorators.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2666 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/parser_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2227 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/regex_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1668 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/parser_utils/simple_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.601551 excitingtools-1.5.0/excitingtools/runner/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/runner/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5740 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/runner/runner.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.601924 excitingtools-1.5.0/excitingtools/structure/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      878 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/structure/ase_utilities.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4137 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/structure/lattice.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1532 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/structure/pymatgen_utilities.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.602745 excitingtools-1.5.0/excitingtools/utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5853 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/utils/dict_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      500 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/utils/jobflow_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     9780 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/utils/schema_parsing.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      622 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/utils/test_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2298 2023-07-28 14:03:41.000000 excitingtools-1.5.0/excitingtools/utils/utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    17497 2023-07-28 14:03:53.000000 excitingtools-1.5.0/excitingtools/utils/valid_attributes.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.596207 excitingtools-1.5.0/excitingtools.egg-info/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    55193 2023-07-28 14:05:01.000000 excitingtools-1.5.0/excitingtools.egg-info/PKG-INFO
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4524 2023-07-28 14:05:01.000000 excitingtools-1.5.0/excitingtools.egg-info/SOURCES.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        1 2023-07-28 14:05:01.000000 excitingtools-1.5.0/excitingtools.egg-info/dependency_links.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       58 2023-07-28 14:05:01.000000 excitingtools-1.5.0/excitingtools.egg-info/requires.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       14 2023-07-28 14:05:01.000000 excitingtools-1.5.0/excitingtools.egg-info/top_level.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      243 2023-07-28 14:03:41.000000 excitingtools-1.5.0/git-blame-ignore-revs
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.603266 excitingtools-1.5.0/paper/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    10387 2023-07-28 14:03:41.000000 excitingtools-1.5.0/paper/joss_latex.template
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14039 2023-07-28 14:03:41.000000 excitingtools-1.5.0/paper/latex.template
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5301 2023-07-28 14:03:41.000000 excitingtools-1.5.0/paper/paper.bib
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8645 2023-07-28 14:03:41.000000 excitingtools-1.5.0/paper/paper.md
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      808 2023-07-28 14:03:53.000000 excitingtools-1.5.0/pyproject.toml
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       81 2023-07-28 14:03:41.000000 excitingtools-1.5.0/pytest.ini
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       33 2023-07-28 14:03:41.000000 excitingtools-1.5.0/requirements.txt
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)       38 2023-07-28 14:05:01.610590 excitingtools-1.5.0/setup.cfg
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.603476 excitingtools-1.5.0/tests/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      416 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/conftest.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.603850 excitingtools-1.5.0/tests/dataclasses/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dataclasses/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3774 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dataclasses/test_band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5438 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dataclasses/test_eigenvalues.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.604759 excitingtools-1.5.0/tests/dict_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    13221 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_bse_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    63026 2023-07-28 14:03:53.000000 excitingtools-1.5.0/tests/dict_parsers/test_groundstate_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.605804 excitingtools-1.5.0/tests/dict_parsers/test_gw/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    17883 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/mock_gw_info_out.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1874 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    16110 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4445 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    14356 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_info_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4471 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6473 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_input_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8348 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_ks_band_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1618 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_properties_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    11166 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/dict_parsers/test_species_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.606068 excitingtools-1.5.0/tests/eigenstates/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/eigenstates/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      954 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/eigenstates/test_eigenstates.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.607475 excitingtools-1.5.0/tests/input/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1431 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_base_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1658 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_dynamic_class.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8196 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_ground_state.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     8876 2023-07-28 14:03:53.000000 excitingtools-1.5.0/tests/input/test_input_xml.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     5352 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_properties.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)    19217 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_structure.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1926 2023-07-28 14:03:53.000000 excitingtools-1.5.0/tests/input/test_xml_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     7670 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/input/test_xs.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.607711 excitingtools-1.5.0/tests/math/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/math/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      340 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/math/test_math_utils.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.608377 excitingtools-1.5.0/tests/obj_parsers/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/obj_parsers/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3508 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/obj_parsers/test_eigenvalue_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1861 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/obj_parsers/test_gw_dos.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     9190 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/obj_parsers/test_gw_eigenvalues.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1606 2023-07-28 14:03:53.000000 excitingtools-1.5.0/tests/obj_parsers/test_input_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.608881 excitingtools-1.5.0/tests/parser_utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/parser_utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1529 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/parser_utils/test_parser_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     3176 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/parser_utils/test_regex_parser.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2122 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/parser_utils/test_simple_parser.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.609024 excitingtools-1.5.0/tests/runner/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     4439 2023-07-28 14:03:53.000000 excitingtools-1.5.0/tests/runner/test_runner.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.609526 excitingtools-1.5.0/tests/structure/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/structure/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)      430 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/structure/test_ase_utilities.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2280 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/structure/test_lattice.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     2254 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/structure/test_pymatgen_utilities.py
+drwxr-xr-x   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:05:01.610064 excitingtools-1.5.0/tests/utils/
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)        0 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/utils/__init__.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     6021 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/utils/test_dict_utils.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1255 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/utils/test_schema_parsing.py
+-rw-r--r--   0 fabianpeschel   (501) staff       (20)     1428 2023-07-28 14:03:41.000000 excitingtools-1.5.0/tests/utils/test_utils.py
```

### Comparing `excitingtools-1.4.0/.github/workflows/actions.yml` & `excitingtools-1.5.0/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/.github/workflows/joss.yml` & `excitingtools-1.5.0/.github/workflows/joss.yml`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/.pylintrc` & `excitingtools-1.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/.style.yapf` & `excitingtools-1.5.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/CITATION.cff` & `excitingtools-1.5.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/CONTRIBUTING.md` & `excitingtools-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/COPYING.LESSER` & `excitingtools-1.5.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/COPYING.md` & `excitingtools-1.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/PKG-INFO` & `excitingtools-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excitingtools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs.
 Author-email: Alexander Buccheri <alexander.buccheri@mpsd.mpg.de>, Fabian Peschel <peschelf@physik.hu-berlin.de>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -882,15 +882,15 @@
 
 #### Binary Execution
 
 Next we can define a runner and run our calculation:
 ```python3
 from excitingtools.runner.runner import BinaryRunner
 
-runner = BinaryRunner('exciting_smp', run_cmd=[''], omp_num_threads=4, time_out=500)
+runner = BinaryRunner('exciting_smp', run_cmd='', omp_num_threads=4, time_out=500)
 run_status = runner.run()
 ```
 
 #### Parsing Outputs
 
 After the successful completion of the calculation, we can parse the relevant output files as dictionaries, using
 `parser_chooser`. These are the main files one would be interested in after performing a ground state calculation, for
```

### Comparing `excitingtools-1.4.0/README.md` & `excitingtools-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 #### Binary Execution
 
 Next we can define a runner and run our calculation:
 ```python3
 from excitingtools.runner.runner import BinaryRunner
 
-runner = BinaryRunner('exciting_smp', run_cmd=[''], omp_num_threads=4, time_out=500)
+runner = BinaryRunner('exciting_smp', run_cmd='', omp_num_threads=4, time_out=500)
 run_status = runner.run()
 ```
 
 #### Parsing Outputs
 
 After the successful completion of the calculation, we can parse the relevant output files as dictionaries, using
 `parser_chooser`. These are the main files one would be interested in after performing a ground state calculation, for
```

### Comparing `excitingtools-1.4.0/excitingtools/constants/units.py` & `excitingtools-1.5.0/excitingtools/constants/units.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Physical constants, defined according to [CODATA 2018])(http://physics.nist.gov/constants)
 One could also consider importing them from scipy
 """
 import enum
 
 bohr_to_angstrom = 0.529177210903
 angstrom_to_bohr = 1. / bohr_to_angstrom
+Hartree_to_eV = 27.211396641308
 
 
 class Unit(enum.Enum):
     """
     Enum class for exciting units. All names are defined with
     as lowercase, for consistency.
 
@@ -27,14 +28,16 @@
     inv_bohr = enum.auto()
     inv_bohr_pow_3 = enum.auto()
     au = enum.auto()
     degrees = enum.auto()
     GK_max = enum.auto()
     electron_rest_mass = enum.auto()
     bohr_velocity_over_bohr_radius = enum.auto()
+    bohr_velocity = enum.auto()
+    force = enum.auto()
     null = enum.auto()
 
 
 # Map Unit enums to strings.
 # Required because JSON cannot dump objects to file.
 enum_to_string = {
     Unit.hartree: 'Hartree',
@@ -47,9 +50,11 @@
     Unit.inv_bohr: 'Bohr^-1',
     Unit.inv_bohr_pow_3: 'Bohr^-3',
     Unit.au: 'a.u.',
     Unit.degrees: 'degrees',
     Unit.GK_max: 'GK_max',
     Unit.electron_rest_mass: 'm_electron',
     Unit.bohr_velocity_over_bohr_radius: 'v_Bohr/r_Bohr',
+    Unit.bohr_velocity: 'Bohr/t_Bohr',
+    Unit.force: 'Hartree/Bohr', 
     Unit.null: 'null'
 }
```

### Comparing `excitingtools-1.4.0/excitingtools/dataclasses/band_structure.py` & `excitingtools-1.5.0/excitingtools/dataclasses/band_structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/dataclasses/data_structs.py` & `excitingtools-1.5.0/excitingtools/dataclasses/data_structs.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/dataclasses/eigenvalues.py` & `excitingtools-1.5.0/excitingtools/dataclasses/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/eigenstates/eigenstates.py` & `excitingtools-1.5.0/excitingtools/eigenstates/eigenstates.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/RT_TDDFT_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -182,7 +182,53 @@
             projection.append([float(x) for x in file[j].split()])
         kpoint['ik'] = ik
         kpoint['projection'] = np.asarray(projection)
 
     data['kpoints'] = kpoints
 
     return data
+
+def parse_atom_position_velocity_force(name: str) -> dict:
+    """ Parser for ATOM_????.OUT 
+    :param str name: name of file to parse
+    :return dict out: each dict key corresponds to time, position (3 columns), velocity (3 columns), total force (3 columns).
+    The 3 columns refer to the x, y, z components
+    """
+    try:
+        data = np.genfromtxt(name, skip_header=0)
+    except:
+        raise ParseError
+    out = {
+        "Time": data[:, 0],
+        "x": data[:, 1],
+        "y": data[:, 2],
+        "z": data[:, 3],
+        "vx": data[:, 4],
+        "vy": data[:, 5],
+        "vz": data[:, 6],
+        "Fx": data[:, 7],
+        "Fy": data[:, 8],
+        "Fz": data[:, 9]
+    }
+
+    return out
+
+def parse_force(name, skiprows=0):
+    """
+    Parser for X_????.OUT, where X can be:
+    - FCR: core corrections to forces
+    - FEXT: external forces (due to e.g. an electric field)
+    - FHF: Hellman-Feynman term of forces
+    - FVAL: valence corrections to forces
+    """
+    try:
+        data = np.genfromtxt(name, skip_header=skiprows)
+    except:
+        raise ParseError
+    out = {
+        "Time": data[:, 0],
+        "Fx": data[:, 1],
+        "Fy": data[:, 2],
+        "Fz": data[:, 3]
+    }
+
+    return out
```

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/bse_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/bse_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/groundstate_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/groundstate_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Ground state file parsers.
 
 All functions in this module could benefit from refactoring.
 """
 import xml.etree.ElementTree as ET
+import re
+import numpy as np
 
 from excitingtools.parser_utils.erroneous_file_error import ErroneousFileError
 from excitingtools.parser_utils.parser_decorators import xml_root
 
 
 def parse_info_out(name: str) -> dict:
     """
@@ -351,7 +353,82 @@
         structure['crystal']['basevect'] = {}
         k = 1
     for item in basevects:
         name = str(k)
         structure['crystal']['basevect'][name] = item
         k = k + 1
     return geometry
+
+
+def parse_linengy(name: str) -> dict:
+    """
+    Parser for: LINENGY.OUT
+
+    :param name: path of the file to parse
+    :returns: dictionary containing parsed file
+    """
+
+    linengy = {}
+
+    with open(file=name, mode='r') as fid:
+        lines = fid.readlines()
+
+    apw_line = []
+    lo_line = []
+
+    for i, line in enumerate(lines):
+        if 'APW functions' in line:
+            apw_line.append(i)
+        if 'local-orbital functions' in line:
+            lo_line.append(i)
+
+    apw_line.append(len(lines))
+
+    for i in range(0, len(lo_line)):
+        linengy[str(i)] = {}
+        apw = []
+        lo = []
+
+        for j in range(apw_line[i], lo_line[i]):
+            if "l =" in lines[j]:
+                apw.append(lines[j].split(':')[1].strip())
+        linengy[str(i)]['apw'] = apw
+
+        for j in range(lo_line[i], apw_line[i+1]):
+            if "l =" in lines[j]:
+                lo.append(lines[j].split(':')[1].strip())
+        linengy[str(i)]['lo'] = lo
+
+    return linengy
+
+
+def parse_lo_recommendation(name: str) -> dict:
+    """
+    Parser for: LO_RECOMMENDATION.OUT
+
+    :param name: path of the file to parse
+    :returns: dictionary containing parsed file                                                                                                  
+    """
+    with open(file=name, mode='r') as fid:
+        lines = fid.readlines()
+
+    n_species = int(lines[2].split(':')[1])
+    n_l_channels = int(lines[3].split(':')[1])
+    n_nodes = int(lines[4].split(':')[1])
+
+    lo_recommendation = {'n_species': n_species, 'n_l_channels': n_l_channels, 'n_nodes': n_nodes}
+
+    blocks = lines[6 :]
+    block_size = n_nodes + 3
+    n_blocks = n_l_channels * n_species
+
+    for iblock in range(0, n_blocks):
+        offset = iblock * block_size
+        matches = re.findall(r':\s(.*?)(?:,|$)', blocks[offset+0])
+        species, l = matches[0], int(matches[1])
+        # Package (node, n, energy) as one likes                                                                                        
+        if not species in lo_recommendation:
+            lo_recommendation.update({species: {}})
+        lo_recommendation[species].update({l: np.loadtxt(blocks[offset+2:offset+n_nodes+2]).tolist()})
+
+    return lo_recommendation
+
```

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_eigenvalues_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_eps00_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_info_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_info_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/gw_vxc_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/input_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/input_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/parser_factory.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/parser_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     'info.xml': groundstate_parser.parse_info_xml,
     'input.xml': input_parser.parse_input_xml,
     'species.xml': species_parser.parse_species_xml,
     'atoms.xml': groundstate_parser.parse_atoms,
     'evalcore.xml': groundstate_parser.parse_evalcore,
     'eigval.xml': groundstate_parser.parse_eigval,
     'geometry.xml': groundstate_parser.parse_geometry,
+    'LINENGY.OUT': groundstate_parser.parse_linengy,
+    'LO_RECOMMENDATION.OUT': groundstate_parser.parse_lo_recommendation,
     'RHO3D.xml': properties_parser.parse_plot_3d,
     'VCL3D.xml': properties_parser.parse_plot_3d,
     'VXC3D.xml': properties_parser.parse_plot_3d,
     'WF3D.xml': properties_parser.parse_plot_3d,
     'ELF3D.xml': properties_parser.parse_plot_3d,
     'EF3D.xml': properties_parser.parse_plot_3d,
     'LSJ.xml': properties_parser.parse_lsj,
@@ -119,14 +121,19 @@
     'VXCNN.DAT': gw_vxc_parser.parse_vxcnn,
     'EPS00_GW.OUT': gw_eps00_parser.parse_eps00_gw,
     'JIND.OUT': RT_TDDFT_parser.parse_jind,
     'NEXC.OUT': RT_TDDFT_parser.parse_nexc,
     'ETOT_RTTDDFT.OUT': RT_TDDFT_parser.parse_etot,
     'EIGVAL_': RT_TDDFT_parser.parse_eigval_screenshots,
     'PROJ_': RT_TDDFT_parser.parse_proj_screenshots,
+    'ATOM_': RT_TDDFT_parser.parse_atom_position_velocity_force,
+    'FCR_': RT_TDDFT_parser.parse_force,
+    'FEXT_': RT_TDDFT_parser.parse_force,
+    'FHF_': RT_TDDFT_parser.parse_force,
+    'FVAL_': RT_TDDFT_parser.parse_force,
     'wf1d-0001-0001.dat': properties_parser.parse_wf1d,
     'wf1d-0003-0001.dat': properties_parser.parse_wf1d,
     'wf2d-0001-0001.xsf': properties_parser.parse_wf2d,
     'wf2d-0003-0001.xsf': properties_parser.parse_wf2d,
     'wf3d-0001-0001.xsf': properties_parser.parse_wf3d,
     'wf3d-0003-0001.xsf': properties_parser.parse_wf3d,
     'wf3d-0001-0001.cube': properties_parser.parse_cube,
@@ -141,15 +148,24 @@
       EIGVAL_00.dat -> EIGVAL_
       EIGVAL_01.dat -> EIGVAL_
 
     :param file_name: File name containing fixed prefix and
     an extension beginning with '_'.
     :return file_name: File name prefix, else input file name.
     """
-    if ('EIGVAL_' in file_name) or ('PROJ_' in file_name):
+    prefixes = [
+        'EIGVAL_',
+        'PROJ_',
+        'ATOM_',
+        'FCR_',
+        'FEXT_',
+        'FHF_',
+        'FVAL_'
+    ]
+    if any( [ prefix in file_name for prefix in prefixes ] ) :
         file_name_prefix = file_name.split('_')[0] + '_'
         return file_name_prefix
 
     return file_name
 
 
 def parser_chooser(full_file_name: str) -> dict:
@@ -158,14 +174,15 @@
     REQUIREMENTS. Parser function must:
      a) accept a file name (not a contents string)
      b) return a dictionary.
 
     param: str, full_file_name: file name prepended by full path
     return: parsed data
     """
+ 
     full_file_name = full_file_name.rstrip()
     if not os.path.exists(full_file_name):
         raise FileNotFoundError(f'File not found: {full_file_name}')
 
     file_name = os.path.split(full_file_name)[1]
     file_name = truncate_fnames_with_exts(file_name)
 
@@ -176,7 +193,8 @@
     parser = _file_to_parser[file_name]
     data = parser(full_file_name)
 
     #  TODO(Alex) Issue 135 Ensure all parsers return appropriate values, not strings.
     #   container_converter should therefore be used as a decorator on parsers with values that are strings.
     #   That will massively speed up parsing
     return container_converter(data)
+
```

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/properties_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/properties_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_dict_parsers/species_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_dict_parsers/species_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py` & `excitingtools-1.5.0/excitingtools/exciting_obj_parsers/eigenvalue_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py` & `excitingtools-1.5.0/excitingtools/exciting_obj_parsers/gw_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_obj_parsers/input_xml.py` & `excitingtools-1.5.0/excitingtools/exciting_obj_parsers/input_xml.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/exciting_obj_parsers/ks_band_structure.py` & `excitingtools-1.5.0/excitingtools/exciting_obj_parsers/ks_band_structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/input/bandstructure.py` & `excitingtools-1.5.0/excitingtools/input/bandstructure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/input/base_class.py` & `excitingtools-1.5.0/excitingtools/input/base_class.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/input/dynamic_class.py` & `excitingtools-1.5.0/excitingtools/input/dynamic_class.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/input/input_classes.py` & `excitingtools-1.5.0/excitingtools/input/input_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,19 +53,15 @@
         self.__dict__["title"].title = title
 
     def to_xml_str(self) -> str:
         """Compose XML ElementTrees from exciting input classes to create an input xml string.
 
         :return: Input XML tree as a string, with pretty formatting.
         """
-        xml_tree = self.to_xml()
-        tags_to_prettify = ["\t<structure", "\t\t<crystal", "\t\t<species", "\t\t\t<atom", "\t<groundstate", "\t<xs",
-                            "\t\t<screening", "\t\t<BSE", "\t\t<energywindow"]
-        input_xml_str = prettify_tag_attributes(xml_tree_to_pretty_str(xml_tree), tags_to_prettify)
-        return input_xml_str
+        return prettify_tag_attributes(xml_tree_to_pretty_str(self.to_xml()))
 
     def write(self, filename: Union[str, Path] = _default_filename):
         """Writes the xml string to file.
 
         :param filename: name of the file.
         """
         with open(filename, "w") as fid:
```

### Comparing `excitingtools-1.4.0/excitingtools/input/structure.py` & `excitingtools-1.5.0/excitingtools/input/structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/input/xml_utils.py` & `excitingtools-1.5.0/excitingtools/input/xml_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Utilities to aid in writing and formatting XML
 """
 import re
-from typing import Union, List
 from xml.dom import minidom
 from xml.etree import ElementTree
 
 
 def xml_tree_to_pretty_str(elem: ElementTree.Element) -> str:
     """Convert an XML element to a pretty string.
 
@@ -13,126 +12,112 @@
     :return str : XML tree string, with pretty formatting.
     """
     rough_string = ElementTree.tostring(elem, 'utf-8')
     reparsed = minidom.parseString(rough_string)
     return reparsed.toprettyxml(indent="\t")
 
 
-def line_reformatter(input_str: str, tag: str) -> str:
+def line_reformatter(input_str: str) -> str:
     """Identify attributes of an XML string element, and reformat them such that they are on new lines.
 
     NOTE: This could be split into two routines. One that finds the (start, end) of
     each attribute, and one that reformats the string, given these indices.
     (or refactored completely - current solution is not very elegant).
 
     Example
     ----------
     Takes:
-        input_str = <groundstate do="fromscratch" ngridk="6 6 6" nosource="false" rgkmax="8.0"
-                     tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> </groundstate>
-        tag = 'groundstate'
+        input_str = '\t<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" rgkmax="8.0"
+                     tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> </groundstate>'
 
     Returns:
         reformatted_str =
-        <groundstate
+        '<groundstate
              do="fromscratch"
              ngridk="6 6 6"
              nosource="false"
              rgkmax="8.0"
              tforce="true"
              vkloff="0 0 0"
              xctype="GGA_PBE_SOL">
-        </groundstate>
+        </groundstate>'
 
     There are 3 possibilities: the xml element has further subelements, than it ends only with a single '>',
     if the xml element has only attributes, than there are two options to close the element: either long with a
     '> </tag>' or short with a '/>'.
 
     :param str input_str: Input string, opened and closed with an XML element.
-    :param str tag: XML element name.
     :return str reformatted_str: Reformatted form of input_str
     """
-    # Get rid of format characters, like \n, \t etc
-    input_str = input_str.strip()
-    number_of_tag_indents = len(tag) - len(tag.strip())
-    tag = tag.strip()
-
-    # This should not occur if the routine is only used with `prettify_tag_attributes`
-    if tag != input_str[0:len(tag)]:
-        raise ValueError(f'tag, "{tag}", is inconsistent the element name, '
-                         f'"{input_str[0:len(tag)]}"')
+    full_tag = input_str.split(" ")[0]
+    tag = full_tag.strip()
+    number_of_tag_indents = len(full_tag) - len(tag)
 
     tag_indent = '\t' * number_of_tag_indents
     attr_indent = tag_indent + ' ' * 3
 
+    # Get rid of format characters, like \n, \t etc
+    input_str = input_str.strip()
+
     # Isolate attributes according to position of quotation marks in string
     # (cannot use whitespaces to split)
     quote_indices = [x.start() for x in re.finditer('\"', input_str)]
-    # if there are only few attributes present:
-    if len(quote_indices) < 5:
-        return tag_indent + input_str
     closing_quote_indices = quote_indices[1::2]
     attribute_start_indices = [len(tag) + 1] + [i + 1 for i in
                                                 closing_quote_indices[:-1]]
 
     reformatted_str = tag_indent + tag + '\n'
 
     for i in range(0, len(attribute_start_indices)):
         i1 = attribute_start_indices[i]
         i2 = closing_quote_indices[i]
         attribute_str = input_str[i1:i2 + 1].strip()
         reformatted_str += attr_indent + attribute_str + '\n'
 
     # short ending option:
     if input_str[-2:] == '/>':
-        return reformatted_str[:-1] + '/>\n'
-    reformatted_str = reformatted_str[:-1] + '>\n'
+        return reformatted_str[:-1] + '/>'
+    reformatted_str = reformatted_str[:-1] + '>'
     # no ending option:
     if not input_str[-(len(tag) + 2):-len(tag)] == '</':
         return reformatted_str
     # long ending option:
-    reformatted_str += tag_indent + input_str[-(len(tag) + 2):] + '\n'
+    reformatted_str += "\n" + tag_indent + input_str[-(len(tag) + 2):] + ''
     return reformatted_str
 
 
-def prettify_tag_attributes(xml_string: str, tag: Union[str, List[str]]) -> str:
-    """Prettify XML string formatting of attributes, for a given XML element.
+def prettify_tag_attributes(xml_string: str) -> str:
+    """Prettify XML string formatting of attributes.
 
-    The routine finds the line containing the XML element which matches <tag, applies
-    a line_reformatter, and replaces the line. If the tag is not matched, the input
-    xml_string is returned.
+    The routine finds the lines containing an XML element, applies
+    a line_reformatter, and replaces the line. Only for long lines with more than 2 attributes.
 
     Example usage:
     ```
         string = <groundstate do="fromscratch" ngridk="6 6 6" nosource="false" rgkmax="8.0" tforce="true" vkloff="0 0 0"
                   xctype="GGA_PBE_SOL"> </groundstate>
-        pretty_string = prettify_tag_attributes(string, '<groundstate')
+        pretty_string = prettify_tag_attributes(string)
         print(pretty_string)
         > <groundstate
              do="fromscratch"
              ngridk="6 6 6"
              nosource="false"
              rgkmax="8.0"
              tforce="true"
              vkloff="0 0 0"
              xctype="GGA_PBE_SOL">
         </groundstate>
     ```
 
     :param str xml_string: Already-prettified XML string (assumes tags are on their own lines)
-    :param str tag: XML element of the form "<tag" or multiple of these tags as list
-    :return str reformatted_xml_string: xml_string, with the tag substring reformatted according to the example
+    :return str reformatted_xml_string: xml_string, with the tag substrings reformatted according to the example
      - Line break per attribute.
     """
-    if isinstance(tag, str):
-        tag = [tag]
-
     xml_list = xml_string.split('\n')
+    min_number_attributes_for_split = 3
 
     for i, line in enumerate(xml_list):
-        for single_tag in tag:
-            match = re.match(single_tag, line)
-            if match:
-                xml_list[i] = line_reformatter(line, single_tag)
-                break
+        if line.count("=") >= min_number_attributes_for_split:
+            xml_list[i] = line_reformatter(line)
 
-    return "".join(x + '\n' for x in xml_list)
+    xml_list_without_blank_lines = filter(lambda x: x.strip(), xml_list)
+    return "".join(x + '\n' for x in xml_list_without_blank_lines)
```

### Comparing `excitingtools-1.4.0/excitingtools/math/math_utils.py` & `excitingtools-1.5.0/excitingtools/math/math_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/parser_utils/grep_parser.py` & `excitingtools-1.5.0/excitingtools/parser_utils/grep_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/parser_utils/parser_decorators.py` & `excitingtools-1.5.0/excitingtools/parser_utils/parser_decorators.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/parser_utils/parser_utils.py` & `excitingtools-1.5.0/excitingtools/parser_utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/parser_utils/regex_parser.py` & `excitingtools-1.5.0/excitingtools/parser_utils/regex_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/parser_utils/simple_parser.py` & `excitingtools-1.5.0/excitingtools/parser_utils/simple_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/runner/runner.py` & `excitingtools-1.5.0/excitingtools/runner/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ Binary runner and results classes.
 """
+from __future__ import annotations
+
 import copy
-from typing import List, Optional, Union
-from pathlib import Path
+import enum
 import os
-import subprocess
 import shutil
+import subprocess
 import time
-import enum
-
+from pathlib import Path
+from typing import List, Optional, Union
 
 from excitingtools.utils.jobflow_utils import special_serialization_attrs
 
 
 class RunnerCode(enum.Enum):
     """ Runner codes.
      By default, the initial value starts at 1.
@@ -38,36 +39,36 @@
 
 class BinaryRunner:
     """ Class to execute a subprocess.
     """
     path_type = Union[str, Path]
 
     def __init__(self,
-                 binary: str,
-                 run_cmd: Union[List[str], str],
-                 omp_num_threads: int,
-                 time_out: int,
-                 directory: Optional[path_type] = './',
-                 args=None) -> None:
+                 binary: path_type,
+                 run_cmd: List[str] | str = "",
+                 omp_num_threads: int = 1,
+                 time_out: int = 60,
+                 directory: path_type = './',
+                 args: Optional[List[str]] = None):
         """ Initialise class.
 
         :param str binary: Binary name prepended by full path, or just binary name (if present in $PATH).
         :param Union[List[str], str] run_cmd: Run commands sequentially as a list. For example:
-          * For serial: ['./'] or ['']
+          * For serial: []
           * For MPI:   ['mpirun', '-np', '2']
         or as a string. For example"
-          * For serial: "./"
+          * For serial: ""
           * For MPI: "mpirun -np 2"
-        :param int omp_num_threads: Number of OMP threads.
-        :param int time_out: Number of seconds before a job is defined to have timed out.
-        :param List[str] args: Optional arguments for the binary.
+        :param omp_num_threads: Number of OMP threads.
+        :param time_out: Number of seconds before a job is defined to have timed out.
+        :param args: Optional arguments for the binary.
         """
         if args is None:
             args = []
-        self.binary = binary
+        self.binary = Path(binary).as_posix()
         self.directory = directory
         self.run_cmd = run_cmd
         self.omp_num_threads = omp_num_threads
         self.time_out = time_out
         self.args = args
 
         if not os.path.isfile(self.binary):
@@ -127,33 +128,18 @@
         except IndexError:
             raise ValueError("Number of MPI processes must be specified after the '-np'")
         except ValueError:
             raise ValueError("Number of MPI processes should be an int")
         if mpi_processes <= 0:
             raise ValueError("Number of MPI processes must be > 0")
 
-    def _compose_execution_list(self) -> list:
-        """Generate a complete list of strings to pass to subprocess.run(), to execute the calculation.
-
-        For example, given:
-          ['mpirun', '-np, '2'] + ['binary.exe'] + ['>', 'std.out']
-
-        return ['mpirun', '-np, '2', 'binary.exe', '>', 'std.out']
-        """
-        run_cmd = self.run_cmd
-
-        if self.run_cmd[0] == './':
-            run_cmd = []
-
-        return run_cmd + [self.binary] + self.args
-
     def run(self) -> SubprocessRunResults:
         """Run a binary.
         """
-        execution_list = self._compose_execution_list()
+        execution_list = self.run_cmd + [self.binary] + self.args
         my_env = {**os.environ, "OMP_NUM_THREADS": str(self.omp_num_threads)}
 
         time_start: float = time.time()
         try:
             result = subprocess.run(execution_list,
                                     env=my_env,
                                     stdout=subprocess.PIPE,
```

### Comparing `excitingtools-1.4.0/excitingtools/structure/ase_utilities.py` & `excitingtools-1.5.0/excitingtools/structure/ase_utilities.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/structure/lattice.py` & `excitingtools-1.5.0/excitingtools/structure/lattice.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/structure/pymatgen_utilities.py` & `excitingtools-1.5.0/excitingtools/structure/pymatgen_utilities.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/utils/dict_utils.py` & `excitingtools-1.5.0/excitingtools/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/utils/schema_parsing.py` & `excitingtools-1.5.0/excitingtools/utils/schema_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -182,15 +182,18 @@
     formatted_string += current_line_string[:-2] + "]"
     return formatted_string
 
 
 def get_all_include_files() -> list:
     """ Gets a list of all included files in the input.xsd file.
     """
-    input_schema_file = get_excitingtools_root() / '../../xml/schema/input.xsd'
+    input_schema_file = (get_excitingtools_root() / '../../xml/schema/input.xsd').resolve()
+    if not input_schema_file.exists():
+        raise ValueError("Couldn't find exciting schema. Most likely you are using excitingtools outside of exciting."
+                         "To fix this, try installing excitingtools from source in editable (-e) mode.")
     return re.findall(r'<xs:include id=".*" schemaLocation="(.*)\.xsd"/>', input_schema_file.read_text())
 
 
 def main():
     """ Main function to read the schema and write it to python readable file.
     """
     filename = Path(__file__).parent / "valid_attributes.py"
```

### Comparing `excitingtools-1.4.0/excitingtools/utils/test_utils.py` & `excitingtools-1.5.0/excitingtools/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/utils/utils.py` & `excitingtools-1.5.0/excitingtools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/excitingtools/utils/valid_attributes.py` & `excitingtools-1.5.0/excitingtools/utils/valid_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 dfthalf_valid_attributes = ['printVSfile'] 
 
 Hybrid_valid_attributes = ['HSEsingularity', 'eccoeff', 'epsmb', 'exchangetype', 'excoeff', 'gmb', 'lmaxmb', 'maxscl', 
                            'mblksiz', 'omega', 'updateRadial'] 
 
 sirius_valid_attributes = ['cfun', 'density', 'densityinit', 'eigenstates', 'sfacg', 'vha', 'xc'] 
 
-solver_valid_attributes = ['evaltol', 'packedmatrixstorage', 'type'] 
+solver_valid_attributes = ['constructHS', 'evaltol', 'minenergy', 'packedmatrixstorage', 'type'] 
 
 OEP_valid_attributes = ['convoep', 'maxitoep', 'tauoep'] 
 
 RDMFT_valid_attributes = ['maxitc', 'maxitn', 'rdmalpha', 'rdmmaxscl', 'rdmtemp', 'rdmxctype', 'taurdmc', 'taurdmn'] 
 
 output_valid_attributes = ['state'] 
 
@@ -258,16 +258,17 @@
 excitonPlot_mandatory_attributes = ['electron', 'hole'] 
 
 exciton_valid_attributes = ['fix', 'lambda'] 
 
 electron_valid_subtrees = ['plot3d', 'plot1d', 'plot2d'] 
 
 realTimeTDDFT_valid_attributes = ['TaylorOrder', 'calculateNExcitedElectrons', 'calculateTotalEnergy', 'endTime', 
-                                  'normalizeWF', 'printAfterIterations', 'printTimingDetailed', 'printTimingGeneral', 
-                                  'propagator', 'readPmatBasis', 'subtractJ0', 'timeStep', 'vectorPotentialSolver'] 
+                                  'forcePmatHermitian', 'normalizeWF', 'printAfterIterations', 'printTimingDetailed', 
+                                  'printTimingGeneral', 'propagator', 'readPmatBasis', 'subtractJ0', 'timeStep', 
+                                  'vectorPotentialSolver'] 
 realTimeTDDFT_valid_subtrees = ['predictorCorrector', 'screenshots', 'laser'] 
 
 predictorCorrector_valid_attributes = [' maxIterations', 'tol'] 
 
 screenshots_valid_attributes = ['niter', 'printAbsProjCoeffs'] 
 
 laser_valid_attributes = ['fieldType']
```

### Comparing `excitingtools-1.4.0/excitingtools.egg-info/PKG-INFO` & `excitingtools-1.5.0/excitingtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excitingtools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs.
 Author-email: Alexander Buccheri <alexander.buccheri@mpsd.mpg.de>, Fabian Peschel <peschelf@physik.hu-berlin.de>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -882,15 +882,15 @@
 
 #### Binary Execution
 
 Next we can define a runner and run our calculation:
 ```python3
 from excitingtools.runner.runner import BinaryRunner
 
-runner = BinaryRunner('exciting_smp', run_cmd=[''], omp_num_threads=4, time_out=500)
+runner = BinaryRunner('exciting_smp', run_cmd='', omp_num_threads=4, time_out=500)
 run_status = runner.run()
 ```
 
 #### Parsing Outputs
 
 After the successful completion of the calculation, we can parse the relevant output files as dictionaries, using
 `parser_chooser`. These are the main files one would be interested in after performing a ground state calculation, for
```

### Comparing `excitingtools-1.4.0/excitingtools.egg-info/SOURCES.txt` & `excitingtools-1.5.0/excitingtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/paper/joss_latex.template` & `excitingtools-1.5.0/paper/joss_latex.template`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/paper/latex.template` & `excitingtools-1.5.0/paper/latex.template`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/paper/paper.bib` & `excitingtools-1.5.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/paper/paper.md` & `excitingtools-1.5.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/pyproject.toml` & `excitingtools-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "excitingtools"
 description = "Utilities for aiding in the construction of exciting inputs and the postprocessing exciting outputs."
-version = "1.4.0"
+version = "1.5.0"
 authors = [
     { name = "Alexander Buccheri", email = "alexander.buccheri@mpsd.mpg.de"},
     { name = "Fabian Peschel",     email = "peschelf@physik.hu-berlin.de"}
 ]
 license = {file = "COPYING.md"}
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `excitingtools-1.4.0/tests/dataclasses/test_band_structure.py` & `excitingtools-1.5.0/tests/dataclasses/test_band_structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dataclasses/test_eigenvalues.py` & `excitingtools-1.5.0/tests/dataclasses/test_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_bse_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_bse_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/mock_gw_info_out.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/mock_gw_info_out.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_dos_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_eignvalues_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_eps00_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_info_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_info_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_gw/test_gw_vxc_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_input_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_input_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_ks_band_structure.py` & `excitingtools-1.5.0/tests/dict_parsers/test_ks_band_structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_properties_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/dict_parsers/test_species_parser.py` & `excitingtools-1.5.0/tests/dict_parsers/test_species_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/eigenstates/test_eigenstates.py` & `excitingtools-1.5.0/tests/eigenstates/test_eigenstates.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_base_class.py` & `excitingtools-1.5.0/tests/input/test_base_class.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_dynamic_class.py` & `excitingtools-1.5.0/tests/input/test_dynamic_class.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_ground_state.py` & `excitingtools-1.5.0/tests/input/test_ground_state.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_input_xml.py` & `excitingtools-1.5.0/tests/input/test_input_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,25 +175,25 @@
     assert energywindow_xml.get('points') == '4000'
 
 
 def test_as_dict(exciting_input_xml: ExcitingInputXML, mock_env_jobflow_missing):
     dict_representation = exciting_input_xml.as_dict()
     assert set(dict_representation.keys()) == {"xml_string"}
     # check only that the xml string starts with the correct first lines:
-    assert dict_representation["xml_string"].startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t \n\t'
+    assert dict_representation["xml_string"].startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t'
                                                         '<title>Test Case</title>\n\t<structure')
 
 
 def test_as_dict_jobflow(exciting_input_xml: ExcitingInputXML, mock_env_jobflow):
     dict_representation = exciting_input_xml.as_dict()
     xml_string = dict_representation.pop("xml_string")
     assert dict_representation == {'@class': 'ExcitingInputXML',
                                    '@module': 'excitingtools.input.input_classes'}
     # check only that the xml string starts with the correct first lines:
-    assert xml_string.startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t \n\t'
+    assert xml_string.startswith('<?xml version="1.0" ?>\n<input sharedfs="true">\n\t'
                                  '<title>Test Case</title>\n\t<structure')
 
 
 def test_from_dict(exciting_input_xml: ExcitingInputXML, mock_env_jobflow_missing):
     new_input_xml = ExcitingInputXML.from_dict(exciting_input_xml.as_dict())
     assert new_input_xml.title.title == "Test Case"  # pylint: disable=no-member
     assert new_input_xml.groundstate.ngridk == [6, 6, 6]  # pylint: disable=no-member
```

### Comparing `excitingtools-1.4.0/tests/input/test_properties.py` & `excitingtools-1.5.0/tests/input/test_properties.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_structure.py` & `excitingtools-1.5.0/tests/input/test_structure.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/input/test_xml_utils.py` & `excitingtools-1.5.0/tests/input/test_xml_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,65 @@
 """Test XML utilities.
 """
-import pytest
 
-from excitingtools.input.xml_utils import line_reformatter, \
-    prettify_tag_attributes
+from excitingtools.input.xml_utils import line_reformatter
 
 
 def test_line_reformatter_long_ending():
     """Test reformatting of XML as a string works."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
         '</groundstate>'
     )
-    pretty_input_str = line_reformatter(input_str, '<groundstate')
+    pretty_input_str = line_reformatter(input_str)
     # Note, whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
    xctype="GGA_PBE_SOL">
-</groundstate>
-"""
+</groundstate>"""
     assert reference == pretty_input_str
 
 
 def test_line_reformatter_short_ending():
     """Test reformatting of XML as a string works for xml strings
     with a different (short) ending."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"/> '
     )
-    pretty_input_str = line_reformatter(input_str, '<groundstate')
+    pretty_input_str = line_reformatter(input_str)
     # Note, whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
-   xctype="GGA_PBE_SOL"/>
-"""
+   xctype="GGA_PBE_SOL"/>"""
     assert reference == pretty_input_str
 
 
 def test_line_reformatter_no_closing():
     """Test reformatting of XML as a string works for xml strings
     with no closing at the end."""
     input_str = (
         '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
         'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
     )
-    pretty_input_str = line_reformatter(input_str, '<groundstate')
+    pretty_input_str = line_reformatter(input_str)
     # Note, whitespace is important
     reference = """<groundstate
    do="fromscratch"
    ngridk="6 6 6"
    nosource="false"
    rgkmax="8.0"
    tforce="true"
    vkloff="0 0 0"
-   xctype="GGA_PBE_SOL">
-"""
+   xctype="GGA_PBE_SOL">"""
     assert reference == pretty_input_str
-
-
-def test_line_reformatter_unmatched_tag():
-    """
-    Test error occurs when tag is inconsistent with the element name.
-
-    Recall the tag is passed to `line_reformatter`. This should not occur if
-    `line_reformatter` is only called from `prettify_tag_attributes`.
-    """
-    input_str = (
-        '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
-        'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
-        '</groundstate>'
-    )
-
-    with pytest.raises(ValueError) as error:
-        line_reformatter(input_str, '<error')
-
-    assert error.value.args[0] == 'tag, "<error", is inconsistent the element name, "<groun"'
-
-
-def test_prettify_tag_attributes():
-    """Test prettifying the tag attributes."""
-    input_str = (
-        '<groundstate do="fromscratch" ngridk="6 6 6" nosource="false" '
-        'rgkmax="8.0" tforce="true" vkloff="0 0 0" xctype="GGA_PBE_SOL"> '
-        '</groundstate>'
-    )
-
-    output = prettify_tag_attributes(input_str, '<unmatched')
-    assert output.rstrip() == input_str, (
-        "If the tag is not matched in the XML string, the input string should "
-        "be returned - (newline character stripped from end)")
```

### Comparing `excitingtools-1.4.0/tests/input/test_xs.py` & `excitingtools-1.5.0/tests/input/test_xs.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/obj_parsers/test_eigenvalue_parser.py` & `excitingtools-1.5.0/tests/obj_parsers/test_eigenvalue_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/obj_parsers/test_gw_dos.py` & `excitingtools-1.5.0/tests/obj_parsers/test_gw_dos.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/obj_parsers/test_gw_eigenvalues.py` & `excitingtools-1.5.0/tests/obj_parsers/test_gw_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/obj_parsers/test_input_parser.py` & `excitingtools-1.5.0/tests/obj_parsers/test_input_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,8 @@
 </input>
 """
 
 
 def test_parse_input_xml_to_object():
     input_xml = parse_input_xml(reference_input_str)
     assert set(vars(input_xml)) == {'xs', 'groundstate', 'structure', 'title'}
-    assert input_xml.to_xml_str().startswith('<?xml version="1.0" ?>\n<input>\n\t \n\t<title>Lithium Fluoride BSE')
+    assert input_xml.to_xml_str().startswith('<?xml version="1.0" ?>\n<input>\n\t<title>Lithium Fluoride BSE')
```

### Comparing `excitingtools-1.4.0/tests/parser_utils/test_parser_utils.py` & `excitingtools-1.5.0/tests/parser_utils/test_parser_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/parser_utils/test_regex_parser.py` & `excitingtools-1.5.0/tests/parser_utils/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/parser_utils/test_simple_parser.py` & `excitingtools-1.5.0/tests/parser_utils/test_simple_parser.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/runner/test_runner.py` & `excitingtools-1.5.0/tests/runner/test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pathlib import Path
 from typing import Any
 
 import pytest
 
 from excitingtools.runner.runner import BinaryRunner
 
-
 mock_binary = "false_exciting_binary"
 
 
 @pytest.mark.xfail(shutil.which(mock_binary) is not None, reason="Binary name exists.")
 def test_no_binary():
     with pytest.raises(FileNotFoundError,
                        match=fr"{mock_binary} binary is not present in the current directory nor in \$PATH"):
@@ -101,19 +100,14 @@
 
 def test_from_dict(tmp_path: Path, runner):
     new_runner = BinaryRunner.from_dict(runner.as_dict())
     assert new_runner.binary == (tmp_path / "exciting_mpismp").as_posix()
     assert new_runner.time_out == 260
 
 
-def test__compose_execution_list(runner):
-    binary = runner.binary
-    assert runner._compose_execution_list() == ['mpirun', '-np', '3', binary, '>', 'std.out']
-
-
 def test_run_with_bash_command(tmp_path: Path):
     """Produces a runner with binary and run dir mocked up.
     Test a simple echo command.
     """
     run_dir = tmp_path / "ab/de"
     run_dir.mkdir(parents=True)
     binary = tmp_path / "hello"
```

### Comparing `excitingtools-1.4.0/tests/structure/test_lattice.py` & `excitingtools-1.5.0/tests/structure/test_lattice.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/structure/test_pymatgen_utilities.py` & `excitingtools-1.5.0/tests/structure/test_pymatgen_utilities.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/utils/test_dict_utils.py` & `excitingtools-1.5.0/tests/utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/utils/test_schema_parsing.py` & `excitingtools-1.5.0/tests/utils/test_schema_parsing.py`

 * *Files identical despite different names*

### Comparing `excitingtools-1.4.0/tests/utils/test_utils.py` & `excitingtools-1.5.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

