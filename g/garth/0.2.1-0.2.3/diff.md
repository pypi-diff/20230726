# Comparing `tmp/garth-0.2.1.tar.gz` & `tmp/garth-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.1.tar", last modified: Sun Jul 23 16:28:07 2023, max compression
+gzip compressed data, was "garth-0.2.3.tar", last modified: Wed Jul 26 14:45:04 2023, max compression
```

## Comparing `garth-0.2.1.tar` & `garth-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.1/LICENSE
--rw-r--r--   0        0        0     3708 2023-07-22 17:44:18.353928 garth-0.2.1/README.md
--rw-r--r--   0        0        0      188 2023-07-23 16:26:05.839179 garth-0.2.1/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.1/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.1/garth/exc.py
--rw-r--r--   0        0        0     4870 2023-07-23 16:06:33.692262 garth-0.2.1/garth/http.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.1/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.2.1/garth/version.py
--rw-r--r--   0        0        0      809 2023-07-23 16:28:07.827793 garth-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.1/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.1/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.1/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.1/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.1/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.1/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.1/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.1/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.1/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.1/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.1/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2940 2023-07-23 16:06:33.706957 garth-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.1/tests/test_auth_token.py
--rw-r--r--   0        0        0     4314 2023-07-23 16:06:33.707155 garth-0.2.1/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.1/tests/test_sso.py
--rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 garth-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4531 2023-07-26 13:24:49.157851 garth-0.2.3/README.md
+-rw-r--r--   0        0        0      408 2023-07-26 13:24:49.158278 garth-0.2.3/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.3/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.3/garth/exc.py
+-rw-r--r--   0        0        0     4870 2023-07-23 16:06:33.692262 garth-0.2.3/garth/http.py
+-rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.3/garth/resources/__init__.py
+-rw-r--r--   0        0        0     2691 2023-07-26 14:41:50.363353 garth-0.2.3/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.3/garth/sso.py
+-rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.3/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-26 14:44:42.196563 garth-0.2.3/garth/version.py
+-rw-r--r--   0        0        0      854 2023-07-26 14:45:04.460126 garth-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.3/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.3/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.3/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.3/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.3/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.3/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.3/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.3/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.3/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.3/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.3/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2940 2023-07-23 16:06:33.706957 garth-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.3/tests/resources/cassettes/test_daily.yaml
+-rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.3/tests/resources/cassettes/test_daily_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.3/tests/resources/cassettes/test_weekly.yaml
+-rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.3/tests/resources/cassettes/test_weekly_pagination.yaml
+-rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.3/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.3/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4314 2023-07-23 16:06:33.707155 garth-0.2.3/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.3/tests/test_sso.py
+-rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 garth-0.2.3/PKG-INFO
```

### Comparing `garth-0.2.1/LICENSE` & `garth-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/README.md` & `garth-0.2.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Garth
 
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
 Garmin SSO auth + Connect client
 
+## Google Colabs
+
+[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+
+
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
 
@@ -17,19 +22,19 @@
 ### Authentication
 
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses the same embedded SSO as the mobile app
-1. Only requires `requests` as a dependency
+1. Only requires `requests` and `pydantic` as a dependencies
 1. Supports MFA
 1. Supports saving and resuming sessions to avoid the need to log in each time
 you run a script, which is particularly useful if you have MFA enabled
-1. Appears to be working on Google Colab thus far 🤞🏽
+1. Works on Google Colab
 
 ### Python 3.10+
 
 Google Colab, currently, uses 3.10. We should take advantage of all the goodies
 that come along with it. If you need to use an earlier version of Python, there
 are other libraries that will meet your needs. There's no intetion to backport.
 
@@ -135,10 +140,50 @@
         "overallStressLevel": 33,
         "restStressDuration": 30960,
         "mediumStressDuration": 8760
     }
 }
 ```
 
-## Google Colabs
+## Resources
 
-[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+### Stress
+
+Daily stress levels
+
+```python
+DailyStress.get("2023-07-23", 2)
+```
+
+```python
+[
+    DailyStress(
+        calendar_date=datetime.date(2023, 7, 22),
+        overall_stress_level=31,
+        rest_stress_duration=31980,
+        low_stress_duration=23820,
+        medium_stress_duration=7440,
+        high_stress_duration=1500
+    ),
+    DailyStress(
+        calendar_date=datetime.date(2023, 7, 23),
+        overall_stress_level=26,
+        rest_stress_duration=38220,
+        low_stress_duration=22500,
+        medium_stress_duration=2520,
+        high_stress_duration=300
+    )
+]
+```
+
+Weekly stress levels
+
+```python
+WeeklyStress.get("2023-07-23", 2)
+```
+
+```python
+[
+    WeeklyStress(calendar_date=datetime.date(2023, 7, 10), value=33),
+    WeeklyStress(calendar_date=datetime.date(2023, 7, 17), value=32)
+]
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `garth-0.2.1/garth/auth_token.py` & `garth-0.2.3/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/garth/http.py` & `garth-0.2.3/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/garth/sso.py` & `garth-0.2.3/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_client_get.yaml` & `garth-0.2.3/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_client_post.yaml` & `garth-0.2.3/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_client_request.yaml` & `garth-0.2.3/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_connectapi.yaml` & `garth-0.2.3/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.3/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_exchange.yaml` & `garth-0.2.3/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_get_username.yaml` & `garth-0.2.3/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.3/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_login_success.yaml` & `garth-0.2.3/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_refresh.yaml` & `garth-0.2.3/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.3/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/conftest.py` & `garth-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/test_auth_token.py` & `garth-0.2.3/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/test_http.py` & `garth-0.2.3/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/tests/test_sso.py` & `garth-0.2.3/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.1/PKG-INFO` & `garth-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.1
+Version: 0.2.3
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: requests>=2.27.0
+Requires-Dist: pydantic>=2.1.1
 Description-Content-Type: text/markdown
 
 # Garth
 
 [![CI](https://github.com/matin/garth/workflows/CI/badge.svg?event=push)](https://github.com/matin/garth/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![codecov](https://codecov.io/gh/matin/garth/branch/main/graph/badge.svg?token=0EFFYJNFIL)](https://codecov.io/gh/matin/garth)
 
 Garmin SSO auth + Connect client
 
+## Google Colabs
+
+[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+
+
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
 
@@ -27,19 +33,19 @@
 ### Authentication
 
 The most important reasoning is to build a library with authentication that
 works on [Google Colab](https://colab.research.google.com/) and doesn't require
 tools like Cloudscraper. Garth, in comparison:
 
 1. Uses the same embedded SSO as the mobile app
-1. Only requires `requests` as a dependency
+1. Only requires `requests` and `pydantic` as a dependencies
 1. Supports MFA
 1. Supports saving and resuming sessions to avoid the need to log in each time
 you run a script, which is particularly useful if you have MFA enabled
-1. Appears to be working on Google Colab thus far 🤞🏽
+1. Works on Google Colab
 
 ### Python 3.10+
 
 Google Colab, currently, uses 3.10. We should take advantage of all the goodies
 that come along with it. If you need to use an earlier version of Python, there
 are other libraries that will meet your needs. There's no intetion to backport.
 
@@ -145,10 +151,50 @@
         "overallStressLevel": 33,
         "restStressDuration": 30960,
         "mediumStressDuration": 8760
     }
 }
 ```
 
-## Google Colabs
+## Resources
 
-[Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
+### Stress
+
+Daily stress levels
+
+```python
+DailyStress.get("2023-07-23", 2)
+```
+
+```python
+[
+    DailyStress(
+        calendar_date=datetime.date(2023, 7, 22),
+        overall_stress_level=31,
+        rest_stress_duration=31980,
+        low_stress_duration=23820,
+        medium_stress_duration=7440,
+        high_stress_duration=1500
+    ),
+    DailyStress(
+        calendar_date=datetime.date(2023, 7, 23),
+        overall_stress_level=26,
+        rest_stress_duration=38220,
+        low_stress_duration=22500,
+        medium_stress_duration=2520,
+        high_stress_duration=300
+    )
+]
+```
+
+Weekly stress levels
+
+```python
+WeeklyStress.get("2023-07-23", 2)
+```
+
+```python
+[
+    WeeklyStress(calendar_date=datetime.date(2023, 7, 10), value=33),
+    WeeklyStress(calendar_date=datetime.date(2023, 7, 17), value=32)
+]
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

