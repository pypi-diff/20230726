# Comparing `tmp/kestrel-lang-1.7.1.tar.gz` & `tmp/kestrel-lang-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.7.1.tar", last modified: Fri Jul 14 00:16:22 2023, max compression
+gzip compressed data, was "kestrel-lang-1.7.2.tar", last modified: Wed Jul 26 16:15:02 2023, max compression
```

## Comparing `kestrel-lang-1.7.1.tar` & `kestrel-lang-1.7.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.955632 kestrel-lang-1.7.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.955632 kestrel-lang-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.959632 kestrel-lang-1.7.1/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.963632 kestrel-lang-1.7.1/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.967632 kestrel-lang-1.7.1/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.971632 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 00:16:22.000000 kestrel-lang-1.7.1/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:16:22.975632 kestrel-lang-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_stixshifter_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-14 00:16:06.000000 kestrel-lang-1.7.1/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.508427 kestrel-lang-1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.520427 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.520427 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_stixshifter_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.1/AUTHORS.rst` & `kestrel-lang-1.7.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/LICENSE.md` & `kestrel-lang-1.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/PKG-INFO` & `kestrel-lang-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.1
+Version: 1.7.2
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
 - Do NOT write the same TTP pattern in different data source queries.
 - Do NOT write one-time-use adapaters to connect hunt steps.
 - Do NOT waste your existing analytic scripts/programs in future hunts.
-- DD construct your hunt-flow from smaller reuseable hunt-flow.
+- Do construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -140,14 +140,15 @@
 
 #. `Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks`_
 #. `Practicing Backward And Forward Tracking Hunts on A Windows Host`_
 #. `Building Your Own Kestrel Analytics and Sharing With the Community`_
 #. `Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow`_
 #. `Try Kestrel in a Cloud Sandbox`_
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
+#. `Kestrel Data Retrieval Explained`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
 - 2023/08 `Black Hat USA 2023`_
@@ -205,14 +206,15 @@
 
 .. _Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks: https://opencybersecurityalliance.org/huntbook-persistent-threat-discovery-kestrel/
 .. _Practicing Backward And Forward Tracking Hunts on A Windows Host: https://opencybersecurityalliance.org/backward-and-forward-tracking-hunts-on-a-windows-host/
 .. _Building Your Own Kestrel Analytics and Sharing With the Community: https://opencybersecurityalliance.org/kestrel-custom-analytics/
 .. _Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow: https://opencybersecurityalliance.org/kestrel-sysflow-open-hunting-stack/
 .. _Try Kestrel in a Cloud Sandbox: https://opencybersecurityalliance.org/try-kestrel-in-a-cloud-sandbox/
 .. _Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator: https://opencybersecurityalliance.org/fun-with-securitydatasets-com-and-the-kestrel-powershell-deobfuscator/
+.. _Kestrel Data Retrieval Explained: https://opencybersecurityalliance.org/kestrel-data-retrieval-explained/
 
 .. _RSA Conference 2021: https://www.rsaconference.com/Library/presentation/USA/2021/The%20Game%20of%20Cyber%20Threat%20Hunting%20The%20Return%20of%20the%20Fun
 .. _RSA'21 session recording: https://www.youtube.com/watch?v=-Xb086R0JTk
 .. _SANS Threat Hunting Summit 2021: https://www.sans.org/blog/a-visual-summary-of-sans-threat-hunting-summit-2021/
 .. _SANS'21 session recording: https://www.youtube.com/watch?v=gyY5DAWLwT0
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
```

### Comparing `kestrel-lang-1.7.1/README.rst` & `kestrel-lang-1.7.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
 - Do NOT write the same TTP pattern in different data source queries.
 - Do NOT write one-time-use adapaters to connect hunt steps.
 - Do NOT waste your existing analytic scripts/programs in future hunts.
-- DD construct your hunt-flow from smaller reuseable hunt-flow.
+- Do construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -121,14 +121,15 @@
 
 #. `Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks`_
 #. `Practicing Backward And Forward Tracking Hunts on A Windows Host`_
 #. `Building Your Own Kestrel Analytics and Sharing With the Community`_
 #. `Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow`_
 #. `Try Kestrel in a Cloud Sandbox`_
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
+#. `Kestrel Data Retrieval Explained`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
 - 2023/08 `Black Hat USA 2023`_
@@ -186,14 +187,15 @@
 
 .. _Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks: https://opencybersecurityalliance.org/huntbook-persistent-threat-discovery-kestrel/
 .. _Practicing Backward And Forward Tracking Hunts on A Windows Host: https://opencybersecurityalliance.org/backward-and-forward-tracking-hunts-on-a-windows-host/
 .. _Building Your Own Kestrel Analytics and Sharing With the Community: https://opencybersecurityalliance.org/kestrel-custom-analytics/
 .. _Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow: https://opencybersecurityalliance.org/kestrel-sysflow-open-hunting-stack/
 .. _Try Kestrel in a Cloud Sandbox: https://opencybersecurityalliance.org/try-kestrel-in-a-cloud-sandbox/
 .. _Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator: https://opencybersecurityalliance.org/fun-with-securitydatasets-com-and-the-kestrel-powershell-deobfuscator/
+.. _Kestrel Data Retrieval Explained: https://opencybersecurityalliance.org/kestrel-data-retrieval-explained/
 
 .. _RSA Conference 2021: https://www.rsaconference.com/Library/presentation/USA/2021/The%20Game%20of%20Cyber%20Threat%20Hunting%20The%20Return%20of%20the%20Fun
 .. _RSA'21 session recording: https://www.youtube.com/watch?v=-Xb086R0JTk
 .. _SANS Threat Hunting Summit 2021: https://www.sans.org/blog/a-visual-summary-of-sans-threat-hunting-summit-2021/
 .. _SANS'21 session recording: https://www.youtube.com/watch?v=gyY5DAWLwT0
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
```

### Comparing `kestrel-lang-1.7.1/setup.cfg` & `kestrel-lang-1.7.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.7.1
+version = 1.7.2
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -23,26 +23,26 @@
 [options]
 packages = find:
 package_dir = 
 	=src
 scripts = bin/kestrel
 python_requires = >= 3.8
 install_requires = 
-	pyyaml
-	lxml
-	pandas
-	requests
-	nest-asyncio>=1.5.6
+	typeguard>=4.0.0
+	pyyaml>=6.0
+	lxml>=4.9.3
 	lark>=1.1.5
+	pandas>=2.0.0
 	pyarrow>=5.0.0
 	docker>=5.0.0
-	stix-shifter>=5.3.1
-	stix-shifter-utils>=5.3.1
-	firepit>=2.3.24
-	typeguard
+	requests>=2.31.0
+	nest-asyncio>=1.5.6
+	stix-shifter==5.3.1
+	stix-shifter-utils==5.3.1
+	firepit>=2.3.25
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
 
 [options.package_data]
```

### Comparing `kestrel-lang-1.7.1/src/kestrel/__main__.py` & `kestrel-lang-1.7.2/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.7.2/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/analytics/interface.py` & `kestrel-lang-1.7.2/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/analytics/manager.py` & `kestrel-lang-1.7.2/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/commands.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,23 +69,32 @@
             return var_struct, None
         else:
             return ret
 
     return wrapper
 
 
-def _guard_empty_input(func):
+def _skip_command_if_empty_input(func):
     @functools.wraps(func)
     def wrapper(stmt, session):
-        for varname in get_all_input_var_names(stmt):
-            v = session.symtable[varname]
-            if v.length + v.records_count == 0:
-                raise EmptyInputVariable(varname)
-        else:
+        var_names = get_all_input_var_names(stmt)
+        if not var_names:
+            return func(stmt, session)
+        elif any(
+            [
+                session.symtable[v].length + session.symtable[v].records_count
+                for v in var_names
+            ]
+        ):
             return func(stmt, session)
+        elif "output" in stmt:
+            var_struct = new_var(session.store, None, [], stmt, session.symtable)
+            return var_struct, None
+        else:
+            return None, None
 
     return wrapper
 
 
 def _debug_logger(func):
     @functools.wraps(func)
     def wrapper(stmt, session):
@@ -98,49 +107,40 @@
 ################################################################
 #                 Code Generation for Commands
 ################################################################
 
 
 @_debug_logger
 @_default_output
+@_skip_command_if_empty_input
 def assign(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
     transform = stmt.get("transformer")
     if transform:
         qry = _transform_query(session.store, entity_table, transform)
     else:
         qry = Query(entity_table)
-
     qry = _build_query(session.store, entity_table, qry, stmt, [])
-
-    try:
-        session.store.assign_query(stmt["output"], qry)
-        output = new_var(session.store, stmt["output"], [], stmt, session.symtable)
-    except InvalidAttr as e:
-        var_attr = str(e).split()[-1]
-        var_name, _, attr = var_attr.rpartition(".")
-        raise MissingEntityAttribute(var_name, attr) from e
-
-    return output, None
+    session.store.assign_query(stmt["output"], qry)
 
 
 @_debug_logger
 @_default_output
+@_skip_command_if_empty_input
 def merge(stmt, session):
     entity_types = list(
         set([session.symtable[var_name].type for var_name in stmt["inputs"]])
     )
     if len(entity_types) > 1:
         raise NonUniformEntityType(entity_types)
     entity_tables = [
         session.symtable[var_name].entity_table for var_name in stmt["inputs"]
     ]
+    entity_tables = [t for t in entity_tables if t is not None]
     session.store.merge(stmt["output"], entity_tables)
-    output = new_var(session.store, stmt["output"], [], stmt, session.symtable)
-    return output, None
 
 
 @_debug_logger
 @_default_output
 def new(stmt, session):
     stmt["type"] = load_data(session.store, stmt["output"], stmt["data"], stmt["type"])
 
@@ -150,23 +150,23 @@
 def load(stmt, session):
     stmt["type"] = load_data_file(
         session.store, stmt["output"], stmt["path"], stmt["type"]
     )
 
 
 @_debug_logger
-@_guard_empty_input
 def save(stmt, session):
     dump_data_to_file(
         session.store, session.symtable[stmt["input"]].entity_table, stmt["path"]
     )
     return None, None
 
 
 @_debug_logger
+@_skip_command_if_empty_input
 def info(stmt, session):
     header = session.store.columns(session.symtable[stmt["input"]].entity_table)
     direct_attrs, associ_attrs, custom_attrs, references = [], [], [], []
     for field in header:
         if field.startswith("x_"):
             custom_attrs.append(field)
         elif (
@@ -198,14 +198,15 @@
         session.symtable[stmt["input"]].dependent_variables
     )
 
     return None, DisplayDict(disp)
 
 
 @_debug_logger
+@_skip_command_if_empty_input
 def disp(stmt, session):
     entity_table = session.symtable[stmt["input"]].entity_table
     transform = stmt.get("transformer")
     if transform and entity_table:
         qry = _transform_query(session.store, entity_table, transform)
     else:
         qry = Query(entity_table)
@@ -220,14 +221,15 @@
     content = cursor.fetchall()
 
     return None, DisplayDataframe(dedup_ordered_dicts(remove_empty_dicts(content)))
 
 
 @_debug_logger
 @_default_output
+@_skip_command_if_empty_input
 def get(stmt, session):
     pattern = stmt["stixpattern"]
     local_var_table = stmt["output"] + "_local"
     return_var_table = stmt["output"]
     return_type = stmt["type"]
     limit = stmt.get("limit")
     display = None
@@ -292,15 +294,15 @@
             display = DisplayWarning(f'unknown entity type "{return_type}"')
 
     return output, display
 
 
 @_debug_logger
 @_default_output
-@_guard_empty_input
+@_skip_command_if_empty_input
 def find(stmt, session):
     # shortcuts
     return_type = stmt["type"]
     input_type = session.symtable[stmt["input"]].type
     local_var_table = stmt["output"] + "_local"
 
     # init
@@ -340,28 +342,28 @@
 
     output = new_var(session.store, return_var_table, [], stmt, session.symtable)
     return output, None
 
 
 @_debug_logger
 @_default_output
-@_guard_empty_input
+@_skip_command_if_empty_input
 def join(stmt, session):
     session.store.join(
         stmt["output"],
         session.symtable[stmt["input"]].entity_table,
         stmt["attribute_1"],
         session.symtable[stmt["input_2"]].entity_table,
         stmt["attribute_2"],
     )
 
 
 @_debug_logger
 @_default_output
-@_guard_empty_input
+@_skip_command_if_empty_input
 def group(stmt, session):
     if "aggregations" in stmt:
         aggs = [(i["func"], i["attr"], i["alias"]) for i in stmt["aggregations"]]
     else:
         aggs = None
     session.store.group(
         stmt["output"],
@@ -369,28 +371,28 @@
         stmt["attributes"],
         aggs,
     )
 
 
 @_debug_logger
 @_default_output
-@_guard_empty_input
+@_skip_command_if_empty_input
 def sort(stmt, session):
     session.store.assign(
         stmt["output"],
         session.symtable[stmt["input"]].entity_table,
         op="sort",
         by=stmt["attribute"],
         ascending=stmt["ascending"],
     )
 
 
 @_debug_logger
 @_default_output
-@_guard_empty_input
+@_skip_command_if_empty_input
 def apply(stmt, session):
     arg_vars = [session.symtable[v_name] for v_name in stmt["inputs"]]
     display = session.analytics_manager.execute(
         stmt["analytics_uri"], arg_vars, session.session_id, stmt["arguments"]
     )
     return None, display
```

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/data.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/display.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/prefetch.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/prefetch.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/queries.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/relations.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/codegen/summary.py` & `kestrel-lang-1.7.2/src/kestrel/codegen/summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Predicate,
     Count,
     Unique,
     Join,
 )
 from collections import OrderedDict
 from kestrel.codegen.relations import get_entity_id_attribute
-from kestrel.exceptions import KestrelInternalError
+from kestrel.exceptions import KestrelInternalError, MissingEntityAttribute
 
 
 def gen_variable_summary(var_name, var_struct):
     """Generate summary dictionary for a variable.
 
     Args:
 
@@ -88,11 +88,17 @@
     return query_ids
 
 
 def get_variable_entity_count(variable):
     entity_count = 0
     if variable.entity_table:
         entity_id_attr = get_entity_id_attribute(variable)
-        if entity_id_attr not in variable.store.columns(variable.entity_table):
-            return 0
-        entity_count = variable.store.count(variable.entity_table)
+        try:
+            columns = variable.store.columns(variable.entity_table)
+        except InvalidAttr as e:
+            # TODO: a better solution needed for tests/test_timestamped.py::test_timestamped_grouped_assign
+            table_attr = str(e).split()[-1]
+            table_name, _, attr = table_attr.rpartition(".")
+            raise MissingEntityAttribute(table_name, attr) from e
+        if entity_id_attr in columns:
+            entity_count = variable.store.count(variable.entity_table)
     return entity_count
```

### Comparing `kestrel-lang-1.7.1/src/kestrel/config.py` & `kestrel-lang-1.7.2/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/config.yaml` & `kestrel-lang-1.7.2/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/datasource/interface.py` & `kestrel-lang-1.7.2/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/datasource/manager.py` & `kestrel-lang-1.7.2/src/kestrel/datasource/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.7.2/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/exceptions.py` & `kestrel-lang-1.7.2/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/semantics/completor.py` & `kestrel-lang-1.7.2/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/semantics/processor.py` & `kestrel-lang-1.7.2/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/semantics/reference.py` & `kestrel-lang-1.7.2/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/session.py` & `kestrel-lang-1.7.2/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.7.2/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/syntax/parser.py` & `kestrel-lang-1.7.2/src/kestrel/syntax/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,18 +191,28 @@
         }
         for arg in args:
             if isinstance(arg, dict):
                 packet.update(arg)
         return packet
 
     def new(self, args):
+        if len(args) == 1:
+            # Try to get entity type from first entity
+            data = args[0]
+            if isinstance(data, list):
+                entity_type = data[0].get("type")
+            else:
+                entity_type = None
+        else:
+            entity_type = _first(args)
+            data = args[1]
         return {
             "command": "new",
-            "type": self._extract_entity_type(args),
-            "data": self._assert_and_extract_single("VAR_DATA", args),
+            "type": entity_type,
+            "data": data,
         }
 
     def expression(self, args):
         packet = args[0]
         for arg in args:
             packet.update(arg)
         return packet
@@ -232,21 +242,21 @@
 
     def expression_and(self, args):
         return ECGPJunction("AND", args[0], args[1])
 
     def comparison_std(self, args):
         etype, attr = _extract_entity_and_attribute(args[0].value)
         # remove more than one spaces; capitalize op
-        op = " ".join(_second(args).split()).upper()
+        op = args[1]
         value = args[2]
         return ECGPComparison(attr, op, value, etype)
 
     def comparison_null(self, args):
         etype, attr = _extract_entity_and_attribute(args[0].value)
-        op = _second(args)
+        op = args[1]
         if "NOT" in op:
             op = "!="
         else:
             op = "="
         value = "NULL"
         return ECGPComparison(attr, op, value, etype)
 
@@ -267,20 +277,17 @@
             variable = _first(args)
             attribute = _second(args)
             v = Reference(variable, attribute)
         else:
             v = _first(args)
         return v
 
-    def string(self, args):
+    def advanced_string(self, args):
         raw = _first(args)
-        if args[0].type == self.token_prefix + "SIMPLE_STRING":
-            value = raw
-        elif args[0].type == self.token_prefix + "ADVANCED_STRING":
-            value = unescape_quoted_string(raw)
+        value = unescape_quoted_string(raw)
         return value
 
     def number(self, args):
         v = _first(args)
         try:
             return int(v)
         except:
@@ -307,33 +314,73 @@
         return {
             "offset": int(_first(args)),
         }
 
     def timespan_relative(self, args):
         num = int(args[0])
         unit = args[1]
-        if unit.type == self.token_prefix + "DAY":
+        if unit == "DAY":
             delta = timedelta(days=num)
-        elif unit.type == self.token_prefix + "HOUR":
+        elif unit == "HOUR":
             delta = timedelta(hours=num)
-        elif unit.type == self.token_prefix + "MINUTE":
+        elif unit == "MINUTE":
             delta = timedelta(minutes=num)
-        elif unit.type == self.token_prefix + "SECOND":
+        elif unit == "SECOND":
             delta = timedelta(seconds=num)
         stop = datetime.utcnow()
         start = stop - delta
         return {"timerange": (start, stop)}
 
     def timespan_absolute(self, args):
         start = to_datetime(args[0])
         stop = to_datetime(args[1])
         return {"timerange": (start, stop)}
 
+    def day(self, _args):
+        return "DAY"
+
+    def hour(self, _args):
+        return "HOUR"
+
+    def minute(self, _args):
+        return "MINUTE"
+
+    def second(self, _args):
+        return "SECOND"
+
     def timestamp(self, args):
-        return self._assert_and_extract_single("ISOTIMESTAMP", args)
+        return args[0]
+
+    def var_data(self, args):
+        if isinstance(args[0], Token):
+            # Restore the brackets
+            v = "[" + _first(args) + "]"
+        else:
+            v = args[0]
+        return v
+
+    def json_objs(self, args):
+        return args
+
+    def json_obj(self, args):
+        return dict(args)
+
+    def json_pair(self, args):
+        v = _first(args)
+        if "ESCAPED_STRING" in args[0].type:
+            v = unescape_quoted_string(v)
+        return v, args[1]
+
+    def json_value(self, args):
+        v = _first(args)
+        if args[0].type == self.token_prefix + "ESCAPED_STRING":
+            v = unescape_quoted_string(v)
+        elif args[0].type == self.token_prefix + "NUMBER":
+            v = float(v) if "." in v else int(v)
+        return v
 
     def entity_type(self, args):
         return _first(args)
 
     def variables(self, args):
         return {"variables": self._extract_vars(args)}
 
@@ -370,15 +417,15 @@
             # bin_func
             return item
 
     def bin_func(self, args):
         attr = _first(args)
         num = int(_second(args))
         if len(args) >= 3:
-            unit = _third(args)
+            unit = args[2][0]  # Only pass 1st letter (d, h, m, or s)
         else:
             unit = None
         alias = f"{attr}_bin"
         return BinnedColumn(attr, num, unit, alias=alias)
 
     def agg_list(self, args):
         return [arg for arg in args]
@@ -394,14 +441,23 @@
         for di in args:
             d.update(di)
         return {"arguments": d}
 
     def arg_kv_pair(self, args):
         return {_first(args): args[1]}
 
+    def op(self, args):
+        return " ".join([arg.upper() for arg in args])
+
+    def op_keyword(self, args):
+        return _first(args)
+
+    def null_op(self, args):
+        return " ".join([arg.upper() for arg in args])
+
     def _extract_vars(self, args):
         var_names = []
         for arg in args:
             if hasattr(arg, "type") and arg.type == self.token_prefix + "VARIABLE":
                 var_names.append(arg.value)
         if not var_names:
             var_names = [self.default_variable]
```

### Comparing `kestrel-lang-1.7.1/src/kestrel/syntax/reference.py` & `kestrel-lang-1.7.2/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/syntax/utils.py` & `kestrel-lang-1.7.2/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel/utils.py` & `kestrel-lang-1.7.2/src/kestrel/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.7.2/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.7.2/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.7.2/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.7.2/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 PROFILE_PATH_DEFAULT = CONFIG_DIR_DEFAULT / "stixshifter.yaml"
 PROFILE_PATH_ENV_VAR = "KESTREL_STIXSHIFTER_CONFIG"
 STIXSHIFTER_DEBUG_ENV_VAR = "KESTREL_STIXSHIFTER_DEBUG"  # debug mode for stix-shifter if the environment variable exists
 ENV_VAR_PREFIX = "STIXSHIFTER_"
 RETRIEVAL_BATCH_SIZE = 2000
 SINGLE_BATCH_TIMEOUT = 60
+COOL_DOWN_AFTER_TRANSMISSION = 0
 FAST_TRANSLATE_CONNECTORS = []  # Suggested: ["qradar", "elastic_ecs"]
 
 
 _logger = logging.getLogger(__name__)
 
 
 def set_stixshifter_logging_level():
@@ -135,53 +136,46 @@
                 "stixshifter",
                 f'invalid {profile_name} configuration section: no "auth" field',
             )
 
         if "options" not in connection:
             connection["options"] = {}
 
-        retrieval_batch_size = RETRIEVAL_BATCH_SIZE
-        if "retrieval_batch_size" in connection["options"]:
-            # remove the non-stix-shifter field "retrieval_batch_size" to avoid stix-shifter error
-            try:
-                retrieval_batch_size = int(
-                    connection["options"].pop("retrieval_batch_size")
-                )
-            except:
-                raise InvalidDataSource(
-                    profile_name,
-                    "stixshifter",
-                    f"invalid {profile_name} connection section: options.retrieval_batch_size",
-                )
-            # rename this field for stix-shifter use; x2 the size to ensure retrieval
-            _logger.debug(
-                f"profile-loaded retrieval_batch_size: {retrieval_batch_size}"
-            )
+        retrieval_batch_size = _extract_integer_param_from_connection_config(
+            "retrieval_batch_size",
+            RETRIEVAL_BATCH_SIZE,
+            connection,
+            profile_name,
+        )
+        # rename this field for stix-shifter use; x2 the size to ensure retrieval
         connection["options"]["result_limit"] = retrieval_batch_size * 2
 
-        single_batch_timeout = SINGLE_BATCH_TIMEOUT
-        if "single_batch_timeout" in connection["options"]:
-            # remove the non-stix-shifter field "single_batch_timeout" to avoid stix-shifter error
-            try:
-                single_batch_timeout = int(
-                    connection["options"].pop("single_batch_timeout")
-                )
-            except:
-                raise InvalidDataSource(
-                    profile_name,
-                    "stixshifter",
-                    f"invalid {profile_name} connection section: options.single_batch_timeout",
-                )
-            # rename this field for stix-shifter use
-            _logger.debug(
-                f"profile-loaded single_batch_timeout: {single_batch_timeout}"
-            )
+        single_batch_timeout = _extract_integer_param_from_connection_config(
+            "single_batch_timeout",
+            SINGLE_BATCH_TIMEOUT,
+            connection,
+            profile_name,
+        )
+        # rename this field for stix-shifter use
         connection["options"]["timeout"] = single_batch_timeout
 
-    return connector_name, connection, configuration, retrieval_batch_size
+        cool_down_after_transmission = _extract_integer_param_from_connection_config(
+            "cool_down_after_transmission",
+            COOL_DOWN_AFTER_TRANSMISSION,
+            connection,
+            profile_name,
+        )
+
+    return (
+        connector_name,
+        connection,
+        configuration,
+        retrieval_batch_size,
+        cool_down_after_transmission,
+    )
 
 
 def load_profiles():
     config = load_user_config(PROFILE_PATH_ENV_VAR, PROFILE_PATH_DEFAULT)
     if config and "profiles" in config:
         _logger.debug(f"stix-shifter profiles found in config file")
         profiles_from_file = {k.lower(): v for k, v in config["profiles"].items()}
@@ -208,7 +202,25 @@
     if "fast_translate" not in config["options"]:
         config["options"]["fast_translate"] = FAST_TRANSLATE_CONNECTORS
     if "translation_workers_count" not in config["options"]:
         config["options"]["translation_workers_count"] = min(
             2, max(1, multiprocessing.cpu_count() - 2)
         )
     return config["options"]
+
+
+def _extract_integer_param_from_connection_config(
+    param_name, default, connection, profile_name
+):
+    value = default
+    if param_name in connection["options"]:
+        # remove the non-stix-shifter field {param_name} to avoid stix-shifter error
+        try:
+            value = int(connection["options"].pop(param_name))
+        except:
+            raise InvalidDataSource(
+                profile_name,
+                "stixshifter",
+                f"invalid {profile_name} connection section: options.{param_name}",
+            )
+        _logger.debug(f"profile-loaded {param_name}: {value}")
+    return value
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                     host: elastic.securitylog.company.com
                     port: 9200
                     selfSignedCert: false # this means do NOT check cert
                     indices: host101
                     options:  # use any of this section when needed
                         retrieval_batch_size: 10000  # set to 10000 to match default Elasticsearch page size; Kestrel default across connectors: 2000
                         single_batch_timeout: 120  # increase it if hit 60 seconds (Kestrel default) timeout error for each batch of retrieval
+                        cool_down_after_transmission: 2  # seconds to cool down between data source API calls, required by some API such as sentinelone; Kestrel default: 0
                         dialects:  # more info: https://github.com/opencybersecurityalliance/stix-shifter/tree/develop/stix_shifter_modules/elastic_ecs#dialects
                           - beats  # need it if the index is created by Filebeat/Winlogbeat/*beat
                 config:
                     auth:
                         id: VuaCfGcBCdbkQm-e5aOx
                         api_key: ui2lp2axTNmsyakw9tvNnw
             host102:
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 @typechecked
 def transmit(
     connector_name: str,
     connection_dict: dict,
     configuration_dict: dict,
     retrieval_batch_size: int,
     translators_count: int,
+    cool_down_after_transmission: int,
     queries: list,
     raw_records_queue: Queue,
     limit: Optional[int],
 ):
     _logger.debug(f"{translators_count} translation workers to be started")
     transmitter_pool = TransmitterPool(
         connector_name,
         connection_dict,
         configuration_dict,
         retrieval_batch_size,
         translators_count,
+        cool_down_after_transmission,
         queries,
         raw_records_queue,
         limit,
     )
 
     try:
         transmitter_pool.start()
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/query.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         # So only give STIX-shifter a copy of the configs.
         # Check `modernize` functions in the `stix_shifter_utils` for details.
         (
             connector_name,
             connection_dict,
             configuration_dict,
             retrieval_batch_size,
+            cool_down_after_transmission,
         ) = map(
             copy.deepcopy, get_datasource_from_profiles(profile, config["profiles"])
         )
 
         check_module_availability(connector_name)
 
         if _logger.isEnabledFor(logging.DEBUG):
@@ -116,14 +117,15 @@
         ):
             with multiproc.transmit(
                 connector_name,
                 connection_dict,
                 configuration_dict,
                 retrieval_batch_size,
                 config["options"]["translation_workers_count"],
+                cool_down_after_transmission,
                 dsl["queries"],
                 raw_records_queue,
                 profile_limit,
             ):
                 for result in multiproc.read_translated_results(
                     translated_data_queue,
                     config["options"]["translation_workers_count"],
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,39 @@
     def __init__(
         self,
         connector_name: str,
         connection_dict: dict,
         configuration_dict: dict,
         retrieval_batch_size: int,
         number_of_translators: int,
+        cool_down_after_transmission: int,
         queries: list,
         output_queue: Queue,
         limit: Optional[int],
     ):
         super().__init__()
 
         self.connector_name = connector_name
         self.connection_dict = connection_dict
         self.configuration_dict = configuration_dict
         self.retrieval_batch_size = retrieval_batch_size
         self.number_of_translators = number_of_translators
+        self.cool_down_after_transmission = cool_down_after_transmission
         self.queries = queries
         self.queue = output_queue
         self.limit = limit
 
     def run(self):
         transmitters = [
             Transmitter(
                 self.connector_name,
                 self.connection_dict,
                 self.configuration_dict,
                 self.retrieval_batch_size,
+                self.cool_down_after_transmission,
                 query,
                 self.queue,
                 self.limit,
             )
             for query in self.queries
         ]
         for transmitter in transmitters:
@@ -57,24 +60,26 @@
 class Transmitter(Process):
     def __init__(
         self,
         connector_name: str,
         connection_dict: dict,
         configuration_dict: dict,
         retrieval_batch_size: int,
+        cool_down_after_transmission: int,
         query: str,
         output_queue: Queue,
         limit: Optional[int],
     ):
         super().__init__()
 
         self.connector_name = connector_name
         self.connection_dict = connection_dict
         self.configuration_dict = configuration_dict
         self.retrieval_batch_size = retrieval_batch_size
+        self.cool_down_after_transmission = cool_down_after_transmission
         self.query = query
         self.queue = output_queue
         self.limit = limit
 
     def run(self):
         self.worker_name = current_process().name
         self.transmission = stix_transmission.StixTransmission(
@@ -112,16 +117,18 @@
         status = {"success": True, "progress": 0, "status": "KINIT"}
 
         while (
             status["success"]
             and status["progress"] < 100
             and status["status"] in ("KINIT", "RUNNING")
         ):
-            if status["status"] == "RUNNING":
-                time.sleep(1)
+            if status["status"] == "KINIT":
+                time.sleep(self.cool_down_after_transmission)
+            elif status["status"] == "RUNNING":
+                time.sleep(max(1, self.cool_down_after_transmission))
             status = self.transmission.status(self.search_id)
             if not status["success"]:
                 err_msg = (
                     status["error"] if "error" in status else "details not avaliable"
                 )
                 packet = TransmissionResult(
                     self.worker_name,
@@ -144,14 +151,15 @@
         is_retry_cycle = False
         batch_size = self.retrieval_batch_size
         if self.limit and self.limit < self.retrieval_batch_size:
             batch_size = self.limit
 
         while has_remaining_results:
             packet = None
+            time.sleep(self.cool_down_after_transmission)
             result_batch = self.transmission.results(
                 self.search_id,
                 result_retrieval_offset,
                 batch_size,
                 metadata,
             )
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.7.2/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.1
+Version: 1.7.2
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 hunt-flow is to hunts as control-flow is to ordinary programs.
 
 What does it mean by *hunt fast*?
 
 - Do NOT write the same TTP pattern in different data source queries.
 - Do NOT write one-time-use adapaters to connect hunt steps.
 - Do NOT waste your existing analytic scripts/programs in future hunts.
-- DD construct your hunt-flow from smaller reuseable hunt-flow.
+- Do construct your hunt-flow from smaller reuseable hunt-flow.
 - Do share your huntbook with your future self and your colleagues.
 - Do get interactive feedback and revise hunt-flow on the fly.
 
 |
 
 .. image:: https://github.com/opencybersecurityalliance/data-bucket-kestrel/raw/main/images/github_homepage_animation.gif
    :width: 90%
@@ -140,14 +140,15 @@
 
 #. `Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks`_
 #. `Practicing Backward And Forward Tracking Hunts on A Windows Host`_
 #. `Building Your Own Kestrel Analytics and Sharing With the Community`_
 #. `Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow`_
 #. `Try Kestrel in a Cloud Sandbox`_
 #. `Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator`_
+#. `Kestrel Data Retrieval Explained`_
 
 Talks And Demos
 ===============
 
 Talk summary (visit `Kestrel documentation on talks`_ to learn details):
 
 - 2023/08 `Black Hat USA 2023`_
@@ -205,14 +206,15 @@
 
 .. _Building a Huntbook to Discover Persistent Threats from Scheduled Windows Tasks: https://opencybersecurityalliance.org/huntbook-persistent-threat-discovery-kestrel/
 .. _Practicing Backward And Forward Tracking Hunts on A Windows Host: https://opencybersecurityalliance.org/backward-and-forward-tracking-hunts-on-a-windows-host/
 .. _Building Your Own Kestrel Analytics and Sharing With the Community: https://opencybersecurityalliance.org/kestrel-custom-analytics/
 .. _Setting Up The Open Hunting Stack in Hybrid Cloud With Kestrel and SysFlow: https://opencybersecurityalliance.org/kestrel-sysflow-open-hunting-stack/
 .. _Try Kestrel in a Cloud Sandbox: https://opencybersecurityalliance.org/try-kestrel-in-a-cloud-sandbox/
 .. _Fun with securitydatasets.com and the Kestrel PowerShell Deobfuscator: https://opencybersecurityalliance.org/fun-with-securitydatasets-com-and-the-kestrel-powershell-deobfuscator/
+.. _Kestrel Data Retrieval Explained: https://opencybersecurityalliance.org/kestrel-data-retrieval-explained/
 
 .. _RSA Conference 2021: https://www.rsaconference.com/Library/presentation/USA/2021/The%20Game%20of%20Cyber%20Threat%20Hunting%20The%20Return%20of%20the%20Fun
 .. _RSA'21 session recording: https://www.youtube.com/watch?v=-Xb086R0JTk
 .. _SANS Threat Hunting Summit 2021: https://www.sans.org/blog/a-visual-summary-of-sans-threat-hunting-summit-2021/
 .. _SANS'21 session recording: https://www.youtube.com/watch?v=gyY5DAWLwT0
 .. _BlackHat Europe 2021: https://www.blackhat.com/eu-21/arsenal/schedule/index.html#an-open-stack-for-threat-hunting-in-hybrid-cloud-with-connected-observability-25112
 .. _Infosec Jupyterthon 2021: https://infosecjupyterthon.com/2021/agenda.html
```

### Comparing `kestrel-lang-1.7.1/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.7.2/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_cli.py` & `kestrel-lang-1.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_assign.py` & `kestrel-lang-1.7.2/tests/test_command_assign.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,7 +85,17 @@
         assert 'binary_ref' in p[0]
         s.execute(REF_PROCS)
         s.execute("q = p WHERE pid IN (ref.pid, 9240, 10020)")
         q = s.get_variable("q", False)
         assert len(q) == 106 + 149 + 1 + 1
         print(q[0])
         assert 'binary_ref' in q[0]
+
+
+def test_assign_from_empty_var(proc_bundle_file):
+    with Session() as s:
+        s.execute(f"p = GET process FROM file://{proc_bundle_file} WHERE [process:pid < 0]")
+        s.execute(REF_PROCS)
+        s.execute("q = p WHERE pid = ref.pid")
+        q = s.symtable["q"]
+        assert len(q) == 0
+        assert q.records_count == 0
```

### Comparing `kestrel-lang-1.7.1/tests/test_command_disp.py` & `kestrel-lang-1.7.2/tests/test_command_disp.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,7 +74,25 @@
         df = pd.DataFrame.from_records(data)
         assert df.columns.tolist() == ["src_ref.value", "src_port"]
 
         out = s.execute("DISP TIMESTAMPED(conns) ATTR src_ref.value, src_port")
         data = out[0].to_dict()["data"]
         df = pd.DataFrame.from_records(data)
         assert df.columns.tolist() == ["first_observed", "src_ref.value", "src_port"]
+
+
+def test_disp_empty_variable():
+    with Session() as s:
+        stmt = """
+newvar = NEW [ {"type": "network-traffic", "src_ref.value": "1.2.3.4", "dst_ref.value": "4.3.2.1"}
+             , {"type": "network-traffic", "src_ref.value": "2.2.3.4", "dst_ref.value": "4.3.2.1"}
+             , {"type": "network-traffic", "src_ref.value": "1.2.3.4", "dst_ref.value": "5.3.2.1"}
+             ]
+
+v2 = GET network-traffic FROM newvar
+     WHERE dst_ref.value = '1.2.3.4'
+
+DISP v2
+"""
+        s.execute(stmt)
+        out = s.execute("DISP v2")
+        assert out == []
```

### Comparing `kestrel-lang-1.7.1/tests/test_command_find.py` & `kestrel-lang-1.7.2/tests/test_command_find.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 @pytest.fixture
 def proc_bundle_file():
     cwd = os.path.dirname(os.path.abspath(__file__))
     return os.path.join(cwd, "doctored-1k.json")
 
 
-def test_return_table_not_exist(fake_bundle_file):
+def test_return_table_not_exist(set_empty_kestrel_config, fake_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         from file://{fake_bundle_file}
                         where [network-traffic:dst_port = 22]
                 procs = FIND process CREATED conns
                 """
@@ -55,41 +55,41 @@
         },
     }
     output_dict = summaries[0].to_dict()
     del output_dict["data"]["execution time"]
     assert output_dict == correct_dict
 
 
-def test_find_srcs(fake_bundle_file):
+def test_find_srcs(set_empty_kestrel_config, fake_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         from file://{fake_bundle_file}
                         where dst_port = 22
                 srcs = FIND ipv4-addr CREATED conns
                 """
         s.execute(stmt)
         srcs = s.get_variable("srcs")
         assert len(srcs) == 24
 
 
-def test_find_srcs_limit(fake_bundle_file):
+def test_find_srcs_limit(set_empty_kestrel_config, fake_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         from file://{fake_bundle_file}
                         where dst_port = 22
                 srcs = FIND ipv4-addr CREATED conns LIMIT 1
                 """
         s.execute(stmt)
         srcs = s.get_variable("srcs")
         assert len(srcs) == 1
 
 
-def test_find_file_linked_to_process(proc_bundle_file):
+def test_find_file_linked_to_process(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where command_line LIKE 'wmic%'
                 files = FIND file LINKED procs
                 """
@@ -98,15 +98,15 @@
         print(json.dumps(procs, indent=4))
         assert len(procs) == 7
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 4
 
 
-def test_find_file_linked_to_process_limit_1(proc_bundle_file):
+def test_find_file_linked_to_process_limit_1(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where command_line LIKE 'wmic%'
                 files = FIND file LINKED procs LIMIT 1
                 """
@@ -115,15 +115,15 @@
         print(json.dumps(procs, indent=4))
         assert len(procs) == 7
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 1
 
 
-def test_find_file_linked_to_process_limit_2(proc_bundle_file):
+def test_find_file_linked_to_process_limit_2(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where command_line LIKE 'wmic%'
                 files = FIND file LINKED procs LIMIT 10
                 """
@@ -132,15 +132,15 @@
         print(json.dumps(procs, indent=4))
         assert len(procs) == 7
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 4
 
 
-def test_find_file_linked_to_process_2():
+def test_find_file_linked_to_process_2(set_empty_kestrel_config):
     stixshifter_data_url = "https://raw.githubusercontent.com/opencybersecurityalliance/stix-shifter/develop/data/cybox"
     bundle = f"{stixshifter_data_url}/carbon_black/cb_observed_156.json"
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from {bundle}
                         where [process:name = 'svctest.exe']
@@ -148,15 +148,15 @@
                 """
         s.execute(stmt)
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 3
 
 
-def test_find_file_linked_to_process_2_limit():
+def test_find_file_linked_to_process_2_limit(set_empty_kestrel_config):
     stixshifter_data_url = "https://raw.githubusercontent.com/opencybersecurityalliance/stix-shifter/develop/data/cybox"
     bundle = f"{stixshifter_data_url}/carbon_black/cb_observed_156.json"
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from {bundle}
                         where [process:name = 'svctest.exe']
@@ -164,15 +164,15 @@
                 """
         s.execute(stmt)
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 2
 
 
-def test_find_file_loaded_by_process(proc_bundle_file):
+def test_find_file_loaded_by_process(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where command_line LIKE 'wmic%'
                 files = FIND file LOADED BY procs
                 """
@@ -181,57 +181,57 @@
         print(json.dumps(procs, indent=4))
         assert len(procs) == 7
         files = s.get_variable("files")
         print(json.dumps(files, indent=4))
         assert len(files) == 1
 
 
-def test_find_process_created_process(proc_bundle_file):
+def test_find_process_created_process(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where command_line LIKE 'wmic%'
                 parents = FIND process CREATED procs
                 """
         s.execute(stmt)
         data = s.get_variable("parents")
         print(json.dumps(data, indent=4))
         assert len(data)
 
 
-def test_find_refs_resolution_not_reversed_src_ref(proc_bundle_file):
+def test_find_refs_resolution_not_reversed_src_ref(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 nt = get network-traffic
                      from file://{proc_bundle_file}
                      where src_port > 0
                 p = FIND process CREATED nt
                 """
         s.execute(stmt)
         p = s.get_variable("p")
         # assert len(p) == 948  # grep -c opened_connection_refs tests/doctored-1k.json
         assert len(p) >= 948  # FIXME: duplicate process objects
 
 
-def test_find_refs_resolution_not_reversed_src_ref_limit(proc_bundle_file):
+def test_find_refs_resolution_not_reversed_src_ref_limit(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 nt = get network-traffic
                      from file://{proc_bundle_file}
                      where src_port > 0
                 p = FIND process CREATED nt LIMIT 10
                 """
         s.execute(stmt)
         p = s.get_variable("p")
         # assert len(p) == 948  # grep -c opened_connection_refs tests/doctored-1k.json
         assert len(p) == 10
  
 
-def test_find_refs_resolution_reversed_src_ref(proc_bundle_file):
+def test_find_refs_resolution_reversed_src_ref(set_empty_kestrel_config, proc_bundle_file):
     with Session(debug_mode=True) as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where name LIKE '%'
                 conns = FIND network-traffic CREATED BY procs
                 """
@@ -243,15 +243,15 @@
 
         # DISP with a ref (parent_ref) and ambiguous column (command_line)
         disp_out = s.execute("DISP procs ATTR name, parent_ref.name, command_line")
         data = disp_out[0].to_dict()["data"]
         print(json.dumps(data, indent=4))
 
 
-def test_find_refs_resolution_reversed_src_ref_limit(proc_bundle_file):
+def test_find_refs_resolution_reversed_src_ref_limit(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 procs = get process
                         from file://{proc_bundle_file}
                         where name LIKE '%'
                 conns = FIND network-traffic CREATED BY procs LIMIT 10
                 """
@@ -263,15 +263,15 @@
 
         # DISP with a ref (parent_ref) and ambiguous column (command_line)
         disp_out = s.execute("DISP procs ATTR name, parent_ref.name, command_line")
         data = disp_out[0].to_dict()["data"]
         print(json.dumps(data, indent=4))
 
 
-def test_find_without_where_ext_pattern(proc_bundle_file):
+def test_find_without_where_ext_pattern(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         FROM file://{proc_bundle_file}
                         WHERE network-traffic:src_ref.value = '127.0.0.1'
 
                 procs = FIND process CREATED conns
@@ -308,15 +308,15 @@
         assert len(conns) == 193
         assert conns.records_count == 203
 
         assert len(procs) == 203
         assert procs.records_count == 203
 
 
-def test_find_with_limit(proc_bundle_file):
+def test_find_with_limit(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         FROM file://{proc_bundle_file}
                         WHERE network-traffic:src_ref.value = '127.0.0.1'
 
                 procs = FIND process CREATED conns LIMIT 100
@@ -329,15 +329,15 @@
         assert len(conns) == 193
         assert conns.records_count == 203
 
         assert len(procs) == 100
         assert procs.records_count == 100
 
 
-def test_find_with_where_centered_pattern(proc_bundle_file):
+def test_find_with_where_centered_pattern(set_empty_kestrel_config, proc_bundle_file):
     with Session() as s:
         stmt = f"""
                 conns = get network-traffic
                         FROM file://{proc_bundle_file}
                         WHERE network-traffic:src_ref.value = '127.0.0.1'
 
                 procs = FIND process CREATED conns
@@ -349,7 +349,29 @@
         procs = s.symtable["procs"]
 
         assert len(conns) == 193
         assert conns.records_count == 203
 
         assert len(procs) == 1
         assert procs.records_count == 1
+
+
+def test_find_from_empty_input(set_empty_kestrel_config, proc_bundle_file):
+    with Session() as s:
+        stmt = f"""
+                conns = get network-traffic
+                        FROM file://{proc_bundle_file}
+                        WHERE network-traffic:src_ref.value = '100.0.0.1'
+
+                procs = FIND process CREATED conns
+                        WHERE name = 'vmware.exe'
+                """
+        s.execute(stmt)
+
+        conns = s.symtable["conns"]
+        procs = s.symtable["procs"]
+
+        assert len(conns) == 0
+        assert conns.records_count == 0
+
+        assert len(procs) == 0
+        assert procs.records_count == 0
```

### Comparing `kestrel-lang-1.7.1/tests/test_command_get.py` & `kestrel-lang-1.7.2/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_group.py` & `kestrel-lang-1.7.2/tests/test_command_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,7 +139,28 @@
         assert len(hist) == 3
         assert hist[0]["src_port_bin"] == 40000
         assert hist[0]["count"] == 4
         assert hist[1]["src_port_bin"] == 50000
         assert hist[1]["count"] == 69
         assert hist[2]["src_port_bin"] == 60000
         assert hist[2]["count"] == 27
+
+
+def test_group_empty_variable(fake_bundle_file):
+    with Session(debug_mode=True) as session:
+        session.execute(
+            f"""conns = get network-traffic
+            from file://{fake_bundle_file}
+            where [network-traffic:dst_port < 0]
+            src_grps = group conns by src_ref.value""",
+        )
+
+        conns = session.symtable["conns"]
+        srcgrps = session.symtable["src_grps"]
+
+        assert len(conns) == 0
+        assert conns.records_count == 0
+
+        assert len(srcgrps) == 0
+        assert srcgrps.records_count == 0
+
+
```

### Comparing `kestrel-lang-1.7.1/tests/test_command_internal.py` & `kestrel-lang-1.7.2/tests/test_command_internal.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_join.py` & `kestrel-lang-1.7.2/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_load.py` & `kestrel-lang-1.7.2/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_merge.py` & `kestrel-lang-1.7.2/tests/test_command_merge.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,7 +35,22 @@
 
         ip3 = s.get_variable("ip3")
         assert len(ip3) == 5
         assert ip3[0]["type"] == "ipv4-addr"
         values = [row["value"] for row in ip3]
         values.sort()
         assert values == ["10.0.1.1", "10.0.2.2", "10.0.3.3", "127.0.0.1", "127.0.1.15"]
+
+
+def test_merge_empty_vars():
+    with Session() as s:
+        stmt = """
+newips = NEW ipv4-addr ["127.0.0.1", "127.0.1.15"]
+ip1 = GET ipv4-addr FROM newips WHERE value = '10.0.0.1'
+ip2 = GET ipv4-addr FROM newips WHERE value = '10.0.0.2'
+ip3 = ip1 + ip2
+"""
+        s.execute(stmt)
+
+        ip3 = s.symtable["ip3"]
+        assert len(ip3) == 0
+        assert ip3.records_count == 0
```

### Comparing `kestrel-lang-1.7.1/tests/test_command_new.py` & `kestrel-lang-1.7.2/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_command_save.py` & `kestrel-lang-1.7.2/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_completion.py` & `kestrel-lang-1.7.2/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_display.py` & `kestrel-lang-1.7.2/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_exceptions.py` & `kestrel-lang-1.7.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_expressions.py` & `kestrel-lang-1.7.2/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_parser.py` & `kestrel-lang-1.7.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_python_analytics.py` & `kestrel-lang-1.7.2/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_records.py` & `kestrel-lang-1.7.2/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_session.py` & `kestrel-lang-1.7.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.1/tests/test_stixshifter.py` & `kestrel-lang-1.7.2/tests/test_stixshifter.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         connection:
             host: elastic.securitylog.company.com
             port: 9200
             indices: host101
             options:
                 retrieval_batch_size: 10000
                 single_batch_timeout: 120
+                cool_down_after_transmission: 5
                 dialects:
                     - beats
         config:
             auth:
                 id: profileB
                 api_key: asdf
 """
@@ -74,31 +75,33 @@
 """
         s.execute(stmt)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         ss_config = s.config["datasources"]["kestrel_datasource_stixshifter"]
         ss_profiles = ss_config["profiles"]
-        connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
+        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileA"
         assert configuration["auth"]["api_key"] == "qwer"
         assert connection["options"]["timeout"] == 60
         assert connection["options"]["result_limit"] == 2000 * 2
         assert retrieval_batch_size == 2000
+        assert cool_down_after_transmission == 0
 
         with open(profile_file, "w") as pf:
             pf.write(profileB)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         # need to refresh the pointers since the dict is updated
         ss_profiles = ss_config["profiles"]
-        connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
+        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileB"
         assert configuration["auth"]["api_key"] == "asdf"
         assert connection["options"]["timeout"] == 120
         assert connection["options"]["result_limit"] == 10000 * 2
         assert retrieval_batch_size == 10000
+        assert cool_down_after_transmission == 5
 
     del os.environ["KESTREL_STIXSHIFTER_CONFIG"]
```

### Comparing `kestrel-lang-1.7.1/tests/test_stixshifter_translator.py` & `kestrel-lang-1.7.2/tests/test_stixshifter_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,14 @@
             assert isinstance(result, pandas.DataFrame)
             assert result.empty == False
 
     for translator in translators:
         assert translator.is_alive() == False
 
 
-@pytest.mark.skip(reason="kestrel v1.7.1 released with issue #370 unfixed")
 def test_stixshifter_fast_translate_with_parquet_writing_to_disk(tmpdir):
     query_id = "8df266aa-2901-4a94-ace9-a4403e310fa1"
     check_module_availability(CONNECTOR_NAME)
     cache_parquet_path_prefix = str(tmpdir.join("test"))
     offset_str = str(SAMPLE_RESULT.offset).zfill(32)
     cache_parquet_path = cache_parquet_path_prefix + f"_{offset_str}.parquet"
```

### Comparing `kestrel-lang-1.7.1/tests/test_timestamped.py` & `kestrel-lang-1.7.2/tests/test_timestamped.py`

 * *Files identical despite different names*

