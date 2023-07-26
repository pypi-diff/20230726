# Comparing `tmp/ghastoolkit-0.6.1.tar.gz` & `tmp/ghastoolkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.6.1.tar", last modified: Wed Jul 26 11:41:32 2023, max compression
+gzip compressed data, was "ghastoolkit-0.6.2.tar", last modified: Wed Jul 26 18:27:31 2023, max compression
```

## Comparing `ghastoolkit-0.6.1.tar` & `ghastoolkit-0.6.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.410597 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.406597 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:41:32.000000 ghastoolkit-0.6.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:41:32.414597 ghastoolkit-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeql_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 11:41:01.000000 ghastoolkit-0.6.1/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.571680 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.567680 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:27:31.000000 ghastoolkit-0.6.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:27:31.575681 ghastoolkit-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-26 18:26:57.000000 ghastoolkit-0.6.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.6.1/LICENSE` & `ghastoolkit-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/PKG-INFO` & `ghastoolkit-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.1/README.md` & `ghastoolkit-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/pyproject.toml` & `ghastoolkit-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.6.1"
+version = "0.6.2"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/__init__.py` & `ghastoolkit-0.6.2/src/ghastoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GitHub Advanced Security Toolkit."""
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.6.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/__main__.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/pack.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/pack.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.6.2/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,27 @@
         self.repository = repository or GitHub.repository
         self.tools: List[str] = []
 
         if not self.repository:
             raise Exception("CodeScanning requires Repository to be set")
         self.rest = RestRequest(self.repository)
 
+    def isEnabled(self) -> bool:
+        """Check to see if Code Scanning is enabled or not on a repository level."""
+        try:
+            self.rest.get(
+                "/repos/{org}/{repo}/code-scanning/analyses",
+                {"ref": self.repository.reference},
+                display_error=False,
+            )
+            return True
+        except:
+            logger.debug(f"Failed to get analyses...")
+        return False
+
     def getOrganizationAlerts(self, state: str = "open") -> list[CodeAlert]:
         """Get list of Organization Alerts.
 
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-an-organization
         """
         results = self.rest.get(
             "/orgs/{org}/code-scanning/alerts", {"state": state}, authenticated=True
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/github.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """GitHub and Repository APIs."""
 import logging
 import os
 import shutil
 import tempfile
 import subprocess
 from dataclasses import dataclass
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 from urllib.parse import urlparse
 
 
 logger = logging.getLogger("ghastoolkit.octokit.github")
 
 
 @dataclass
@@ -95,14 +95,61 @@
                 "/repos/{owner}/{repo}/pulls/{pull_number}/commits",
                 {"pull_number": pull_number},
             )
             for commit in response:
                 result.append(commit.get("sha"))
         return result
 
+    def getPullRequestComments(self) -> list[dict[str, Union[int, str]]]:
+        """Get list of Pull Request comments."""
+        result = []
+        if self.isInPullRequest():
+            from ghastoolkit.octokit.octokit import RestRequest
+
+            issue_number = self.getPullRequestNumber()
+            response = RestRequest().get(
+                "/repos/{owner}/{repo}/issues/{issue_number}/comments",
+                {"issue_number": issue_number},
+            )
+            for comment in response:
+                result.append(
+                    {
+                        "id": comment.get("id"),
+                        "body": comment.get("body", ""),
+                    }
+                )
+        return result
+
+    def createPullRequestComment(self, comment_body: str) -> None:
+        """Create a new Pull Request comment."""
+        if self.isInPullRequest():
+            from ghastoolkit.octokit.octokit import RestRequest
+
+            issue_number = self.getPullRequestNumber()
+            RestRequest().postJson(
+                "/repos/{owner}/{repo}/issues/{issue_number}/comments",
+                {"body": comment_body},
+                expected=201,
+                parameters={"issue_number": issue_number},
+            )
+        return
+
+    def updatePullRequestComment(self, comment_id: int, comment_body: str) -> None:
+        """Update an existing Pull Request comment."""
+        if self.isInPullRequest():
+            from ghastoolkit.octokit.octokit import RestRequest
+
+            RestRequest().patchJson(
+                "/repos/{owner}/{repo}/issues/comments/{comment_id}",
+                {"body": comment_body},
+                expected=200,
+                parameters={"comment_id": comment_id},
+            )
+        return
+
     @property
     def clone_url(self) -> str:
         """Repository clone URL."""
         if GitHub.github_app:
             url = urlparse(GitHub.instance)
             return f"{url.scheme}://x-access-token:{GitHub.token}@{url.netloc}/{self.owner}/{self.repo}.git"
         elif GitHub.token:
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/octokit.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             "Accept": "application/vnd.github.v3+json",
             "X-GitHub-Api-Version": RestRequest.VERSION,
             "Authorization": f"token {GitHub.token}",
         }
 
     @staticmethod
     def restGet(url: str, authenticated: bool = False):
-        """Get Request Wrapper"""
+        """Get Request Wrapper."""
 
         def decorator(func):
             def wrap(self, *args, **kwargs):
                 # if the current class has a rest variable, use it
                 rest = getattr(self, "rest") if hasattr(self, "rest") else RestRequest()
 
                 params = {}
@@ -169,16 +169,17 @@
     @limits(calls=REST_MAX_CALLS, period=60)
     def get(
         self,
         path: str,
         parameters: dict = {},
         expected: int = 200,
         authenticated: bool = False,
+        display_errors: bool = True,
     ) -> Union[dict, list[dict]]:
-        """Get Request
+        """Get Request.
 
         Limits requests based on token
         """
         repo = self.repository or GitHub.repository
         if not repo:
             raise Exception("Repository needs to be set")
 
@@ -202,16 +203,18 @@
         while True:
             params["page"] = page
 
             responce = self.session.get(url, params=params)
             responce_json = responce.json()
 
             if responce.status_code != expected:
-                logger.error(f"Error code from server :: {responce.status_code}")
-                logger.error(f"Content :: {responce_json}")
+                if display_errors:
+                    logger.error(f"Error code from server :: {responce.status_code}")
+                    logger.error(f"Content :: {responce_json}")
+
                 known_error = __OCTOKIT_ERRORS__.get(responce.status_code)
                 if known_error:
                     raise Exception(known_error)
                 raise Exception("REST Request failed :: non-expected server error")
 
             if isinstance(responce_json, dict) and responce_json.get("errors"):
                 logger.error(responce_json.get("message"))
@@ -225,34 +228,58 @@
             if len(responce_json) < RestRequest.PER_PAGE:
                 break
 
             page += 1
 
         return result
 
-    def postJson(self, path: str, data: dict, expected: int = 200) -> dict:
+    def postJson(
+        self, path: str, data: dict, expected: int = 200, parameters={}
+    ) -> dict:
         repo = self.repository or GitHub.repository
         if not repo:
             raise Exception("Repository needs to be set")
 
-        url = Octokit.route(path, repo, rtype="rest")
+        url = Octokit.route(path, repo, rtype="rest", **parameters)
         logger.debug(f"Posting content from URL :: {url}")
 
         response = self.session.post(url, json=data)
 
         if response.status_code != expected:
             logger.error(f"Error code from server :: {response.status_code}")
             logger.error(f"{response.content}")
             known_error = __OCTOKIT_ERRORS__.get(response.status_code)
             if known_error:
                 raise Exception(known_error)
             raise Exception(f"Failed to post data")
 
         return response.json()
 
+    def patchJson(
+        self, path: str, data: dict, expected: int = 200, parameters={}
+    ) -> dict:
+        repo = self.repository or GitHub.repository
+        if not repo:
+            raise Exception("Repository needs to be set")
+
+        url = Octokit.route(path, repo, rtype="rest", **parameters)
+        logger.debug(f"Patching content from URL :: {url}")
+
+        response = self.session.patch(url, json=data)
+
+        if response.status_code != expected:
+            logger.error(f"Error code from server :: {response.status_code}")
+            logger.error(f"{response.content}")
+            known_error = __OCTOKIT_ERRORS__.get(response.status_code)
+            if known_error:
+                raise Exception(known_error)
+            raise Exception("Failed to patch data")
+
+        return response.json()
+
 
 DEFAULT_GRAPHQL_PATHS = [os.path.join(__OCTOKIT_PATH__, "graphql")]
 
 
 class GraphQLRequest:
     def __init__(self, repository: Optional[Repository] = None) -> None:
         self.repository = repository or GitHub.repository
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.6.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.6.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.6.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.6.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.6.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.6.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_advisories.py` & `ghastoolkit-0.6.2/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_codeql_dataext.py` & `ghastoolkit-0.6.2/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_codeql_packs.py` & `ghastoolkit-0.6.2/tests/test_codeql_packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_codeqldb.py` & `ghastoolkit-0.6.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_codescanning.py` & `ghastoolkit-0.6.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_default.py` & `ghastoolkit-0.6.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_dependencies.py` & `ghastoolkit-0.6.2/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_depgraph.py` & `ghastoolkit-0.6.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_github.py` & `ghastoolkit-0.6.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_licenses.py` & `ghastoolkit-0.6.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_octokit.py` & `ghastoolkit-0.6.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.6.1/tests/test_secretscanning.py` & `ghastoolkit-0.6.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

