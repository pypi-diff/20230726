# Comparing `tmp/healthcheck_pinger-0.0.5.tar.gz` & `tmp/HealthCheck_Pinger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthcheck_pinger-0.0.5.tar", last modified: Sun Jan 22 18:45:12 2023, max compression
+gzip compressed data, was "HealthCheck_Pinger-0.0.6.tar", last modified: Wed Jul 26 16:01:41 2023, max compression
```

## Comparing `healthcheck_pinger-0.0.5.tar` & `HealthCheck_Pinger-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-22 18:45:12.434698 healthcheck_pinger-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-01-22 18:45:12.402120 healthcheck_pinger-0.0.5/HealthCheck_Pinger/
--rw-rw-rw-   0        0        0       58 2022-09-13 07:43:13.000000 healthcheck_pinger-0.0.5/HealthCheck_Pinger/__init__.py
--rw-rw-rw-   0        0        0     1113 2022-09-13 07:47:03.000000 healthcheck_pinger-0.0.5/HealthCheck_Pinger/core.py
--rw-rw-rw-   0        0        0      602 2022-09-13 07:37:56.000000 healthcheck_pinger-0.0.5/HealthCheck_Pinger/decorator.py
--rw-rw-rw-   0        0        0     1088 2022-09-13 07:22:16.000000 healthcheck_pinger-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1407 2023-01-22 18:45:12.433315 healthcheck_pinger-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      764 2023-01-21 22:19:46.000000 healthcheck_pinger-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-22 18:45:12.428491 healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/
--rw-rw-rw-   0        0        0     1407 2023-01-22 18:45:12.000000 healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-01-22 18:45:12.000000 healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-22 18:45:12.000000 healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-01-22 18:45:12.000000 healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-01-22 18:44:23.000000 healthcheck_pinger-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-22 18:45:12.435198 healthcheck_pinger-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-01-22 18:44:42.000000 healthcheck_pinger-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:01:41.449353 HealthCheck_Pinger-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-26 16:01:41.433135 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/
+-rw-rw-rw-   0        0        0       58 2022-09-13 07:43:13.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/__init__.py
+-rw-rw-rw-   0        0        0     1113 2022-09-13 07:47:03.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/core.py
+-rw-rw-rw-   0        0        0      646 2023-07-26 15:58:00.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/decorator.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:01:41.444037 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/
+-rw-rw-rw-   0        0        0     1169 2023-07-26 16:01:41.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-07-26 16:01:41.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:01:41.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 16:01:41.000000 HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-09-13 07:22:16.000000 HealthCheck_Pinger-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1169 2023-07-26 16:01:41.448309 HealthCheck_Pinger-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-01-21 22:19:46.000000 HealthCheck_Pinger-0.0.6/README.md
+-rw-rw-rw-   0        0        0      625 2023-07-26 15:58:00.000000 HealthCheck_Pinger-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:01:41.449638 HealthCheck_Pinger-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-07-26 15:58:00.000000 HealthCheck_Pinger-0.0.6/setup.py
```

### Comparing `healthcheck_pinger-0.0.5/HealthCheck_Pinger/core.py` & `HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/core.py`

 * *Files identical despite different names*

### Comparing `healthcheck_pinger-0.0.5/HealthCheck_Pinger/decorator.py` & `HealthCheck_Pinger-0.0.6/HealthCheck_Pinger/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         @wraps(function)
         def wrapper(*args, **kwargs):
             if server:
                 ping =PingHC(uuid, server)
             else:
                 ping = PingHC(uuid)
             try:
-                function(*args, **kwargs)
+                result =function(*args, **kwargs)
             except:
                 ping.failure
-            else:
-                ping.success
+                return False
+            ping.success
+            return result
         return wrapper
-    return inner_function
+    return inner_function
```

### Comparing `healthcheck_pinger-0.0.5/LICENSE` & `HealthCheck_Pinger-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `healthcheck_pinger-0.0.5/PKG-INFO` & `HealthCheck_Pinger-0.0.6/HealthCheck_Pinger.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
-Name: healthcheck_pinger
-Version: 0.0.5
+Name: HealthCheck-Pinger
+Version: 0.0.6
 Summary: easily ping HealthCheck server
 Home-page: https://github.com/Gregorek85/HealthCheck_Pinger
 Author: Gregorek85
-Author-email: Gregorek85 <grerad@gmail.com>
+Author-email: grerad@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/Gregorek85/HealthCheck_Pinger
 Project-URL: Bug Tracker, https://github.com/Gregorek85/HealthCheck_Pinger/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HealthCheck_Pinger
 
 HealthCheck_Pinger is a small and simple Python package that contains class and decorator to easily ping HealthCheck (https://healthchecks.io/) server.
 
@@ -41,7 +37,8 @@
 from HealthCheck_Pinger import pingDecor
 @pingDecor("your uuid here") #or uuid and server url
 def your_function():
     your_code
 ```
 ## License
 [MIT](https://github.com/Gregorek85/HealthCheck_Pinger/blob/main/LICENSE)
+
```

### Comparing `healthcheck_pinger-0.0.5/README.md` & `HealthCheck_Pinger-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `healthcheck_pinger-0.0.5/healthcheck_pinger.egg-info/PKG-INFO` & `HealthCheck_Pinger-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
-Name: healthcheck-pinger
-Version: 0.0.5
+Name: HealthCheck_Pinger
+Version: 0.0.6
 Summary: easily ping HealthCheck server
 Home-page: https://github.com/Gregorek85/HealthCheck_Pinger
 Author: Gregorek85
-Author-email: Gregorek85 <grerad@gmail.com>
+Author-email: grerad@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/Gregorek85/HealthCheck_Pinger
 Project-URL: Bug Tracker, https://github.com/Gregorek85/HealthCheck_Pinger/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HealthCheck_Pinger
 
 HealthCheck_Pinger is a small and simple Python package that contains class and decorator to easily ping HealthCheck (https://healthchecks.io/) server.
 
@@ -41,7 +37,8 @@
 from HealthCheck_Pinger import pingDecor
 @pingDecor("your uuid here") #or uuid and server url
 def your_function():
     your_code
 ```
 ## License
 [MIT](https://github.com/Gregorek85/HealthCheck_Pinger/blob/main/LICENSE)
+
```

### Comparing `healthcheck_pinger-0.0.5/pyproject.toml` & `HealthCheck_Pinger-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "healthcheck_pinger"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Gregorek85", email = "grerad@gmail.com" }]
 description = "easily ping HealthCheck server"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `healthcheck_pinger-0.0.5/setup.py` & `HealthCheck_Pinger-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HealthCheck_Pinger",
-    version="0.0.5",
+    version="0.0.6",
     author="Gregorek85",
     author_email="grerad@gmail.com",
     description="easily ping HealthCheck server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gregorek85/HealthCheck_Pinger",
     project_urls={
```

