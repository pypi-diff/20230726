# Comparing `tmp/garth-0.2.3.tar.gz` & `tmp/garth-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.2.3.tar", last modified: Wed Jul 26 14:45:04 2023, max compression
+gzip compressed data, was "garth-0.2.4.tar", last modified: Wed Jul 26 14:57:14 2023, max compression
```

## Comparing `garth-0.2.3.tar` & `garth-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.3/LICENSE
--rw-r--r--   0        0        0     4531 2023-07-26 13:24:49.157851 garth-0.2.3/README.md
--rw-r--r--   0        0        0      408 2023-07-26 13:24:49.158278 garth-0.2.3/garth/__init__.py
--rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.3/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.3/garth/exc.py
--rw-r--r--   0        0        0     4870 2023-07-23 16:06:33.692262 garth-0.2.3/garth/http.py
--rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.3/garth/resources/__init__.py
--rw-r--r--   0        0        0     2691 2023-07-26 14:41:50.363353 garth-0.2.3/garth/resources/stress.py
--rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.3/garth/sso.py
--rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.3/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-26 14:44:42.196563 garth-0.2.3/garth/version.py
--rw-r--r--   0        0        0      854 2023-07-26 14:45:04.460126 garth-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.3/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.3/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.3/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.3/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.3/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.3/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.3/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.3/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.3/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.3/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.3/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     2940 2023-07-23 16:06:33.706957 garth-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.3/tests/resources/cassettes/test_daily.yaml
--rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.3/tests/resources/cassettes/test_daily_pagination.yaml
--rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.3/tests/resources/cassettes/test_weekly.yaml
--rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.3/tests/resources/cassettes/test_weekly_pagination.yaml
--rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.3/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.3/tests/test_auth_token.py
--rw-r--r--   0        0        0     4314 2023-07-23 16:06:33.707155 garth-0.2.3/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.3/tests/test_sso.py
--rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 garth-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4531 2023-07-26 13:24:49.157851 garth-0.2.4/README.md
+-rw-r--r--   0        0        0      408 2023-07-26 13:24:49.158278 garth-0.2.4/garth/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-23 13:39:36.444380 garth-0.2.4/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.2.4/garth/exc.py
+-rw-r--r--   0        0        0     4870 2023-07-23 16:06:33.692262 garth-0.2.4/garth/http.py
+-rw-r--r--   0        0        0       89 2023-07-26 13:24:49.158749 garth-0.2.4/garth/resources/__init__.py
+-rw-r--r--   0        0        0     2698 2023-07-26 14:56:27.975003 garth-0.2.4/garth/resources/stress.py
+-rw-r--r--   0        0        0     3552 2023-07-23 16:09:16.949253 garth-0.2.4/garth/sso.py
+-rw-r--r--   0        0        0      573 2023-07-26 14:44:24.360714 garth-0.2.4/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-26 14:57:08.603253 garth-0.2.4/garth/version.py
+-rw-r--r--   0        0        0      854 2023-07-26 14:57:14.010285 garth-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.2.4/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.2.4/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.2.4/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-23 16:06:33.706591 garth-0.2.4/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-23 16:06:33.706751 garth-0.2.4/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-23 13:06:17.267462 garth-0.2.4/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.2.4/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.2.4/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.2.4/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-23 13:09:36.525519 garth-0.2.4/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-23 13:36:21.976543 garth-0.2.4/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     2940 2023-07-23 16:06:33.706957 garth-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     6252 2023-07-26 13:24:49.161636 garth-0.2.4/tests/resources/cassettes/test_daily.yaml
+-rw-r--r--   0        0        0    10389 2023-07-26 13:24:49.161944 garth-0.2.4/tests/resources/cassettes/test_daily_pagination.yaml
+-rw-r--r--   0        0        0     4717 2023-07-26 13:24:49.162252 garth-0.2.4/tests/resources/cassettes/test_weekly.yaml
+-rw-r--r--   0        0        0     7522 2023-07-26 13:24:49.162569 garth-0.2.4/tests/resources/cassettes/test_weekly_pagination.yaml
+-rw-r--r--   0        0        0     1172 2023-07-26 13:24:49.162843 garth-0.2.4/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.2.4/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4314 2023-07-23 16:06:33.707155 garth-0.2.4/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-23 13:18:13.595293 garth-0.2.4/tests/test_sso.py
+-rw-r--r--   0        0        0      562 2023-07-26 14:44:24.930577 garth-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 garth-0.2.4/PKG-INFO
```

### Comparing `garth-0.2.3/LICENSE` & `garth-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/README.md` & `garth-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/garth/auth_token.py` & `garth-0.2.4/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/garth/http.py` & `garth-0.2.4/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/garth/resources/stress.py` & `garth-0.2.4/garth/resources/stress.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @dataclass(frozen=True)
 class DailyStress:
     calendar_date: date
     overall_stress_level: int
     rest_stress_duration: int
     low_stress_duration: int
     medium_stress_duration: int
-    high_stress_duration: int
+    high_stress_duration: int | None
 
     _path: ClassVar[str] = f"{BASE_PATH}/daily"
     _page_size: ClassVar[int] = 28
 
     @classmethod
     def get(
         cls,
```

### Comparing `garth-0.2.3/garth/sso.py` & `garth-0.2.4/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/garth/utils.py` & `garth-0.2.4/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/pyproject.toml` & `garth-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "requests>=2.27.0",
     "pydantic>=2.1.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.2.3/tests/cassettes/test_client_get.yaml` & `garth-0.2.4/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_client_post.yaml` & `garth-0.2.4/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_client_request.yaml` & `garth-0.2.4/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_connectapi.yaml` & `garth-0.2.4/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.2.4/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_exchange.yaml` & `garth-0.2.4/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_get_username.yaml` & `garth-0.2.4/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.2.4/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_login_success.yaml` & `garth-0.2.4/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_refresh.yaml` & `garth-0.2.4/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/cassettes/test_refresh_expired.yaml` & `garth-0.2.4/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/conftest.py` & `garth-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/resources/cassettes/test_daily.yaml` & `garth-0.2.4/tests/resources/cassettes/test_daily.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/resources/cassettes/test_daily_pagination.yaml` & `garth-0.2.4/tests/resources/cassettes/test_daily_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/resources/cassettes/test_weekly.yaml` & `garth-0.2.4/tests/resources/cassettes/test_weekly.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/resources/cassettes/test_weekly_pagination.yaml` & `garth-0.2.4/tests/resources/cassettes/test_weekly_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/resources/test_stress.py` & `garth-0.2.4/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/test_auth_token.py` & `garth-0.2.4/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/test_http.py` & `garth-0.2.4/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/test_sso.py` & `garth-0.2.4/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/tests/test_utils.py` & `garth-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.2.3/PKG-INFO` & `garth-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.2.3
+Version: 0.2.4
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: requests>=2.27.0
 Requires-Dist: pydantic>=2.1.1
 Description-Content-Type: text/markdown
```

