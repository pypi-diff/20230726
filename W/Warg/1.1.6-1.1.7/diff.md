# Comparing `tmp/Warg-1.1.6.tar.gz` & `tmp/Warg-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.1.6.tar", last modified: Wed Jun 21 08:55:19 2023, max compression
+gzip compressed data, was "Warg-1.1.7.tar", last modified: Wed Jul 26 11:18:12 2023, max compression
```

## Comparing `Warg-1.1.6.tar` & `Warg-1.1.7.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:55:07.000000 Warg-1.1.6/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-21 08:55:07.000000 Warg-1.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 08:55:07.000000 Warg-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-21 08:55:19.820976 Warg-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-21 08:55:07.000000 Warg-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 08:55:07.000000 Warg-1.1.6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:55:07.000000 Warg-1.1.6/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-21 08:55:07.000000 Warg-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 08:55:07.000000 Warg-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 08:55:19.820976 Warg-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-21 08:55:07.000000 Warg-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.808975 Warg-1.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/platform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.133507 Warg-1.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:18:05.000000 Warg-1.1.7/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 11:18:05.000000 Warg-1.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-26 11:18:05.000000 Warg-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-26 11:18:12.149507 Warg-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 11:18:05.000000 Warg-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-26 11:18:05.000000 Warg-1.1.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.133507 Warg-1.1.7/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.137507 Warg-1.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:18:05.000000 Warg-1.1.7/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 11:18:05.000000 Warg-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 11:18:05.000000 Warg-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-26 11:18:12.149507 Warg-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-26 11:18:05.000000 Warg-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.137507 Warg-1.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/platform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/typing_extension.py
```

### Comparing `Warg-1.1.6/.github/CODE_OF_CONDUCT.md` & `Warg-1.1.7/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/LICENSE.md` & `Warg-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/PKG-INFO` & `Warg-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.6
+Version: 1.1.7
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,17 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: docs
 Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
```

### Comparing `Warg-1.1.6/README.md` & `Warg-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/SECURITY.md` & `Warg-1.1.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/Warg.egg-info/PKG-INFO` & `Warg-1.1.7/Warg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.6
+Version: 1.1.7
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,17 +19,17 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: docs
 Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
```

### Comparing `Warg-1.1.6/Warg.egg-info/SOURCES.txt` & `Warg-1.1.7/Warg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 warg/decorators/caching/look_up_table.py
 warg/decorators/caching/property_caching.py
 warg/generators/README.md
 warg/generators/__init__.py
 warg/generators/cyclic_generators.py
 warg/generators/filtering.py
 warg/generators/mapping_generator.py
+warg/generators/numbers.py
 warg/generators/zipping_generator.py
 warg/math_utilities/README.md
 warg/math_utilities/__init__.py
 warg/math_utilities/multiples.py
 warg/math_utilities/ordinals.py
 warg/math_utilities/powers.py
 warg/metas/README.md
```

### Comparing `Warg-1.1.6/Warg.egg-info/requires.txt` & `Warg-1.1.7/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 setuptools>=60.9.3
 
 [all]
 apppath
-warg
-tox
-sphinxcontrib-programoutput
 setuptools>=60.9.3
-wheel>=0.33.0
-black>=18.9b0
-sphinx
-pip>=19.0.3
 pytest-runner
+tox
+black>=18.9b0
+sphinxcontrib-programoutput
 twine>=1.13.0
-coveralls>=1.6.0
 pytest-cov>=2.6.1
+sphinx
+wheel>=0.33.0
+coveralls>=1.6.0
+pip>=19.0.3
+warg
 pytest>=4.3.0
 
 [dev]
 apppath
-tox
-warg
-sphinxcontrib-programoutput
 setuptools>=60.9.3
-wheel>=0.33.0
-black>=18.9b0
-sphinx
-pip>=19.0.3
 pytest-runner
+tox
+black>=18.9b0
+sphinxcontrib-programoutput
 twine>=1.13.0
-coveralls>=1.6.0
 pytest-cov>=2.6.1
+sphinx
+wheel>=0.33.0
+coveralls>=1.6.0
+pip>=19.0.3
+warg
 pytest>=4.3.0
 
 [docs]
 apppath
-warg
 sphinxcontrib-programoutput
 sphinx
+warg
 
 [setup]
 pytest-runner
 
 [tests]
 tox
 pytest-cov>=2.6.1
```

### Comparing `Warg-1.1.6/pyproject.toml` & `Warg-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/setup.py` & `Warg-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_arguments.py` & `Warg-1.1.7/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_ast_ops.py` & `Warg-1.1.7/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_auto_dict.py` & `Warg-1.1.7/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_collective.py` & `Warg-1.1.7/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_gdkc.py` & `Warg-1.1.7/tests/test_gdkc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any, Any
 
 import pytest
 
 from warg.gdkc import GeneralisedDelayedKwargConstruction
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
@@ -13,31 +13,31 @@
             kwargs until actual call.
            """
 
 
 class A:
     """description"""
 
-    def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+    def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         self.args_a = args
         self.kwargs_a = kwargs
 
     def something(self):
         """description"""
         print(self.kwargs_a)
 
     def something_else(self, *args: Sequence):
         """description"""
         print(args, self.kwargs_a)
 
-    def another(self, *args: Sequence, **kwargs: MutableMapping):
+    def another(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         print(args, self.kwargs_a, kwargs)
 
-    def clearly_something(self, *args: Sequence, **kwargs: MutableMapping):
+    def clearly_something(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         print(self.args_a, args, self.kwargs_a, kwargs)
 
 
 def test_not_both():
     try:
         GeneralisedDelayedKwargConstruction(A, [1], a=2)
```

### Comparing `Warg-1.1.6/tests/test_imports.py` & `Warg-1.1.7/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_kw_passing.py` & `Warg-1.1.7/tests/test_kw_passing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import inspect
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 from warg.decorators.kw_passing import (
     drop_unused_kws,
     passes_kws_to,
     super_init_pass_on_kws,
 )
 
@@ -321,15 +321,15 @@
 
     def l(im_here=None, **kwargs: MutableMapping):
         """description"""
         pass
 
     @passes_kws_to(b)
     @passes_kws_to(l)
-    def a(e, *args: Sequence, **kwargs: MutableMapping):
+    def a(e, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         b(1, 2, **kwargs)
         l(**kwargs)
 
     print(inspect.signature(a))
     a(1, d=None, im_here=2)
 
@@ -341,15 +341,15 @@
 
     def l(im_here=None, **kwargs: MutableMapping):
         """description"""
         pass
 
     @passes_kws_to(b, keep_from_var_kw=True)
     @passes_kws_to(l, keep_from_var_kw=True)
-    def a(e, *args: Sequence, **kwargs: MutableMapping):
+    def a(e, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         b(1, 2, **kwargs)
         l(**kwargs)
 
     print(inspect.signature(a))
     a(1, d=None, im_here=2)
 
@@ -366,28 +366,28 @@
         :param im_here: Nice to meet you
         :param kwargs:
         :return:"""
         pass
 
     @passes_kws_to(b)
     @passes_kws_to(l)
-    def a1(e: int, *args: Sequence, **kwargs: MutableMapping):
+    def a1(e: int, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """
 
         :param e:
         :param args:
         :param kwargs:
         :return:"""
         b(1, 2, **kwargs)
         l(1, **kwargs)
 
     print("a1", inspect.signature(a1))
 
     @passes_kws_to(b, l)
-    def a(e: int, *args: Sequence, **kwargs: MutableMapping):
+    def a(e: int, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         pass
         b(1, 2, **kwargs)
         l(1, **kwargs)
 
     print(inspect.signature(a))
     a(1, d=None, im_here=None)
@@ -405,29 +405,29 @@
         :param im_here: Nice to meet you
         :param kwargs:
         :return:"""
         pass
 
     @passes_kws_to(b)
     @passes_kws_to(l)
-    def a1(e: int, *args: Sequence, **kwargs: MutableMapping):
+    def a1(e: int, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """
 
         :param e:
         :param args:
         :param kwargs:
         :return:"""
         b(1, 2, **kwargs)
         l(1, **kwargs)
 
     print("a1", inspect.signature(a1))
 
     @drop_unused_kws
     @passes_kws_to(b, l)
-    def a(e: int, *args: Sequence, **kwargs: MutableMapping):
+    def a(e: int, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """description"""
         pass
         b(1, 2, **kwargs)
         l(1, **kwargs)
 
     print(inspect.signature(a))
     a(1, d=None, im_here=None)
```

### Comparing `Warg-1.1.6/tests/test_nod.py` & `Warg-1.1.7/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/tests/test_post_init.py` & `Warg-1.1.7/tests/test_post_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any
 
 from warg import drop_unused_kws
 from warg.metas.post_init import PostInit
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
            """
@@ -12,21 +12,21 @@
 
 def test_post_init_class():
     class MyTestingClass(metaclass=PostInit):
         """
         class with the metaclass passed as an argument"""
 
         @drop_unused_kws
-        def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             print(kwargs)
 
-        def __post_init__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __post_init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             print(args, kwargs)
 
-        def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             print("a")
 
     a = MyTestingClass("asdc", kas=2)
 
     a()
 
 
@@ -39,15 +39,15 @@
         def __init__(self, *args: Sequence):
             print("Init class")
 
         @drop_unused_kws
         def __post_init__(self, *args: Sequence):
             print(args)
 
-        def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             print("a")
 
     a = MyTestingClass("asdc", kas=2)
 
     a()
 
 
@@ -55,13 +55,13 @@
     class MyTestingClass(metaclass=PostInit):
         """
         class with the metaclass passed as an argument"""
 
         def __init__(self):
             print("Init class")
 
-        def __call__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __call__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             print("a")
 
     a = MyTestingClass()
 
     a()
```

### Comparing `Warg-1.1.6/tests/test_singleton.py` & `Warg-1.1.7/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/__init__.py` & `Warg-1.1.7/warg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from warnings import warn
 
 import pkg_resources
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
```

### Comparing `Warg-1.1.6/warg/arguments.py` & `Warg-1.1.7/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/ast_ops/arg_indentifier.py` & `Warg-1.1.7/warg/ast_ops/arg_indentifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
            Created on 26-01-2021
            """
 
 __all__ = ["ArgIdentifier", "get_arg_names", "cprinta", "cprintz"]
 
 import ast
-from typing import Optional, Any
+from typing import Optional, Any, Callable
 
 
 class ArgIdentifier(ast.NodeVisitor):
     """description"""
 
     def __init__(
         self,
@@ -125,30 +125,30 @@
     :return:
     :rtype:
     """
     pass  # TODO: For e.g. description in progress_bar(range(_name_,_name2_))
     raise NotImplementedError
 
 
-def cprinta(*v: Any, writer: callable = print, deliminator: str = ":") -> None:
+def cprinta(*v: Any, writer: Callable = print, deliminator: str = ":") -> None:
     """
 
     :param v:
     :type v:
     :param writer:
     :type writer:
     :param deliminator:
     :type deliminator:
     """
     if isinstance(v, str) and v.strip() == "":
         v = '""'
     writer(f"{get_arg_names('cprinta')}{deliminator}", v)
 
 
-def cprintz(*v: Any, writer: callable = print) -> None:
+def cprintz(*v: Any, writer: Callable = print) -> None:
     """
 
     :param v:
     :type v:
     :param writer:
     :type writer:
     """
```

### Comparing `Warg-1.1.6/warg/ast_ops/first_arg_identifier.py` & `Warg-1.1.7/warg/ast_ops/first_arg_identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
            Created on 26-01-2021
            """
 
 __all__ = ["FirstArgIdentifier", "get_first_arg_name", "cprint"]
 
 import ast
-from typing import Optional, Any
+from typing import Optional, Any, Callable
 
 
 def recurse_first_args(args):
     """
 
     :param args:
     :type args:
@@ -155,15 +155,15 @@
     :return:
     :rtype:
     """
     pass  # TODO: For e.g. description in progress_bar(range(_name_))
     raise NotImplementedError
 
 
-def cprint(v: Any, writer: callable = print, deliminator: str = ":") -> None:
+def cprint(v: Any, writer: Callable = print, deliminator: str = ":") -> None:
     """
 
     :param v:
     :type v:
     :param writer:
     :type writer:
     :param deliminator:
```

### Comparing `Warg-1.1.6/warg/bases/property_settings.py` & `Warg-1.1.7/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/boolean_tests.py` & `Warg-1.1.7/warg/boolean_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     "is_none_or_zero_or_negative_or_mod_zero",
     "xor",
     "xnor",
     "nand",
 ]
 
 import math
-from typing import Any, Optional
+from typing import Any, Optional, Callable
 
 from warg import Number
 from warg.decorators import drop_unused_kws, passes_kws_to
 
 
 @drop_unused_kws
 def is_positive_and_mod_zero(
     mod: Optional[Number],
     counter: int,
     *,
     ret: Any = True,
     alt: Any = False,
-    residual_printer: callable = None,
+    residual_printer: Callable = None,
 ) -> Any:
     """
 
     test if mod is positive
     then test if counter % mod is 0
     if both tests are true return ret
     else return alt
@@ -66,15 +66,15 @@
 def is_zero_or_mod_below(
     mod: Optional[Number],
     below: Number,
     counter: int,
     *,
     ret: Any = True,
     alt: Any = False,
-    residual_printer: callable = None,
+    residual_printer: Callable = None,
 ) -> Any:
     """
 
     test if mod is zero or if counter % mod is 0
     if any of the tests are true return ret
     else return alt
 
@@ -103,15 +103,15 @@
 @drop_unused_kws
 def is_zero_or_mod_zero(
     mod: Optional[Number],
     counter: int,
     *,
     ret: Any = True,
     alt: Any = False,
-    residual_printer: callable = None,
+    residual_printer: Callable = None,
 ) -> Any:
     """
 
     test if mod is zero or if counter % mod is 0
     if any of the tests are true return ret
     else return alt
 
@@ -133,15 +133,15 @@
     if residual_printer is not None:
         residual_printer(m)
 
     return ret if (m == 0) else alt
 
 
 @drop_unused_kws
-def is_none_or_zero_or_negative(obj: Optional[Number], residual_printer: callable = None) -> bool:
+def is_none_or_zero_or_negative(obj: Optional[Number], residual_printer: Callable = None) -> bool:
     """
 
     :param residual_printer:
     :type residual_printer:
     :param obj:
     :return:"""
     is_none = obj is None
```

### Comparing `Warg-1.1.6/warg/business.py` & `Warg-1.1.7/warg/business.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 17/03/2020
            """
 
 from itertools import cycle
-from typing import Iterable
+from typing import Iterable, Callable
 
 
 def busy_indicator(
     *,
-    stream: callable = print,
+    stream: Callable = print,
     indicator_interval: int = 1,
     phases: Iterable[str] = ("◑", "◒", "◐", "◓"),
-) -> Iterable:
+) -> int:
     """
     You can choose arbitrary phases like ['|','/','-','\\']
 
     :param stream:
     :type stream:
     :param indicator_interval:
     :type indicator_interval:
@@ -36,15 +36,15 @@
             stream(f"{next(phases)}", end="\r", flush=True)
         yield i
         i += 1
 
 
 if __name__ == "__main__":
 
-    def iasd():
+    def iasd() -> None:
         """description"""
         import time
 
         for i in busy_indicator(indicator_interval=10):
             time.sleep(0.1)
             if i > 100:
                 break
```

### Comparing `Warg-1.1.6/warg/colors/color_conversion.py` & `Warg-1.1.7/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/colors/css_colors.py` & `Warg-1.1.7/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/colors/label_colors.py` & `Warg-1.1.7/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/config_shell.py` & `Warg-1.1.7/warg/config_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
            Created on 17/03/2020
            """
 __all__ = ["PlaybackShell", "ConfigShell"]
 
 import cmd
 from pathlib import Path
-from typing import MutableMapping, Optional
+from typing import MutableMapping, Optional, Callable
 
 from warg import passes_kws_to, PropertySettings
 
 
 class PlaybackShell(cmd.Cmd):
     """description"""
 
@@ -115,16 +115,16 @@
                     deleter = None
                 self.add_option(p, getter=getter, setter=setter, deleter=deleter)
 
     def add_option(
         self,
         key: str,
         *,
-        getter: callable,
-        setter: callable,
+        getter: Callable,
+        setter: Callable,
         deleter: Optional[callable] = None,
     ) -> None:
         """
 
         :param key:
         :type key:
         :param getter:
@@ -135,15 +135,15 @@
         :type deleter:
         """
         self.add_func(f"get_{key}", getter)
         self.add_func(f"set_{key}", setter)
         if deleter:
             self.add_func(f"del_{key}", deleter)
 
-    def add_func(self, key: str, func: callable) -> None:
+    def add_func(self, key: str, func: Callable) -> None:
         """
 
         :param key:
         :type key:
         :param func:
         :type func:
         """
```

### Comparing `Warg-1.1.6/warg/context_wrapper.py` & `Warg-1.1.7/warg/context_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
            Created on 01/07/2020
            """
 
 __all__ = ["ContextWrapper", "NopContext"]
 
 import contextlib
 import inspect
-from typing import Callable, Sequence
+from typing import Callable, Sequence, Mapping, Optional
 
 
 class NopContext(contextlib.AbstractContextManager):
     def __enter__(self):
         return
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -26,18 +26,18 @@
     """
     Allows for conditional application of contexts, if uninstantiated context manager classes are passed no arguments is supplied in construction.
     if disabled None is returned
     if enabled return of context manager is propagated"""
 
     def __init__(
         self,
-        context_manager: callable,
+        context_manager: Callable,
         enabled: bool,
         construction_args: Sequence = (),
-        construction_kwargs=None,
+        construction_kwargs: Optional[Mapping] = None,
     ):
         if construction_kwargs is None:
             construction_kwargs = {}
 
         self._context_manager = context_manager
         self._enabled = enabled
         self._construction_args = construction_args
```

### Comparing `Warg-1.1.6/warg/contexts.py` & `Warg-1.1.7/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/data_structures/auto_dict.py` & `Warg-1.1.7/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/data_structures/mappings.py` & `Warg-1.1.7/warg/data_structures/mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping, Iterable, Hashable, Dict
+from typing import Mapping, Iterable, Hashable, Dict, Callable
 
 __all__ = [
     "invert_mapping",
     "invert_dict",
     "AppendingDict",
     "pivot_dict_object",
     "pivot_dict",
@@ -31,15 +31,15 @@
         # append_to_dict(self, key, value)
         if key in self:
             self[key].append(value)
         else:
             super().__setitem__(key, [value])
 
 
-def recurse_mapping(a: Mapping, call: callable = print) -> None:
+def recurse_mapping(a: Mapping, call: Callable = print) -> None:
     for k, v in a.items():
         if isinstance(v, Mapping):
             recurse_mapping(v)
         call(v)
 
 
 def invert_mapping(m: Mapping) -> Mapping:
```

### Comparing `Warg-1.1.6/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.1.7/warg/data_structures/named_ordered_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,18 +221,18 @@
 
 :rtype: object
 """
 nod = NamedOrderedDictionary()
 
 for arg, value in zip(frame_info.call.args[-len(args) :], args):
 try:
-  arg_key = node_name(arg)
-  nod[arg_key] = value
+arg_key = node_name(arg)
+nod[arg_key] = value
 except TypeError:
-  nod.add_unnamed_arg(value)
+nod.add_unnamed_arg(value)
 
 nod.update(kwargs)
 
 return nod
 '''
 
     def __getattr__(self, item: Any) -> Any:
```

### Comparing `Warg-1.1.6/warg/data_structures/ordered_set.py` & `Warg-1.1.7/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/data_structures/sequences.py` & `Warg-1.1.7/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/datetimes.py` & `Warg-1.1.7/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/debug.py` & `Warg-1.1.7/warg/debug.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 __doc__ = r"""
 
            Created on 09/03/2020
            """
 
 __all__ = ["evaluate_context"]
 
-from typing import Any, Callable, MutableMapping, Tuple, Sequence
+from typing import Any, Callable, MutableMapping, Tuple, Sequence, List, Dict
 
 
-def evaluate_context(x: Any, *args: Sequence, **kwargs: MutableMapping) -> Tuple:
+def evaluate_context(
+    x: Any, *args: Any, **kwargs: MutableMapping[str, Any]
+) -> Tuple[List, Dict, object, type]:
     """
 
-    :rtype: Tuple
+    :rtype: Tuple[List,Dict,object,type]
     :param x:
     :param args:
     :param kwargs:
     :return:"""
     if isinstance(x, Callable):
         x = x(*args, **kwargs)
     return (
```

### Comparing `Warg-1.1.6/warg/decorators/caching/look_up_table.py` & `Warg-1.1.7/warg/decorators/caching/look_up_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 __doc__ = r"""
           Automatically generates a look up data
 
            Created on 06/03/2020
            """
 
 from time import sleep, time
-from typing import Iterable, Mapping, Set, Tuple, Sequence, MutableMapping, Any
+from typing import Iterable, Mapping, Set, Tuple, Sequence, MutableMapping, Any, Callable
 
 from warg.decorators.hashing import make_hash
 
 global_table = {}
 
 __all__ = ["add_lut", "look_up", "look_up_args", "look_up_kws"]
 
 
-def add_lut(f: callable) -> callable:
+def add_lut(f: Callable) -> callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
     global_table[f] = {}
     return f
 
 
-def look_up(f: callable, *args: Sequence, **kwargs: MutableMapping) -> Any:
+def look_up(f: Callable, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]) -> Any:
     """
 
     :param f:
     :type f:
     :param args:
     :type args:
     :param kwargs:
@@ -49,15 +49,15 @@
         return res
 
     global_table[f] = {}
     res = global_table[f][ag_hash] = f(*args, **kwargs)
     return res
 
 
-def look_up_args(f: callable, *args: Sequence) -> Any:
+def look_up_args(f: Callable, *args: Sequence) -> Any:
     """
 
     :param f:
     :type f:
     :param args:
     :type args:
     :return:
@@ -70,15 +70,15 @@
         return res
 
     global_table[f] = {}
     res = global_table[f][args] = f(*args)
     return res
 
 
-def look_up_kws(f: callable, **kwargs: MutableMapping) -> Any:
+def look_up_kws(f: Callable, **kwargs: MutableMapping) -> Any:
     """
 
     :param f:
     :type f:
     :param kws:
     :type kws:
     :return:
@@ -92,15 +92,15 @@
         return res
 
     global_table[f] = {}
     res = global_table[f][kw_hash] = f(**kwargs)
     return res
 
 
-def precompute_lut(f: callable, arg_sets: Set[Tuple[Iterable, Mapping]], *, verbose=False) -> callable:
+def precompute_lut(f: Callable, arg_sets: Set[Tuple[Iterable, Mapping]], *, verbose=False) -> callable:
     """
 
     :param f:
     :type f:
     :param arg_sets:
     :type arg_sets:
     :param verbose:
@@ -110,15 +110,15 @@
     for arg_set, kws_set in arg_sets:
         res = look_up(f, *arg_set, **kws_set)
         if verbose:
             print(f"precompute {f},{arg_set},{kws_set}->{res}")
     return f
 
 
-def precompute_lut_args(f: callable, arg_sets: Set[Iterable], *, verbose=False) -> callable:
+def precompute_lut_args(f: Callable, arg_sets: Set[Iterable], *, verbose=False) -> callable:
     """
 
     :param f:
     :type f:
     :param arg_sets:
     :type arg_sets:
     :param verbose:
@@ -128,15 +128,15 @@
     for arg_set in arg_sets:
         res = look_up_args(f, *arg_set)
         if verbose:
             print(f"precompute {f},{arg_sets}->{res}")
     return f
 
 
-def precompute_lut_kws(f: callable, arg_sets: Set[Mapping], *, verbose=False) -> callable:
+def precompute_lut_kws(f: Callable, arg_sets: Set[Mapping], *, verbose=False) -> callable:
     """
 
     :param f:
     :type f:
     :param arg_sets:
     :type arg_sets:
     :param verbose:
```

### Comparing `Warg-1.1.6/warg/decorators/caching/property_caching.py` & `Warg-1.1.7/warg/decorators/caching/property_caching.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,25 @@
            Created on 16/02/2020
            """
 
 # TODO: Will be part of functools in the future!
 
 __all__ = ["cached_property"]
 
+from typing import Any
+
 # cached_property = property
 
 ################################################################################
 ### cached_property() - computed once per instance, cached as attribute
 ################################################################################
-from _thread import RLock
+try:
+    from _thread import RLock
+except:
+    pass
 
 _NOT_FOUND = object()
 
 
 class cached_property:
     """description"""
 
@@ -36,15 +41,15 @@
             self.attrname = name
         elif name != self.attrname:
             raise TypeError(
                 "Cannot assign the same cached_property to two different names "
                 f"({self.attrname!r} and {name!r})."
             )
 
-    def __get__(self, instance, owner=None):
+    def __get__(self, instance, owner=None) -> Any:
         if instance is None:
             return self
         if self.attrname is None:
             raise TypeError("Cannot use cached_property instance without calling __set_name__ on it.")
         try:
             cache = instance.__dict__
         except AttributeError:  # not all objects have __dict__ (e.g. class defines slots)
```

### Comparing `Warg-1.1.6/warg/decorators/exporting.py` & `Warg-1.1.7/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/decorators/hashing.py` & `Warg-1.1.7/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/decorators/kw_passing.py` & `Warg-1.1.7/warg/decorators/kw_passing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import functools
 import inspect
 import types
 from functools import wraps
 from logging import warning
-from typing import Dict, MutableMapping, Sequence, Tuple, Any
+from typing import Dict, MutableMapping, Sequence, Tuple, Any, Callable
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
           The concept "kw passing" implemented here lets one make a contract with the caller that all
           kwargs with be passed onwards to a receiver, this lets the caller inspect available kwargs of the
           the receiver function allowing for autocompletion, typing and documentation fetching.
            """
@@ -41,15 +41,15 @@
         val._kind = inspect._ParameterKind.KEYWORD_ONLY
     return val
 
 
 # noinspection PyUnresolvedReferences
 def eval_sig_kw_params(
     passing_sig: inspect.Signature,
-    receiver_func: callable,
+    receiver_func: Callable,
     keep_from_var_kw: bool = False,
 ) -> Tuple[inspect.Signature, Dict[str, inspect.Parameter]]:
     """
 
     :param passing_sig:
     :type passing_sig:
     :param receiver_func:
@@ -100,49 +100,49 @@
                 f"kwargs onwards TypeErrors might occur, to fix this let this receiver accept any arbitrary "
                 f"kwargs by adding ..,**kwargs): to the receivers function declaration"
             )
 
     return passing_sig, passing_params
 
 
-def passes_kws_to(*receiver_funcs: callable, keep_from_var_kw: bool = False) -> callable:
+def passes_kws_to(*receiver_funcs: Callable, keep_from_var_kw: bool = False) -> Callable:
     """
     A contract decorator, attaching this to a function you explicitly state that kws will be passed onward to
     a receiver function. No call graph checks if this actually enforces this yet. Also all receiver kwargs
     must be able to be received by receivers if multiple contracts are use
 
     :param receiver_funcs:
     :param keep_from_var_kw:
     :return:"""
     for receiver_func in receiver_funcs:
         if isinstance(receiver_func, types.BuiltinFunctionType):
             raise AssertionError(f"'Built In Receiver' function: {receiver_func}, is not supported")
 
-    def _func(passing_func: callable) -> callable:
+    def _func(passing_func: Callable) -> Callable:
         passing_sig = inspect.signature(passing_func)
         for rf in receiver_funcs:
             passing_sig, new_params = eval_sig_kw_params(passing_sig, rf, keep_from_var_kw)
             passing_sig = passing_sig.replace(parameters=list(new_params.values()))
         passing_func.__signature__ = passing_sig
         return passing_func
 
     return _func
 
 
 def super_init_pass_on_kws(
-    f: callable = None, *, super_base: type = None, keep_from_var_kw: bool = False
-) -> callable:
+    f: Callable = None, *, super_base: type = None, keep_from_var_kw: bool = False
+) -> Callable:
     """
 
     :param f:
     :param super_base:
     :param keep_from_var_kw:
     :return:"""
 
-    def _func(func) -> callable:
+    def _func(func) -> Callable:
         if super_base:
             to_func = super_base.__init__
         else:
             to_func = inspect.getmro(func)[0].__init__
 
         from_func = func.__init__
 
@@ -153,15 +153,15 @@
 
     if f:
         return _func(f)
 
     return _func
 
 
-def drop_args(f: callable) -> callable:
+def drop_args(f: Callable) -> Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
@@ -174,15 +174,15 @@
         :return:
         :rtype:"""
         return f(**kwargs)
 
     return wrapper
 
 
-def drop_kws(f: callable) -> callable:
+def drop_kws(f: Callable) -> Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
@@ -195,15 +195,15 @@
         :return:
         :rtype:"""
         return f(*args)
 
     return wrapper
 
 
-def drop_args_and_kws(f: callable) -> callable:
+def drop_args_and_kws(f: Callable) -> Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
@@ -225,15 +225,15 @@
     - {
         "__annotations__",
     }
 )
 
 
 def pack_args(
-    f: callable,
+    f: Callable,
     *,
     pack_name: str = "arg_pack",
     allow_passing: bool = True,
     verbose: bool = False,
 ) -> callable:
     """
 
@@ -269,15 +269,15 @@
                 new_kwargs[pack_name] = args
         return f(*args, **new_kwargs)
 
     return wrapper
 
 
 def pack_kws(
-    f: callable,
+    f: Callable,
     *,
     pack_name: str = "kw_pack",
     allow_passing: bool = True,
     verbose: bool = False,
 ) -> callable:
     """
 
@@ -313,15 +313,15 @@
                 new_kwargs[pack_name] = kwargs
         return f(*args, **new_kwargs)
 
     return wrapper
 
 
 def pack_args_and_kws(
-    f: callable,
+    f: Callable,
     *,
     pack_name: str = "arg_kw_pack",
     allow_passing: bool = True,
     verbose: bool = False,
 ) -> callable:
     """
 
@@ -356,15 +356,15 @@
             else:
                 new_kwargs[pack_name] = (args, kwargs)
         return f(*args, **kwargs)
 
     return wrapper
 
 
-def drop_unused_args(f: callable) -> callable:
+def drop_unused_args(f: Callable) -> Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
@@ -378,15 +378,15 @@
         :rtype:"""
         return f(**kwargs)
 
     return wrapper
 
 
 # noinspection PyUnresolvedReferences
-def drop_unused_kws(f: callable) -> callable:
+def drop_unused_kws(f: Callable) -> Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
@@ -417,15 +417,15 @@
 class AlsoDecorator:
     """
     Lets you use a function as a decorator too
     """
 
     def __call__(self, func):
         @functools.wraps(func)
-        def decorate_func(*args: Sequence, **kwargs: MutableMapping):
+        def decorate_func(*args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             """
 
             :param args:
             :type args:
             :param kwargs:
             :type kwargs:
             :return:
```

### Comparing `Warg-1.1.6/warg/decorators/timing.py` & `Warg-1.1.7/warg/decorators/timing.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 __all__ = ["timeit", "StopWatch"]
 
 import contextlib
 import functools
 import time
 import typing
 from functools import wraps
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any, Any
 
 
-def timeit(f: callable):
+def timeit(f: typing.Callable) -> typing.Callable:
     """
 
     :param f:
     :type f:
     :return:
     :rtype:"""
 
     @wraps(f)
-    def wrapper(*args, **kwds):
+    def wrapper(*args, **kwds) -> typing.Tuple[float, Any]:
         """
 
         :param args:
         :type args:
         :param kwds:
         :type kwds:
         :return:
@@ -191,15 +191,15 @@
 
         :param function:
         :type function:
         :return:
         :rtype:"""
 
         @functools.wraps(function)
-        def decorated(*args: Sequence, **kwargs: MutableMapping):
+        def decorated(*args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             """description"""
             self.start_timer()
             values = function(*args, **kwargs)
             self.stop_timer()
             return values, self.since_start
 
         return decorated
```

### Comparing `Warg-1.1.6/warg/decorators/wrapping.py` & `Warg-1.1.7/warg/decorators/wrapping.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 __doc__ = r"""
 
            Created on 14/11/2019
            """
 
 __all__ = ["pre_decorate", "post_decorate"]
 
+from typing import Callable
 
-def pre_decorate(method: callable, *callables: callable):
-    def pre_call_func(self: object = None, *args, **kwargs):
+
+def pre_decorate(method: Callable, *callables: Callable) -> callable:
+    def pre_call_func(self: object = None, *args, **kwargs) -> callable:
         for c in callables:
             c(self, *args, **kwargs)
         return method(self, *args, **kwargs)
 
     return pre_call_func
 
 
-def post_decorate(method: callable, *callables: callable):
-    def post_call_func(self: object = None, *args, **kwargs):
+def post_decorate(method: Callable, *callables: Callable) -> callable:
+    def post_call_func(self: object = None, *args, **kwargs) -> callable:
         res = method(self, *args, **kwargs)
         for c in callables:
             c(self, *args, res=res, **kwargs)
         return res
 
     return post_call_func
 
 
 if __name__ == "__main__":
 
-    def juahsdu():
+    def juahsdu() -> None:
         def c(d):
             print(d)
             return f"c_{d}"
 
         a = pre_decorate(c, lambda *args, **kwargs: print(f"pre {args, kwargs}"))
         b = post_decorate(c, lambda *args, **kwargs: print(f"post {args, kwargs}"))
```

### Comparing `Warg-1.1.6/warg/exceptions.py` & `Warg-1.1.7/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/functions.py` & `Warg-1.1.7/warg/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             None, return the items that are true.
     """
     for f in filters:
         it = filter(f, it)
     return it
 
 
-def chain_apply(it: Iterable, *callables: Callable) -> Iterable:
+def chain_apply(it: Iterable, *callables: Callable) -> Iterable[Any]:
     """
     Apply a sequence of callables to an iterable; apply the iterable sequentially in callables order
 
     Args:
         it (Iterable):
             iterable to be applied to
         callables (Callable):
```

### Comparing `Warg-1.1.6/warg/gdkc.py` & `Warg-1.1.7/warg/gdkc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 Generalised wrapper for delayed construction of class objects. Encapsulates kwargs and callable constructor with the option of modifying construction arguments before construction is finally performed.
 
 """
 
 __all__ = ["GeneralisedDelayedKwargConstruction", "GDKC"]
 
 import logging
-from typing import Any, Mapping, MutableMapping, Sequence
+from typing import Any, Mapping, MutableMapping, Sequence, Callable
 
 
 class GeneralisedDelayedKwargConstruction(object):
     """
     A generalised class for setting up kwargs for later construction of an instance of an object
     [constructor, args, kwargs]
     """
 
-    def __init__(self, constructor: callable, *args: Sequence, **kwargs: Any):
+    def __init__(self, constructor: Callable, *args: Sequence, **kwargs: Any):
         """
         [constructor, args, kwargs]
         :param constructor:
         :param args:
         :param kwargs:"""
-        self.constructor: callable = constructor
+        self.constructor: Callable = constructor
         assert len(args) < 2, f"Does not support multiple args, only a single mapping type"
         if len(args) == 1:
             assert isinstance(
                 args[0], Mapping
             ), f"Arg[0] type is not a mapping type, was {type(args[0])} which is not supported"
         assert not (
             len(kwargs) > 0 and len(args) > 0
@@ -80,15 +80,15 @@
 
     class UnreachableError(Exception):
         pass
 
     class A:
         """description"""
 
-        def __init__(self, *args: Sequence, **kwargs: MutableMapping):
+        def __init__(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             pass
 
     def stest_not_both() -> None:
         """
         :rtype: None
         """
         GeneralisedDelayedKwargConstruction(A, [1], a=2)
```

### Comparing `Warg-1.1.6/warg/generators/cyclic_generators.py` & `Warg-1.1.7/warg/generators/cyclic_generators.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     :type magnitude:
     :param iterable:
     :type iterable:"""
     for a in iterable:
         yield sin(a) * magnitude
 
 
-def cos_gen(iterable: Iterable, magnitude: Number = 1) -> Iterable[Number]:
+def cos_gen(iterable: Iterable[Number], magnitude: Number = 1) -> Iterable[Number]:
     """
 
     :param magnitude:
     :type magnitude:
     :param iterable:
     :type iterable:"""
     for a in iterable:
```

### Comparing `Warg-1.1.6/warg/generators/filtering.py` & `Warg-1.1.7/warg/generators/filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "exclude_postfix",
         "exclude_prefix",
         "exclude_fully",
     )
 
 
 def symbol_filter(
-    string_stream: Iterable,
+    string_stream: Iterable[str],
     symbol: str = "#",
     *,
     exclusion_mode: FilterModeEnum = FilterModeEnum.exclude_postfix,
 ) -> Any:
     """description"""
     if exclusion_mode == FilterModeEnum.exclude_fully:
         yield from filter(lambda s: symbol not in s, string_stream)
```

### Comparing `Warg-1.1.6/warg/generators/mapping_generator.py` & `Warg-1.1.7/warg/generators/mapping_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Any, Iterable, Mapping, Tuple
+from typing import Any, Iterable, Mapping, Tuple, Callable
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 11/11/2019
            """
 
 __all__ = ["yield_and_map", "inner_map", "kw_map"]
 
 
-def yield_and_map(iterable: Iterable, level: int = 0, func: callable = print) -> Any:
+def yield_and_map(iterable: Iterable[Any], level: int = 0, func: Callable = print) -> Any:
     """
 
     :param iterable:
     :type iterable:
     :param level:
     :type level:
     :param func:
@@ -33,15 +33,15 @@
         for a in iterable:
             for b in a:
                 for c in b:
                     func(c)
                     yield c
 
 
-def inner_map(func: callable, iterable: Iterable, aggregate_yield: bool = True) -> Any:
+def inner_map(func: Callable, iterable: Iterable[Any], aggregate_yield: bool = True) -> Any:
     """
 
     :param func:
     :type func:
     :param iterable:
     :type iterable:
     :param aggregate_yield:
@@ -51,44 +51,46 @@
             yield [func(b) for b in a]
     else:
         for a in iterable:
             for b in a:
                 yield func(b)
 
 
-def kw_map(func: callable, kw: str, iterable: Iterable) -> Any:
+def kw_map(func: Callable, kw: str, iterable: Iterable[Any]) -> Any:
     """
 
     :param func:
     :type func:
     :param kw:
     :type kw:
     :param iterable:
     :type iterable:"""
     for a in iterable:
         yield func(**{kw: a})
 
 
-def select_key(tuple_iterator: Iterable, *a) -> Tuple:
+def select_key(tuple_iterator: Iterable[Any], *a) -> Tuple[Any, Any]:
     """
     Yield keys from mapping if in a
 
+    TODO: Why return the key itself?
+
     :param tuple_iterator:
     :type tuple_iterator:
     :param a:
     :type a:
     :return:
     :rtype:
     """
     for k, _ in tuple_iterator:
         if k in a:
             yield k, _
 
 
-def select_dict(mapping: Mapping, *a) -> Mapping:
+def select_dict(mapping: Mapping[Any, Any], *a) -> Mapping[Any, Any]:
     """
     Select keys from mapping if in a
 
     Args:
       mapping:
       *a:
 
@@ -96,15 +98,15 @@
 
     """
     return {k: v for k, v in select_key(mapping.items(), *a)}
 
 
 if __name__ == "__main__":
 
-    def uahsd():
+    def uahsd() -> None:
         agfas = (2, 3)
         # TODO
 
         sadd = {a: b for a, b in zip("abcdef", range(6))}
         print(select_dict(sadd, "a", "d"))
 
     uahsd()
```

### Comparing `Warg-1.1.6/warg/generators/zipping_generator.py` & `Warg-1.1.7/warg/generators/zipping_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
            Created on 28/10/2019
            """
 
 __all__ = ["unzip", "unzipper"]
 
 
-def unzip(iterable: Iterable) -> Iterable:
+def unzip(iterable: Iterable[Any]) -> Iterable[Any]:
     """description"""
     return zip(*iterable)
 
 
-def unzipper(_iterable: Iterable[Iterable]) -> Iterable:
+def unzipper(_iterable: Iterable[Iterable[Any]]) -> Iterable[Any]:
     """
     Unzips an iterable of an iterable
 
-    Be carefully has undefined and expected behaviour
+    Be careful, functionality maybe have undefined and unexpected behaviour
 
     :param _iterable:
     :return:Iterable
     """
 
     def check_next_iter(iterable_: Any) -> Any:
         """description"""
@@ -44,15 +44,14 @@
                 yield unzipper(a)
         elif check_a:
             for a in _iterable:
                 yield unzip(a)
         else:
             for i in _iterable:
                 yield i
-    return
 
 
 if __name__ == "__main__":
 
     def recursive_eval(node: Any):
         """description"""
         if isinstance(node, (Iterable, Generator, Iterator)):
```

### Comparing `Warg-1.1.6/warg/importing.py` & `Warg-1.1.7/warg/importing.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 import importlib
 import sys
 from importlib import reload
 from importlib.util import find_spec
 from pathlib import Path
-from typing import Optional, Any, Union, List, Iterable
+from typing import Optional, Any, Union, List, Iterable, Callable
 from warnings import warn
 
 import pkg_resources
 
 from warg import passes_kws_to
 
 """
@@ -57,50 +57,80 @@
       # there are some problems that are swept under the rug here
       pass
 init()
 """
 
 
 def contain(q: Any, s: Iterable) -> bool:
+    """
+
+    :param q:
+    :param s:
+    :return:
+    """
     return q in s
 
 
-def reload_module(module_name: str, containment_test: callable = contain) -> None:
+def reload_module(module_name: str, containment_test: Callable = contain) -> None:
+    """
+
+    :param module_name:
+    :param containment_test:
+    :return:
+    """
     if module_name in sys.modules:
         reload_set = {x for x in sys.modules if containment_test(module_name, x)}
         for a in reload_set:
             del sys.modules[a]
             # importlib.reload(sys.modules[mod_str]) #DOES NOT WORK ON FROM IMPORTS...
             sys.modules[a] = importlib.import_module(a)
     else:
         sys.modules[module_name] = importlib.import_module(module_name)
 
 
-def reload_requirements(requirements_path: Path, containment_test: callable = contain) -> None:
+def reload_requirements(requirements_path: Path, containment_test: Callable = contain) -> None:
+    """
+
+    :param requirements_path:
+    :param containment_test:
+    :return:
+    """
     with open(requirements_path) as f:
         for r in pkg_resources.parse_requirements(f.readlines()):
             reload_module(r.project_name, containment_test=containment_test)
 
 
 def reload_all_modules(catch_exceptions: bool = True, verbose: bool = True) -> None:
+    """
+
+    :param catch_exceptions:
+    :param verbose:
+    :return:
+    """
     try:
         for mod in sys.modules.values():
             reload(mod)
     except Exception as e:
         if verbose:
             print(mod)
         if catch_exceptions:
             if verbose:
                 print(e)
         else:
             raise e
 
 
 def import_file(path: Path, from_list=None) -> Any:
-    """Import a module given its filename, works both on absolute and relative paths"""
+    """
+    Import a module given its filename, works both on absolute and relative paths
+
+    :param path:
+    :param from_list:
+    :return:
+    """
     if from_list is None:
         from_list = {}
     globals_ = {}  # globals() # determines package context
     locals_ = {}  # locals() # Should not be used in import anyway
 
     sys_path = sys.path  # Save original sys.path
     try:
@@ -109,27 +139,40 @@
             path.stem, globals=globals_, locals=locals_, fromlist=from_list, level=0
         )  # Get the module name (no extension)
     finally:
         sys.path = sys_path  # Restore original sys.path
 
 
 def walk_up(path: Path, top: Path, max_ascent: int = None):
+    """
+
+    :param path:
+    :param top:
+    :param max_ascent:
+    :return:
+    """
     i = 0
     while True:
         yield path
         i += 1
         if max_ascent and max_ascent < i:
             break
         if path == top:
             break
         else:
             path = path.parent
 
 
 def walk_down(path: Path, max_descent: int = None):
+    """
+
+    :param path:
+    :param max_descent:
+    :return:
+    """
     if max_descent == 0:
         return
 
     queue = []
     for c in path.iterdir():
         if c.is_dir():
             yield c
@@ -140,24 +183,37 @@
             yield from walk_down(q, max_descent=max_descent - 1 if max_descent else None)
         except:
             yield
 
 
 def find_ancestral_relatives(
     target: Union[str, Path],
-    context: Path = Path.cwd(),
+    context: Path,  # = Path.cwd(),
     *,
     from_parent_of_context: bool = True,
     ancestral_levels: int = 2,
     descendant_levels: int = 2,
     top_level: Path = None,
     return_parent_of_target: bool = True,
     no_duplicates: bool = True,
     terminate_first: bool = False,
 ) -> List[Path]:
+    """
+
+    :param target:
+    :param context:
+    :param from_parent_of_context:
+    :param ancestral_levels:
+    :param descendant_levels:
+    :param top_level:
+    :param return_parent_of_target:
+    :param no_duplicates:
+    :param terminate_first:
+    :return:
+    """
     relatives = []
 
     if top_level is None:
         top_level = context.root
 
     if from_parent_of_context:
         context = context.parent
@@ -182,37 +238,49 @@
         return list(set(relatives))
 
     return relatives
 
 
 @passes_kws_to(find_ancestral_relatives)
 def find_nearest_ancestral_relative(*args, **kwargs) -> Optional[Path]:
+    """
+
+    :param args:
+    :param kwargs:
+    :return:
+    """
     kwargs.update(terminate_first=True)
     result = find_ancestral_relatives(*args, **kwargs)
     if result:
         return result[0]
 
 
 def clean_sys_path() -> None:
     """
-    Clean the sys.path for dead paths or duplicates
+      Clean the sys.path for dead paths or duplicates
+
+    :return:
     """
     out = []
     for path in sys.path:
         p = Path(path).resolve()
         if p.exists():
             if p not in out:
                 out.append(p)
 
     sys.path[:] = [str(o.absolute()) for o in out]
 
 
 def remove_from_sys_path(target: Path, missing_ok: bool = True):
     """
-    Clean the sys.path for dead paths or duplicates
+      Clean the sys.path for target path
+
+    :param target:
+    :param missing_ok:
+    :return:
     """
     out = []
 
     target = target.resolve()
 
     for path in sys.path:
         p = Path(path).resolve()
@@ -224,31 +292,34 @@
 
 
 def ensure_in_sys_path(
     path: Optional[Union[str, Path]],
     position: Optional[int] = None,
     resolve: bool = False,
     absolute: bool = True,
+    verbose: bool = False,
 ) -> None:
     """
 
     Ensures that a path is in sys.path, but avoids duplicates.
     Can also resolve and absolute paths for duplication.
     Does not clean the existing paths in sys.path
 
-    :param path:
-    :type path:
-    :param position:
-    :type position:
-    :param resolve:
-    :type resolve:
-    :param absolute:
-    :type absolute:
-    :return:
-    :rtype:
+    :param verbose: Whether to print verbose info
+    :type verbose: bool
+    :param path: The path to be inserted
+    :type path: Optional[Union[str, Path]]
+    :param position: If not supplied, the path will be appended at the end of the existing sys.path
+    :type position: Optional[int]
+    :param resolve: Whether to resolve the absolute path
+    :type resolve: bool
+    :param absolute: Insert the absolute path
+    :type absolute: bool
+    :return: None
+    :rtype: None
     """
     if path is None:  # may be the case if the supplied path is being solved programmatically
         warn("No path was supplied")
         return
 
     path = Path(path)
 
@@ -266,36 +337,33 @@
 
     if not inclusion_test:
         if position:
             sys.path.insert(position, str_path)
         else:
             sys.path.append(str_path)
     else:
-        print(f"{path} is already in sys path")
+        if verbose:
+            print(f"{path} is already in sys path")
 
 
 def is_module_available(module: str) -> bool:
-    """**Return True if module is available.**
+    """Returns True if module is available.
+
 
-    Parameters
-    ----------
-    module: str
-          Name of the module to be checked.
-
-    Returns
-    -------
-    bool
-          True if installed.
+    :param module: Name of the module to be checked.
+    :type module: str
+    :return:  True if installed.
+    :rtype: bool
     """
     return find_spec(module) is not None
 
 
 def import_warning(module_name: str) -> None:
     """
-    Inform the user that module has been imported,
+    Inform the user that a module has been imported,
     useful when repeated imports are heavy in the contexts of multiprocessing.
     Lets the user identify which file is reporting heavy loading and restructure code to avoid repeated importing
 
     :param module_name:
     :return:
     """
     from sys import modules
```

### Comparing `Warg-1.1.6/warg/manipulation.py` & `Warg-1.1.7/warg/manipulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 __all__ = ["recursive_flatten"]
 
 from typing import Sequence
 
 
 def recursive_flatten(seq: Sequence) -> Sequence:
-    """description"""
+    """Depth first flatten"""
     if not seq:  # is empty Sequence
         return seq
     if isinstance(seq[0], Sequence):
         return (*recursive_flatten(seq[0]), *recursive_flatten(seq[1:]))
     return (*seq[:1], *recursive_flatten(seq[1:]))
```

### Comparing `Warg-1.1.6/warg/map_itertools.py` & `Warg-1.1.7/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/math_utilities/ordinals.py` & `Warg-1.1.7/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/math_utilities/powers.py` & `Warg-1.1.7/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/metas/post_init.py` & `Warg-1.1.7/warg/metas/post_init.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 __doc__ = r"""
 
            Created on 11/12/2019
            """
 
 __all__ = ["PostInit"]
 
-from typing import Sequence, MutableMapping
+from typing import Sequence, MutableMapping, Any, Any
 
 
 class PostInit(type):
     """
     define a new metaclass which overrides the "__call__" function"""
 
-    def __call__(cls, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(cls, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]) -> object:
         """
         Called when you call a class type constructor()"""
         obj = type.__call__(cls, *args, **kwargs)
         if hasattr(obj, "__post_init__"):
             obj.__post_init__(*args, **kwargs)
         return obj
 
@@ -29,13 +29,13 @@
 
     class SAD(metaclass=PostInit):
         """description"""
 
         def __init__(self):
             print("init")
 
-        def __post_init__(self):
+        def __post_init__(self) -> None:
             """description"""
             print("post_init")
 
     SAD()
     SAD()
```

### Comparing `Warg-1.1.6/warg/metas/singleton.py` & `Warg-1.1.7/warg/metas/singleton.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 @author: cnheider
 """
 
 __all__ = ["SingletonBase", "SingletonMeta", "key_singleton", "singleton"]
 
 import functools
 from functools import wraps
-from typing import Any, Sequence, MutableMapping
+from typing import Any, Sequence, MutableMapping, Callable
 
 
 class SingletonBase:
     """
     A base class for creating singleton class where all subtypes(Derivations) should also return the first
     and only
     instantiation of a particular singleton base type, if this property is not wanted consider using the
     SingletonMeta class instead."""
 
     instance = None
 
-    def __new__(cls, *args: Sequence, **kwargs: MutableMapping):
+    def __new__(cls, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         if cls.instance is None:
             cls.instance = super().__new__(cls, *args, **kwargs)
 
         return cls.instance
 
 
 class SingletonMeta(type):
@@ -44,28 +44,28 @@
     the
     SingletonBase class instead."""
 
     def __init__(cls, name, bases, namespace):
         super().__init__(name, bases, namespace)
         cls.instance = None
 
-    def __call__(cls, *args: Sequence, **kwargs: MutableMapping):
+    def __call__(cls, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         if cls.instance is None:
             cls.instance = super().__call__(*args, **kwargs)
 
         return cls.instance
 
 
 def singleton(cls):
     """Use class as singleton."""
 
     cls.__new_original__ = cls.__new__
 
     @functools.wraps(cls.__new__)
-    def singleton_new(cls_, *args: Sequence, **kwargs: MutableMapping):
+    def singleton_new(cls_, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
         """
 
         :param cls_:
         :param args:
         :param kwargs:
         :return:
         """
@@ -80,24 +80,24 @@
     cls.__new__ = singleton_new
     cls.__init_original__ = cls.__init__
     cls.__init__ = object.__init__
 
     return cls
 
 
-def key_singleton(cache_key: Any) -> callable:
+def key_singleton(cache_key: Any) -> Callable:
     """
     TODO: finish
     """
 
-    def inner_fn(fn: callable) -> Any:
+    def inner_fn(fn: Callable) -> Any:
         """description"""
 
         @wraps(fn)
-        def wrapper(self, *args: Sequence, **kwargs: MutableMapping):
+        def wrapper(self, *args: Sequence[Any], **kwargs: MutableMapping[str, Any]):
             """description"""
             instance = getattr(self, cache_key)
             if instance is not None:
                 return instance
 
             instance = fn(self, *args, **kwargs)
             setattr(self, cache_key, instance)
```

### Comparing `Warg-1.1.6/warg/mixins/dict_mixins.py` & `Warg-1.1.7/warg/mixins/dict_mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 
 __all__ = [
     "IterDictItemsMixin",
     "IterDictKeysMixin",
     "IterDictValuesMixin",
 ]
 
+from typing import Any, Tuple
+
 
 class IterDictItemsMixin:
     """
     Mixin class for iterating kw pairs in a class instance __dict__"""
 
-    def __iter__(self):
+    def __iter__(self) -> Tuple[Any, Any]:
         for attr, value in self.__dict__.items():
             yield attr, value
 
 
 class IterDictKeysMixin:
     """
     Mixin class for iterating only the keys of a class instance __dict__"""
 
-    def __iter__(self):
+    def __iter__(self) -> Any:
         for attr in self.__dict__.keys():
             yield attr
 
 
 class IterDictValuesMixin:
     """
     Mixin class for iterating only the values of a class instance __dict__"""
 
-    def __iter__(self):
+    def __iter__(self) -> Any:
         for value in self.__dict__.values():
             yield value
 
 
 if __name__ == "__main__":
 
     def asdij() -> None:
```

### Comparing `Warg-1.1.6/warg/mixins/ordinal_index_mixin.py` & `Warg-1.1.7/warg/mixins/ordinal_index_mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = ""
 
 __all__ = [
     "OrdinalIndexingDictMixin",
 ]
 
+from typing import Union, Any
+
 
 class OrdinalIndexingDictMixin:
     """
     Mixin class for indexing a class instance __dict__ (SortedDict) with both integer (ordinal) indexing or
     key:str attributes (non-ordinal) access."""
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: Union[int, Any]) -> Any:
         if isinstance(item, int):
             return list(self.__dict__.values())[item]
         else:
             return self.__dict__[item]
 
 
 if __name__ == "__main__":
```

### Comparing `Warg-1.1.6/warg/ode.py` & `Warg-1.1.7/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/os_utilities/filtering.py` & `Warg-1.1.7/warg/os_utilities/filtering.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     Negate a function return
     """
 
     assert isinstance(f, Callable), "ensure you did not call the callable with parameters directly"
 
     @wraps(f)
-    def wrapper(*args: Sequence, **kwargs: MutableMapping) -> Any:
+    def wrapper(*args: Sequence[Any], **kwargs: MutableMapping[str, Any]) -> Any:
         """
 
         :param args:
         :type args:
         :param kwargs:
         :type kwargs:
         :return:
```

### Comparing `Warg-1.1.6/warg/os_utilities/os_platform.py` & `Warg-1.1.7/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/os_utilities/path_functions.py` & `Warg-1.1.7/warg/os_utilities/path_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,52 +3,54 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 08/03/2020
            """
 
-__all__ = ["ensure_existence", "path_rmtree", "sanitise_path", "path_join"]
+__all__ = ["ensure_existence", "path_rmtree", "sanitise_path", "path_join", "keep_last_n_modified"]
 
+import collections
 import os
 from itertools import cycle
 from pathlib import Path
-from shutil import rmtree
-from typing import Iterable, Union
 
-from warg.decorators import passes_kws_to
+from typing import Iterable, Union, Callable
 
 
 def path_join(*p: Union[Path, str]) -> Path:
     """
-    drop-in replacement for os.path.join, returning a Path instead
+    Drop-in replacement for os.path.join, returning a Path instead
 
     :param p: Sequence of path components to be joined
-    :type p:  Union[Path,str]
+    :type p:  Union[Path, str]
     :return: Joined path
     :rtype: Path
     """
     p, *rest = p
     p = Path(p)
     for r in rest:
         p /= r
     return p
 
 
-@passes_kws_to(rmtree)
+# @passes_kws_to(rmtree)
 def path_rmtree(path: Path, **kwargs) -> None:
     """
-    asses_kws_to rmtree from shutil
+    Passes_kws_to rmtree from shutil
+
     :param path:
     :type path: Path
     :param kwargs:
     :type kwargs:
     :return: None
     :rtype: None
     """
+    from shutil import rmtree
+
     rmtree(str(path), **kwargs)
 
 
 def sanitise_path(
     path: Path,
     naughty_directory_symbols: Iterable[str] = (
         " ",
@@ -95,15 +97,15 @@
     out: Union[Path, str],
     *,
     enabled: bool = True,
     declare_file: bool = False,
     overwrite_on_wrong_type: bool = False,
     force_overwrite: bool = False,
     verbose: bool = False,
-    sanitisation_func: callable = sanitise_path,
+    sanitisation_func: Callable = sanitise_path,
 ) -> Path:
     """
 
     :param verbose:
     :type verbose:
     :param overwrite_on_wrong_type:
     :type overwrite_on_wrong_type:
@@ -153,14 +155,39 @@
                 out.unlink()  # missing_ok=True)
             if not out.exists():
                 out.mkdir(parents=True, exist_ok=True)
 
     return out
 
 
+# @passes_kws_to(rmtree)
+def keep_last_n_modified(
+    directory: Union[Path, str], n: int, only_directories: bool = False, only_files: bool = False, **kwargs
+):
+    directory = Path(directory)
+    from shutil import rmtree
+
+    assert not (only_files and only_directories)  # Ensure that only of them is True or both are False
+
+    timeline = {}
+    for dir_entry in directory.iterdir():
+        if only_directories and not dir_entry.is_dir():
+            continue
+        if only_files and not dir_entry.is_file():
+            continue
+        timeline[os.path.getmtime(str(dir_entry))] = dir_entry
+
+    sorted_timeline = collections.OrderedDict(sorted(timeline.items()))
+    for _ in range(min(len(sorted_timeline), n)):  # Keep the last n versions of tiles
+        sorted_timeline.popitem()
+
+    for j in sorted_timeline.values():
+        rmtree(j, **kwargs)
+
+
 if __name__ == "__main__":
 
     def main():
         """description"""
         ensure_existence(Path.cwd() / "exclude", force_overwrite=True)
         ensure_existence(Path.cwd() / "exclude" / "0.log")
         ensure_existence(Path.cwd() / "exclude" / "log.d")
@@ -189,10 +216,11 @@
         """
         :rtype: None
         """
         pa = Path.cwd() / "uhas.asudh ojas.a." / "....  a -." / "   bci"
 
         print(pa, sanitise_path(pa))
 
-    clean_naughty_file()
-    clean_naughty_dir()
+    # clean_naughty_file()
+    # clean_naughty_dir()
     # main()
+    keep_last_n_modified(Path("exclude"), 2)
```

### Comparing `Warg-1.1.6/warg/os_utilities/path_utilities.py` & `Warg-1.1.7/warg/os_utilities/path_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
            Created on 07-05-2021
            """
 
 import os
 import subprocess
 from pathlib import Path
-
-__all__ = ["latest_file", "exist_any_extension", "system_open_path"]
+from typing import Optional
 
 from warg.os_utilities.os_platform import is_windows, is_mac, has_x_server
 
+__all__ = ["latest_file", "exist_any_extension", "system_open_path"]
+
 
 def system_open_path(path: Path, *, verbose: bool = False) -> None:
     """
     Use system defaults for opening path/uris
 
     :param path:
     :type path:
@@ -49,15 +50,15 @@
 
 def latest_file(
     directory: Path,
     extension: str = "",
     *,
     recurse: bool = False,
     raise_on_failure: bool = True,
-) -> Path:
+) -> Optional[Path]:
     """
 
     :param directory:
     :param extension:
     :param recurse:
     :param raise_on_failure:
     :return:
@@ -75,15 +76,15 @@
         print(f"{msg}, returning None!")
         return
     return max(list_of_files, key=os.path.getctime)  # USES CREATION TIME
 
 
 def exist_any_extension(p: Path) -> bool:
     """
-    If any file with that stem exist in parent directory, return True.
+    If any file with that stem exists in the parent directory, return True.
 
     :param p:
     :type p:
     :return:
     :rtype:
     """
     for _ in p.parent.glob(f"{p.stem}.*"):
```

### Comparing `Warg-1.1.6/warg/os_utilities/platform_selection.py` & `Warg-1.1.7/warg/os_utilities/platform_selection.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,23 @@
     "get_system",
     # "set_system",
     "SystemEnum",
 ]
 
 from types import ModuleType
 
+
+class SystemEnum(enum.Enum):
+    """
+    Enum for the system type
+    """
+
+    windows, linux, mac, other = range(4)
+
+
 if sys.platform.startswith("java"):
     import platform
 
     os_name = platform.java_ver()[3][0]
     if os_name.startswith("Windows"):  # "Windows XP", "Windows 7", etc.
         SYSTEM_ = "win32"
     elif os_name.startswith("Mac"):  # "Mac OS X", etc.
@@ -32,23 +41,22 @@
         # Setting this to "linux2" is not ideal, but only Windows or Mac
         # are actually checked for and the rest of the module expects
         # *sys.platform* style strings.
         SYSTEM_ = "linux2"
 else:
     SYSTEM_ = sys.platform
 
-SYSTEM = SYSTEM_
-
+SYSTEM = SystemEnum.other
 
-class SystemEnum(enum.Enum):
-    """
-    Enum for the system type
-    """
-
-    windows, linux, mac, other = range(4)
+if SYSTEM_ == "darwin":
+    SYSTEM = SystemEnum.mac
+elif SYSTEM_ == "linux2" or SYSTEM_ == "linux":
+    SYSTEM = SystemEnum.linux
+elif SYSTEM_ == "win32":
+    SYSTEM = SystemEnum.windows
 
 
 def set_system(system: SystemEnum) -> None:
     """
 
     :param system:
     :type system:
@@ -62,24 +70,14 @@
 
     :return:
     :rtype:
     """
     return SYSTEM
 
 
-if SYSTEM == "darwin":
-    SYSTEM = SystemEnum.mac
-elif SYSTEM == "linux2" or SYSTEM == "linux":
-    SYSTEM = SystemEnum.linux
-elif SYSTEM == "win32":
-    SYSTEM = SystemEnum.windows
-else:
-    SYSTEM = SystemEnum.other
-
-
 def get_backend_module(project_name: str, backend_name: str = sys.platform) -> ModuleType:
     """Returns the backend module.
 
     :param project_name:
     :type project_name:
     :param backend_name:
     :type backend_name:
@@ -117,15 +115,15 @@
         except ImportError as e:
             errors.append(e)
 
     # Did not find any backend, raise error
     raise ImportError(f'{sys.platform} platform is not supported: {"; ".join(str(e) for e in errors)}')
 
 
-def is_py3():
+def is_py3() -> bool:
     """
 
     :return:
     :rtype:
     """
     return sys.version_info[0] == 3
```

### Comparing `Warg-1.1.6/warg/packages.py` & `Warg-1.1.7/warg/packages.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/plugin.py` & `Warg-1.1.7/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/replication.py` & `Warg-1.1.7/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/strings.py` & `Warg-1.1.7/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/styling.py` & `Warg-1.1.7/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/text.py` & `Warg-1.1.7/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.6/warg/typing_extension.py` & `Warg-1.1.7/warg/typing_extension.py`

 * *Files identical despite different names*

