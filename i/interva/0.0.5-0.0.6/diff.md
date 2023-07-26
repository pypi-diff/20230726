# Comparing `tmp/interva-0.0.5.tar.gz` & `tmp/interva-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interva-0.0.5.tar", last modified: Thu Jun  1 14:44:20 2023, max compression
+gzip compressed data, was "interva-0.0.6.tar", last modified: Wed Jul 26 19:46:18 2023, max compression
```

## Comparing `interva-0.0.5.tar` & `interva-0.0.6.tar`

### file list

```diff
@@ -1,102 +1,271 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.746485 interva-0.0.5/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-07-29 15:44:16.000000 interva-0.0.5/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      114 2022-07-29 16:28:38.000000 interva-0.0.5/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-06-01 14:44:20.746164 interva-0.0.5/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3462 2023-03-13 22:54:59.000000 interva-0.0.5/README.md
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.688978 interva-0.0.5/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.694603 interva-0.0.5/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689223 interva-0.0.5/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.693873 interva-0.0.5/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689473 interva-0.0.5/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.693293 interva-0.0.5/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689719 interva-0.0.5/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.692689 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689969 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.691881 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.690393 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.691169 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.700483 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.701522 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.703277 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.705399 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.706148 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.707967 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.709855 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.710948 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.712441 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.714404 interva-0.0.5/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.715061 interva-0.0.5/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.717046 interva-0.0.5/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.719309 interva-0.0.5/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.720178 interva-0.0.5/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.721792 interva-0.0.5/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.723993 interva-0.0.5/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.724718 interva-0.0.5/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.726689 interva-0.0.5/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.730946 interva-0.0.5/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.5/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.738060 interva-0.0.5/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.5/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   459264 2023-03-22 19:50:10.000000 interva-0.0.5/interva/data/probbase.xls
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   164661 2022-07-29 16:52:08.000000 interva-0.0.5/interva/data/probbaseV5_19.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   286521 2022-11-03 17:23:26.000000 interva-0.0.5/interva/data/randomva5.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.5/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.5/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    18966 2023-05-31 17:21:29.000000 interva-0.0.5/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.745234 interva-0.0.5/interva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3185 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       26 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       25 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/top_level.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-29 15:51:31.000000 interva-0.0.5/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-06-01 14:44:20.746605 interva-0.0.5/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1367 2023-03-13 22:54:59.000000 interva-0.0.5/setup.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.742959 interva-0.0.5/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.5/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.5/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.5/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.772920 interva-0.0.6/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-07-29 15:44:16.000000 interva-0.0.6/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      114 2022-07-29 16:28:38.000000 interva-0.0.6/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-07-26 19:46:18.772365 interva-0.0.6/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3462 2023-03-13 22:54:59.000000 interva-0.0.6/README.md
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.578948 interva-0.0.6/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.599965 interva-0.0.6/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579188 interva-0.0.6/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.599252 interva-0.0.6/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579523 interva-0.0.6/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.598685 interva-0.0.6/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579941 interva-0.0.6/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.597729 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.580372 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.596719 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.580788 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.595670 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581035 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.594922 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581420 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.594058 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581850 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.593126 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.582311 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.592180 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.582728 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.590935 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583047 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.590116 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583336 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.589309 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583860 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.588163 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.584271 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.586759 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.584717 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.585646 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.608922 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.610404 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.613818 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.618613 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.619381 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.621820 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.626904 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.627820 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.631137 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.636053 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.637079 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.640105 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.644861 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.645796 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.648945 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.653357 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.654373 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.657408 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.662220 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.663450 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.666768 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.672169 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.673276 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.676437 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.681302 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.682403 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.687498 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.695228 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.696500 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.700135 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.705581 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.706673 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.709733 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.714236 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.715267 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.718343 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.722983 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.724007 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.726916 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.731541 interva-0.0.6/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.732793 interva-0.0.6/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.735636 interva-0.0.6/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.740044 interva-0.0.6/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.741051 interva-0.0.6/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.743906 interva-0.0.6/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.748310 interva-0.0.6/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.749281 interva-0.0.6/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.752115 interva-0.0.6/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.756702 interva-0.0.6/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-07-11 18:27:06.000000 interva-0.0.6/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.762835 interva-0.0.6/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   459264 2023-03-22 19:50:10.000000 interva-0.0.6/interva/data/probbase.xls
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   164661 2022-07-29 16:52:08.000000 interva-0.0.6/interva/data/probbaseV5_19.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   286521 2022-11-03 17:23:26.000000 interva-0.0.6/interva/data/randomva5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    41483 2023-07-22 00:30:31.000000 interva-0.0.6/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19116 2023-07-18 17:19:33.000000 interva-0.0.6/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.770901 interva-0.0.6/interva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    18050 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       26 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       25 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/top_level.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-29 15:51:31.000000 interva-0.0.6/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-07-26 19:46:18.773107 interva-0.0.6/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     1367 2023-03-13 22:54:59.000000 interva-0.0.6/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.767465 interva-0.0.6/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4718 2023-07-11 18:18:34.000000 interva-0.0.6/tests/test_utils.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      570 2023-07-26 13:34:24.000000 interva-0.0.6/tests/tmp.py
```

### Comparing `interva-0.0.5/LICENSE` & `interva-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/PKG-INFO` & `interva-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python implementation of the InterVA Algorithm.
 Home-page: https://github.com/verbal-autopsy-software/interva
 Author: Sherry Zhao & Jason Thomas
 Author-email: zhao.3248@buckeyemail.osu.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `interva-0.0.5/README.md` & `interva-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/build/lib/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.5/build/lib/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,41 @@
 
 """
 interva.interva5
 -------------------
 
 This module contains the class for the InterVA5 algorithm.
 """
-
+from __future__ import annotations
+from typing import Union, TYPE_CHECKING
+if TYPE_CHECKING:
+    import PyQt5
 from pandas import (DataFrame, Index, Series, read_csv, read_excel, to_numeric,
                     isna, set_option)
 from numpy import (ndarray, nan, nansum, nanmax, argsort, array, delete, where,
                    concatenate, copy)
 from decimal import Decimal
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
-from time import time
+import datetime
 from pkgutil import get_data
 from io import BytesIO
-from typing import Union
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
-    :type va_input: pandas data.frame or path to CSV file
+    :type va_input: pandas DataFrame or path to CSV file
     :param hiv: likelihood of HIV as a cause of death.  Possible values are
     "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
     :type hiv: string
     :param malaria: likelihood of malaria as a cause of death.  Possible values
     are "H" for high (~ 1:100 deaths), "L" for low (~ 1:1000), or "V" for very
     low (~ 1:10000)
@@ -46,114 +49,181 @@
     created.  If no path is given and the parameter for "write" is True, then
     the function stops and an error message is produced.
     :type directory: directory or string
     :param filename: the filename the user wishes to save the output.
     No extension needed. The output is in .csv format by default.
     :type filename: string
     :param output: the format of the output. Possible Values are
-    "classic": the same deliminated output format as InterVA5, or
+    "classic": the same delimited output format as InterVA5, or
     "extended": delimited output followed by full distribution of cause of
     death probability
     :type output: string
     :param append: a logical value indicating whether or not the new output
     should be appended to the existing file.
     :type append: boolean
     :param groupcode: a logical value indicating whether or not the group code
     will be included in the output causes.
     :type groupcode: boolean
     :param sci: an array containing the symptom-cause-information
     (aka Probbase) that InterVA uses to assign a cause of death.
-    :type sci: pandas data.frame or numpy ndarray
+    :type sci: pandas DataFrame or numpy ndarray
     :param return_checked_data: a logical value indicating if the checked data
     (i.e., the data that have been modified by the consistency checks) should
     be returned.
     :type return_checked_data: boolean
     :param openva_app: instance of the openva_app (used for updating progress
     bar, which requires the PyQt5 package to be installed).
     """
 
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
-                 openva_app=None) -> dict:
+                 openva_app: Union[None,
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
+        self.checked_data: Union[DataFrame, str] = ""
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
-    def _check_data(self, va_input: Series, va_id: str,
+    @staticmethod
+    def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
 
+    @staticmethod
+    def _va5(id: str, malprev: str, hivprev: str, pregstat: str,
+             preglik: Union[str, int], cause1: str, lik1: Union[str, int],
+             cause2: str, lik2: Union[str, int], cause3: str,
+             lik3: Union[str, int], indet: int, comcat: str,
+             comnum: Union[str, int], wholeprob: Series) -> list:
+        """ Returns an individual VA result. """
+
+        return [id, str(malprev), str(hivprev), pregstat, preglik,
+                cause1, lik1, cause2, lik2, cause3, lik3, indet,
+                str(comcat), comnum, wholeprob]
+
+    @staticmethod
+    def _save_va5(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, without propensities. """
+
+        if not write:
+            return ()
+        del x[14]
+        filename = filename + ".csv"
+        with open(filename, 'a', newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
+    @staticmethod
+    def _save_va5_prob(x: list, filename: str, write: bool) -> None:
+        """ Saves the VA5 result to csv, with propensities. """
+
+        if not write:
+            return ()
+        prob = x.pop(14)
+        x = array(x)
+        filename = filename + ".csv"
+        x = concatenate((x, prob))
+        with open(filename, "a", newline="") as csvfile:
+            csv_writer = writer(csvfile)
+            csv_writer.writerow(x)
+
     def run(self) -> None:
-        """Assign causes of death.
-        
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas data.frame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas data.frame).
-        """
+        """Assign causes of death to valid VA records.
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        def va5(id: str, malprev: str, hivprev: str, pregstat: str,
-                preglik: Union[str, int], cause1: str, lik1: Union[str, int],
-                cause2: str, lik2: Union[str, int], cause3: str,
-                lik3: Union[str, int], indet: int, comcat: str,
-                comnum: Union[str, int], wholeprob: Series) -> list:
-            """ Returns an individual VA result. """
-
-            return [id, str(malprev), str(hivprev), pregstat, preglik,
-                    cause1, lik1, cause2, lik2, cause3, lik3, indet,
-                    str(comcat), comnum, wholeprob]
-
-        def save_va5(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, without propensities. """
-
-            if not write:
-                return()
-            del x[14]
-            filename = filename + ".csv"
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
-
-        def save_va5_prob(x: list, filename: str, write: bool) -> None:
-            """ Saves the VA5 result to csv, with propensities. """
-
-            if not write:
-                return()
-            prob = x.pop(14)
-            x = array(x)
-            filename = filename + ".csv"
-            x = concatenate((x, prob))
-            with open(filename, 'a', newline="") as csvfile:
-                csv_writer = writer(csvfile)
-                csv_writer.writerow(x)
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -165,52 +235,63 @@
 
         probbaseV5 = None
         if self.sci is None:
             probbase_df = get_probbase(version="19").copy()
             probbaseV5 = probbase_df.to_numpy()
         if self.sci is not None:
             valid_sci = True
-            if not isinstance(self.sci, DataFrame) and not isinstance(self.sci, ndarray):
+            if not isinstance(self.sci, DataFrame) and \
+                    not isinstance(self.sci, ndarray):
                 valid_sci = False
             if self.sci.shape[0] != 354 or self.sci.shape[1] != 87:
                 valid_sci = False
             if not valid_sci:
                 raise IOError(
-                    "Error: Invalid SCI (must be Pandas DataFrame or " +
+                    "Error: Invalid SCI (must be Pandas DataFrame or "
                     "Numpy ndarray with 354 rows and 87 columns).")
             if isinstance(self.sci, DataFrame):
+                probbase_df = self.sci.copy()
                 self.sci = self.sci.to_numpy()
             probbaseV5 = self.sci
+
+        pb_for_datacheck = probbase_df.fillna(".")
+        pb_for_datacheck["qdesc"] = ""
+        pb_for_datacheck = pb_for_datacheck.to_numpy(dtype=str)
+
         self.probbaseV5Version = probbaseV5[0, 2]
         print(f"Using Probbase version: {self.probbaseV5Version}")
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
         if self.groupcode:
             # adding groupcode to cause
             for i in range(3, 64):
                 cause = str(self.causetextV5.iloc[i, 0])
                 code = str(self.causetextV5.iloc[i, 1])
                 self.causetextV5.iloc[i, 1] = code + " " + cause
-            self.causetextV5.drop(self.causetextV5.columns[0], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[0],
+                                  axis=1, inplace=True)
         else:
-            self.causetextV5.drop(self.causetextV5.columns[1], axis=1, inplace=True)
+            self.causetextV5.drop(self.causetextV5.columns[1],
+                                  axis=1, inplace=True)
         logger = None
         if self.write:
-            logger = getLogger()
+            logger = getLogger(__name__)
             logger.setLevel(INFO)
-            file_handler = FileHandler("errorlogV5.txt")
+            file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
-            logger.info("Error & warning log built for InterVA5 %f \n", time())
+            now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={'i183o': 'i183a'}, axis='columns',
+            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
                                  inplace=True)
-            print("Due to the inconsistent names in the early version of " +
-                  "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
+            print(
+                "Due to the inconsistent names in the early version of "
+                "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
         va_data = va_data.to_numpy()
         if va_data.shape[0] < 1:
             raise IOError("error: no data input")
@@ -225,47 +306,49 @@
         randomVA5 = read_csv(BytesIO(va_data_csv))
         valabels = randomVA5.columns
         count_changelabel = 0
         for i in range(S):
             input_col = va_input_names[i]
             std_col = valabels[i]
             if input_col.lower() != std_col.lower():
-                logger.warning("Input column '{input_col}' does not match \
-                        InterVA5 standard: '{std_col}'")
+                logger.warning(f"Input column '{input_col}' does not match "
+                               f"InterVA5 standard: '{std_col}'")
                 count_changelabel = count_changelabel + 1
         if count_changelabel > 0:
-            logger.warning("{count_changelabel} column names changed in input.\n" +
-                    "If the change is undesirable, please change in the input " +
-                    "to match standard InterVA5 input format.")
+            logger.warning(
+                f"{count_changelabel} column names changed in input.\n"
+                "If the change is undesirable, please change in the input "
+                "to match standard InterVA5 input format.")
             va_input_names = valabels
-        prob_ncol = probbaseV5.shape[1]
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "I"] = 1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A+"] = 0.8
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A"] = 0.5
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "A-"] = 0.2
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B+"] = 0.1
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B"] = 0.05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B-"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "B -"] = 0.02
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C+"] = 0.01
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C"] = 0.005
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "C-"] = 0.002
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D+"] = 0.001
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D"] = 5e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "D-"] = 1e-04
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "E"] = 1e-05
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == "N"] = 0
-        probbaseV5[:,17:prob_ncol][probbaseV5[:,17:prob_ncol] == ""] = 0
+        pb_ncol = probbaseV5.shape[1]
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "I"] = 1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A+"] = 0.8
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A"] = 0.5
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "A-"] = 0.2
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B+"] = 0.1
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B"] = 0.05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B-"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "B -"] = 0.02
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C+"] = 0.01
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C"] = 0.005
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "C-"] = 0.002
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D+"] = 0.001
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D"] = 5e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "D-"] = 1e-04
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "E"] = 1e-05
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == "N"] = 0
+        probbaseV5[:, 17:pb_ncol][probbaseV5[:, 17:pb_ncol] == ""] = 0
         probbaseV5[0, 0:17] = 0
         Sys_Prior = copy(to_numeric(probbaseV5[0, :]))
         D = len(Sys_Prior)
         self.hiv = self.hiv.lower()
         self.malaria = self.malaria.lower()
-        if self.hiv not in ['h', 'l', 'v'] or self.malaria not in ['h', 'l', 'v']:
-            raise IOError("error: the HIV and Malaria indicator " +
+        hlv_set = ["h", "l", "v"]
+        if self.hiv not in hlv_set or self.malaria not in hlv_set:
+            raise IOError("error: the HIV and Malaria indicator "
                           "should be one of the three: 'h', 'l', 'v'")
         if self.hiv == "h":
             Sys_Prior[22] = 0.05
         if self.hiv == "l":
             Sys_Prior[22] = 0.005
         if self.hiv == "v":
             Sys_Prior[22] = 1e-05
@@ -279,35 +362,36 @@
             Sys_Prior[24] = 1e-05
             Sys_Prior[44] = 1e-05
 
         ID_list = [nan for _ in range(N)]
         VA_result = [[] for _ in range(N)]
         if self.write and not self.append:
             header = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                            "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
-                            "INDET", "COMCAT", "COMNUM"]
+                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3",
+                      "INDET", "COMCAT", "COMNUM"]
             if self.output == "extended":
                 header = header + list(self.causetextV5.iloc[:, 0])
-            with open(self.filename + ".csv", 'w', newline="") as write_obj:
+            with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\n the following records are incomplete and " +
-                "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
-        if self.return_checked_data:
-            self.checked_data = [[] for _ in range(N)]
-            # id_inputs declared & assigned above
+        list_checked_data = []
+        list_dem_group = []
+
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -323,43 +407,48 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
-            tmp = datacheck5(va_input=input_current, va_id=index_current)
+            tmp = datacheck5(va_input=input_current, va_id=index_current,
+                             probbase=pb_for_datacheck)
+
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
-                self.checked_data[i] = [id_inputs[i]] + list(tmp["output"][1:S])
+                list_checked_data.append(
+                    [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
 
             subst_vector = array([nan for _ in range(S)])
             subst_vector[probbaseV5[:, 5] == "N"] = 0
             subst_vector[probbaseV5[:, 5] == "Y"] = 1
 
             new_input = array([0 for _ in range(S)])
-            for y in range(1,S):
+            for y in range(1, S):
                 if not isna(input_current[y]):
                     if input_current[y] == subst_vector[y]:
                         new_input[y] = 1
 
             input_current[input_current == 0] = 1
             input_current[0] = 0
             input_current[isna(input_current)] = 0
@@ -389,21 +478,24 @@
             # Determine Preg_State and Likelihood
             if nansum(prob_A) == 0 or reproductiveAge == 0:
                 preg_state = "n/a"
                 lik_preg = " "
             if nanmax(prob_A) < 0.1 and reproductiveAge == 1:
                 preg_state = "indeterminate"
                 lik_preg = " "
-            if where(prob_A == nanmax(prob_A))[0][0] == 0 and prob_A[0] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 0 and \
+                    prob_A[0] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Not pregnant or recently delivered"
                 lik_preg = round(prob_A[0]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 1 and prob_A[1] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 1 and \
+                    prob_A[1] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnancy ended within 6 weeks of death"
                 lik_preg = round(prob_A[1]/nansum(prob_A) * 100)
-            if where(prob_A == nanmax(prob_A))[0][0] == 2 and prob_A[2] >= 0.1 and reproductiveAge == 1:
+            if where(prob_A == nanmax(prob_A))[0][0] == 2 and \
+                    prob_A[2] >= 0.1 and reproductiveAge == 1:
                 preg_state = "Pregnant at death"
                 lik_preg = round(prob_A[2]/nansum(prob_A) * 100)
 
             # Determine the output of InterVA
             prob_temp = copy(prob_B)
             prob_temp_names = prob_names.iloc[3:64].copy()
             top3 = []
@@ -436,15 +528,15 @@
                 cause3 = prob_temp_names.iloc[max3_loc]
                 if nanmax(prob_temp) < 0.5 * nanmax(prob_B):
                     lik3 = cause3 = " "
                 top3.append(lik3)
                 top3 = array([int(x) if x != " " else 0 for x in top3])
                 indet = round(100 - nansum(top3))
 
-            # Determine the Circumstances of Mortality CATegory (COMCAT) 
+            # Determine the Circumstances of Mortality CATegory (COMCAT)
             # and probability
             prob_C_names = prob_names[64:70]
             comcat = ""
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
@@ -453,57 +545,73 @@
             if nanmax(prob_C) >= 0.5:
                 comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
-            VA_result[i] = va5(index_current, self.malaria, self.hiv,
-                               preg_state, lik_preg, cause1, lik1, cause2,
-                               lik2, cause3, lik3, indet, comcat, comnum,
-                               wholeprob=combined_prob)
+            VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
+                                         preg_state, lik_preg, cause1, lik1,
+                                         cause2, lik2, cause3, lik3, indet,
+                                         comcat, comnum,
+                                         wholeprob=combined_prob)
             if self.output == "classic":
-                save_va5(VA_result[i].copy(),
-                         filename=self.filename,
-                         write=self.write)
+                InterVA5._save_va5(VA_result[i].copy(),
+                                   filename=self.filename,
+                                   write=self.write)
             if self.output == "extended":
-                save_va5_prob(VA_result[i].copy(),
-                              filename=self.filename,
-                              write=self.write)
+                InterVA5._save_va5_prob(VA_result[i].copy(),
+                                        filename=self.filename,
+                                        write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("\n the following data discrepancies were identified and " +
-                 "handled: \n" + str(first_pass) + "\nSecond pass\n" +
-                 str(second_pass))
-
+            logger.info("\nThe following data discrepancies were identified "
+                        "and handled:\n")
+            for j in range(len(first_pass)):
+                item = first_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
+            logger.info("\nSecond pass\n")
+            for j in range(len(second_pass)):
+                item = second_pass[j]
+                if item:
+                    for k in item:
+                        logger.info(k)
         chdir(global_dir)
         if not self.return_checked_data:
             self.checked_data = "return_checked_data = False"
         else:
-            self.checked_data = DataFrame(self.checked_data)
+            self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -516,54 +624,55 @@
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
         else:
-            print(f"The provided HIV level \"{hiv_level}\" is invalid.")
+            print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
         print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
         else:
-            print(f"The provided malaria level \"{malaria_level}\" is invalid.")
+            print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
         print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -580,22 +689,22 @@
                 else:
                     cause_with_code = causenames[i]
                     temp_names[i] = cause_with_code.split(" ", 1)[1]
             causenames = Index(temp_names)
 
         # fix for removing the first 3 preg related death in standard input
         if ("Not pregnant or recently delivered" in causenames[0] and
-            "Pregnancy ended within 6 weeks of death" in causenames[1] and
-            "Pregnant at death" in causenames[2] and
-            "Culture" in causenames[64] and
-            "Emergency" in causenames[65] and
-            "Health" in causenames[66] and
-            "Inevitable" in causenames[67] and
-            "Knowledge" in causenames[68] and
-            "Resources" in causenames[69]):
+                "Pregnancy ended within 6 weeks of death" in causenames[1] and
+                "Pregnant at death" in causenames[2] and
+                "Culture" in causenames[64] and
+                "Emergency" in causenames[65] and
+                "Health" in causenames[66] and
+                "Inevitable" in causenames[67] and
+                "Knowledge" in causenames[68] and
+                "Resources" in causenames[69]):
             del causeindex[64:70]
             del causeindex[0:3]
             causenames = causenames.delete([0, 1, 2, 64, 65, 66, 67, 68, 69])
             include_probAC = True
 
         causetextV5_horizontal = DataFrame(CAUSETEXTV5)
         self.causetextV5 = causetextV5_horizontal.transpose()
@@ -609,53 +718,59 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
-            if va.iloc[i, 14] is None:  #wholeprob exists
+            if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
             this_dist_copy = va.iloc[i, 14].copy()
             this_dist = this_dist_copy.to_numpy()
             if include_probAC:
                 this_dist[0:3] = 0
                 this_dist[64:70] = 0
             if max(this_dist) < 0.4:
-                this_undeter = 1 if isclose(sum(this_dist), 0) else sum(this_dist)
+                if isclose(sum(this_dist), 0):
+                    this_undeter = 1
+                else:
+                    this_undeter = sum(this_dist)
                 undeter = undeter + this_undeter
             else:
                 cutoff_3 = Decimal(this_dist[argsort(-this_dist)][2])
                 cutoff_2 = Decimal(this_dist[argsort(-this_dist)][1])
                 cutoff_1 = Decimal(this_dist[argsort(-this_dist)][0])
                 cutoff_1_halved = cutoff_1 / Decimal('2')
                 cutoff_pt1 = cutoff_3.max(cutoff_1_halved)
                 cutoff_pt2 = cutoff_2.max(cutoff_1_halved)
                 cutoff = cutoff_pt1.min(cutoff_pt2)
                 adj_cutoff = cutoff - Decimal(1e-15)
 
-                undeter = undeter + sum(this_dist[where(this_dist < adj_cutoff)[0]])
+                undeter = undeter + sum(
+                    this_dist[where(this_dist < adj_cutoff)[0]])
                 this_dist[where(this_dist < adj_cutoff)[0]] = 0
 
                 temp_len = len(this_dist[where(this_dist > 0)[0]])
                 close_indices = []
                 for j in range(temp_len):
-                    if abs(Decimal(this_dist[where(this_dist > 0)[0]][j]) - cutoff) < 4e-29:
+                    val = Decimal(
+                        this_dist[where(this_dist > 0)[0]][j]) - cutoff
+                    if abs(val) < 4e-29:
                         close_indices.append(where(this_dist > 0)[0][j])
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
@@ -685,53 +800,57 @@
         # show causes with top non-zero values
         show_top = 0
         while dist_cod_sorted[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
             a = dist_cod_sorted[show_top]
             b = dist_cod_sorted[show_top-1]
-            while show_top < len(dist_cod_sorted) and (abs(a-b) < (a+b) * 1e-5):
+            while show_top < len(dist_cod_sorted) and \
+                    (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
-        
+
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param filename: the filename the user wishes to save the CSMF. 
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
+        :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         csmf = self.get_csmf(top=top, groupcode=groupcode)
         filename = filename + ".csv"
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
-        :rtype: pandas data.frame
+        :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -771,30 +890,31 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
-    def write_indiv_prob(self, top: int = 0, include_propensities: bool = False,
+    def write_indiv_prob(self, top: int = 0,
+                         include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
-        
+
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
-         cause distribution. No extension needed. The output is in .csv 
+         cause distribution. No extension needed. The output is in .csv
          format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
         indiv_prob = self.get_indiv_prob(top, include_propensities)
```

### Comparing `interva-0.0.5/build/lib/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,97 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
 probbasev5 = data(r_iva5).fetch("probbaseV5")["probbaseV5"]
 
 robjects.r("data(probbaseV5, package='InterVA5')")
 robjects.r("data(RandomVA5, package='InterVA5')")
 robjects.r('''
   ra5 <- as.matrix(RandomVA5)
-  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".", groupcode=FALSE)$VA5
+  r_va5 <- InterVA5(ra5, HIV="h", Malaria="l", directory=".",
+                    groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
-  
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
+
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
-iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".", groupcode=False)
+iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
+                  groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
+
 
-def test_r_VA5_comparison():
+def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
             assert a == b
 
-def test_r_CSMF_top15_comparison():
+
+def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.5/build/lib/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pandas import read_csv, DataFrame, Series, read_excel
+from pandas import read_csv, DataFrame, Series
 from pkgutil import get_data
 from io import BytesIO
 from os.path import isfile
 
 from interva.interva5 import InterVA5
 from interva.interva5 import get_probbase
 
@@ -74,31 +74,31 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
-    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK", 
-    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3", "LIK3", 
-    #                      "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
+    va5_output = iv5out.results["VA5"]
+    # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
+    #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
+    #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
     preg_stat_valid_values = ["n/a",
                               "indeterminate",
                               "Not pregnant or recently delivered",
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -243,51 +243,51 @@
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     iv5out.run()
     iv5out.write_csmf(top=5, filename="csmf_top_5")
     assert isfile('csmf_top_5.csv')
     rowcount = 0
     for _ in open("csmf_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     assert rowcount == 5
 
 
 def test_get_indiv_prob_top_none(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
-      rowcount = rowcount + 1
+        rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

### Comparing `interva-0.0.5/interva/data/causetext.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/data/probbase.xls` & `interva-0.0.6/interva/data/probbase.xls`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/data/probbaseV5_19.csv` & `interva-0.0.6/interva/data/probbaseV5_19.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/data/randomva5.csv` & `interva-0.0.6/interva/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/exceptions.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/interva/utils.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 -------------------
 
 This module provides utility functions for manipulating and summarizing
 output from InterVA5 (i.e., the out attribute).
 """
 
 from __future__ import annotations
-from typing import Union
+from typing import Union, TYPE_CHECKING
 from pandas import DataFrame, Index, Series, isna
 from numpy import append, argsort, delete, nanmax, where, zeros
 from decimal import Decimal
 from math import isclose
 
 from interva.exceptions import ArgumentException
-import interva.interva5
+if TYPE_CHECKING:
+    import interva.interva5
 
 
 def _get_dem_groups(va_series: Series, detailed=False) -> dict:
     """Retrieve age and sex from the VA record."""
 
     if not isinstance(va_series, Series):
         raise ArgumentException(
```

### Comparing `interva-0.0.5/interva.egg-info/PKG-INFO` & `interva-0.0.6/interva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python implementation of the InterVA Algorithm.
 Home-page: https://github.com/verbal-autopsy-software/interva
 Author: Sherry Zhao & Jason Thomas
 Author-email: zhao.3248@buckeyemail.osu.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `interva-0.0.5/setup.py` & `interva-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/tests/test_compare_r.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/tests/test_interva5.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.5/tests/test_utils.py` & `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py`

 * *Files identical despite different names*

