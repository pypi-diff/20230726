# Comparing `tmp/selenium_profiles-2.2.7.4.tar.gz` & `tmp/selenium_profiles-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_profiles-2.2.7.4.tar", last modified: Mon Jul 17 11:12:08 2023, max compression
+gzip compressed data, was "dist\selenium_profiles-2.2.8.tar", last modified: Wed Jul 26 12:38:01 2023, max compression
```

## Comparing `selenium_profiles-2.2.7.4.tar` & `selenium_profiles-2.2.8.tar`

### file list

```diff
@@ -1,61 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.4/LICENSE.md
--rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.4/MANIFEST.in
--rw-rw-rw-   0        0        0    14332 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/PKG-INFO
--rw-rw-rw-   0        0        0    12984 2023-07-16 17:28:04.000000 selenium_profiles-2.2.7.4/README.md
--rw-rw-rw-   0        0        0     1740 2023-07-03 16:17:23.000000 selenium_profiles-2.2.7.4/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.4/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/setup.cfg
--rw-rw-rw-   0        0        0     2083 2023-07-14 14:01:27.000000 selenium_profiles-2.2.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/
--rw-rw-rw-   0        0        0       25 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/export_profile.js
--rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/fetch.js
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/__init.py
--rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/
--rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/
--rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
--rw-rw-rw-   0        0        0     2997 2023-07-16 17:33:38.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/default.json
--rw-rw-rw-   0        0        0     1816 2023-07-16 17:28:04.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/example.json
--rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/__init__.py
--rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    24206 2023-07-17 11:06:31.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/profiles.py
--rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/proxy.py
--rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/
--rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/colab_utils.py
--rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/utils/utils.py
--rw-rw-rw-   0        0        0    10234 2023-07-14 13:57:17.000000 selenium_profiles-2.2.7.4/src/selenium_profiles/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/
--rw-rw-rw-   0        0        0    14332 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-17 11:12:07.000000 selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 11:12:08.000000 selenium_profiles-2.2.7.4/tests/
--rw-rw-rw-   0        0        0     1617 2023-06-27 16:34:45.000000 selenium_profiles-2.2.7.4/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.8/LICENSE.md
+-rw-rw-rw-   0        0        0      157 2023-07-19 10:05:57.000000 selenium_profiles-2.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    15324 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    13978 2023-07-26 12:36:09.000000 selenium_profiles-2.2.8/README.md
+-rw-rw-rw-   0        0        0     1740 2023-07-22 14:23:01.000000 selenium_profiles-2.2.8/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2281 2023-07-26 11:53:16.000000 selenium_profiles-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/
+-rw-rw-rw-   0        0        0       23 2023-07-26 11:38:14.000000 selenium_profiles-2.2.8/src/selenium_profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/files/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.8/src/selenium_profiles/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.8/src/selenium_profiles/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/undetected/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/undetected/__init.py
+-rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.8/src/selenium_profiles/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/
+-rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/
+-rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2997 2023-07-16 17:33:38.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/default.json
+-rw-rw-rw-   0        0        0     1816 2023-07-16 17:28:04.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/example.json
+-rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.8/src/selenium_profiles/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24221 2023-07-26 10:52:41.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/profiles.py
+-rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/proxy.py
+-rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.8/src/selenium_profiles/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.8/src/selenium_profiles/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.8/src/selenium_profiles/utils/colab_utils.py
+-rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.8/src/selenium_profiles/utils/utils.py
+-rw-rw-rw-   0        0        0    10814 2023-07-26 11:06:44.000000 selenium_profiles-2.2.8/src/selenium_profiles/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/
+-rw-rw-rw-   0        0        0    15324 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1629 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/src/selenium_profiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 12:38:01.000000 selenium_profiles-2.2.8/tests/
+-rw-rw-rw-   0        0        0     1623 2023-07-26 12:36:08.000000 selenium_profiles-2.2.8/tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.7.4/LICENSE.md` & `selenium_profiles-2.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/PKG-INFO` & `selenium_profiles-2.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_profiles
-Version: 2.2.7.4
+Version: 2.2.8
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -30,17 +30,17 @@
 
 # Selenium-Profiles
 
 [![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
 
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
-* **Undetected** by Google, Cloudflare, creep-js ..
+* **Undetected** by Google, Cloudflare, creep-js using [selenium-driverless](# with selenium-driverless)
 * [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
-* [Touch Actions](#Touch_actions)
+* [Touch Actions](# Touch_actions)
 * dynamic proxies with authentication
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.profiles.fetch(url)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
 * apply profile on already running driver with `driver.profiles.apply(profiles.Android())`
 * use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
@@ -144,14 +144,38 @@
 "proxy":{
   "proxy":"socks5://user1:pass@example_jost.com:5001", 
   "bypass_list":["localhost"]
   }
 }
 ```
 
+### with selenium-driverless
+warning: 
+- this package is experimental and might include bugs, please report them at [bug-reports](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues)
+- only for python >=3.8
+- you'll need to install __pycdp__ first with `* `pip install git+https://github.com/HMaker/python-cdp.git@latest``
+```python
+from selenium_profiles.webdriver import Chrome
+from selenium_profiles.profiles import profiles
+from selenium_driverless.webdriver import ChromeOptions
+from selenium_driverless.types.by import By
+
+profile = profiles.Windows()  # or .Android
+options = ChromeOptions()
+# options.add_argument("--headless=new")
+driver = Chrome(profile, options=options, driverless_options=True)
+
+# get url
+driver.get('https://nowsecure.nl#relax')  # test fingerprint
+
+driver.quit()  # Execute on the End!
+```
+see [documentation](https://github.com/kaliiiiiiiiii/Selenium-Driverless) for usages
+
+
 ### Modify-headers
 
 using selenium-wire
 ```python
 from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
```

### Comparing `selenium_profiles-2.2.7.4/README.md` & `selenium_profiles-2.2.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Selenium-Profiles
 
 [![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
 
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
-* **Undetected** by Google, Cloudflare, creep-js ..
+* **Undetected** by Google, Cloudflare, creep-js using [selenium-driverless](# with selenium-driverless)
 * [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
-* [Touch Actions](#Touch_actions)
+* [Touch Actions](# Touch_actions)
 * dynamic proxies with authentication
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.profiles.fetch(url)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
 * apply profile on already running driver with `driver.profiles.apply(profiles.Android())`
 * use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
@@ -114,14 +114,38 @@
 "proxy":{
   "proxy":"socks5://user1:pass@example_jost.com:5001", 
   "bypass_list":["localhost"]
   }
 }
 ```
 
+### with selenium-driverless
+warning: 
+- this package is experimental and might include bugs, please report them at [bug-reports](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues)
+- only for python >=3.8
+- you'll need to install __pycdp__ first with `* `pip install git+https://github.com/HMaker/python-cdp.git@latest``
+```python
+from selenium_profiles.webdriver import Chrome
+from selenium_profiles.profiles import profiles
+from selenium_driverless.webdriver import ChromeOptions
+from selenium_driverless.types.by import By
+
+profile = profiles.Windows()  # or .Android
+options = ChromeOptions()
+# options.add_argument("--headless=new")
+driver = Chrome(profile, options=options, driverless_options=True)
+
+# get url
+driver.get('https://nowsecure.nl#relax')  # test fingerprint
+
+driver.quit()  # Execute on the End!
+```
+see [documentation](https://github.com/kaliiiiiiiiii/Selenium-Driverless) for usages
+
+
 ### Modify-headers
 
 using selenium-wire
 ```python
 from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
```

### Comparing `selenium_profiles-2.2.7.4/build_upload.md` & `selenium_profiles-2.2.8/build_upload.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 # 3.11
 C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install C:\Users\aurin\PycharmProjects\selenium_profiles
 ```
 
 ## install all python versions from pypi
 ```shell
 # 3.7
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles==2.2.7.2
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles==2.2.7.4
 # 3.8
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.4
 # 3.9
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles==2.2.7.2
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles==2.2.7.4
 # 3.10
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.4
 # 3.11
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.4
 ```
 
 ## install from GitHub
 ```shell
 pip install https://github.com/kaliiiiiiiiii/Selenium-Profiles/archive/refs/heads/master.zip
 ```
```

### Comparing `selenium_profiles-2.2.7.4/setup.py` & `selenium_profiles-2.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import setuptools
 import sys
 
 
-requirements = ['selenium', 'requests', 'selenium-interceptor', "undetected-chromedriver", "selenium-wire", "webdriver-manager", "selenium-injector>=2.3"]
+requirements = ['selenium', 'requests', 'selenium-interceptor',
+                "undetected-chromedriver", "selenium-wire", "webdriver-manager",
+                "selenium-injector>=2.3"]
+
+py_version = sys.version_info
+if py_version.major >= 3 and py_version.minor >= 8:
+    # requires python >= 3.8
+    requirements.append("selenium-driverless>=1.2.2")
 
 if 'google.colab' in sys.modules: # we're on google-colab
     requirements.extend(['PyVirtualDisplay', "google-colab-shell"])
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
```

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/js/export_profile.js` & `selenium_profiles-2.2.8/src/selenium_profiles/js/export_profile.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/js/fetch.js` & `selenium_profiles-2.2.8/src/selenium_profiles/js/fetch.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/default.json` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/default.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/example.json` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/example.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/profiles.py` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/profiles/scratch.json` & `selenium_profiles-2.2.8/src/selenium_profiles/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/driver_utils.py` & `selenium_profiles-2.2.8/src/selenium_profiles/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/profiles.py` & `selenium_profiles-2.2.8/src/selenium_profiles/scripts/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
         :param duplicate_policy: for args | "raise" or "replace" or "warn-replace" or "skip" or "warn-skip" or "add" or "warn-add"
         exact duplicates always get removed with a warning
         """
         if not options_profile:
             options_profile = {}
         self.profile = defaultdict(lambda: None)
         self.profile.update(options_profile)
+        self._extensions = []
 
         self.duplicate_policy = duplicate_policy
         self.duplicates = defaultdict(lambda: set())
         if not safe_duplicates:
             safe_duplicates = []
         self.safe_duplicates = safe_duplicates
 
@@ -523,10 +524,10 @@
                 file_type = extension_path[-4:]
                 if os.path.exists(extension_path):
                     if os.path.isfile(extension_path):
                         if not (file_type == ".crx" or file_type == ".zip"):
                             warnings.warn("Extension-file isn't *.zip or *.crx")
                         self.Options.add_extension(extension_path)
                     elif os.path.isdir(extension_path):
-                        self.add_argument('--load-extension=' + extension_path)
+                        self._extensions.append(extension_path)
                 else:
                     raise LookupError("Extension-path doesn't exist")
```

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/proxy.py` & `selenium_profiles-2.2.8/src/selenium_profiles/scripts/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/scripts/undetected.py` & `selenium_profiles-2.2.8/src/selenium_profiles/scripts/undetected.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/utils/colab_utils.py` & `selenium_profiles-2.2.8/src/selenium_profiles/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/utils/utils.py` & `selenium_profiles-2.2.8/src/selenium_profiles/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles/webdriver.py` & `selenium_profiles-2.2.8/src/selenium_profiles/webdriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from selenium_profiles.scripts.profiles import options as options_handler
 
 from selenium.webdriver import Chrome as BaseDriver
 class Chrome(BaseDriver):
 
     # noinspection PyDefaultArgument
     def __init__(self, profile: dict = None, chrome_binary: str = None, executable_path: str = None,
-                 options=None, duplicate_policy: str = "warn-add", safe_duplicates: list = ["--add-extension"],
+                 options=None, duplicate_policy: str = "warn-add", safe_duplicates: list = list(),
                  base_drivers:tuple=None,
-                 uc_driver: bool or None = None, seleniumwire_options: dict or bool or None = None, injector_options:dict or bool or None = None,
+                 uc_driver: bool or None = None, seleniumwire_options: dict or bool or None = None,
+                 injector_options:dict or bool or None = None, driverless_options = None,
                  **kwargs):
 
         import seleniumwire.undetected_chromedriver as wire_uc_webdriver
         import undetected_chromedriver as uc_webdriver
         from seleniumwire import webdriver as wire_webdriver
 
         from selenium_profiles.utils.utils import valid_key
@@ -43,14 +44,22 @@
         if not options:
             if webdriver:
                 options = webdriver.ChromeOptions()
             else:
                 from selenium.webdriver import ChromeOptions
                 options = ChromeOptions()
 
+        if driverless_options:
+            try:
+                # noinspection PyUnresolvedReferences
+                from selenium_driverless.sync.webdriver import Chrome as DriverlessChrome
+            except:
+                raise RuntimeError("selenium-driverless requires Python>=3.8")
+            base_drivers = base_drivers + (DriverlessChrome,)
+
         if len(base_drivers) > 1:
             warnings.warn("More than one base_driver might not initialize correctly, seems buggy.\n Also, you might try different order")
         if (len(base_drivers) == 1) and (base_drivers[0] == Chrome.__base__):
             pass # got selenium.webdriver.Chrome as BaseDriver
         elif not base_drivers:
             pass
         else :
@@ -101,14 +110,16 @@
         # chrome executable path
         if not chrome_binary:
             options_manager.Options.binary_location = chrome_binary
 
         if (uc_webdriver.Chrome in base_drivers) or (wire_uc_webdriver.Chrome in base_drivers):
             if executable_path:
                 kwargs.update({"driver_executable_path": executable_path})
+        elif driverless_options:
+            pass
         else:
             # detectability options
             from selenium_profiles.scripts import undetected
 
             # is adb used ?
             try:
                 # noinspection PyUnresolvedReferences
@@ -126,18 +137,20 @@
 
         injector = None
         if injector_options:
             from selenium_injector.scripts.injector import Injector
             if (injector_options is True) or injector_options == {}:
                 injector_options = {}
             injector = Injector(**injector_options)
+            options_manager.add_extensions(injector.paths)
 
-            options_manager.add_argument(f'--load-extension={",".join(injector.paths)}')
 
         # add options to kwargs
+        # noinspection PyProtectedMember,PyUnresolvedReferences
+        options_manager.add_argument(f'--load-extension={",".join(options_manager._extensions)}')
         kwargs.update({"options": options_manager.Options})
 
         # Actual start of chrome
         super().__init__(**kwargs)
         # cdp tools
 
         self.get("chrome://version/")  # wait browser to start
```

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/PKG-INFO` & `selenium_profiles-2.2.8/src/selenium_profiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-profiles
-Version: 2.2.7.4
+Version: 2.2.8
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -30,17 +30,17 @@
 
 # Selenium-Profiles
 
 [![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
 
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
-* **Undetected** by Google, Cloudflare, creep-js ..
+* **Undetected** by Google, Cloudflare, creep-js using [selenium-driverless](# with selenium-driverless)
 * [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
-* [Touch Actions](#Touch_actions)
+* [Touch Actions](# Touch_actions)
 * dynamic proxies with authentication
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.profiles.fetch(url)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
 * apply profile on already running driver with `driver.profiles.apply(profiles.Android())`
 * use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
@@ -144,14 +144,38 @@
 "proxy":{
   "proxy":"socks5://user1:pass@example_jost.com:5001", 
   "bypass_list":["localhost"]
   }
 }
 ```
 
+### with selenium-driverless
+warning: 
+- this package is experimental and might include bugs, please report them at [bug-reports](https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues)
+- only for python >=3.8
+- you'll need to install __pycdp__ first with `* `pip install git+https://github.com/HMaker/python-cdp.git@latest``
+```python
+from selenium_profiles.webdriver import Chrome
+from selenium_profiles.profiles import profiles
+from selenium_driverless.webdriver import ChromeOptions
+from selenium_driverless.types.by import By
+
+profile = profiles.Windows()  # or .Android
+options = ChromeOptions()
+# options.add_argument("--headless=new")
+driver = Chrome(profile, options=options, driverless_options=True)
+
+# get url
+driver.get('https://nowsecure.nl#relax')  # test fingerprint
+
+driver.quit()  # Execute on the End!
+```
+see [documentation](https://github.com/kaliiiiiiiiii/Selenium-Driverless) for usages
+
+
 ### Modify-headers
 
 using selenium-wire
 ```python
 from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
```

### Comparing `selenium_profiles-2.2.7.4/src/selenium_profiles.egg-info/SOURCES.txt` & `selenium_profiles-2.2.8/src/selenium_profiles.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 src/selenium_profiles/webdriver.py
 src/selenium_profiles.egg-info/PKG-INFO
 src/selenium_profiles.egg-info/SOURCES.txt
 src/selenium_profiles.egg-info/dependency_links.txt
 src/selenium_profiles.egg-info/requires.txt
 src/selenium_profiles.egg-info/top_level.txt
 src/selenium_profiles/files/__init__.py
-src/selenium_profiles/files/proxy_extension/background.js
-src/selenium_profiles/files/proxy_extension/manifest.json
 src/selenium_profiles/files/tmp/__init__.py
-src/selenium_profiles/files/tmp/proxy_extension/background.js
-src/selenium_profiles/files/tmp/proxy_extension/manifest.json
 src/selenium_profiles/js/__init__.py
 src/selenium_profiles/js/export_profile.js
 src/selenium_profiles/js/fetch.js
 src/selenium_profiles/js/undetected/__init.py
 src/selenium_profiles/js/undetected/get_cdc_props.js
 src/selenium_profiles/js/undetected/navigator_webdriver.js
 src/selenium_profiles/js/undetected/remove_cdc_props.js
```

### Comparing `selenium_profiles-2.2.7.4/tests/test_driver.py` & `selenium_profiles-2.2.8/tests/test_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 def test_driver(choose: str, headless: bool = True, uc_driver=False):
     profile = read_json(filename='profiles\\default.json')
     testprofile = profile[choose]
     testprofile["cdp"]["patch_version"] = None # don't change version :)
     testprofile["options"]["headless"] = headless
     driver = Chrome(profile=testprofile, uc_driver=uc_driver)
     driver.get('https://browserleaks.com/client-hints')
-    useragent = driver.find_element(By.XPATH, '//*[@id="content"]/table[1]/tbody/tr/td[2]').accessible_name
+    elem = driver.find_element(By.XPATH, '//*[@id="content"]/table[1]/tbody/tr/td[2]')
+    useragent = elem.text
     exported_profile = driver.profiles.get_profile()
     driver.quit()
 
     print(choose+'\n'+useragent+'\n')
     return {"profile": driver.profiles._profile, "exported_profile": exported_profile, "useragent":useragent}
```

