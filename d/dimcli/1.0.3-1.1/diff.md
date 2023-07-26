# Comparing `tmp/dimcli-1.0.3.tar.gz` & `tmp/dimcli-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimcli-1.0.3.tar", last modified: Tue May 23 13:59:47 2023, max compression
+gzip compressed data, was "dimcli-1.1.tar", last modified: Wed Jul 26 10:35:09 2023, max compression
```

## Comparing `dimcli-1.0.3.tar` & `dimcli-1.1.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.797957 dimcli-1.0.3/
--rw-r--r--   0 michele.pasin   (501) staff       (20)     1070 2018-05-18 16:18:19.000000 dimcli-1.0.3/LICENSE
--rw-r--r--   0 michele.pasin   (501) staff       (20)       59 2021-12-22 19:09:31.000000 dimcli-1.0.3/MANIFEST.in
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2373 2023-05-23 13:59:47.798066 dimcli-1.0.3/PKG-INFO
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2064 2022-06-19 21:07:50.000000 dimcli-1.0.3/README.md
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.774594 dimcli-1.0.3/dimcli/
--rw-r--r--   0 michele.pasin   (501) staff       (20)      398 2023-05-23 13:25:52.000000 dimcli-1.0.3/dimcli/VERSION.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     6013 2022-07-18 17:33:07.000000 dimcli-1.0.3/dimcli/__init__.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.782316 dimcli-1.0.3/dimcli/core/
--rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-04-10 08:16:04.000000 dimcli-1.0.3/dimcli/core/__init__.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    38909 2022-07-18 16:47:50.000000 dimcli-1.0.3/dimcli/core/api.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    13005 2022-07-18 17:15:49.000000 dimcli-1.0.3/dimcli/core/auth.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    14418 2022-06-30 15:51:01.000000 dimcli-1.0.3/dimcli/core/dataframe_factory.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    10195 2022-05-09 14:13:01.000000 dimcli-1.0.3/dimcli/core/dsl_grammar.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    69745 2020-04-01 21:04:32.000000 dimcli-1.0.3/dimcli/core/dsl_grammar_categories.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)   198407 2023-05-23 13:25:12.000000 dimcli-1.0.3/dimcli/core/dsl_grammar_core.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)   196722 2023-02-17 16:05:21.000000 dimcli-1.0.3/dimcli/core/dsl_grammar_core_BK.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     3656 2023-02-17 12:05:13.000000 dimcli-1.0.3/dimcli/core/dsl_grammar_extras.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2540 2020-10-23 13:00:00.000000 dimcli-1.0.3/dimcli/core/extras.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    24468 2021-10-14 15:35:08.000000 dimcli-1.0.3/dimcli/core/functions.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      162 2020-10-14 17:11:47.000000 dimcli-1.0.3/dimcli/functions.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.783118 dimcli-1.0.3/dimcli/jupyter/
--rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-03-30 19:27:13.000000 dimcli-1.0.3/dimcli/jupyter/__init__.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    21234 2022-07-01 11:10:39.000000 dimcli-1.0.3/dimcli/jupyter/magics.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     3715 2020-10-22 09:03:53.000000 dimcli-1.0.3/dimcli/main_cli.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.786113 dimcli-1.0.3/dimcli/repl/
--rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-01-25 16:54:16.000000 dimcli-1.0.3/dimcli/repl/__init__.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     8035 2020-10-12 14:58:02.000000 dimcli-1.0.3/dimcli/repl/autocompletion.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      871 2021-11-25 16:17:17.000000 dimcli-1.0.3/dimcli/repl/history.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      758 2019-02-21 16:01:09.000000 dimcli-1.0.3/dimcli/repl/key_bindings.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     3335 2020-10-12 14:58:02.000000 dimcli-1.0.3/dimcli/repl/lexer.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    11364 2021-12-08 18:01:01.000000 dimcli-1.0.3/dimcli/repl/repl.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      438 2019-02-07 12:19:35.000000 dimcli-1.0.3/dimcli/repl/validator.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      304 2020-10-23 12:59:36.000000 dimcli-1.0.3/dimcli/shortcuts.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.786589 dimcli-1.0.3/dimcli/templates/
--rw-r--r--   0 michele.pasin   (501) staff       (20)   449738 2019-12-18 13:27:16.000000 dimcli-1.0.3/dimcli/templates/pyvis_inline.html
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.792838 dimcli-1.0.3/dimcli/tests/
--rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2018-03-22 14:00:12.000000 dimcli-1.0.3/dimcli/tests/__init__.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      863 2022-06-24 15:51:19.000000 dimcli-1.0.3/dimcli/tests/_test_converters.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2669 2022-07-18 16:27:12.000000 dimcli-1.0.3/dimcli/tests/quicktest.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)       53 2021-11-05 14:39:59.000000 dimcli-1.0.3/dimcli/tests/settings.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2633 2022-01-25 10:18:58.000000 dimcli-1.0.3/dimcli/tests/test_cris.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     7316 2022-06-30 15:57:47.000000 dimcli-1.0.3/dimcli/tests/test_dataframes.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     1252 2021-10-14 15:21:50.000000 dimcli-1.0.3/dimcli/tests/test_export.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     1706 2021-10-14 15:21:50.000000 dimcli-1.0.3/dimcli/tests/test_export_gsheets.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    13532 2021-10-14 15:21:50.000000 dimcli-1.0.3/dimcli/tests/test_functions.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     5203 2021-10-14 15:42:05.000000 dimcli-1.0.3/dimcli/tests/test_grammar.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     6484 2022-07-18 16:23:05.000000 dimcli-1.0.3/dimcli/tests/test_login.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2066 2022-06-29 17:56:21.000000 dimcli-1.0.3/dimcli/tests/test_magics.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     9677 2021-10-14 15:23:30.000000 dimcli-1.0.3/dimcli/tests/test_queries.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.797597 dimcli-1.0.3/dimcli/utils/
--rw-r--r--   0 michele.pasin   (501) staff       (20)      392 2022-06-24 15:51:13.000000 dimcli-1.0.3/dimcli/utils/__init__.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)      201 2020-10-22 08:36:54.000000 dimcli-1.0.3/dimcli/utils/all.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    20548 2022-06-30 17:44:31.000000 dimcli-1.0.3/dimcli/utils/converters.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    13803 2022-07-01 13:34:51.000000 dimcli-1.0.3/dimcli/utils/dim_utils.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     1196 2020-11-30 20:05:22.000000 dimcli-1.0.3/dimcli/utils/gists_utils.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2235 2020-05-22 10:42:55.000000 dimcli-1.0.3/dimcli/utils/html.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    14208 2022-06-18 14:10:49.000000 dimcli-1.0.3/dimcli/utils/misc_utils.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2389 2020-10-12 15:26:14.000000 dimcli-1.0.3/dimcli/utils/networkviz.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)    23335 2022-10-13 12:22:39.000000 dimcli-1.0.3/dimcli/utils/repl_utils.py
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2418 2020-05-22 10:41:07.000000 dimcli-1.0.3/dimcli/utils/version_utils.py
-drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-05-23 13:59:47.775813 dimcli-1.0.3/dimcli.egg-info/
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2373 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/PKG-INFO
--rw-r--r--   0 michele.pasin   (501) staff       (20)     1543 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/SOURCES.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)        1 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/dependency_links.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)      128 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/entry_points.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)       88 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/requires.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)        7 2023-05-23 13:59:47.000000 dimcli-1.0.3/dimcli.egg-info/top_level.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)      820 2021-12-22 18:27:26.000000 dimcli-1.0.3/requirements.txt
--rw-r--r--   0 michele.pasin   (501) staff       (20)       79 2023-05-23 13:59:47.798339 dimcli-1.0.3/setup.cfg
--rw-r--r--   0 michele.pasin   (501) staff       (20)     2247 2022-05-09 14:40:40.000000 dimcli-1.0.3/setup.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.533494 dimcli-1.1/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     1070 2018-05-18 16:18:19.000000 dimcli-1.1/LICENSE
+-rw-r--r--   0 michele.pasin   (501) staff       (20)       59 2021-12-22 19:09:31.000000 dimcli-1.1/MANIFEST.in
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2371 2023-07-26 10:35:09.533556 dimcli-1.1/PKG-INFO
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2064 2022-06-19 21:07:50.000000 dimcli-1.1/README.md
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.519228 dimcli-1.1/dimcli/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      396 2023-07-26 09:54:43.000000 dimcli-1.1/dimcli/VERSION.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     6013 2022-07-18 17:33:07.000000 dimcli-1.1/dimcli/__init__.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.523469 dimcli-1.1/dimcli/core/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-04-10 08:16:04.000000 dimcli-1.1/dimcli/core/__init__.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    39265 2023-07-26 10:25:10.000000 dimcli-1.1/dimcli/core/api.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    13005 2022-07-18 17:15:49.000000 dimcli-1.1/dimcli/core/auth.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    14418 2022-06-30 15:51:01.000000 dimcli-1.1/dimcli/core/dataframe_factory.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    10195 2022-05-09 14:13:01.000000 dimcli-1.1/dimcli/core/dsl_grammar.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    69745 2020-04-01 21:04:32.000000 dimcli-1.1/dimcli/core/dsl_grammar_categories.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)   198407 2023-05-23 13:25:12.000000 dimcli-1.1/dimcli/core/dsl_grammar_core.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     3656 2023-02-17 12:05:13.000000 dimcli-1.1/dimcli/core/dsl_grammar_extras.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2540 2020-10-23 13:00:00.000000 dimcli-1.1/dimcli/core/extras.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    24468 2021-10-14 15:35:08.000000 dimcli-1.1/dimcli/core/functions.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      162 2020-10-14 17:11:47.000000 dimcli-1.1/dimcli/functions.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.524150 dimcli-1.1/dimcli/jupyter/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-03-30 19:27:13.000000 dimcli-1.1/dimcli/jupyter/__init__.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    21234 2022-07-01 11:10:39.000000 dimcli-1.1/dimcli/jupyter/magics.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     3715 2020-10-22 09:03:53.000000 dimcli-1.1/dimcli/main_cli.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.526026 dimcli-1.1/dimcli/repl/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2019-01-25 16:54:16.000000 dimcli-1.1/dimcli/repl/__init__.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     8035 2020-10-12 14:58:02.000000 dimcli-1.1/dimcli/repl/autocompletion.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      871 2021-11-25 16:17:17.000000 dimcli-1.1/dimcli/repl/history.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      758 2019-02-21 16:01:09.000000 dimcli-1.1/dimcli/repl/key_bindings.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     3335 2020-10-12 14:58:02.000000 dimcli-1.1/dimcli/repl/lexer.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    11364 2021-12-08 18:01:01.000000 dimcli-1.1/dimcli/repl/repl.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      438 2019-02-07 12:19:35.000000 dimcli-1.1/dimcli/repl/validator.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      304 2020-10-23 12:59:36.000000 dimcli-1.1/dimcli/shortcuts.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.526273 dimcli-1.1/dimcli/templates/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)   449738 2019-12-18 13:27:16.000000 dimcli-1.1/dimcli/templates/pyvis_inline.html
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.530521 dimcli-1.1/dimcli/tests/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        0 2018-03-22 14:00:12.000000 dimcli-1.1/dimcli/tests/__init__.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      863 2022-06-24 15:51:19.000000 dimcli-1.1/dimcli/tests/_test_converters.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2669 2022-07-18 16:27:12.000000 dimcli-1.1/dimcli/tests/quicktest.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)       53 2021-11-05 14:39:59.000000 dimcli-1.1/dimcli/tests/settings.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2633 2022-01-25 10:18:58.000000 dimcli-1.1/dimcli/tests/test_cris.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     7316 2022-06-30 15:57:47.000000 dimcli-1.1/dimcli/tests/test_dataframes.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     1252 2021-10-14 15:21:50.000000 dimcli-1.1/dimcli/tests/test_export.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     1706 2021-10-14 15:21:50.000000 dimcli-1.1/dimcli/tests/test_export_gsheets.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    13532 2021-10-14 15:21:50.000000 dimcli-1.1/dimcli/tests/test_functions.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     5203 2021-10-14 15:42:05.000000 dimcli-1.1/dimcli/tests/test_grammar.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     6484 2022-07-18 16:23:05.000000 dimcli-1.1/dimcli/tests/test_login.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2066 2022-06-29 17:56:21.000000 dimcli-1.1/dimcli/tests/test_magics.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     9677 2021-10-14 15:23:30.000000 dimcli-1.1/dimcli/tests/test_queries.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.533245 dimcli-1.1/dimcli/utils/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      392 2022-06-24 15:51:13.000000 dimcli-1.1/dimcli/utils/__init__.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      201 2020-10-22 08:36:54.000000 dimcli-1.1/dimcli/utils/all.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    20548 2022-06-30 17:44:31.000000 dimcli-1.1/dimcli/utils/converters.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    13803 2022-07-01 13:34:51.000000 dimcli-1.1/dimcli/utils/dim_utils.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     1196 2020-11-30 20:05:22.000000 dimcli-1.1/dimcli/utils/gists_utils.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2235 2020-05-22 10:42:55.000000 dimcli-1.1/dimcli/utils/html.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    14208 2022-06-18 14:10:49.000000 dimcli-1.1/dimcli/utils/misc_utils.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2389 2020-10-12 15:26:14.000000 dimcli-1.1/dimcli/utils/networkviz.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)    23335 2022-10-13 12:22:39.000000 dimcli-1.1/dimcli/utils/repl_utils.py
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2418 2020-05-22 10:41:07.000000 dimcli-1.1/dimcli/utils/version_utils.py
+drwxr-xr-x   0 michele.pasin   (501) staff       (20)        0 2023-07-26 10:35:09.520111 dimcli-1.1/dimcli.egg-info/
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2371 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/PKG-INFO
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     1508 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/SOURCES.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        1 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/dependency_links.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      128 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/entry_points.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)       88 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/requires.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)        7 2023-07-26 10:35:09.000000 dimcli-1.1/dimcli.egg-info/top_level.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)      820 2021-12-22 18:27:26.000000 dimcli-1.1/requirements.txt
+-rw-r--r--   0 michele.pasin   (501) staff       (20)       79 2023-07-26 10:35:09.533759 dimcli-1.1/setup.cfg
+-rw-r--r--   0 michele.pasin   (501) staff       (20)     2247 2022-05-09 14:40:40.000000 dimcli-1.1/setup.py
```

### Comparing `dimcli-1.0.3/LICENSE` & `dimcli-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/PKG-INFO` & `dimcli-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimcli
-Version: 1.0.3
+Version: 1.1
 Summary: Python REPL/API for accessing dimensions.ai.
 Home-page: https://github.com/digital-science/dimcli
 Author: Michele Pasin @lambdaman
 Author-email: m.pasin@digital-science.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dimcli-1.0.3/README.md` & `dimcli-1.1/README.md`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/__init__.py` & `dimcli-1.1/dimcli/__init__.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/api.py` & `dimcli-1.1/dimcli/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,17 +196,19 @@
                 response.raise_for_status()
 
 
 
     def query_iterative(self, q, show_results=None, limit=1000, skip=0, pause=1.5, force=False, maxlimit=0, verbose=None, _tot_count_prev_query=0, _warnings_tot=None):       
         """Runs a DSL query and then keep querying until all matching records have been extracted. 
         
-        The API returns a maximum of 1000 records per call. If a DSL query results in more than 1000 matches, it is possible to use pagination to get more results. 
+        The API returns a maximum of 1000 records per call. If a DSL query results in more than 1000 matches, it is possible to use pagination to get more results, up to 50k. 
         
         Iterative querying works by automatically paginating through all records available for a result set. The original query gets turned into a loop that uses the `limit` / `skip` operators until all the results available have been extracted. 
+
+        NOTE If any of the iterative queries produce warning messages, these are aggregated and added to the `_warnings`section of the output data.
         
         Parameters
         ----------
         q: str 
             The DSL query. Important: pagination keywords eg `limit` / `skip` should be omitted.
         show_results : bool, default=True
             Determines whether the final results are rendered via the iPython display widget (for Jupyter notebooks).
@@ -315,18 +317,19 @@
         if tot > 0 and new_skip > tot:
             new_skip = tot
         if verbose and tot:  # if not first iteration
             t = "%.2f" % elapsed
             printDebug(f"{skip}-{new_skip} / {tot} ({t}s)")
 
         if res["_warnings"]:
+            warnings = [f"""{x} (iteration: {skip}-{new_skip})""" for x in res["_warnings"]]
             if _warnings_tot:
-                _warnings_tot += res["_warnings"]
+                _warnings_tot += warnings
             else:
-                _warnings_tot = res["_warnings"]
+                _warnings_tot = warnings
 
         if flag_force:
             output = self.query_iterative(q, show_results, limit, new_skip, pause, force, maxlimit, verbose, _tot_count_prev_query, _warnings_tot)                    
 
         elif not IS_UNNEST and len(res[sourcetype]) == limit and not flag_last_round:
             output = res[sourcetype] + self.query_iterative(q, show_results, limit, new_skip, pause, force,maxlimit, verbose, tot, _warnings_tot)
 
@@ -353,15 +356,18 @@
                 sourcetype: output
             }
             if _warnings_tot:
                 response_simulation["_warnings"] = _warnings_tot
             result = DslDataset(response_simulation)
             if show_results or (show_results is None and self._show_results):
                 IPython.display.display(result)
-            if verbose: printDebug(f"===\nRecords extracted: {len(output)}")
+            if verbose: 
+                printDebug(f"===\nRecords extracted: {len(output)}")
+                if _warnings_tot: 
+                    printDebug(f"Warnings:  {len(_warnings_tot)}")
             return result
         else:
             return output
 
 
     def __repr__(self):
         return f"<dimcli.Dsl #{id(self)}. API endpoint: {self._url}>"
```

### Comparing `dimcli-1.0.3/dimcli/core/auth.py` & `dimcli-1.1/dimcli/core/auth.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/dataframe_factory.py` & `dimcli-1.1/dimcli/core/dataframe_factory.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/dsl_grammar.py` & `dimcli-1.1/dimcli/core/dsl_grammar.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/dsl_grammar_categories.py` & `dimcli-1.1/dimcli/core/dsl_grammar_categories.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/dsl_grammar_core.py` & `dimcli-1.1/dimcli/core/dsl_grammar_core.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/dsl_grammar_extras.py` & `dimcli-1.1/dimcli/core/dsl_grammar_extras.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/extras.py` & `dimcli-1.1/dimcli/core/extras.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/core/functions.py` & `dimcli-1.1/dimcli/core/functions.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/jupyter/magics.py` & `dimcli-1.1/dimcli/jupyter/magics.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/main_cli.py` & `dimcli-1.1/dimcli/main_cli.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/repl/autocompletion.py` & `dimcli-1.1/dimcli/repl/autocompletion.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/repl/history.py` & `dimcli-1.1/dimcli/repl/history.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/repl/key_bindings.py` & `dimcli-1.1/dimcli/repl/key_bindings.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/repl/lexer.py` & `dimcli-1.1/dimcli/repl/lexer.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/repl/repl.py` & `dimcli-1.1/dimcli/repl/repl.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/templates/pyvis_inline.html` & `dimcli-1.1/dimcli/templates/pyvis_inline.html`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/_test_converters.py` & `dimcli-1.1/dimcli/tests/_test_converters.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/quicktest.py` & `dimcli-1.1/dimcli/tests/quicktest.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_cris.py` & `dimcli-1.1/dimcli/tests/test_cris.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_dataframes.py` & `dimcli-1.1/dimcli/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_export.py` & `dimcli-1.1/dimcli/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_export_gsheets.py` & `dimcli-1.1/dimcli/tests/test_export_gsheets.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_functions.py` & `dimcli-1.1/dimcli/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_grammar.py` & `dimcli-1.1/dimcli/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_login.py` & `dimcli-1.1/dimcli/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_magics.py` & `dimcli-1.1/dimcli/tests/test_magics.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/tests/test_queries.py` & `dimcli-1.1/dimcli/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/converters.py` & `dimcli-1.1/dimcli/utils/converters.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/dim_utils.py` & `dimcli-1.1/dimcli/utils/dim_utils.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/gists_utils.py` & `dimcli-1.1/dimcli/utils/gists_utils.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/html.py` & `dimcli-1.1/dimcli/utils/html.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/misc_utils.py` & `dimcli-1.1/dimcli/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/networkviz.py` & `dimcli-1.1/dimcli/utils/networkviz.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/repl_utils.py` & `dimcli-1.1/dimcli/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli/utils/version_utils.py` & `dimcli-1.1/dimcli/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/dimcli.egg-info/PKG-INFO` & `dimcli-1.1/dimcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimcli
-Version: 1.0.3
+Version: 1.1
 Summary: Python REPL/API for accessing dimensions.ai.
 Home-page: https://github.com/digital-science/dimcli
 Author: Michele Pasin @lambdaman
 Author-email: m.pasin@digital-science.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `dimcli-1.0.3/dimcli.egg-info/SOURCES.txt` & `dimcli-1.1/dimcli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 dimcli/core/__init__.py
 dimcli/core/api.py
 dimcli/core/auth.py
 dimcli/core/dataframe_factory.py
 dimcli/core/dsl_grammar.py
 dimcli/core/dsl_grammar_categories.py
 dimcli/core/dsl_grammar_core.py
-dimcli/core/dsl_grammar_core_BK.py
 dimcli/core/dsl_grammar_extras.py
 dimcli/core/extras.py
 dimcli/core/functions.py
 dimcli/jupyter/__init__.py
 dimcli/jupyter/magics.py
 dimcli/repl/__init__.py
 dimcli/repl/autocompletion.py
```

### Comparing `dimcli-1.0.3/requirements.txt` & `dimcli-1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `dimcli-1.0.3/setup.py` & `dimcli-1.1/setup.py`

 * *Files identical despite different names*

