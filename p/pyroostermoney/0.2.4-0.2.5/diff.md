# Comparing `tmp/pyroostermoney-0.2.4.tar.gz` & `tmp/pyroostermoney-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.2.4.tar", last modified: Sun Jul 23 10:01:18 2023, max compression
+gzip compressed data, was "pyroostermoney-0.2.5.tar", last modified: Wed Jul 26 16:41:17 2023, max compression
```

## Comparing `pyroostermoney-0.2.4.tar` & `pyroostermoney-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.512096 pyroostermoney-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/standing_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/child/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/master_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-23 10:01:18.000000 pyroostermoney-0.2.4/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-23 10:01:18.000000 pyroostermoney-0.2.4/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 10:01:18.000000 pyroostermoney-0.2.4/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-23 10:01:18.000000 pyroostermoney-0.2.4/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-23 10:01:18.000000 pyroostermoney-0.2.4/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-23 10:01:18.516096 pyroostermoney-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-23 10:01:07.000000 pyroostermoney-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/standing_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/master_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 16:41:17.947302 pyroostermoney-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/setup.py
```

### Comparing `pyroostermoney-0.2.4/.github/workflows/build.yml` & `pyroostermoney-0.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/.gitignore` & `pyroostermoney-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/LICENSE` & `pyroostermoney-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/PKG-INFO` & `pyroostermoney-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.4
+Version: 0.2.5
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.4/cli.py` & `pyroostermoney-0.2.5/cli.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/api.py` & `pyroostermoney-0.2.5/pyroostermoney/api.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/__init__.py` & `pyroostermoney-0.2.5/pyroostermoney/child/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/card.py` & `pyroostermoney-0.2.5/pyroostermoney/child/card.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/jobs.py` & `pyroostermoney-0.2.5/pyroostermoney/child/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ANYTIME = 1
     UNKNOWN = -1
 
 class JobTime(Enum):
     """Job times."""
     MORNING = 12
     AFTERNOON = 17
+    EVENING = 22
     ANYTIME = 23
 
 class JobState(Enum):
     """Job states."""
     NO_PREVIOUS_STATE = 0
     TODO = 1
     AWAITING_APPROVAL = 2
```

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.2.5/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/standing_order.py` & `pyroostermoney-0.2.5/pyroostermoney/child/standing_order.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/child/transaction.py` & `pyroostermoney-0.2.5/pyroostermoney/child/transaction.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/const.py` & `pyroostermoney-0.2.5/pyroostermoney/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.2.4"
+VERSION="0.2.5"
 BASE_URL="https://api.rooster.money"
 OAUTH_TOKEN_URL="https://auth.rooster.money/oidc/token"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
```

### Comparing `pyroostermoney-0.2.4/pyroostermoney/events.py` & `pyroostermoney-0.2.5/pyroostermoney/events.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/exceptions.py` & `pyroostermoney-0.2.5/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/family_account.py` & `pyroostermoney-0.2.5/pyroostermoney/family_account.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/master_jobs.py` & `pyroostermoney-0.2.5/pyroostermoney/master_jobs.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney/roostermoney.py` & `pyroostermoney-0.2.5/pyroostermoney/roostermoney.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.4/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.2.5/pyroostermoney.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.4
+Version: 0.2.5
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.4/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.2.5/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

