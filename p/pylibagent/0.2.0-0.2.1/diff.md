# Comparing `tmp/pylibagent-0.2.0.tar.gz` & `tmp/pylibagent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibagent-0.2.0.tar", last modified: Tue May 30 10:04:26 2023, max compression
+gzip compressed data, was "pylibagent-0.2.1.tar", last modified: Wed Jul 26 08:04:32 2023, max compression
```

## Comparing `pylibagent-0.2.0.tar` & `pylibagent-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.932541 pylibagent-0.2.0/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.936541 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.940541 pylibagent-0.2.0/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-15 21:09:32.000000 pylibagent-0.2.0/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 pylibagent-0.2.0/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 pylibagent-0.2.0/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-05-30 10:04:26.944541 pylibagent-0.2.0/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     2617 2022-12-05 07:42:14.000000 pylibagent-0.2.0/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/pylibagent/
--rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-07-04 09:31:51.000000 pylibagent-0.2.0/pylibagent/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    12918 2023-05-30 09:48:07.000000 pylibagent-0.2.0/pylibagent/agent.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      823 2022-11-15 14:58:49.000000 pylibagent-0.2.0/pylibagent/check.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1576 2022-11-18 11:52:45.000000 pylibagent-0.2.0/pylibagent/logger.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-05-30 09:48:48.000000 pylibagent-0.2.0/pylibagent/version.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/pylibagent.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      433 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       66 2022-11-16 21:17:54.000000 pylibagent-0.2.0/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-30 10:04:26.944541 pylibagent-0.2.0/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1550 2022-11-16 21:18:12.000000 pylibagent-0.2.0/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.780537 pylibagent-0.2.1/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.772536 pylibagent-0.2.1/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.776536 pylibagent-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 pylibagent-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 pylibagent-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.776536 pylibagent-0.2.1/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-15 21:09:32.000000 pylibagent-0.2.1/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 pylibagent-0.2.1/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 pylibagent-0.2.1/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-07-26 08:04:32.780537 pylibagent-0.2.1/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2617 2022-12-05 07:42:14.000000 pylibagent-0.2.1/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.776536 pylibagent-0.2.1/pylibagent/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-07-04 09:31:51.000000 pylibagent-0.2.1/pylibagent/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    12918 2023-05-30 09:48:07.000000 pylibagent-0.2.1/pylibagent/agent.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      823 2022-11-15 14:58:49.000000 pylibagent-0.2.1/pylibagent/check.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1576 2022-11-18 11:52:45.000000 pylibagent-0.2.1/pylibagent/logger.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-07-26 08:02:44.000000 pylibagent-0.2.1/pylibagent/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-07-26 08:04:32.780537 pylibagent-0.2.1/pylibagent.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-07-26 08:04:32.000000 pylibagent-0.2.1/pylibagent.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      433 2023-07-26 08:04:32.000000 pylibagent-0.2.1/pylibagent.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-07-26 08:04:32.000000 pylibagent-0.2.1/pylibagent.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-07-26 08:04:32.000000 pylibagent-0.2.1/pylibagent.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-07-26 08:04:32.000000 pylibagent-0.2.1/pylibagent.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       66 2023-07-26 08:03:28.000000 pylibagent-0.2.1/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-07-26 08:04:32.780537 pylibagent-0.2.1/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1550 2022-11-16 21:18:12.000000 pylibagent-0.2.1/setup.py
```

### Comparing `pylibagent-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pylibagent-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pylibagent-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/.github/workflows/ci.yml` & `pylibagent-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/.gitignore` & `pylibagent-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/LICENSE` & `pylibagent-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/PKG-INFO` & `pylibagent-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylibagent
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for building InfraSonar agents
 Home-page: https://github.com/infrasonar/python-libagent
-Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.0
+Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.1
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,agent
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pylibagent-0.2.0/README.md` & `pylibagent-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/pylibagent/agent.py` & `pylibagent-0.2.1/pylibagent/agent.py`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/pylibagent/check.py` & `pylibagent-0.2.1/pylibagent/check.py`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/pylibagent/logger.py` & `pylibagent-0.2.1/pylibagent/logger.py`

 * *Files identical despite different names*

### Comparing `pylibagent-0.2.0/pylibagent.egg-info/PKG-INFO` & `pylibagent-0.2.1/pylibagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylibagent
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for building InfraSonar agents
 Home-page: https://github.com/infrasonar/python-libagent
-Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.0
+Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.1
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,agent
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pylibagent-0.2.0/setup.py` & `pylibagent-0.2.1/setup.py`

 * *Files identical despite different names*

