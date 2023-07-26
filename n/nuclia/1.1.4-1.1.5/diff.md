# Comparing `tmp/nuclia-1.1.4.tar.gz` & `tmp/nuclia-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.4.tar", last modified: Fri Jul 21 09:26:28 2023, max compression
+gzip compressed data, was "nuclia-1.1.5.tar", last modified: Wed Jul 26 11:51:07 2023, max compression
```

## Comparing `nuclia-1.1.4.tar` & `nuclia-1.1.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.444298 nuclia-1.1.4/
--rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-21 09:26:27.000000 nuclia-1.1.4/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-21 09:26:27.000000 nuclia-1.1.4/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)      886 2023-07-21 09:26:27.000000 nuclia-1.1.4/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-21 09:26:27.000000 nuclia-1.1.4/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-21 09:26:27.000000 nuclia-1.1.4/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-21 09:26:27.000000 nuclia-1.1.4/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:26:28.444494 nuclia-1.1.4/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-21 09:26:27.000000 nuclia-1.1.4/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-21 09:26:27.000000 nuclia-1.1.4/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-21 09:26:27.000000 nuclia-1.1.4/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.431593 nuclia-1.1.4/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/EXTRACT.md
--rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-21 09:26:27.000000 nuclia-1.1.4/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.432830 nuclia-1.1.4/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.435443 nuclia-1.1.4/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     3068 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.437064 nuclia-1.1.4/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/nua_responses.py
--rw-r--r--   0 ebr        (501) staff       (20)      472 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/lib/utils.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.441634 nuclia-1.1.4/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     3555 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/resource.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.443505 nuclia-1.1.4/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.443899 nuclia-1.1.4/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-21 09:26:27.000000 nuclia-1.1.4/nuclia/tests/test_resource.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-21 09:26:28.434619 nuclia-1.1.4/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-21 09:26:28.000000 nuclia-1.1.4/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-21 09:26:27.000000 nuclia-1.1.4/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-21 09:26:28.445120 nuclia-1.1.4/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-21 09:26:27.000000 nuclia-1.1.4/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-21 09:26:27.000000 nuclia-1.1.4/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.515290 nuclia-1.1.5/
+-rw-r--r--   0 ebr        (501) staff       (20)       43 2023-07-26 11:51:06.000000 nuclia-1.1.5/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-26 11:51:06.000000 nuclia-1.1.5/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)     1002 2023-07-26 11:51:06.000000 nuclia-1.1.5/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-26 11:51:06.000000 nuclia-1.1.5/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-26 11:51:06.000000 nuclia-1.1.5/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-26 11:51:06.000000 nuclia-1.1.5/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-26 11:51:07.515452 nuclia-1.1.5/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-26 11:51:06.000000 nuclia-1.1.5/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-26 11:51:06.000000 nuclia-1.1.5/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-26 11:51:06.000000 nuclia-1.1.5/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.501650 nuclia-1.1.5/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/EXTRACT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-26 11:51:06.000000 nuclia-1.1.5/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.503769 nuclia-1.1.5/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      339 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.506920 nuclia-1.1.5/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6734 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3473 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.508817 nuclia-1.1.5/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     5507 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/nua_responses.py
+-rw-r--r--   0 ebr        (501) staff       (20)      472 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/lib/utils.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.513106 nuclia-1.1.5/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      388 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      647 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     8210 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2091 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      311 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3570 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.514796 nuclia-1.1.5/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.515042 nuclia-1.1.5/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      894 2023-07-26 11:51:06.000000 nuclia-1.1.5/nuclia/tests/test_resource.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-26 11:51:07.506113 nuclia-1.1.5/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1311 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-26 11:51:07.000000 nuclia-1.1.5/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-26 11:51:06.000000 nuclia-1.1.5/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-26 11:51:07.515964 nuclia-1.1.5/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-26 11:51:06.000000 nuclia-1.1.5/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-26 11:51:06.000000 nuclia-1.1.5/test-requirements.txt
```

### Comparing `nuclia-1.1.4/CHANGELOG.md` & `nuclia-1.1.5/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 1.1.5 (2023-07-26)
+
+- Support summary as resource attribute
+- Allow to create kb
+- Allow to set default account
+
 ## 1.1.4 (2023-07-21)
 
 - Fix http status check
 
 ## 1.1.3 (2023-07-21)
 
 - Use pyyaml==5.3.1 as 5.4 is broken
```

### Comparing `nuclia-1.1.4/LICENSE` & `nuclia-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/PKG-INFO` & `nuclia-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.4
+Version: 1.1.5
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.4/README.md` & `nuclia-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/AUTH.md` & `nuclia-1.1.5/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/CONVERSATION.md` & `nuclia-1.1.5/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/DEFAULT.md` & `nuclia-1.1.5/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/EXTRACT.md` & `nuclia-1.1.5/docs/EXTRACT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/README.md` & `nuclia-1.1.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/SEARCH.md` & `nuclia-1.1.5/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/docs/UPLOAD.md` & `nuclia-1.1.5/docs/UPLOAD.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/cli/run.py` & `nuclia-1.1.5/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/cli/utils.py` & `nuclia-1.1.5/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/config.py` & `nuclia-1.1.5/nuclia/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     def __str__(self):
         return f"{self.slug:15} => {self.title:40}"
 
 
 class Selection(BaseModel):
     nua: Optional[str] = None
     kbid: Optional[str] = None
+    account: Optional[str] = None
 
 
 class Config(BaseModel):
     accounts: Optional[List[Account]] = []
     kbs: Optional[List[KnowledgeBox]] = []
     kbs_token: List[KnowledgeBox] = []
     nuas_token: List[NuaKey] = []
@@ -151,30 +152,41 @@
 
         if yes_no(f"Do you want to setup KB {url} as default one?"):
             if self.default is None:
                 self.default = Selection()
             self.default.kbid = kbid
         self.save()
 
-    def get_default_kb(self) -> str:
-        if self.default is None or self.default.kbid is None:
-            raise NotDefinedDefault()
-        return self.default.kbid
-
     def get_default_nua(self) -> str:
         if self.default is None or self.default.nua is None:
             raise NotDefinedDefault()
         return self.default.nua
 
     def set_default_nua(self, nua: str):
         if self.default is None:
             self.default = Selection()
         self.default.nua = nua
         self.save()
 
+    def get_default_account(self) -> str:
+        if self.default is None or self.default.account is None:
+            raise NotDefinedDefault()
+        return self.default.account
+
+    def set_default_account(self, account: str):
+        if self.default is None:
+            self.default = Selection()
+        self.default.account = account
+        self.save()
+
+    def get_default_kb(self) -> str:
+        if self.default is None or self.default.kbid is None:
+            raise NotDefinedDefault()
+        return self.default.kbid
+
     def set_default_kb(self, kbid: str):
         if self.default is None:
             self.default = Selection()
         self.default.kbid = kbid
         self.save()
 
     def save(self):
```

### Comparing `nuclia-1.1.4/nuclia/data.py` & `nuclia-1.1.5/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/decorators.py` & `nuclia-1.1.5/nuclia/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,14 +91,29 @@
         )
         kwargs["nc"] = nc
         return func(*args, **kwargs)
 
     return wrapper_checkout_nua
 
 
+def account(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        if not kwargs.get("account"):
+            auth = get_auth()
+            account_slug = auth._config.get_default_account()
+            if account_slug is None:
+                raise NotDefinedDefault()
+            else:
+                kwargs["account"] = account_slug
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 def pretty(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
         if kwargs.get("json"):
             return result.json(indent=2)
         if kwargs.get("yaml"):
```

### Comparing `nuclia-1.1.4/nuclia/lib/kb.py` & `nuclia-1.1.5/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/lib/nua.py` & `nuclia-1.1.5/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/sdk/auth.py` & `nuclia-1.1.5/nuclia/sdk/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 import json
 import readline  # noqa
 import webbrowser
-from typing import Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 
 from nuclia import BASE, get_global_url
 from nuclia.cli.utils import yes_no
 from nuclia.config import Account, Config, KnowledgeBox, Zone
 from nuclia.exceptions import NeedUserToken, UserTokenExpired
@@ -28,19 +28,26 @@
             from nuclia.data import get_config
 
             self._inner_config = get_config()
         return self._inner_config
 
     def show(self):
         if self._config.default:
-            print("Default Knowledge Box")
-            print("=====================")
-            print()
-            print(self._config.get_kb(self._config.default.kbid))
-            print()
+            if self._config.default.account:
+                print("Default Account")
+                print("===============")
+                print()
+                print(self._config.default.account)
+                print()
+            if self._config.default.kbid:
+                print("Default Knowledge Box")
+                print("=====================")
+                print()
+                print(self._config.get_kb(self._config.default.kbid))
+                print()
 
         if self._config.token:
             print("User Auth")
             print("=========")
             print()
             self._show_user()
             print()
@@ -124,15 +131,15 @@
         if resp.status_code == 200:
             data = resp.json()
             return data.get("uuid"), data.get("config", {}).get("title")
         else:
             return None, None
 
     def _show_user(self):
-        resp = self.get_user(MEMBER)
+        resp = self._request("GET", MEMBER)
         print(f"User: {resp.get('name')} <{resp.get('email')}>")
         print(f"Type: {resp.get('type')}")
 
     def login(self):
         """
         Lets redirect the user to the UI to capture a token
         """
@@ -180,67 +187,63 @@
         else:
             return False
 
     def post_login(self):
         self.accounts()
         self.zones()
 
-    def post_user(self, path: str, payload: Dict[str, str]):
-        if not self._config.token:
-            raise NeedUserToken()
-        resp = requests.post(
-            path,
-            headers={"Authorization": f"Bearer {self._config.token}"},
-            data=payload,
-        )
-        if resp.status_code == 201:
-            return resp.json()
-        elif resp.status_code == 403:
-            raise UserTokenExpired()
-
-    def get_user(self, path: str):
+    def _request(self, method: str, path: str, data: Optional[Any] = None):
         if not self._config.token:
             raise NeedUserToken()
-        resp = requests.get(
+        kwargs = {"headers": {"Authorization": f"Bearer {self._config.token}"}}
+        if data is not None:
+            non_null_values = {k: v for k, v in data.items() if v is not None}
+            kwargs["data"] = json.dumps(non_null_values)
+        resp = requests.request(
+            method,
             path,
-            headers={"Authorization": f"Bearer {self._config.token}"},
+            **kwargs,
         )
-        if resp.status_code == 200:
+        if resp.status_code == 204:
+            return None
+        elif resp.status_code >= 200 and resp.status_code < 300:
             return resp.json()
         elif resp.status_code == 403:
             raise UserTokenExpired()
+        else:
+            raise Exception(resp.text)
 
     def accounts(self) -> List[Account]:
-        accounts = self.get_user(ACCOUNTS)
+        accounts = self._request("GET", ACCOUNTS)
         result = []
         self._config.accounts = []
         for account in accounts:
             account_obj = Account.parse_obj(account)
             result.append(account_obj)
             self._config.accounts.append(account_obj)
         self._config.save()
         return result
 
     def zones(self) -> List[Zone]:
-        zones = self.get_user(ZONES)
+        zones = self._request("GET", ZONES)
         if self._config.accounts is None:
             self._config.accounts = []
         self._config.zones = []
         result = []
         for zone in zones:
             zone_obj = Zone.parse_obj(zone)
             result.append(zone_obj)
             self._config.zones.append(zone_obj)
         self._config.save()
         return result
 
     def kbs(self, account: str):
         path = LIST_KBS.format(account=account)
         try:
-            kbs = self.get_user(path)
+            kbs = self._request("GET", path)
         except UserTokenExpired:
             return []
         result = []
         zones = self.zones()
         region = {zone.id: zone.slug for zone in zones}
         for kb in kbs:
             zone = region[kb["zone"]]
```

### Comparing `nuclia-1.1.4/nuclia/sdk/kb.py` & `nuclia-1.1.5/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/sdk/nuas.py` & `nuclia-1.1.5/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/sdk/resource.py` & `nuclia-1.1.5/nuclia/sdk/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "extra",
     "conversations",
     "links",
     "texts",
     "usermetadata",
     "fieldmetadata",
     "title",
+    "summary",
 ]
 
 
 class NucliaResource:
     """
     Manage existing resource
```

### Comparing `nuclia-1.1.4/nuclia/sdk/search.py` & `nuclia-1.1.5/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/sdk/upload.py` & `nuclia-1.1.5/nuclia/sdk/upload.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/tests/fixtures.py` & `nuclia-1.1.5/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/tests/test_conversation.py` & `nuclia-1.1.5/nuclia/tests/test_conversation.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia/tests/test_resource.py` & `nuclia-1.1.5/nuclia/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.5/nuclia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.4
+Version: 1.1.5
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.4/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.5/nuclia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.4/setup.py` & `nuclia-1.1.5/setup.py`

 * *Files identical despite different names*

