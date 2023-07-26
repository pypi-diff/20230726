# Comparing `tmp/jf_ingest-0.0.2.tar.gz` & `tmp/jf_ingest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jf_ingest-0.0.2.tar", last modified: Tue Jul 25 19:08:07 2023, max compression
+gzip compressed data, was "jf_ingest-0.0.3.tar", last modified: Wed Jul 26 15:55:55 2023, max compression
```

## Comparing `jf_ingest-0.0.2.tar` & `jf_ingest-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.2/LICENSE
--rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.2/README.md
--rw-r--r--   0        0        0      619 2023-07-25 19:08:07.247513 jf_ingest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 jf_ingest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.3/LICENSE
+-rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 15:55:41.201986 jf_ingest-0.0.3/jf_ingest/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:28:01.314868 jf_ingest-0.0.3/jf_ingest/jf_jira/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-21 18:28:01.315993 jf_ingest-0.0.3/jf_ingest/jf_jira/downloaders.py
+-rw-r--r--   0        0        0      679 2023-07-26 15:55:55.443279 jf_ingest-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:55:41.203566 jf_ingest-0.0.3/tests/jf_jira/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-26 15:55:41.204174 jf_ingest-0.0.3/tests/jf_jira/fixtures/jira_fields_response.json
+-rw-r--r--   0        0        0     3162 2023-07-26 15:55:41.204525 jf_ingest-0.0.3/tests/jf_jira/test_jira_downloaders.py
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 jf_ingest-0.0.3/PKG-INFO
```

### Comparing `jf_ingest-0.0.2/LICENSE` & `jf_ingest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.2/pyproject.toml` & `jf_ingest-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jf_ingest"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 description = "library used for ingesting jira data"
 authors = [
     { name = "jellyfish-oss", email = "oss@jellyfish.co" },
 ]
 dependencies = [
     "jira >= 2.0.0, < 2.1",
@@ -19,14 +19,19 @@
 Homepage = "https://github.com/Jellyfish-AI/jf_ingest"
 
 [tool.pdm]
 source = [
     { url = "https://pypi.org/simple", verify_ssl = true, name = "pypi" },
 ]
 
+[tool.pdm.build]
+excludes = [
+    "**/.pytest_cache/**",
+]
+
 [tool.pdm.dev-dependencies]
 dev = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

