# Comparing `tmp/selenium_driverless-1.2.1.tar.gz` & `tmp/selenium_driverless-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.2.1.tar", last modified: Wed Jul 26 11:31:02 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.2.tar", last modified: Wed Jul 26 11:52:17 2023, max compression
```

## Comparing `selenium_driverless-1.2.1.tar` & `selenium_driverless-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.421173 selenium_driverless-1.2.1/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.1/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3823 2023-07-26 11:31:02.422304 selenium_driverless-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2.1/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.1/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-26 11:31:02.423327 selenium_driverless-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.368348 selenium_driverless-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.383256 selenium_driverless-1.2.1/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-26 11:28:48.000000 selenium_driverless-1.2.1/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.396752 selenium_driverless-1.2.1/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.1/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.406099 selenium_driverless-1.2.1/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.1/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.413942 selenium_driverless-1.2.1/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.1/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.418377 selenium_driverless-1.2.1/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.1/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.1/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    45635 2023-07-26 11:23:33.000000 selenium_driverless-1.2.1/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.394708 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 11:31:02.000000 selenium_driverless-1.2.1/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 11:31:02.420038 selenium_driverless-1.2.1/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.1/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.2/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3823 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2.2/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.2/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-26 11:52:17.822306 selenium_driverless-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.795854 selenium_driverless-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.803913 selenium_driverless-1.2.2/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-07-26 11:52:13.000000 selenium_driverless-1.2.2/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.809236 selenium_driverless-1.2.2/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.2/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.812238 selenium_driverless-1.2.2/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.816291 selenium_driverless-1.2.2/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1351 2023-07-26 11:21:31.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.818272 selenium_driverless-1.2.2/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.820306 selenium_driverless-1.2.2/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.2/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.2/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    45635 2023-07-26 11:23:33.000000 selenium_driverless-1.2.2/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.809236 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1079 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.2/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2.1/LICENSE.md` & `selenium_driverless-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/PKG-INFO` & `selenium_driverless-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.2.1
+Version: 1.2.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2.1/README.md` & `selenium_driverless-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/build_upload.md` & `selenium_driverless-1.2.2/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/setup.py` & `selenium_driverless-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2.2/src/selenium_driverless/scripts/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2.2/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2.2/src/selenium_driverless/scripts/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.2.2/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/types/by.py` & `selenium_driverless-1.2.2/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.2.2/src/selenium_driverless/types/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2.2/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2.2/src/selenium_driverless/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2.2/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.2.1
+Version: 1.2.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2.1/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.2.2/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,13 +13,19 @@
 src/selenium_driverless.egg-info/requires.txt
 src/selenium_driverless.egg-info/top_level.txt
 src/selenium_driverless/files/__init__.py
 src/selenium_driverless/scripts/__init__.py
 src/selenium_driverless/scripts/alert.py
 src/selenium_driverless/scripts/options.py
 src/selenium_driverless/scripts/switch_to.py
+src/selenium_driverless/sync/__init__.py
+src/selenium_driverless/sync/alert.py
+src/selenium_driverless/sync/executor.py
+src/selenium_driverless/sync/switch_to.py
+src/selenium_driverless/sync/webdriver.py
+src/selenium_driverless/sync/webelement.py
 src/selenium_driverless/types/__init__.py
 src/selenium_driverless/types/by.py
 src/selenium_driverless/types/webelement.py
 src/selenium_driverless/utils/__init__.py
 src/selenium_driverless/utils/utils.py
 tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2.1/tests/test_driverless.py` & `selenium_driverless-1.2.2/tests/test_driverless.py`

 * *Files identical despite different names*

