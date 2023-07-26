# Comparing `tmp/percy-appium-app-2.0.0b0.tar.gz` & `tmp/percy-appium-app-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-2.0.0b0.tar", last modified: Fri Jul 14 15:32:33 2023, max compression
+gzip compressed data, was "percy-appium-app-2.0.0b1.tar", last modified: Wed Jul 26 10:51:58 2023, max compression
```

## Comparing `percy-appium-app-2.0.0b0.tar` & `percy-appium-app-2.0.0b1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.246371 percy-appium-app-2.0.0b0/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/configs/devices.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/percy_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.535960 percy-appium-app-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-26 10:51:58.535960 percy-appium-app-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.523960 percy-appium-app-2.0.0b1/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.523960 percy-appium-app-2.0.0b1/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.523960 percy-appium-app-2.0.0b1/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/configs/devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.523960 percy-appium-app-2.0.0b1/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.523960 percy-appium-app-2.0.0b1/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/percy_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.527960 percy-appium-app-2.0.0b1/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.527960 percy-appium-app-2.0.0b1/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.531960 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 10:51:58.000000 percy-appium-app-2.0.0b1/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:51:58.535960 percy-appium-app-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:51:58.535960 percy-appium-app-2.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-26 10:51:32.000000 percy-appium-app-2.0.0b1/tests/test_tile.py
```

### Comparing `percy-appium-app-2.0.0b0/LICENSE` & `percy-appium-app-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/PKG-INFO` & `percy-appium-app-2.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `percy-appium-app-2.0.0b0/README.md` & `percy-appium-app-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/__init__.py` & `percy-appium-app-2.0.0b1/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/configs/devices.json` & `percy-appium-app-2.0.0b1/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/lib/app_percy.py` & `percy-appium-app-2.0.0b1/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/lib/cache.py` & `percy-appium-app-2.0.0b1/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/lib/cli_wrapper.py` & `percy-appium-app-2.0.0b1/percy/lib/cli_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
             return True
         except Exception as e:
             log('Percy is not running, disabling screenshots')
             log(e, on_debug=True)
             return False
 
-    def post_screenshots(self, name, tag, tiles, external_debug_url=None, ignored_elements_data=None):
-        body = self._request_body(name, tag, tiles, external_debug_url, ignored_elements_data)
+    def post_screenshots(self, name, tag, tiles, external_debug_url=None, ignored_elements_data=None, considered_elements_data=None):
+        body = self._request_body(name, tag, tiles, external_debug_url, ignored_elements_data, considered_elements_data)
 
         body['client_info'] = Environment._get_client_info()
         body['environment_info'] = Environment._get_env_info()
 
         response = requests.post(f'{PERCY_CLI_API}/percy/comparison', json=body, timeout=30)
         # Handle errors
         response.raise_for_status()
@@ -72,10 +72,17 @@
         data = response.json()
 
         if response.status_code != 200:
             raise CLIException(data.get('error', 'UnknownException'))
         return data
 
     @staticmethod
-    def _request_body(name, tag, tiles, external_debug_url, ignored_elements_data):
+    def _request_body(name, tag, tiles, external_debug_url, ignored_elements_data, considered_elements_data):
         tiles = list(map(dict, tiles))
-        return {"name": name, "tag": tag, "tiles": tiles, "ignored_elements_data": ignored_elements_data, "external_debug_url": external_debug_url}
+        return {
+            "name": name,
+            "tag": tag,
+            "tiles": tiles,
+            "ignored_elements_data": ignored_elements_data,
+            "external_debug_url": external_debug_url,
+            "considered_elements_data": considered_elements_data 
+        }
```

### Comparing `percy-appium-app-2.0.0b0/percy/lib/ignore_region.py` & `percy-appium-app-2.0.0b1/percy/lib/region.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class IgnoreRegion:
+class Region:
     def __init__(self, top, bottom, left, right):
         if top < 0 or bottom < 0 or left < 0 or right < 0:
             raise ValueError('Only Positive integer is allowed!')
 
         if top >= bottom or left >= right:
             raise ValueError('Invalid ignore region parameters!')
```

### Comparing `percy-appium-app-2.0.0b0/percy/lib/percy_options.py` & `percy-appium-app-2.0.0b1/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/lib/tile.py` & `percy-appium-app-2.0.0b1/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/metadata/android_metadata.py` & `percy-appium-app-2.0.0b1/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/metadata/ios_metadata.py` & `percy-appium-app-2.0.0b1/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/metadata/metadata.py` & `percy-appium-app-2.0.0b1/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/providers/app_automate.py` & `percy-appium-app-2.0.0b1/percy/providers/app_automate.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,25 +32,29 @@
     def set_debug_url(self, session_details):
         build_hash = str(session_details.get("buildHash"))
         session_hash = str(session_details.get("sessionHash"))
         self.debug_url = "https://app-automate.browserstack.com/dashboard/v2/builds/" + build_hash + "/sessions/" + session_hash
 
     def _get_tiles(self, **kwargs):
         fullpage_ss = kwargs.get('fullpage', False)
-        if not fullpage_ss:
+        if os.environ.get('PERCY_DISABLE_REMOTE_UPLOADS') == 'true':
+            if fullpage_ss:
+                log('Full page screenshots are only supported when "PERCY_DISABLE_REMOTE_UPLOADS" is not set')
             return super()._get_tiles(**kwargs)
+        screenshotType = 'fullpage' if fullpage_ss else 'singlepage'
         screen_lengths = kwargs.get('screen_lengths', 4)
         scrollable_xpath = kwargs.get('scollable_xpath')
         scrollable_id = kwargs.get('scrollable_id')
         data = self.execute_percy_screenshot(
             self.metadata.device_screen_size.get('height', 1),
+            screenshotType,
             screen_lengths,
             scrollable_xpath,
             scrollable_id,
-            self.metadata.scale_factor,
+            self.metadata.scale_factor
         )
         tiles = []
         status_bar_height = self.metadata.status_bar_height
         nav_bar_height = self.metadata.navigation_bar_height
         for tile_data in json.loads(data.get('result')):
             tiles.append(Tile(
                 status_bar_height,
@@ -95,28 +99,39 @@
             if status_message: request_body['arguments']['statusMessage'] = status_message
             command = f'browserstack_executor: {json.dumps(request_body)}'
             self.metadata.execute_script(command)
         except Exception as e:
             log('Error occurred during end call', on_debug=True)
             log(e, on_debug=True)
 
-    def execute_percy_screenshot(self, device_height, screen_lengths, scrollable_xpath=None, scrollable_id=None, scale_factor=1):
+    def execute_percy_screenshot(
+        self,
+        device_height,
+        screenshotType,
+        screen_lengths,
+        scrollable_xpath=None,
+        scrollable_id=None,
+        scale_factor=1
+    ):
         try:
+            projectId = 'percy-dev' if os.environ.get('PERCY_ENABLE_DEV') == 'true' else 'percy-prod'
             request_body = {
                 'action': 'percyScreenshot',
                 'arguments': {
                     'state': 'screenshot',
                     'percyBuildId':  Environment.percy_build_id,
-                    'screenshotType': 'fullpage',
+                    'screenshotType': screenshotType,
+                    'projectId': projectId,
                     'scaleFactor': scale_factor,
                     'options': { 
                         "numOfTiles": screen_lengths,
                         "deviceHeight": device_height,
                         "scrollableXpath":  scrollable_xpath,
-                        "scrollableId": scrollable_id
+                        "scrollableId": scrollable_id,
+                        "FORCE_FULL_PAGE": os.environ.get('FORCE_FULL_PAGE') == 'true'
                     },
                 }
             }
             command = f'browserstack_executor: {json.dumps(request_body)}'
             response = self.metadata.execute_script(command)
             response = json.loads(response)
             return response
```

### Comparing `percy-appium-app-2.0.0b0/percy/providers/generic_provider.py` & `percy-appium-app-2.0.0b1/percy/providers/generic_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,32 @@
     @staticmethod
     def supports(_remote_url):
         return True
 
     def screenshot(self, name, **kwargs):
         tiles = self._get_tiles(**kwargs)
         tag = self._get_tag(**kwargs)
-        ignore_regions = self._find_ignored_regions(**kwargs)
+        ignore_regions = {
+            'ignoreElementsData': self._find_regions(
+                xpaths = kwargs.get("ignore_regions_xpaths", []),
+                accessibility_ids = kwargs.get("ignore_region_accessibility_ids", []),
+                appium_elements = kwargs.get("ignore_region_appium_elements", []),
+                custom_locations = kwargs.get("custom_ignore_regions", [])
+            )
+        }
+        consider_regions = {
+            'considerElementsData': self._find_regions(
+                xpaths = kwargs.get("consider_regions_xpaths", []),
+                accessibility_ids = kwargs.get("consider_region_accessibility_ids", []),
+                appium_elements = kwargs.get("consider_region_appium_elements", []),
+                custom_locations = kwargs.get("custom_consider_regions", [])
+            )
+        }
 
-        return self._post_screenshots(name, tag, tiles, self.get_debug_url(), ignore_regions)
+        return self._post_screenshots(name, tag, tiles, self.get_debug_url(), ignore_regions, consider_regions)
 
     def _get_tag(self, **kwargs):
         name = kwargs.get('device_name', self.metadata.device_name)
         os_name = self.metadata.os_name
         os_version = self.metadata.os_version
         width = self.metadata.device_screen_size.get('width', 1)
         height = self.metadata.device_screen_size.get('height', 1)
@@ -60,29 +75,23 @@
         nav_bar_height = kwargs.get('nav_bar_height') or self.metadata.navigation_bar_height
         header_height = 0
         footer_height = 0
         return [
             Tile(status_bar_height, nav_bar_height, header_height, footer_height, filepath=path, fullscreen=fullscreen)
         ]
 
-    def _find_ignored_regions(self, **kwargs):
-        ignored_elements_array = []
-        ignore_region_xpaths = kwargs.get("ignore_regions_xpaths", [])
-        ignore_region_accessibility_ids = kwargs.get("ignore_region_accessibility_ids", [])
-        ignore_region_appium_elements = kwargs.get("ignore_region_appium_elements", [])
-        custom_ignore_regions = kwargs.get("custom_ignore_regions", [])
-        self.ignore_regions_by_xpaths(ignored_elements_array, ignore_region_xpaths)
-        self.ignore_regions_by_ids(ignored_elements_array, ignore_region_accessibility_ids)
-        self.ignore_regions_by_elements(ignored_elements_array, ignore_region_appium_elements)
-        self.add_custom_ignore_regions(ignored_elements_array, custom_ignore_regions)
-        return {
-            "ignoreElementsData": ignored_elements_array
-        }
+    def _find_regions(self, xpaths, accessibility_ids, appium_elements, custom_locations):
+        elementsArray = []
+        self.get_regions_by_xpath(elementsArray, xpaths)
+        self.get_regions_by_ids(elementsArray, accessibility_ids)
+        self.get_regions_by_elements(elementsArray, appium_elements)
+        self.get_regions_by_location(elementsArray, custom_locations)
+        return elementsArray
 
-    def ignore_element_object(self, selector, element):
+    def get_region_object(self, selector, element):
         scale_factor = self.metadata.scale_factor
         location = element.location
         size = element.size
         co_ordinates = {
             "top": location["y"] * scale_factor,
             "bottom": (location["y"] + size["height"]) * scale_factor,
             "left": location["x"] * scale_factor,
@@ -91,68 +100,68 @@
         ignore_region = {
             "selector": selector,
             "coOrdinates": co_ordinates
         }
 
         return ignore_region
 
-    def ignore_regions_by_xpaths(self, ignored_elements_array, xpaths):
+    def get_regions_by_xpath(self, elements_array, xpaths):
         for xpath in xpaths:
             try:
                 element = self.driver.find_element(by=AppiumBy.XPATH, value=xpath)
                 selector = f"xpath: {xpath}"
-                ignored_region = self.ignore_element_object(selector, element)
-                ignored_elements_array.append(ignored_region)
+                region = self.get_region_object(selector, element)
+                elements_array.append(region)
             except NoSuchElementException as e:
                 log(f"Appium Element with xpath: {xpath} not found. Ignoring this xpath.")
                 log(e, on_debug=True)
 
-    def ignore_regions_by_ids(self, ignored_elements_array, ids):
+    def get_regions_by_ids(self, elements_array, ids):
         for id in ids:
             try:
                 element = self.driver.find_element(by=AppiumBy.ACCESSIBILITY_ID, value=id)
                 selector = f"id: {id}"
-                ignored_region = self.ignore_element_object(selector, element)
-                ignored_elements_array.append(ignored_region)
+                region = self.get_region_object(selector, element)
+                elements_array.append(region)
             except NoSuchElementException as e:
                 log(f"Appium Element with id: {id} not found. Ignoring this id.")
                 log(e, on_debug=True)
 
-    def ignore_regions_by_elements(self, ignored_elements_array, elements):
+    def get_regions_by_elements(self, elements_array, elements):
         for idx, element in enumerate(elements):
             try:
                 class_name = element.get_attribute('class')
                 selector = f"element: {idx} {class_name}"
-                ignored_region = self.ignore_element_object(selector, element)
-                ignored_elements_array.append(ignored_region)
+                region = self.get_region_object(selector, element)
+                elements_array.append(region)
             except NoSuchElementException as e:
                 log(f"Correct Element not passed at index {idx}")
                 log(e, on_debug=True)
 
-    def add_custom_ignore_regions(self, ignored_elements_array, custom_locations):
+    def get_regions_by_location(self, elements_array, custom_locations):
         for idx, custom_location in enumerate(custom_locations):
             screen_width = self.metadata.device_screen_size['width']
             screen_height = self.metadata.device_screen_size['height']
             if custom_location.is_valid(screen_height, screen_width):
-                ignored_region = {
+                region = {
                     "selector": f"custom ignore region: {idx}",
                     "coOrdinates": {
                         "top": custom_location.top,
                         "bottom": custom_location.bottom,
                         "left": custom_location.left,
                         "right": custom_location.right
                     }
                 }
-                ignored_elements_array.append(ignored_region)
+                elements_array.append(region)
             else:
                 log(f"Values passed in custom ignored region at index: {idx} is not valid")
 
     @staticmethod
-    def _post_screenshots(name, tag, tiles, debug_url, ignored_regions):
-        response = CLIWrapper().post_screenshots(name, tag, tiles, debug_url, ignored_regions)
+    def _post_screenshots(name, tag, tiles, debug_url, ignored_regions, considered_regions):
+        response = CLIWrapper().post_screenshots(name, tag, tiles, debug_url, ignored_regions, considered_regions)
         return response
 
     def _write_screenshot(self, png_bytes, directory):
         filepath = self._get_path(directory)
         with open(filepath, 'wb') as f:
             f.write(png_bytes)
         return filepath
```

### Comparing `percy-appium-app-2.0.0b0/percy/providers/provider_resolver.py` & `percy-appium-app-2.0.0b1/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy/screenshot.py` & `percy-appium-app-2.0.0b1/percy/screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-2.0.0b1/percy_appium_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `percy-appium-app-2.0.0b0/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-2.0.0b1/percy_appium_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 percy/lib/__init__.py
 percy/lib/app_percy.py
 percy/lib/cache.py
 percy/lib/cli_wrapper.py
 percy/lib/ignore_region.py
 percy/lib/percy_automate.py
 percy/lib/percy_options.py
+percy/lib/region.py
 percy/lib/tile.py
 percy/metadata/__init__.py
 percy/metadata/android_metadata.py
 percy/metadata/ios_metadata.py
 percy/metadata/metadata.py
 percy/metadata/metadata_resolver.py
 percy/providers/__init__.py
```

### Comparing `percy-appium-app-2.0.0b0/setup.py` & `percy-appium-app-2.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_android_metadata.py` & `percy-appium-app-2.0.0b1/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_app_automate.py` & `percy-appium-app-2.0.0b1/tests/test_app_automate.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def test_app_automate_execute_percy_screenshot_end(self):
         self.mock_webdriver.execute_script.return_value = {}
         self.assertIsNone(self.app_automate.execute_percy_screenshot_end('Screenshot 1', self.comparison_response['link'], 'success'))
         self.mock_webdriver.execute_script.assert_called()
 
     def test_app_automate_execute_percy_screenshot(self):
         self.mock_webdriver.execute_script.return_value = '{"result": "result"}'
-        self.app_automate.execute_percy_screenshot(1080, 5)
+        self.app_automate.execute_percy_screenshot(1080, 'singlepage', 5)
         self.mock_webdriver.execute_script.assert_called()
 
     @patch('percy.providers.app_automate.log')
     def test_execute_percy_screenshot_end_throws_error(self, mock_log):
         self.mock_webdriver.execute_script.side_effect = Exception('SomeException')
         self.app_automate.execute_percy_screenshot_end('Screenshot 1', 'snapshot-url', 'success')
         mock_log.assert_called()
```

### Comparing `percy-appium-app-2.0.0b0/tests/test_app_percy.py` & `percy-appium-app-2.0.0b1/tests/test_app_percy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint: disable=[arguments-differ, protected-access]
 import copy
 import unittest
+import os
 from unittest.mock import patch, Mock, MagicMock, PropertyMock
 
 from appium.webdriver.webdriver import WebDriver
 from percy.errors import DriverNotSupported, UnknownProvider
 
 from percy import percy_screenshot
 from percy.lib.app_percy import AppPercy
 from percy.lib.cli_wrapper import CLIWrapper
 from percy.metadata import IOSMetadata, Metadata
 from percy.providers.app_automate import AppAutomate
 from percy.providers.generic_provider import GenericProvider
 from percy.metadata import AndroidMetadata
 from tests.mocks.mock_methods import android_capabilities, ios_capabilities
 
-
 class TestAppPercy(unittest.TestCase):
     comparison_response = {'link': 'https://snapshot_url', 'success': True}
 
     @patch('appium.webdriver.webdriver.WebDriver')
     def setUp(self, mock_webdriver):
         mock_webdriver.__class__ = WebDriver
         self.mock_android_webdriver = copy.deepcopy(mock_webdriver)
@@ -43,14 +43,15 @@
     @patch.object(AppAutomate, 'execute_percy_screenshot_begin', MagicMock(return_value={'deviceName': 'Google Pixel 4',
         'osVersion': '12.0',
         'buildHash': 'abc',
         'sessionHash': 'def'
     }))
     @patch.object(AppAutomate, 'execute_percy_screenshot_end', MagicMock(return_value=None))
     @patch.object(Metadata, 'session_id', PropertyMock(return_value='unique_session_id'))
+    @patch.dict(os.environ, {"PERCY_DISABLE_REMOTE_UPLOADS": "true"})
     def test_android_on_app_automate(self):
         with patch('percy.metadata.AndroidMetadata.remote_url', new_callable=PropertyMock) as mock_remote_url:
             mock_remote_url.return_value = 'url-of-browserstack-cloud'
             app_percy = AppPercy(self.mock_android_webdriver)
             app_percy.screenshot('screenshot 1')
             self.assertTrue(isinstance(app_percy.metadata, AndroidMetadata))
             self.assertTrue(isinstance(app_percy.provider, AppAutomate))
@@ -74,22 +75,37 @@
     @patch.object(CLIWrapper, 'post_screenshots', MagicMock(return_value=comparison_response))
     @patch.object(AppAutomate, 'execute_percy_screenshot_begin', MagicMock(return_value={'deviceName': 'iPhone 14',
         'osVersion': '14',
         'buildHash': 'abc',
         'sessionHash': 'def'
     }))
     @patch.object(AppAutomate, 'execute_percy_screenshot_end', MagicMock(return_value=None))
+    @patch.dict(os.environ, {"PERCY_DISABLE_REMOTE_UPLOADS": "true"})
     def test_ios_on_app_automate(self):
         with patch('percy.metadata.IOSMetadata.remote_url', new_callable=PropertyMock) as mock_remote_url:
             mock_remote_url.return_value = 'url-of-browserstack-cloud'
             app_percy = AppPercy(self.mock_ios_webdriver)
             app_percy.screenshot('screenshot 1')
             self.assertTrue(isinstance(app_percy.metadata, IOSMetadata))
             self.assertTrue(isinstance(app_percy.provider, AppAutomate))
 
+    @patch.object(AppAutomate, 'execute_percy_screenshot_end', MagicMock(return_value=None))
+    @patch.object(AppAutomate, 'execute_percy_screenshot', MagicMock(return_value={
+        "result":"[{\"sha\":\"sha-25568755\",\"status_bar\":null,\"nav_bar\":null,\"header_height\":120,\"footer_height\":80,\"index\":0}]"
+    }))
+    @patch.object(CLIWrapper, 'post_screenshots', MagicMock(return_value=comparison_response))
+    @patch.object(Metadata, 'session_id', PropertyMock(return_value='unique_session_id'))
+    def test_ios_on_app_automate_with_remote_upload(self):
+        with patch('percy.metadata.IOSMetadata.remote_url', new_callable=PropertyMock) as mock_remote_url:
+            mock_remote_url.return_value = 'url-of-browserstack-cloud'
+            app_percy = AppPercy(self.mock_ios_webdriver)
+            app_percy.screenshot('screenshot 1')
+            self.assertTrue(isinstance(app_percy.metadata, IOSMetadata))
+            self.assertTrue(isinstance(app_percy.provider, AppAutomate))
+
     @patch.object(GenericProvider, '_write_screenshot', MagicMock(return_value='path-to-png-file'))
     @patch.object(CLIWrapper, 'post_screenshots', MagicMock(return_value=comparison_response))
     @patch.object(Metadata, 'session_id', PropertyMock(return_value='unique_session_id'))
     def test_ios_on_non_app_automate(self):
         with patch('percy.metadata.IOSMetadata.remote_url', new_callable=PropertyMock) as mock_remote_url:
             mock_remote_url.return_value = ''
             app_percy = AppPercy(self.mock_ios_webdriver)
```

### Comparing `percy-appium-app-2.0.0b0/tests/test_cache.py` & `percy-appium-app-2.0.0b1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_cli_wrapper.py` & `percy-appium-app-2.0.0b1/tests/test_cli_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,20 @@
         self.cli_wrapper = cli_wrapper.CLIWrapper()
         self.ignored_elements_data = {
             "ignore_elements_data": {
                 "selector": "xpath: some_xpath",
                 "coOrdinates": {"top": 123, "bottom": 234, "left": 234, "right": 455},
             }
         }
+        self.considered_elements_data = {
+            "consider_elements_data": {
+                "selector": "xpath: some_xpath",
+                "coOrdinates": {"top": 50, "bottom": 100, "left": 0, "right": 100},
+            }
+        }
 
     @patch.object(cli_wrapper.CLIWrapper, "_request_body", return_value={})
     def test_post_screenshot_throws_error(self, _mock_request_body):
         with patch("requests.post") as mock_requests:
             error = "some random error"
             response = Mock()
             response.json.return_value = {"error": error}
@@ -85,31 +91,35 @@
 
     def test_request_body(self):
         tile = Tile("some-file-path", 10, 10, 20, 20)
         tag = {"name": "Tag"}
         name = "some-name"
         debug_url = "debug-url"
         response = self.cli_wrapper._request_body(
-            name, tag, [tile], debug_url, self.ignored_elements_data
+            name, tag, [tile], debug_url, self.ignored_elements_data, self.considered_elements_data
         )
         self.assertEqual(response["name"], name)
         self.assertEqual(response["external_debug_url"], debug_url)
         self.assertDictEqual(response["tag"], tag)
         self.assertListEqual(response["tiles"], [dict(tile)])
         self.assertDictEqual(
             response["ignored_elements_data"], self.ignored_elements_data
         )
+        self.assertDictEqual(
+            response["considered_elements_data"], self.considered_elements_data
+        )
 
     def test_request_body_when_optional_values_are_null(self):
         tile = Tile("some-file-path", 10, 10, 20, 20)
         tag = {"name": "Tag"}
         name = "some-name"
         debug_url = None
         ignored_elements_data = None
+        considered_elements_data = None
         response = self.cli_wrapper._request_body(
-            name, tag, [tile], debug_url, ignored_elements_data
+            name, tag, [tile], debug_url, ignored_elements_data, considered_elements_data
         )
         self.assertEqual(response["name"], name)
         self.assertEqual(response["external_debug_url"], debug_url)
         self.assertDictEqual(response["tag"], tag)
         self.assertListEqual(response["tiles"], [dict(tile)])
         self.assertEqual(response["ignored_elements_data"], None)
```

### Comparing `percy-appium-app-2.0.0b0/tests/test_generic_provider.py` & `percy-appium-app-2.0.0b1/tests/test_generic_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from appium.webdriver.webdriver import WebDriver
 from appium.webdriver.common.appiumby import AppiumBy
 from selenium.common.exceptions import NoSuchElementException
 
 from percy.lib.cli_wrapper import CLIWrapper
 from percy.metadata import AndroidMetadata, Metadata
 from percy.providers.generic_provider import GenericProvider
-from percy.lib.ignore_region import IgnoreRegion
+from percy.lib.region import Region
 from tests.mocks.mock_methods import android_capabilities
 
 
 class TestGenericProvider(unittest.TestCase):
     comparison_response = {"comparison": {"id": 123, "url": "https://percy-build-url"}}
 
     @patch("appium.webdriver.webdriver.WebDriver")
@@ -144,15 +144,15 @@
     @patch.object(
         Metadata, "session_id", PropertyMock(return_value="unique_session_id")
     )
     def test_post_screenshots(self):
         tag = self.generic_provider._get_tag()
         tiles = self.generic_provider._get_tiles()
         response = self.generic_provider._post_screenshots(
-            "screenshot 1", tag, tiles, "", []
+            "screenshot 1", tag, tiles, "", [], []
         )
         self.assertEqual(response, self.comparison_response)
 
     def test_supports(self):
         self.assertTrue(self.generic_provider.supports("some-dummy-url"))
 
     @patch.object(
@@ -173,162 +173,162 @@
         response = self.generic_provider.screenshot("screenshot 1")
         self.assertDictEqual(response, self.comparison_response)
 
     def test_get_device_name(self):
         device_name = self.generic_provider.get_device_name()
         self.assertEqual(device_name, "")
 
-    def test_ignore_element_object(self):
+    def test_get_region_object(self):
         # create a mock element object
         mock_element = MagicMock()
         mock_element.location = {"x": 10, "y": 20}
         mock_element.size = {"width": 100, "height": 200}
 
         # call the function with the mock inputs
-        result = self.generic_provider.ignore_element_object(
+        result = self.generic_provider.get_region_object(
             "my-selector", mock_element
         )
         expected_result = {
             "selector": "my-selector",
             "coOrdinates": {"top": 20, "bottom": 220, "left": 10, "right": 110},
         }
         # check the result
         self.assertDictEqual(result, expected_result)
 
-    def test_ignore_regions_by_xpaths(self):
+    def test_get_regions_by_xpath(self):
         # create a mock driver object with a mock find_element() method
         mock_element = MagicMock()
         mock_element.location = {"x": 10, "y": 20}
         mock_element.size = {"width": 100, "height": 200}
 
         self.mock_webdriver.find_element.return_value = mock_element
 
         expected_result = {
             "selector": "xpath: //path/to/element",
             "coOrdinates": {"top": 20, "bottom": 220, "left": 10, "right": 110},
         }
 
         # call the function with a mock ignored_elements_array and xpaths
-        ignored_elements_array = []
+        elements_array = []
         xpaths = ["//path/to/element"]
-        self.generic_provider.ignore_regions_by_xpaths(ignored_elements_array, xpaths)
+        self.generic_provider.get_regions_by_xpath(elements_array, xpaths)
 
         # check the result
-        expected_ignored_elements_array = [expected_result]
-        self.assertEqual(ignored_elements_array, expected_ignored_elements_array)
+        expected_elements_array = [expected_result]
+        self.assertEqual(elements_array, expected_elements_array)
 
         # check that the driver's find_element() method was called twice
         self.mock_webdriver.find_element.assert_called_with(
             by=AppiumBy.XPATH, value="//path/to/element"
         )
         self.assertEqual(self.mock_webdriver.find_element.call_count, 1)
 
-    def test_ignore_regions_by_xpaths_with_non_existing_element(self):
+    def test_get_regions_by_xpath_with_non_existing_element(self):
         # mock find_element method of the driver to raise NoSuchElementException
         self.mock_webdriver.find_element.side_effect = NoSuchElementException
 
-        ignored_elements_array = []
+        elements_array = []
         xpaths = ["xpath1"]
-        self.generic_provider.ignore_regions_by_xpaths(ignored_elements_array, xpaths)
+        self.generic_provider.get_regions_by_xpath(elements_array, xpaths)
 
         # check the result
-        self.assertEqual(len(ignored_elements_array), 0)
+        self.assertEqual(len(elements_array), 0)
 
-    def test_ignore_regions_by_ids(self):
+    def test_get_regions_by_ids(self):
         # create a mock driver object with a mock find_element() method
         mock_element = MagicMock()
         mock_element.location = {"x": 10, "y": 20}
         mock_element.size = {"width": 100, "height": 200}
 
         self.mock_webdriver.find_element.return_value = mock_element
 
         expected_result = {
             "selector": "id: some_id",
             "coOrdinates": {"top": 20, "bottom": 220, "left": 10, "right": 110},
         }
 
-        # call the function with a mock ignored_elements_array and xpaths
-        ignored_elements_array = []
+        # call the function with a mock elements_array and xpaths
+        elements_array = []
         ids = ["some_id"]
-        self.generic_provider.ignore_regions_by_ids(ignored_elements_array, ids)
+        self.generic_provider.get_regions_by_ids(elements_array, ids)
 
         # check the result
-        expected_ignored_elements_array = [expected_result]
-        self.assertEqual(ignored_elements_array, expected_ignored_elements_array)
+        expected_elements_array = [expected_result]
+        self.assertEqual(elements_array, expected_elements_array)
 
         # check that the driver's find_element() method was called twice
         self.mock_webdriver.find_element.assert_called_with(
             by=AppiumBy.ACCESSIBILITY_ID, value="some_id"
         )
         self.assertEqual(self.mock_webdriver.find_element.call_count, 1)
 
-    def test_ignore_regions_by_ids_with_non_existing_element(self):
+    def test_get_regions_by_ids_with_non_existing_element(self):
         # mock find_element method of the driver to raise NoSuchElementException
         self.mock_webdriver.find_element.side_effect = NoSuchElementException
 
-        ignored_elements_array = []
+        elements_array = []
         ids = ["id1", "id2", "id3"]
-        self.generic_provider.ignore_regions_by_ids(ignored_elements_array, ids)
+        self.generic_provider.get_regions_by_ids(elements_array, ids)
 
         # check the result
-        self.assertEqual(len(ignored_elements_array), 0)
+        self.assertEqual(len(elements_array), 0)
 
-    def test_ignore_regions_by_elements(self):
+    def test_get_regions_by_elements(self):
         # create a mock driver object with a mock find_element() method
         mock_element = MagicMock()
         mock_element.location = {"x": 10, "y": 20}
         mock_element.size = {"width": 100, "height": 200}
         mock_element.get_attribute.return_value = "textView"
 
         expected_result = {
             "selector": "element: 0 textView",
             "coOrdinates": {"top": 20, "bottom": 220, "left": 10, "right": 110},
         }
 
-        # call the function with a mock ignored_elements_array and xpaths
-        ignored_elements_array = []
+        # call the function with a mock elements_array and xpaths
+        elements_array = []
         elements = [mock_element]
-        self.generic_provider.ignore_regions_by_elements(
-            ignored_elements_array, elements
+        self.generic_provider.get_regions_by_elements(
+            elements_array, elements
         )
 
         # check the result
-        expected_ignored_elements_array = [expected_result]
-        self.assertEqual(ignored_elements_array, expected_ignored_elements_array)
+        expected_elements_array = [expected_result]
+        self.assertEqual(elements_array, expected_elements_array)
 
         # check that the driver's find_element() method was called twice
         mock_element.get_attribute.assert_called_with("class")
         self.assertEqual(mock_element.get_attribute.call_count, 1)
 
-    def test_ignore_regions_by_elements_with_non_existing_element(self):
+    def test_get_regions_by_elements_with_non_existing_element(self):
         # mock find_element method of the driver to raise NoSuchElementException
         mock_element = MagicMock()
         mock_element.get_attribute.side_effect = NoSuchElementException
 
-        ignored_elements_array = []
+        elements_array = []
         elements = [mock_element]
-        self.generic_provider.ignore_regions_by_elements(
-            ignored_elements_array, elements
+        self.generic_provider.get_regions_by_elements(
+            elements_array, elements
         )
 
         # check the result
-        self.assertEqual(len(ignored_elements_array), 0)
+        self.assertEqual(len(elements_array), 0)
 
-    def test_add_custom_ignore_regions(self):
+    def test_get_regions_by_location(self):
         # width 1080 height 2280
-        valid_ignore_region = IgnoreRegion(100, 200, 200, 300)
-        invalid_ignore_region = IgnoreRegion(100, 2390, 200, 300)
-        # call the function with mock ignored_elements_array and custom_locations
-        ignored_elements_array = []
-        custom_ignore_regions = [valid_ignore_region, invalid_ignore_region]
-        self.generic_provider.add_custom_ignore_regions(
-            ignored_elements_array, custom_ignore_regions
+        valid_ignore_region = Region(100, 200, 200, 300)
+        invalid_ignore_region = Region(100, 2390, 200, 300)
+        # call the function with mock elements_array and custom_locations
+        elements_array = []
+        custom_locations = [valid_ignore_region, invalid_ignore_region]
+        self.generic_provider.get_regions_by_location(
+            elements_array, custom_locations
         )
         # check the result
-        expected_ignored_elements_array = [
+        expected_elements_array = [
             {
                 "selector": "custom ignore region: 0",
                 "coOrdinates": {"top": 100, "bottom": 200, "left": 200, "right": 300},
             }
         ]
-        self.assertEqual(len(ignored_elements_array), 1)
-        self.assertEqual(ignored_elements_array, expected_ignored_elements_array)
+        self.assertEqual(len(elements_array), 1)
+        self.assertEqual(elements_array, expected_elements_array)
```

### Comparing `percy-appium-app-2.0.0b0/tests/test_ignore_region.py` & `percy-appium-app-2.0.0b1/tests/test_ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_ios_metadata.py` & `percy-appium-app-2.0.0b1/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_metadata.py` & `percy-appium-app-2.0.0b1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_metadata_resolver.py` & `percy-appium-app-2.0.0b1/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_percy_options.py` & `percy-appium-app-2.0.0b1/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-2.0.0b0/tests/test_screenshot.py` & `percy-appium-app-2.0.0b1/tests/test_screenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,18 +258,21 @@
         driver.capabilities = { 'key': 'value' }
         driver.desired_capabilities = { 'key': 'value' }
         driver.command_executor = Mock()
         driver.command_executor._url = 'https://hub-cloud.browserstack.com/wd/hub'
 
         element = Mock()
         element.id = 'Dummy_id'
+
+        consider_element = Mock()
+        consider_element.id = 'Consider_Dummy_id'
         self.mock_webdriver.capabilities = { 'key': 'value' }
         percy_screenshot(driver, 'Snapshot 1')
         percy_screenshot(driver, 'Snapshot 2', options = {'enable_javascript': True,
-                          'ignore_region_appium_elements': [element]})
+                          'ignore_region_appium_elements': [element], 'consider_region_appium_elements' : [consider_element]})
 
         self.assertEqual(httpretty.last_request().path, '/percy/automateScreenshot')
 
         s1 = httpretty.latest_requests()[1].parsed_body
         self.assertEqual(s1['snapshotName'], 'Snapshot 1')
         self.assertEqual(s1['sessionId'], driver.session_id)
         self.assertEqual(s1['commandExecutorUrl'], driver.command_executor._url) # pylint: disable=W0212
@@ -278,10 +281,11 @@
         self.assertRegex(s1['client_info'], r'percy-appium-app/\d+')
         self.assertRegex(s1['environment_info'][0], r'appium/\d+')
         self.assertRegex(s1['environment_info'][1], r'python/\d+')
         s2 = httpretty.latest_requests()[-1].parsed_body
         self.assertEqual(s2['snapshotName'], 'Snapshot 2')
         self.assertEqual(s2['options']['enable_javascript'], True)
         self.assertEqual(s2['options']['ignore_region_elements'], ['Dummy_id'])
+        self.assertEqual(s2['options']['consider_region_elements'], ['Consider_Dummy_id'])
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `percy-appium-app-2.0.0b0/tests/test_tile.py` & `percy-appium-app-2.0.0b1/tests/test_tile.py`

 * *Files identical despite different names*

