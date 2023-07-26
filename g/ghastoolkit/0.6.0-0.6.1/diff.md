# Comparing `tmp/ghastoolkit-0.6.0.tar.gz` & `tmp/ghastoolkit-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.6.0.tar", last modified: Tue Jul 18 17:01:51 2023, max compression
+gzip compressed data, was "ghastoolkit-0.6.1.tar", last modified: Wed Jul 26 11:41:32 2023, max compression
```

## Comparing `ghastoolkit-0.6.0.tar` & `ghastoolkit-0.6.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.801986 ghastoolkit-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeql_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.6.0/LICENSE` & `ghastoolkit-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/PKG-INFO` & `ghastoolkit-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.0/README.md` & `ghastoolkit-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/pyproject.toml` & `ghastoolkit-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [project]
 name = "ghastoolkit"
-version = "0.6.0"
+version = "0.6.1"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
+
 dependencies = [
-    "certifi==2023.5.7",
+    "certifi==2023.7.22",
     "charset-normalizer==3.2.0",
     "idna==3.4",
-    "PyYAML==6.0",
+    "PyYAML==6.0.1",
     "ratelimit==2.2.1",
     "requests==2.31.0",
-    "urllib3==2.0.3",
+    "semantic-version==2.10.0",
+    "urllib3==2.0.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/ghastoolkit"
 "Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
 
 [build-system]
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/__init__.py` & `ghastoolkit-0.6.1/src/ghastoolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""GitHub Advanced Security Toolkit."""
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.6.1/src/ghastoolkit/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+"""ghastoolkit main workflow."""
 import os
 import logging
 import argparse
 
 from ghastoolkit import __name__ as name, __banner__
 from ghastoolkit.octokit.github import GitHub
 from ghastoolkit.octokit.codescanning import CodeScanning
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/__main__.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.6.1/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/codescanning.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """GitHub Code Scanning API Module."""
 from dataclasses import dataclass
 import json
 import logging
-from typing import Any, List, Optional
+from typing import List, Optional
 from ghastoolkit.octokit.github import GitHub, Repository
-from ghastoolkit.octokit.octokit import OctoItem, RestRequest
+from ghastoolkit.octokit.octokit import OctoItem, RestRequest, loadOctoItem
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
 @dataclass
 class CodeAlert(OctoItem):
     """Code Alert from Code Scanning API."""
@@ -77,24 +77,24 @@
         self.repository = repository or GitHub.repository
         self.tools: List[str] = []
 
         if not self.repository:
             raise Exception("CodeScanning requires Repository to be set")
         self.rest = RestRequest(self.repository)
 
-    def getOrganizationAlerts(self, state: str = "open") -> list[dict[Any, Any]]:
-        """Get Organization Alerts.
+    def getOrganizationAlerts(self, state: str = "open") -> list[CodeAlert]:
+        """Get list of Organization Alerts.
 
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-an-organization
         """
         results = self.rest.get(
             "/orgs/{org}/code-scanning/alerts", {"state": state}, authenticated=True
         )
         if isinstance(results, list):
-            return results
+            return [loadOctoItem(CodeAlert, alert) for alert in results]
         raise Exception(f"Error getting alerts from Organization")
 
     def getAlerts(
         self,
         state: str = "open",
         tool_name: Optional[str] = None,
         ref: Optional[str] = None,
@@ -113,15 +113,15 @@
                 "ref": ref,
                 "sort": sort,
                 "severity": severity,
             },
             authenticated=True,
         )
         if isinstance(results, list):
-            return results
+            return [loadOctoItem(CodeAlert, alert) for alert in results]
         raise Exception(f"Error getting alerts from Repository")
 
     def getAlertsInPR(self, base: str) -> list[CodeAlert]:
         """Get the open alerts in a Pull Request (delta / diff).
 
         Note this operation is slow due to it needing to lookup each alert instance
         information.
@@ -138,23 +138,26 @@
         for alert in alerts:
             number = alert.get("number")
             alert_info = self.getAlertInstances(number, ref=base)
             if len(alert_info) == 0:
                 results.append(alert)
         return results
 
-    @RestRequest.restGet(
-        "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}", authenticated=True
-    )
     def getAlert(self, alert_number: int) -> CodeAlert:
         """Get Single Alert information from Code Scanning.
 
         https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
         """
-        return {}
+        result = self.rest.get(
+            "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}",
+            {"alert_number": alert_number},
+        )
+        if isinstance(result, dict):
+            return loadOctoItem(CodeAlert, result)
+        raise Exception(f"Error getting alert from Repository")
 
     def getAlertInstances(
         self, alert_number: int, ref: Optional[str] = None
     ) -> list[dict]:
         """Get a list of alert instances."""
         result = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}/instances",
@@ -236,15 +239,15 @@
 
     def getCodeQLDatabase(self, language: str) -> dict:
         """Get a CodeQL database for a repository.
 
         https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#get-a-codeql-database-for-a-repository
         """
         return self.rest.get(
-            "/repos/{oner}/{repo}/code-scanning/codeql/databases/{language}",
+            "/repos/{owner}/{repo}/code-scanning/codeql/databases/{language}",
             {"language": language},
         )
 
     def getPacks(self, visibility: str = "internal") -> List[dict]:
         """Get all CodeQL Packs from remote GitHub instance.
 
         CodeQL Packs are stored in GitHub's container registry so this function might
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependabot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+"""Dependabot API."""
 import logging
 from typing import Optional
 
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import GraphQLRequest
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 
 
 logger = logging.getLogger("ghastoolkit.octokit.dependabot")
 
 
 class Dependabot:
+    """Dependabot API instance."""
+
     def __init__(self, repository: Optional[Repository] = None) -> None:
+        """Initialise Dependabot API class."""
         self.repository = repository or GitHub.repository
         self.graphql = GraphQLRequest(repository)
 
     def getAlerts(self) -> list[DependencyAlert]:
-        """Get Dependabot alerts from GraphQL API"""
+        """Get All Dependabot alerts from GraphQL API using the `GetDependencyAlerts` query."""
         results = []
 
         while True:
             data = self.graphql.query(
                 "GetDependencyAlerts",
                 options={"owner": self.repository.owner, "repo": self.repository.repo},
             )
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-import json
+"""Dependency Graph Octokit."""
 import logging
-from threading import main_thread
 from typing import Any
 import urllib.parse
 
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependencies, Dependency
 from ghastoolkit.octokit.octokit import GraphQLRequest, Optional, RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.dependencygraph")
 
 
 class DependencyGraph:
+    """Dependency Graph API."""
+
     def __init__(
         self,
         repository: Optional[Repository] = None,
         enable_graphql: bool = True,
         enable_clearlydefined: bool = False,
     ) -> None:
+        """Initialise Dependency Graph."""
         self.repository = repository or GitHub.repository
         self.rest = RestRequest(repository)
         self.graphql = GraphQLRequest(repository)
 
         self.enable_graphql = enable_graphql
         self.enable_clearlydefined = enable_clearlydefined
 
     def getDependencies(self) -> Dependencies:
-        """Get Dependencies"""
+        """Get Dependencies."""
         deps = self.getDependenciesSbom()
 
         if self.enable_graphql:
             logger.debug("Enabled GraphQL Dependencies")
             graph_deps = self.getDependenciesGraphQL()
 
             deps.updateDependencies(graph_deps)
 
         if self.enable_clearlydefined:
             logger.debug("Applying ClearlyDefined on dependencies")
             deps.applyClearlyDefined()
         return deps
 
     def getDependenciesSbom(self) -> Dependencies:
-        """Get Dependencies from SBOM"""
+        """Get Dependencies from SBOM."""
         result = Dependencies()
         spdx_bom = self.exportBOM()
 
         for package in spdx_bom.get("sbom", {}).get("packages", []):
             extref = False
             dep = Dependency("")
             for ref in package.get("externalRefs", []):
@@ -72,15 +74,15 @@
                 dep.license = package.get("licenseConcluded")
 
             result.append(dep)
 
         return result
 
     def getDependenciesGraphQL(self) -> Dependencies:
-        """Get Dependencies from GraphQL"""
+        """Get Dependencies from GraphQL."""
         deps = Dependencies()
         data = self.graphql.query(
             "GetDependencyInfo",
             {"owner": self.repository.owner, "repo": self.repository.repo},
         )
         graph_manifests = (
             data.get("data", {})
@@ -112,15 +114,15 @@
                         license=license,
                     )
                 )
 
         return deps
 
     def getDependenciesInPR(self, base: str, head: str) -> Dependencies:
-        """Get all the dependencies from a Pull Request"""
+        """Get all the dependencies from a Pull Request."""
         dependencies = Dependencies()
         base = urllib.parse.quote(base, safe="")
         head = urllib.parse.quote(head, safe="")
         basehead = f"{base}...{head}"
         logger.debug(f"PR basehead :: {basehead}")
         results = self.rest.get(
             "/repos/{owner}/{repo}/dependency-graph/compare/{basehead}",
@@ -157,36 +159,37 @@
                 dep.alerts.append(dep_alert)
 
             dependencies.append(dep)
 
         return dependencies
 
     def exportBOM(self) -> Dependencies:
-        """Download / Export DependencyGraph SBOM"""
+        """Download / Export DependencyGraph SBOM."""
         return self.rest.get("/repos/{owner}/{repo}/dependency-graph/sbom")
 
     def submitDependencies(
         self,
         dependencies: Dependencies,
         tool: str,
         path: str,
         sha: str = "",
         ref: str = "",
         version: str = "0.0.0",
         url: str = "",
     ):
-        """
+        """Submit dependencies to GitHub Dependency Graph snapshots API.
+
         https://docs.github.com/en/rest/dependency-graph/dependency-submission?apiVersion=2022-11-28#create-a-snapshot-of-dependencies-for-a-repository
         """
         self.rest.postJson(
             "/repos/{owner}/{repo}/dependency-graph/snapshots",
             dependencies.exportBOM(tool, path, sha, ref, version, url),
             expected=201,
         )
 
     def submitSbom(self, sbom: dict[Any, Any]):
-        """Submit SBOM"""
+        """Submit SBOM."""
         self.rest.postJson(
             "/repos/{owner}/{repo}/dependency-graph/snapshots",
             sbom,
             expected=201,
         )
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""GitHub and Repository APIs."""
 import logging
 import os
 import shutil
 import tempfile
 import subprocess
 from dataclasses import dataclass
 from typing import Optional, Tuple
@@ -9,15 +10,15 @@
 
 
 logger = logging.getLogger("ghastoolkit.octokit.github")
 
 
 @dataclass
 class Repository:
-    """GitHub Repository"""
+    """GitHub Repository."""
 
     owner: str
     """Owner"""
     repo: str
     """Repository name"""
 
     reference: Optional[str] = None
@@ -41,53 +42,54 @@
         if self.branch and not self.reference:
             self.reference = f"refs/heads/{self.branch}"
 
         if not self.clone_path:
             self.clone_path = os.path.join(tempfile.gettempdir(), self.repo)
 
     def __str__(self) -> str:
+        """To String."""
         name = f"{self.owner}/{self.repo}"
         if self.reference:
             return f"{name}:{self.reference}"
         elif self.branch:
             return f"{name}@{self.branch}"
         return name
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def isInPullRequest(self) -> bool:
-        """Is in Pull Request?"""
+        """Check if the current reference is in a Pull Request."""
         if self.reference:
             return self.reference.startswith("refs/pull")
         return False
 
     def getPullRequestNumber(self) -> int:
-        """Get Pull Request Number"""
+        """Get Pull Request Number / ID."""
         if self.isInPullRequest() and self.reference:
             return int(self.reference.split("/")[2])
         return 0
 
     def getPullRequestInfo(self) -> dict:
-        """Get information for the current pull request
+        """Get information for the current Pull Request.
 
         https://docs.github.com/en/enterprise-cloud@latest/rest/pulls/pulls#get-a-pull-request
         """
         if not self.__prinfo__:
             from ghastoolkit.octokit.octokit import RestRequest
 
             pull_number = self.getPullRequestNumber()
             self.__prinfo__ = RestRequest().get(
                 "/repos/{owner}/{repo}/pulls/{pull_number}",
                 {"pull_number": pull_number},
             )
         return self.__prinfo__
 
     def getPullRequestCommits(self) -> list[str]:
-        """Get Pull Request Commits"""
+        """Get list of Pull Request commits."""
         result = []
         if self.isInPullRequest():
             from ghastoolkit.octokit.octokit import RestRequest
 
             pull_number = self.getPullRequestNumber()
             response = RestRequest().get(
                 "/repos/{owner}/{repo}/pulls/{pull_number}/commits",
@@ -95,15 +97,15 @@
             )
             for commit in response:
                 result.append(commit.get("sha"))
         return result
 
     @property
     def clone_url(self) -> str:
-        """Repository clone URL"""
+        """Repository clone URL."""
         if GitHub.github_app:
             url = urlparse(GitHub.instance)
             return f"{url.scheme}://x-access-token:{GitHub.token}@{url.netloc}/{self.owner}/{self.repo}.git"
         elif GitHub.token:
             url = urlparse(GitHub.instance)
             return f"{url.scheme}://{GitHub.token}@{url.netloc}/{self.owner}/{self.repo}.git"
         return f"{GitHub.instance}/{self.owner}/{self.repo}.git"
@@ -119,16 +121,17 @@
 
     def clone(
         self,
         path: Optional[str] = None,
         clobber: bool = False,
         depth: Optional[int] = None,
     ):
-        """Clone Repository
-        The clone path if left None will create a tmp folder for you
+        """Clone Repository based on url.
+
+        path: str - if left `None`, it will create a tmp folder for you.
         """
         if path:
             self.clone_path = path
         if not self.clone_path:
             raise Exception(f"Clone path not set")
 
         if os.path.exists(self.clone_path) and clobber:
@@ -142,49 +145,51 @@
         cmd = self._cloneCmd(self.clone_path, depth=depth)
         logger.debug(f"Cloning Command :: {cmd}")
 
         with open(os.devnull, "w") as null:
             subprocess.check_call(cmd, stdout=null, stderr=null)
 
     def gitsha(self) -> str:
-        """Get the Git SHA"""
+        """Get the current Git SHA."""
         cmd = ["git", "rev-parse", "HEAD"]
         result = (
             subprocess.check_output(cmd, cwd=self.clone_path).decode("ascii").strip()
         )
         return result
 
     def getFile(self, path: str) -> str:
-        """Get a path relative from the base of the cloned repository"""
+        """Get a path relative from the base of the cloned repository."""
         if not self.clone_path:
             raise Exception(f"Unknown clone path")
         return os.path.join(self.clone_path, path)
 
     def display(self) -> str:
-        """Display the repository as a string"""
+        """Display the repository as a string."""
         if self.reference:
             return f"{self.owner}/{self.repo}@{self.reference}"
         return f"{self.owner}/{self.repo}"
 
     @staticmethod
     def parseRepository(name: str) -> "Repository":
-        """Parse the repository name"""
+        """Parse the repository name."""
         ref = None
         branch = None
         if "@" in name:
             name, branch = name.split("@", 1)
             ref = f"refs/heads/{branch}"
 
         owner, repo = name.split("/", 1)
         return Repository(owner, repo, reference=ref, branch=branch)
 
 
 class GitHub:
-    """The GitHub class is used to configure the state for all Octokit
-    apis. Its a standard interface across all projects.
+    """The GitHub Class.
+
+    This API is used to configure the state for all Octokit apis.
+    Its a standard interface across all projects.
     """
 
     repository: Repository = Repository("GeekMasher", "ghastoolkit")
     """Repository"""
     token: Optional[str] = None
     """GitHub Access Token"""
 
@@ -208,15 +213,15 @@
         repo: Optional[str] = None,
         reference: Optional[str] = None,
         branch: Optional[str] = None,
         token: Optional[str] = None,
         instance: Optional[str] = None,
         enterprise: Optional[str] = None,
     ) -> None:
-        """Initialise a GitHub class using a number of properties"""
+        """Initialise a GitHub class using a number of properties."""
         if repository:
             GitHub.repository = Repository.parseRepository(repository)
         elif owner and repo:
             GitHub.repository = Repository(owner, repo)
 
         if GitHub.repository:
             if reference:
@@ -235,23 +240,23 @@
 
         GitHub.enterprise = enterprise
 
         return
 
     @staticmethod
     def parseInstance(instance: str) -> Tuple[str, str]:
-        """Parse GitHub Instance"""
+        """Parse GitHub Instance."""
         url = urlparse(instance)
 
         # GitHub Cloud (.com)
         if url.netloc == "github.com":
             api = url.scheme + "://api." + url.netloc
             return (api, f"{api}/graphql")
         # GitHub Ent Server
         api = url.scheme + "://" + url.netloc + "/api/v3"
 
         return (api, f"{api}/graphql")
 
     @staticmethod
     def display() -> str:
-        """Display the GitHub Settings"""
+        """Display the GitHub Settings."""
         return f"GitHub('{GitHub.repository.display()}', '{GitHub.instance}')"
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.6.1/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.6.1/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.0
+Version: 0.6.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.6.1/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_advisories.py` & `ghastoolkit-0.6.1/tests/test_advisories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-from semantic_version import Version
 from ghastoolkit.supplychain.advisories import (
     Advisory,
     Advisories,
     AdvisoryAffect,
     parseVersion,
 )
 from ghastoolkit.supplychain.dependencies import Dependency
```

### Comparing `ghastoolkit-0.6.0/tests/test_codeql_dataext.py` & `ghastoolkit-0.6.1/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_codeql_packs.py` & `ghastoolkit-0.6.1/tests/test_codeql_packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_codeqldb.py` & `ghastoolkit-0.6.1/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_codescanning.py` & `ghastoolkit-0.6.1/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_default.py` & `ghastoolkit-0.6.1/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_dependencies.py` & `ghastoolkit-0.6.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_depgraph.py` & `ghastoolkit-0.6.1/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_github.py` & `ghastoolkit-0.6.1/tests/test_github.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,25 @@
         return super().setUp()
 
     def test_branch(self):
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/heads/main")
         self.assertEqual(repo.reference, "refs/heads/main")
         self.assertEqual(repo.branch, "main")
 
+        repo = Repository(
+            "GeekMasher", "ghastoolkit", reference="refs/heads/random-branch/name"
+        )
+        self.assertEqual(repo.reference, "refs/heads/random-branch/name")
+        self.assertEqual(repo.branch, "random-branch/name")
+
+    def test_branch_tag(self):
+        repo = Repository("GeekMasher", "ghastoolkit", reference="refs/tags/0.4.0")
+        self.assertEqual(repo.reference, "refs/tags/0.4.0")
+        self.assertEqual(repo.branch, "0.4.0")
+
     def test_pull_request(self):
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/heads/main")
         self.assertFalse(repo.isInPullRequest())
 
         repo = Repository("GeekMasher", "ghastoolkit", reference="refs/pull/1/merge")
         self.assertTrue(repo.isInPullRequest())
         self.assertEqual(repo.getPullRequestNumber(), 1)
```

### Comparing `ghastoolkit-0.6.0/tests/test_licenses.py` & `ghastoolkit-0.6.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_octokit.py` & `ghastoolkit-0.6.1/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.0/tests/test_secretscanning.py` & `ghastoolkit-0.6.1/tests/test_secretscanning.py`

 * *Files identical despite different names*

