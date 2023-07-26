# Comparing `tmp/mknodes-0.4.2.tar.gz` & `tmp/mknodes-0.5.0.tar.gz`

## Comparing `mknodes-0.4.2.tar` & `mknodes-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,86 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.2/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.2/Makefile
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.4.2/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.2/docs/gen_pages.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.2/docs/gen_qt.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkadmonition.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkimage.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkinstallguide.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mklink.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mklist.py
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mknode.py
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkpage.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/helpers.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/linkprovider.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_admonition.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_image.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_list.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_modulepage.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_nav.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.2/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.2/README.md
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.5.0/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.5.0/Makefile
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.5.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.5.0/docs/gen_pages.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.5.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkannotations.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkimage.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mklink.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mklist.py
+-rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mknode.py
+-rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.5.0/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_admonition.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_annotations.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_image.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_linkreplacer.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_modulepage.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_nav.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.5.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.5.0/README.md
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.5.0/PKG-INFO
```

### Comparing `mknodes-0.4.2/.pre-commit-config.yaml` & `mknodes-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/Makefile` & `mknodes-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mkdocs.yml` & `mknodes-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/.github/workflows/build.yml` & `mknodes-0.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/.github/workflows/documentation.yml` & `mknodes-0.5.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/docs/gen_pages.py` & `mknodes-0.5.0/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/docs/gen_qt.py` & `mknodes-0.5.0/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/__init__.py` & `mknodes-0.5.0/mknodes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .mkbinaryimage import MkBinaryImage
 from .mklist import MkList
 from .mkdiagram import MkDiagram
 from .mktable import MkTable
 from .mktabcontainer import MkTabBlock, MkTabbed
 from .mksnippet import MkSnippet
 from .mkcritic import MkCritic
+from .mkannotations import MkAnnotations
 from .mksourceandresult import MkSourceAndResult
 from .mkshields import MkShields
 from .mkpage import MkPage
 from .mkpageinclude import MkPageInclude
 from .mkinstallguide import MkInstallGuide
 
 from .classnodes.mkclassdiagram import MkClassDiagram
@@ -50,19 +51,20 @@
     "ConnectionBuilder",
     "MkTable",
     "MkClassTable",
     "MkList",
     "MkClassPage",
     "MkModulePage",
     "MkModuleTable",
+    "MkAnnotations",
     "MkDoc",
     "MkTabBlock",
     "MkTabbed",
     "MkSourceAndResult",
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
     "MkInstallGuide",
 ]
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
```

### Comparing `mknodes-0.4.2/mknodes/mkadmonition.py` & `mknodes-0.5.0/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkbinaryimage.py` & `mknodes-0.5.0/mknodes/mkbinaryimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class MkBinaryImage(mkimage.MkImage):
     """Binary data of an image which will become a file when the tree is written."""
 
     def __init__(
         self,
-        data: bytes,
+        data: bytes | str,
         path: str,
         *,
         caption: str = "",
         title: str = "Image title",
         header: str = "",
     ):
         super().__init__(path=path, header=header, caption=caption, title=title)
```

### Comparing `mknodes-0.4.2/mknodes/mkblock.py` & `mknodes-0.5.0/mknodes/mkblock.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkcode.py` & `mknodes-0.5.0/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkcontainer.py` & `mknodes-0.5.0/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkcritic.py` & `mknodes-0.5.0/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkdiagram.py` & `mknodes-0.5.0/mknodes/mkdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkdoc.py` & `mknodes-0.5.0/mknodes/mkdoc.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkdocstrings.py` & `mknodes-0.5.0/mknodes/mkdocstrings.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkimage.py` & `mknodes-0.5.0/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkinstallguide.py` & `mknodes-0.5.0/mknodes/mkinstallguide.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mklink.py` & `mknodes-0.5.0/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mklist.py` & `mknodes-0.5.0/mknodes/mklist.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 
 class MkList(mkcontainer.MkContainer):
-    """Class to show a formatted list."""
+    """Node for showing a formatted list."""
 
     def __init__(
         self,
         items: list[str | mknode.MkNode] | None = None,
         *,
         ordered: bool = False,
         shorten_after: int | None = None,
```

### Comparing `mknodes-0.4.2/mknodes/mknav.py` & `mknodes-0.5.0/mknodes/mknav.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,15 @@
         nav = cls(folder.name if parent else None, parent=parent)
         for path in folder.iterdir():
             if path.is_dir():
                 subnav = cls.from_folder(folder / path.parts[-1], parent=nav)
                 nav._register(subnav)
             elif path.suffix == ".md" and path.name != "SUMMARY.md":
                 page = mkpage.MkPage(path.relative_to(folder))
-                text = path.read_text()
-                page += text
+                page += path.read_text()
                 nav._register(page)
         return nav
 
 
 if __name__ == "__main__":
     docs = MkNav()
     nav_tree_path = pathlib.Path(__file__).parent.parent / "tests/data/nav_tree/"
```

### Comparing `mknodes-0.4.2/mknodes/mknode.py` & `mknodes-0.5.0/mknodes/mknode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mkpage.py` & `mknodes-0.5.0/mknodes/mkpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     mkcode,
     mkcontainer,
     mkdocstrings,
     mklink,
     mknav,
     mknode,
     mktabcontainer,
+    mktext,
 )
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 HEADER = "---\n{options}\n---\n\n"
@@ -96,23 +97,25 @@
             url: URL to link to.
             title: Text to display for the link
         """
         item = mklink.MkLink(url)
         self.append(item)
         return item
 
-    def add_header(self, text: str, level: int = 2):
+    def add_header(self, text: str, level: int = 2) -> mktext.MkText:
         """Add line separators to the page.
 
         Arguments:
             text: header text
             level: header level
         """
         prefix = "#" * level
-        self.append(f"{prefix} {text}")
+        node = mktext.MkText(f"{prefix} {text}")
+        self.append(node)
+        return node
 
     def add_admonition(
         self,
         text: str,
         typ: mkadmonition.AdmonitionTypeStr = "info",
         *,
         title: str | None = None,
```

### Comparing `mknodes-0.4.2/mknodes/mkpageinclude.py` & `mknodes-0.5.0/mknodes/mkpageinclude.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 logger = logging.getLogger(__name__)
 
 CriticMarkStr = Literal["addition", "deletion", "substitution", "comment", "highlight"]
 
 
 class MkPageInclude(mknode.MkNode):
-    """MkCritic block."""
+    """Node to include other MkPages / Md files."""
 
     def __init__(
         self,
         page: str | os.PathLike | mkpage.MkPage,
         **kwargs,
     ):
         super().__init__(**kwargs)
```

### Comparing `mknodes-0.4.2/mknodes/mkshields.py` & `mknodes-0.5.0/mknodes/mkshields.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mksnippet.py` & `mknodes-0.5.0/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mksourceandresult.py` & `mknodes-0.5.0/mknodes/mksourceandresult.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 
 class MkSourceAndResult(mknode.MkNode):
-    """Class to show the source of a Callable combined with its stringified result."""
+    """Node for showing the source of a Callable combined with its stringified result."""
 
     def __init__(
         self,
         fn: Callable,
         header: str = "",
     ):
         super().__init__(header)
```

### Comparing `mknodes-0.4.2/mknodes/mktabcontainer.py` & `mknodes-0.5.0/mknodes/mktabcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mktable.py` & `mknodes-0.5.0/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mktabs.py` & `mknodes-0.5.0/mknodes/mktabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/mktext.py` & `mknodes-0.5.0/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/node.py` & `mknodes-0.5.0/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.5.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.5.0/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/classnodes/mkclasspage.py` & `mknodes-0.5.0/mknodes/classnodes/mkclasspage.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import os
 import pathlib
 
 from typing import Any
 
-from mknodes import mkdocstrings, mkpage
+from mknodes import mkpage
 from mknodes.classnodes import mkclassdiagram, mkclasstable
 from mknodes.utils import classhelpers, helpers
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -57,28 +57,39 @@
     def __repr__(self):
         return helpers.get_repr(self, klass=self.klass, path=str(self.path))
 
     @staticmethod
     def examples():
         yield dict(klass=MkClassPage)
 
-    def add_class_diagram(self, mode: mkclassdiagram.DiagramModeStr = "parent_tree"):
-        diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode)
+    def add_class_diagram(
+        self,
+        mode: mkclassdiagram.DiagramModeStr = "parent_tree",
+        header: str = "",
+    ):
+        diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode, header=header)
         self.append(diagram)
         return diagram
 
     def _build(self):
+        if len(self.klass.mro()) > 2:  # noqa: PLR2004
+            bases = list(self.klass.__bases__)
+            table = mkclasstable.MkClassTable(bases, header="Base classes")
+            self.append(table)
+        if len(subklasses := self.klass.__subclasses__()) > 0:
+            table = mkclasstable.MkClassTable(
+                subklasses,
+                header="Subclasses",
+                layout="compact",
+            )
+            self.append(table)
+        self.add_class_diagram(header="⋔ Inheritance diagram")
         module_path = ".".join(self.parts).rstrip(".")
         path = f"{module_path}.{self.klass.__name__}"
-        item = mkdocstrings.MkDocStrings(path, header="⁇ DocStrings")
-        self.append(item)
-        if tbl := mkclasstable.MkClassTable(list(self.klass.__bases__)):
-            self.append(tbl)
-        item = mkclassdiagram.MkClassDiagram(self.klass, header="⋔ Inheritance diagram")
-        self.append(item)
+        self.add_mkdocstrings(path, header="🛈 DocStrings", show_root_toc_entry=False)
 
 
 if __name__ == "__main__":
     doc = MkClassPage(MkClassPage)
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
     # print(doc.children)
```

### Comparing `mknodes-0.4.2/mknodes/classnodes/mkclasstable.py` & `mknodes-0.5.0/mknodes/classnodes/mkclasstable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/manual/page_1.py` & `mknodes-0.5.0/mknodes/manual/page_1.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/manual/page_2.py` & `mknodes-0.5.0/mknodes/manual/page_2.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/manual/page_3.py` & `mknodes-0.5.0/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.5.0/mknodes/modulenodes/mkmodulepage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.5.0/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/classhelpers.py` & `mknodes-0.5.0/mknodes/utils/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/connectionbuilder.py` & `mknodes-0.5.0/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/helpers.py` & `mknodes-0.5.0/mknodes/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/inventorymanager.py` & `mknodes-0.5.0/mknodes/utils/inventorymanager.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/linkprovider.py` & `mknodes-0.5.0/mknodes/utils/linkprovider.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/mermaid.py` & `mknodes-0.5.0/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/mknodes/utils/noderesolver.py` & `mknodes-0.5.0/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/tests/test_nav.py` & `mknodes-0.5.0/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/tests/data/nav_tree/test_file.md` & `mknodes-0.5.0/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/.gitignore` & `mknodes-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/LICENSE` & `mknodes-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/README.md` & `mknodes-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/pyproject.toml` & `mknodes-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.2/PKG-INFO` & `mknodes-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.4.2
+Version: 0.5.0
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
-Metadata-Version: 2.1 Name: mknodes Version: 0.4.2 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.5.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

