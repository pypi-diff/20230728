# Comparing `tmp/mknodes-0.6.0.tar.gz` & `tmp/mknodes-0.8.3.tar.gz`

## Comparing `mknodes-0.6.0.tar` & `mknodes-0.8.3.tar`

### file list

```diff
@@ -1,91 +1,92 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.6.0/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.6.0/Makefile
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.6.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 mknodes-0.6.0/docs/gen_pages.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.6.0/docs/gen_qt.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkadmonition.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkannotations.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkimage.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkinstallguide.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mklink.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mklist.py
--rw-r--r--   0        0        0     8975 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mknode.py
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkpage.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/__init__.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/introduce_nodes.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/resources/codeofconduct.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/debugging.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/helpers.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/linkprovider.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mknodes-0.6.0/mknodes/utils/packageinfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_admonition.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_annotations.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_image.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_linkreplacer.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_modulepage.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_nav.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_packageinfo.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.6.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.6.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.6.0/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.6.0/README.md
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 mknodes-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mknodes-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.8.3/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.8.3/Makefile
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.8.3/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.8.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.8.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 mknodes-0.8.3/docs/gen_pages.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 mknodes-0.8.3/docs/gen_qt.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkannotations.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkhtmlblock.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkimage.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mklink.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mklist.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mknode.py
+-rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkshields.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktable.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktabs.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/introduce_nodes.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/resources/codeofconduct.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/debugging.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/packageinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_admonition.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_annotations.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_image.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_linkreplacer.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_list.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_modulepage.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_nav.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_packageinfo.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.8.3/README.md
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 mknodes-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mknodes-0.8.3/PKG-INFO
```

### Comparing `mknodes-0.6.0/.pre-commit-config.yaml` & `mknodes-0.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/Makefile` & `mknodes-0.8.3/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mkdocs.yml` & `mknodes-0.8.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/.github/workflows/build.yml` & `mknodes-0.8.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/.github/workflows/documentation.yml` & `mknodes-0.8.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/docs/gen_qt.py` & `mknodes-0.8.3/docs/gen_qt.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import mknodes
 
 prettyqt.import_all()
 
 QT_MODULE_ATTR = "QT_MODULE"
 
 root_nav = mknodes.MkNav()
-page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
-page.add_header("Not in the mood to write documentation? Let´s code it then!", level=3)
+page = root_nav.add_index_page("Overview", hide_toc=True, hide_nav=True)
+page.add_header("Test script: Build the PrettyQt documentation", level=1)
 
-qt_docs = root_nav.add_doc(prettyqt, section_name="qt_modules")
-extra_docs = root_nav.add_doc(prettyqt, section_name="additional_modules")
+qt_docs = root_nav.add_doc(prettyqt, section_name="Qt modules")
+extra_docs = root_nav.add_doc(prettyqt, section_name="Additional modules")
 
 for submod in qt_docs.iter_modules(predicate=lambda x: hasattr(x, QT_MODULE_ATTR)):
     subdoc = qt_docs.add_doc(submod, flatten_nav=True)
     subdoc.collect_classes()
 for submod in extra_docs.iter_modules(predicate=lambda x: not hasattr(x, QT_MODULE_ATTR)):
-    subdoc = extra_docs.add_doc(submod, flatten_nav=True)
+    subdoc = extra_docs.add_doc(submod)
     subdoc.collect_classes()
 
 
 # root_nav.pretty_print()
 root_nav.write()  # Finally, we write the whole tree.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mknodes-0.6.0/mknodes/__init__.py` & `mknodes-0.8.3/mknodes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from .mkblock import MkBlock
+from .mkhtmlblock import MkHtmlBlock
 from .mkadmonition import MkAdmonition
 from .mknode import MkNode
 from .mktext import MkText
 from .mkcontainer import MkContainer
 from .mkcode import MkCode
 from .mkdocstrings import MkDocStrings
 from .mkimage import MkImage
@@ -33,14 +34,15 @@
 from .mknav import MkNav
 from .mkdoc import MkDoc
 
 
 __all__ = [
     "MkNode",
     "MkBlock",
+    "MkHtmlBlock",
     "MkContainer",
     "MkNav",
     "MkDocStrings",
     "MkText",
     "MkCode",
     "MkImage",
     "MkBinaryImage",
@@ -63,8 +65,8 @@
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
     "MkInstallGuide",
 ]
 
-__version__ = "0.6.0"
+__version__ = "0.8.3"
```

### Comparing `mknodes-0.6.0/mknodes/mkadmonition.py` & `mknodes-0.8.3/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkannotations.py` & `mknodes-0.8.3/mknodes/mkannotations.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkbinaryimage.py` & `mknodes-0.8.3/mknodes/mkbinaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkblock.py` & `mknodes-0.8.3/mknodes/mkblock.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class MkBlock(mknode.MkNode):
     """pymdownx-based block."""
 
     def __init__(
         self,
         typ: str,
         content: str | mknode.MkNode = "",
+        *,
         title: str = "",
         attributes: dict[str, str | bool] | None = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.typ = typ
         self.attributes = attributes or {}
```

### Comparing `mknodes-0.6.0/mknodes/mkcode.py` & `mknodes-0.8.3/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkcontainer.py` & `mknodes-0.8.3/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkcritic.py` & `mknodes-0.8.3/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkdiagram.py` & `mknodes-0.8.3/mknodes/mkdiagram.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,11 +58,19 @@
 
     def _to_markdown(self) -> str:
         items = list(self.items) + [f"{a} --> {b}" for a, b in self.connections]
         item_str = textwrap.indent("\n".join(items), "  ")
         text = f"{self.graph_type} {self.orientation}\n{item_str}"
         return f"```mermaid\n{text}\n```"
 
+    @staticmethod
+    def examples():
+        yield dict(
+            graph_type="flow",
+            items=["1", "2", "3"],
+            connections=[("1", "2"), ("2", "3")],
+        )
+
 
 if __name__ == "__main__":
     diagram = MkDiagram(graph_type="flow")
     print(diagram)
```

### Comparing `mknodes-0.6.0/mknodes/mkdoc.py` & `mknodes-0.8.3/mknodes/mkdoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             self,
             module=self.module_name,
             section=self.section or "<root>",
             filename=self.filename,
         )
 
     def to_markdown(self) -> str:
-        self.add_module_overview()
+        self._add_module_overview()
         for klass in self.klasses:
             self.add_class_page(klass=klass, flatten=self.flatten_nav)
         for submod in self.submodules:
             self.add_doc(submod, class_page=self.ClassPage, flatten_nav=self.flatten_nav)
         return super().to_markdown()
 
     def collect_classes(
@@ -217,37 +217,35 @@
     #         hide_toc=True,
     #         path=pathlib.Path("index.md"),
     #         # parent=self,
     #     )
     #     page += mknodes.ModuleTable(self.module_name, predicate=predicate)
     #     return page
 
-    def add_module_overview(
+    def _add_module_overview(
         self,
         title: str | None = None,
         **kwargs: Any,
     ) -> mkmodulepage.MkModulePage:
         """Add a page showing all submodules.
 
         Arguments:
             title: Override title for the section.
             kwargs: kwargs passed to MkModulePage.
         """
-        # TODO: slugify?
-        path = pathlib.Path("index.md" if title is None else f"{title}.md")
-        # parts = path.parts[:-1]
         page = mkmodulepage.MkModulePage(
             hide_toc=True,
             module=self.module,
             klasses=self.klasses,
-            path=path,
+            path="index.md" if title is None else f"{title}.md",
             parent=self,
             **kwargs,
         )
-        self.nav[title or self.module_name] = page
+        self.index_title = title or self.module_name
+        self.index_page = page
         return page
 
     # def iter_files(self, glob: str = "*/*.py") -> Iterator[pathlib.Path]:
     #     """Iter through files based on glob.
 
     #     Arguments:
     #         glob: glob to use for filtering
```

### Comparing `mknodes-0.6.0/mknodes/mkdocstrings.py` & `mknodes-0.8.3/mknodes/mkdocstrings.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkimage.py` & `mknodes-0.8.3/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkinstallguide.py` & `mknodes-0.8.3/mknodes/mkinstallguide.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mklink.py` & `mknodes-0.8.3/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mklist.py` & `mknodes-0.8.3/mknodes/mklist.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mknav.py` & `mknodes-0.8.3/mknodes/mknav.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Sequence
 import logging
 import os
 import pathlib
 import re
 import types
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import mkdocs_gen_files
 
 from typing_extensions import Self
 
 from mknodes import mknav, mknode, mkpage, mktext
 from mknodes.utils import helpers
@@ -48,14 +48,16 @@
         self.filename = filename
         self.path = (
             pathlib.Path(section) / self.filename
             if section
             else pathlib.Path(self.filename)
         ).as_posix()
         self.nav: dict[tuple | str | None, mknav.MkNav | mkpage.MkPage] = {}
+        self.index_page: mkpage.MkPage | None = None
+        self.index_title: str | None = None
         # self._mapping = {}
         # self._editor = mkdocs_gen_files.editor.FilesEditor.current()
         # self._docs_dir = pathlib.Path(self._editor.config["docs_dir"])
         # self.files = self._editor.files
 
     def __repr__(self):
         return helpers.get_repr(
@@ -78,15 +80,18 @@
 
     @property
     def pages(self):
         return [node for node in self.nav.values() if isinstance(node, mkpage.MkPage)]
 
     @property
     def children(self):
-        return list(self.nav.values())
+        navs = list(self.nav.values())
+        if self.index_page:
+            navs.append(self.index_page)
+        return navs
 
     @children.setter
     def children(self, items):
         self.nav = dict(items)
 
     def add_nav(self, section: str) -> MkNav:
         """Create a Sub-Nav, register it to given Nav and return it.
@@ -96,65 +101,77 @@
         """
         navi = mknav.MkNav(section=section, parent=self)
         self._register(navi)
         return navi
 
     def add_index_page(
         self,
-        title: str | None = None,
-        *,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
+        title: str,
+        **kwargs,
     ) -> mkpage.MkPage:
         page = mkpage.MkPage(
             path="index.md",
-            hide_toc=hide_toc,
-            hide_nav=hide_nav,
             parent=self,
+            **kwargs,
         )
-        self.nav[title] = page
+        self.index_page = page
+        self.index_title = title
         return page
 
     def virtual_files(self) -> dict[str, str]:
         return {str(self.path): self.to_markdown()}
 
     def to_markdown(self) -> str:
         nav = mkdocs_gen_files.Nav()
+        # In a nav, the first inserted item becomes the index page in case
+        # the section-index plugin is used, so we add it first.
+        if self.index_page and self.index_title:
+            nav[self.index_title] = pathlib.Path(self.index_page.path).as_posix()
         for path, item in self.nav.items():
-            # current approach: index pages have path = None, they dont become part
-            # of the literate nav.
-            # Not sure what`s best here, lot of combinations possible with
-            # section-index etc.
-            if path is None:
+            if path is None:  # this check is just to make mypy happy
                 continue
             match item:
                 case mkpage.MkPage():
                     nav[path] = pathlib.Path(item.path).as_posix()
                 case MkNav():
                     nav[path] = f"{item.section}/"
                 case _:
                     raise TypeError(item)
         return "".join(nav.build_literate_nav())
 
     def add_page(
         self,
-        title: str,
+        name: str,
         *,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
-        hide_path: bool = False,
         filename: str | None = None,
+        hide_toc: bool | None = None,
+        hide_nav: bool | None = None,
+        hide_path: bool | None = None,
+        search_boost: float | None = None,
+        exclude_from_search: bool | None = None,
+        icon: str | None = None,
+        status: Literal["new", "deprecated"] | None = None,
+        title: str | None = None,
+        subtitle: str | None = None,
+        description: str | None = None,
     ) -> mkpage.MkPage:
         """Add a page to the Nav."""
         page = mkpage.MkPage(
-            path=filename or f"{title}.md",
+            path=filename or f"{name}.md",
             parent=self,
             hide_toc=hide_toc,
             hide_nav=hide_nav,
             hide_path=hide_path,
+            search_boost=search_boost,
+            exclude_from_search=exclude_from_search,
+            icon=icon,
+            status=status,
+            title=title,
+            subtitle=subtitle,
+            description=description,
         )
         self._register(page)
         return page
 
     def add_doc(
         self,
         module: types.ModuleType | Sequence[str] | str,
```

### Comparing `mknodes-0.6.0/mknodes/mknode.py` & `mknodes-0.8.3/mknodes/mknode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkpage.py` & `mknodes-0.8.3/mknodes/mkpage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from collections.abc import Mapping
 import logging
 import os
 import types
 
 from typing import Any, Literal
 
+import yaml
+
 from mknodes import (
     mkadmonition,
     mkcode,
     mkcontainer,
     mkdocstrings,
     mklink,
     mknav,
@@ -19,43 +21,64 @@
     mktext,
 )
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
-HEADER = "---\n{options}\n---\n\n"
+HEADER = "---\n{options}---\n\n"
 
 
 class MkPage(mkcontainer.MkContainer):
     """A node container representing a Markdown page.
 
     A page contains a list of other Markdown nodes, has a virtual Markdown file
     associated, and can have metadata (added as header)
     """
 
     def __init__(
         self,
         path: str | os.PathLike = "",
         *,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
-        hide_path: bool = False,
+        hide_toc: bool | None = None,
+        hide_nav: bool | None = None,
+        hide_path: bool | None = None,
+        search_boost: float | None = None,
+        exclude_from_search: bool | None = None,
+        icon: str | None = None,
+        status: Literal["new", "deprecated"] | None = None,
+        title: str | None = None,
+        subtitle: str | None = None,
+        description: str | None = None,
         parent: mknav.MkNav | None = None,
         **kwargs: Any,
     ):
         super().__init__(parent=parent, **kwargs)
         self.path = str(path)
-        self.header_options: dict[str, Any] = {}
-        if hide_toc:
-            self.header_options.setdefault("hide", []).append("toc")
-        if hide_nav:
-            self.header_options.setdefault("hide", []).append("navigation")
-        if hide_path:
-            self.header_options.setdefault("hide", []).append("path")
+        self.metadata: dict[str, Any] = {}
+        if hide_toc is not None:
+            self.metadata.setdefault("hide", []).append("toc")
+        if hide_nav is not None:
+            self.metadata.setdefault("hide", []).append("navigation")
+        if hide_path is not None:
+            self.metadata.setdefault("hide", []).append("path")
+        if search_boost is not None:
+            self.metadata.setdefault("search", {})["boost"] = search_boost
+        if exclude_from_search is not None:
+            self.metadata.setdefault("search", {})["exclude"] = exclude_from_search
+        if icon is not None:
+            self.metadata["icon"] = icon
+        if status is not None:
+            self.metadata["status"] = status
+        if subtitle is not None:
+            self.metadata["subtitle"] = subtitle
+        if title is not None:
+            self.metadata["title"] = title
+        if description is not None:
+            self.metadata["description"] = description
 
     def __repr__(self):
         return helpers.get_repr(self, path=str(self.path))
 
     def __str__(self):
         return self.to_markdown()
 
@@ -65,22 +88,18 @@
     def to_markdown(self) -> str:
         header = self.formatted_header()
         content_str = self._to_markdown()
         return header + content_str if header else content_str
 
     def formatted_header(self) -> str:
         """Return the formatted header (containing metadata) for the page."""
-        lines = []
-        keys = self.header_options.keys()
-        if not keys:
+        if not self.metadata:
             return ""
-        for option in keys:
-            lines.append(f"{option}:")
-            lines.extend(f"  - {area}" for area in self.header_options[option])
-        return HEADER.format(options="\n".join(lines))
+        options = yaml.dump(self.metadata, Dumper=yaml.Dumper, indent=2)
+        return HEADER.format(options=options)
 
     def add_newlines(self, num: int):
         """Add line separators to the page.
 
         Arguments:
             num: Amount of newlines to add.
         """
@@ -93,15 +112,15 @@
     ) -> mklink.MkLink:
         """Add a Link to the page.
 
         Arguments:
             url: URL to link to.
             title: Text to display for the link
         """
-        item = mklink.MkLink(url)
+        item = mklink.MkLink(url, title)
         self.append(item)
         return item
 
     def add_header(self, text: str, level: int = 2) -> mktext.MkText:
         """Add line separators to the page.
 
         Arguments:
@@ -313,12 +332,12 @@
         else:
             tabblock = mktabcontainer.MkTabBlock(data, parent=self, **kwargs)
         self.append(tabblock)
         return tabblock
 
 
 if __name__ == "__main__":
-    doc = MkPage()
+    doc = MkPage(hide_toc=True, search_boost=2)
     doc.add_link("test")
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
     # print(doc.children)
```

### Comparing `mknodes-0.6.0/mknodes/mkpageinclude.py` & `mknodes-0.8.3/mknodes/mkpageinclude.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mkshields.py` & `mknodes-0.8.3/mknodes/mkshields.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mksnippet.py` & `mknodes-0.8.3/mknodes/mksnippet.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     """Snippet to include markdown from another file.
 
     [More info](https://facelessuser.github.io/pymdown-extensions/extensions/snippets/)
     """
 
     REQUIRED_EXTENSIONS = "pymdownx.snippets"
 
-    def __init__(self, path: str | os.PathLike, header: str = ""):
+    def __init__(
+        self,
+        path: str | os.PathLike,
+        *,
+        header: str = "",
+    ):
         super().__init__(header)
         self.path = path
 
     def __str__(self):
         return self.to_markdown()
 
     def __repr__(self):
```

### Comparing `mknodes-0.6.0/mknodes/mksourceandresult.py` & `mknodes-0.8.3/mknodes/mksourceandresult.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mktabcontainer.py` & `mknodes-0.8.3/mknodes/mktabcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 class MkTabContainer(mkcontainer.MkContainer):
     items: list[mktabs.MkTab]
 
     def __init__(
         self,
         tabs: Mapping[str, str | mknode.MkNode] | list[mktabs.MkTab],
+        *,
         header: str = "",
         select_tab: int | str | None = None,
         **kwargs,
     ):
         if isinstance(tabs, list):
             items = tabs
         else:
```

### Comparing `mknodes-0.6.0/mknodes/mktable.py` & `mknodes-0.8.3/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/mktabs.py` & `mknodes-0.8.3/mknodes/mktabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class MkBlockTab(mkblock.MkBlock):
     def __init__(
         self,
         content: str,
         title: str,
+        *,
         new: bool | None = None,
         select: bool | None = None,
     ):
         super().__init__(
             "tab",
             content=content,
             title=title,
```

### Comparing `mknodes-0.6.0/mknodes/mktext.py` & `mknodes-0.8.3/mknodes/mktext.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 
 class MkText(mknode.MkNode):
     """Class for any Markup text.
 
     All classes inheriting from MkNode can get converted to this Type.
     """
 
-    def __init__(self, text: str | mknode.MkNode = "", header: str = "", parent=None):
+    def __init__(
+        self,
+        text: str | mknode.MkNode = "",
+        *,
+        header: str = "",
+        parent=None,
+    ):
         super().__init__(header=header, parent=parent)
         self.text = text
 
     def __repr__(self):
         return helpers.get_repr(self, text=self.text)
 
     def _to_markdown(self) -> str:
```

### Comparing `mknodes-0.6.0/mknodes/node.py` & `mknodes-0.8.3/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.8.3/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.8.3/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/classnodes/mkclasspage.py` & `mknodes-0.8.3/mknodes/classnodes/mkclasspage.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,29 +27,20 @@
     """
 
     def __init__(
         self,
         klass: type,
         *,
         module_path: tuple[str, ...] | str | None = None,
-        hide_toc: bool = False,
-        hide_nav: bool = False,
-        hide_path: bool = False,
         path: str | os.PathLike = "",
         **kwargs: Any,
     ):
         # TODO: should path be settable?
         path = pathlib.Path(f"{klass.__name__}.md")
-        super().__init__(
-            path=path,
-            hide_toc=hide_toc,
-            hide_nav=hide_nav,
-            hide_path=hide_path,
-            **kwargs,
-        )
+        super().__init__(path=path, **kwargs)
         self.klass = klass
         match module_path:
             case None:
                 self.parts = klass.__module__.split(".")
             case _:
                 self.parts = classhelpers.to_module_parts(module_path)
         self._build()
@@ -60,14 +51,15 @@
     @staticmethod
     def examples():
         yield dict(klass=MkClassPage)
 
     def add_class_diagram(
         self,
         mode: mkclassdiagram.DiagramModeStr = "parent_tree",
+        *,
         header: str = "",
     ):
         diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode, header=header)
         self.append(diagram)
         return diagram
 
     def _build(self):
```

### Comparing `mknodes-0.6.0/mknodes/classnodes/mkclasstable.py` & `mknodes-0.8.3/mknodes/classnodes/mkclasstable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/manual/introduce_nodes.py` & `mknodes-0.8.3/mknodes/manual/introduce_nodes.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/manual/page_1.py` & `mknodes-0.8.3/mknodes/manual/page_1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,81 @@
 from __future__ import annotations
 
-import inspect
-
 import mknodes
 
 from mknodes.utils import classhelpers, helpers
 
 
 INTRO_TEXT = """
 Basically everything interesting in this library inherits from MkNode.
 It`s the base class for all tree nodes we are building. The tree goes from the root nav
 down to single markup elements. We can show the subclass tree by using
 the MkClassDiagram Node.
 """
 
 
-def create_page_1(root_nav: mknodes.MkNav):
+def create_nodes_section(root_nav: mknodes.MkNav):
     # Basic structure: Theres one root nav, navs can contain pages and other navs,
     # pages contain more atomic markup nodes, like text, tables, and diagrams.
     # These markup nodes in some cases can contain other Markup nodes.
     # It`s all one big tree.
 
-    home_nav = root_nav.add_nav("User guide")
-    overview = home_nav.add_page("Overview", hide_toc=True)
+    home_nav = root_nav.add_nav("The nodes")
+    overview = home_nav.add_index_page("Overview", hide_toc=True)
 
     # this here is what you are reading right now.
-    overview.add_code(inspect.getsource(create_page_1))
+    overview += mknodes.MkCode.for_object(create_nodes_section)
     nodes_nav = home_nav.add_nav("Nodes")
 
     # for convenience, we can add strings directly to pages.
     # they will get converted to a mknodes.Text node.
     overview += INTRO_TEXT
+    create_subclass_page(home_nav)
 
+    # let`s take a look at some of the mentioned Markup nodes.
+    # Some of them have a `examples` classmethod which yields some example signatures
+    #  to show the functionality.
+    for kls in classhelpers.get_subclasses(mknodes.MkNode):
+        # get_subclasses just calls __subclasses__ recursively.
+        create_page_for_class(nodes_nav, kls)
+
+
+def create_page_for_class(nav: mknodes.MkNav, kls: type):
+    subpage = nav.add_page(kls.__name__)
+    subpage += mknodes.MkCode.for_object(create_page_for_class)
+    if hasattr(kls, "examples"):
+        subpage += mknodes.MkCode.for_object(
+            kls.examples,
+            header="Example signatures",
+        )
+        for i, sig in enumerate(kls.examples(), start=1):
+            subpage.add_header(f"Example {i}", level=2)
+            sig_txt = helpers.format_kwargs(sig)
+            text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
+            subpage.add_code(code=text, title=f"example_{i}.py")
+            node = kls(**sig)
+            subpage += mknodes.MkText(str(node), header="Preview")
+            subpage += mknodes.MkCode(
+                language="md",
+                code=node,
+                title="Resulting markdown",
+            )
+            subpage.add_newlines(3)
+    subpage.add_mkdocstrings(kls)
+
+
+def create_subclass_page(nav: mknodes.MkNav):
     # Lets take a look at the relations of the included nodes.
     # It`s easy to show different diagrams for classes.
-    subcls_page = home_nav.add_page("Subclass tree", hide_toc=True)
+    subcls_page = nav.add_page("Subclass tree", hide_toc=True)
+    subcls_page += mknodes.MkCode.for_object(create_subclass_page)
     subcls_page += mknodes.MkClassDiagram(
         mknodes.MkNode,
         mode="subclass_tree",
         orientation="LR",
     )
-    # let`s take a look at some of the mentioned Markup nodes.
-    # Some of them have a `examples` classmethod which yields some example signatures
-    #  to show the functionality.
-    for kls in classhelpers.get_subclasses(mknodes.MkNode):
-        # get_subclasses just calls __subclasses__ recursively.
-        subpage = nodes_nav.add_page(kls.__name__)
-        if hasattr(kls, "examples"):
-            subpage += mknodes.MkCode.for_object(
-                kls.examples,
-                header="Example signatures",
-            )
-            for i, sig in enumerate(kls.examples(), start=1):
-                subpage.add_header(f"Example {i}", level=2)
-                sig_txt = helpers.format_kwargs(sig)
-                text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
-                subpage.add_code(code=text, title=f"example_{i}.py")
-                node = kls(**sig)
-                subpage += mknodes.MkText(str(node), header="Preview")
-                subpage += mknodes.MkCode(
-                    language="md",
-                    code=node,
-                    title="Resulting markdown",
-                )
-                subpage.add_newlines(3)
-        subpage.add_mkdocstrings(kls)
 
 
 if __name__ == "__main__":
     nav = mknodes.MkNav()
-    create_page_1(nav)
+    create_nodes_section(nav)
     print(nav.children[0])
```

### Comparing `mknodes-0.6.0/mknodes/manual/page_2.py` & `mknodes-0.8.3/mknodes/manual/page_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 from __future__ import annotations
 
-import inspect
-
 import mknodes
 
 
 INTRO_TEXT = """now lets create the documentation.
 This code will show how to build a simple documentation section.
 """
 
 
-def create_page_2(root_nav: mknodes.MkNav):
+def create_documentation_section(root_nav: mknodes.MkNav):
     doc_section = root_nav.add_nav("Documentation")
 
-    overview = doc_section.add_page("Overview", hide_toc=True)
+    overview = doc_section.add_index_page("Overview", hide_toc=True)
     overview += mknodes.MkText(INTRO_TEXT)
-
-    # we are here right now.
-    overview.add_code(inspect.getsource(create_page_2))
+    overview += mknodes.MkCode.for_object(create_documentation_section)
 
     # lets create the complete documentation for our module.
     # Each Documentation section can have global filters for what it should include.
     # In this case, we only want to document stuff which is listed in "__all__".
     mknodes_docs = doc_section.add_doc(module=mknodes, filter_by___all__=True)
 
     # the Documentation Nav hast some helper methods to iterate through the submodules
     # / classes of a module. We can also pass a predicate to filter specific subclasses,
     # or do other fancy stuff to generate a customized, automated documentation.
     # now we add some pre-defined pages ("MkClassPages") to our docs.
     # they contain MkDocStrings, a table for eventual subclasses and an
     # inheritance graph. It`s also possible to build custom pages of course.
     mknodes_docs.collect_classes(recursive=True)
 
-    # Not enough documentation for your taste? Let`s document random stuff.
-    # What about the std library?
-    std_lib_nav = doc_section.add_nav("std_library")
-    for stdlib_mod in ["pathlib", "inspect", "logging"]:
-        docs = std_lib_nav.add_doc(module=stdlib_mod)
-        docs.collect_classes(recursive=True)
+    # There is also an extension available for this module which offers tools and
+    # new nodes based on PySide6 / PyQt6. We can add its documentation easily:
+    # from prettyqt import prettyqtmarkdown
+
+    # addon_docs = doc_section.add_doc(module=prettyqtmarkdown, flatten_nav=True)
+    # addon_docs.collect_classes(recursive=True)
 
     overview.add_admonition(text="That was easy, right?")
 
 
 if __name__ == "__main__":
     nav = mknodes.MkNav()
-    create_page_2(nav)
+    create_documentation_section(nav)
     print(nav.children[0])
```

### Comparing `mknodes-0.6.0/mknodes/manual/page_3.py` & `mknodes-0.8.3/mknodes/manual/page_3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from __future__ import annotations
 
-import inspect
 import pprint
 
 import mknodes
 
 
 INTRO_TEXT = """Lets show some info about the tree we built.
 The tree starts from the root nav down to the Markup elements.
 """
 
 
-def create_page_3(root_nav: mknodes.MkNav):
+def create_internals_section(root_nav: mknodes.MkNav):
     internals_nav = root_nav.add_nav("Internals")
 
-    overview = internals_nav.add_page("Overview", hide_toc=True)
+    overview = internals_nav.add_index_page("Overview", hide_toc=True)
     overview += INTRO_TEXT
-
-    # we are here right now.
-    overview.add_code(inspect.getsource(create_page_3))
+    overview += mknodes.MkCode.for_object(create_internals_section)
 
     # the "Tree" section in the left sidebar shows what we have done up to now.
     # we create a new page and add a formatted represenation of our Tree.
 
     tree_page = internals_nav.add_page("Tree", hide_toc=True)
     tree_page.add_header("This is the tree we built up to now.", level=3)
     lines = [f"{level * '    '} {node!r}" for level, node in root_nav.iter_nodes()]
@@ -36,9 +33,9 @@
     file_txt = pprint.pformat(list(virtual_files.keys()))
     files_page += mknodes.MkCode(file_txt)
     # print(nodes_nav.to_tree_graph())
 
 
 if __name__ == "__main__":
     nav = mknodes.MkNav()
-    create_page_3(nav)
+    create_internals_section(nav)
     print(nav.children[0])
```

### Comparing `mknodes-0.6.0/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.8.3/mknodes/modulenodes/mkmodulepage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.8.3/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/resources/codeofconduct.md` & `mknodes-0.8.3/mknodes/resources/codeofconduct.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/classhelpers.py` & `mknodes-0.8.3/mknodes/utils/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/connectionbuilder.py` & `mknodes-0.8.3/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/debugging.py` & `mknodes-0.8.3/mknodes/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/helpers.py` & `mknodes-0.8.3/mknodes/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/inventorymanager.py` & `mknodes-0.8.3/mknodes/utils/inventorymanager.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/linkprovider.py` & `mknodes-0.8.3/mknodes/utils/linkprovider.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/mermaid.py` & `mknodes-0.8.3/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/noderesolver.py` & `mknodes-0.8.3/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/mknodes/utils/packageinfo.py` & `mknodes-0.8.3/mknodes/utils/packageinfo.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/tests/test_annotations.py` & `mknodes-0.8.3/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/tests/test_nav.py` & `mknodes-0.8.3/tests/test_nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 TREE_TOTAL = TREE_NUM_PAGES + TREE_NUM_NAVS + TREE_NUM_TEXT
 
 
 def test_nav():
     nav = mknodes.MkNav()
     nav.add_doc(mknodes)
     nav.add_page("Test")
-    nav.add_index_page()
+    nav.add_index_page("Test Index page")
     nav.add_nav("sub")
 
 
 def test_from_file(test_data_dir):
     nav = mknodes.MkNav.from_folder(test_data_dir / "nav_tree")
     assert len(list(nav.descendants)) == TREE_TOTAL - 1
```

### Comparing `mknodes-0.6.0/tests/data/nav_tree/test_file.md` & `mknodes-0.8.3/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/.gitignore` & `mknodes-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/LICENSE` & `mknodes-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/README.md` & `mknodes-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.6.0/pyproject.toml` & `mknodes-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,29 @@
     "mkdocs-section-index",
     "mkdocs-gen-files",
     # "mkdocs-macros-plugin",
     "markdown-exec[ansi]",
     "mkdocs-coverage",
     "pygments",
     "typing_extensions",
+    # "prettyqt",
+    # "PySide6",
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest"
 test-cov-xml = "pytest --cov-report=xml"
+test-cov-html = "pytest --cov-report=html"
 lint = [
-  "black .",
+  "black . --preview",
   "ruff --fix .",
   "mypy mknodes/",
 ]
 lint-check = [
-  "black --check .",
+  "black --check . --preview",
   "ruff .",
   "mypy mknodes/",
 ]
 docs-serve = "hatch run mkdocs serve"
 docs-build = "hatch run mkdocs build"
 
 [build-system]
```

### Comparing `mknodes-0.6.0/PKG-INFO` & `mknodes-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.6.0
+Version: 0.8.3
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: docs,docstrings,documentation,framework,internet,markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.6.0 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.8.3 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

