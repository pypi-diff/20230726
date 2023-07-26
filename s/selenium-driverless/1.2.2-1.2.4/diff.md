# Comparing `tmp/selenium_driverless-1.2.2.tar.gz` & `tmp/selenium_driverless-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.2.2.tar", last modified: Wed Jul 26 11:52:17 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.4.tar", last modified: Wed Jul 26 16:36:10 2023, max compression
```

## Comparing `selenium_driverless-1.2.2.tar` & `selenium_driverless-1.2.4.tar`

### file list

```diff
@@ -1,42 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.2/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3823 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-07-26 09:25:36.000000 selenium_driverless-1.2.2/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-26 11:52:17.822306 selenium_driverless-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.795854 selenium_driverless-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.803913 selenium_driverless-1.2.2/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-26 11:52:13.000000 selenium_driverless-1.2.2/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.809236 selenium_driverless-1.2.2/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.2/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.812238 selenium_driverless-1.2.2/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.2/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.816291 selenium_driverless-1.2.2/src/selenium_driverless/sync/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/__init__.py
--rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/alert.py
--rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/executor.py
--rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/switch_to.py
--rw-rw-rw-   0        0        0     1351 2023-07-26 11:21:31.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/webdriver.py
--rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.2/src/selenium_driverless/sync/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.818272 selenium_driverless-1.2.2/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.2/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.820306 selenium_driverless-1.2.2/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.2/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.2/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    45635 2023-07-26 11:23:33.000000 selenium_driverless-1.2.2/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.809236 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1079 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 11:52:17.000000 selenium_driverless-1.2.2/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 11:52:17.821325 selenium_driverless-1.2.2/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.2/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.796627 selenium_driverless-1.2.4/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.4/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3870 2023-07-26 16:36:10.796627 selenium_driverless-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2554 2023-07-26 16:22:00.000000 selenium_driverless-1.2.4/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.4/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-26 16:36:10.797628 selenium_driverless-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2122 2023-07-26 16:30:17.000000 selenium_driverless-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.683036 selenium_driverless-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.692944 selenium_driverless-1.2.4/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-07-26 16:35:45.000000 selenium_driverless-1.2.4/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.702585 selenium_driverless-1.2.4/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.4/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.709537 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/
+-rw-rw-rw-   0        0        0     1176 2023-07-26 16:14:27.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/asyncio.py
+-rw-rw-rw-   0        0        0     1361 2023-07-26 16:14:27.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/base.py
+-rw-rw-rw-   0        0        0     7313 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/browser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.778508 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/
+-rw-rw-rw-   0        0        0      798 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/__init__.py
+-rw-rw-rw-   0        0        0    23896 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11602 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/animation.py
+-rw-rw-rw-   0        0        0    52280 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/audits.py
+-rw-rw-rw-   0        0        0     6066 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/background_service.py
+-rw-rw-rw-   0        0        0    21594 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/browser.py
+-rw-rw-rw-   0        0        0     8567 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4435 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/cast.py
+-rw-rw-rw-   0        0        0     2882 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/console.py
+-rw-rw-rw-   0        0        0    66950 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/css.py
+-rw-rw-rw-   0        0        0     4086 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/database.py
+-rw-rw-rw-   0        0        0    52264 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3373 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1154 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    63790 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom.py
+-rw-rw-rw-   0        0        0     9800 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    40830 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5935 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    26766 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1230 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     5466 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    20431 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/fetch.py
+-rw-rw-rw-   0        0        0     4985 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14046 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    15583 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    28365 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/input_.py
+-rw-rw-rw-   0        0        0     1712 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/inspector.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/io.py
+-rw-rw-rw-   0        0        0    15942 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     5784 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/log.py
+-rw-rw-rw-   0        0        0     7923 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/media.py
+-rw-rw-rw-   0        0        0     7010 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/memory.py
+-rw-rw-rw-   0        0        0   135424 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/network.py
+-rw-rw-rw-   0        0        0    56704 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/overlay.py
+-rw-rw-rw-   0        0        0   109903 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/page.py
+-rw-rw-rw-   0        0        0     3080 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance.py
+-rw-rw-rw-   0        0        0     7184 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    15687 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/preload.py
+-rw-rw-rw-   0        0        0    13542 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/profiler.py
+-rw-rw-rw-   0        0        0    61736 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1143 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/schema.py
+-rw-rw-rw-   0        0        0    18042 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/security.py
+-rw-rw-rw-   0        0        0    11603 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    36250 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/storage.py
+-rw-rw-rw-   0        0        0    12090 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/system_info.py
+-rw-rw-rw-   0        0        0    24638 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/target.py
+-rw-rw-rw-   0        0        0     1526 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14160 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/util.py
+-rw-rw-rw-   0        0        0    18058 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    16287 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/cdp/web_authn.py
+-rw-rw-rw-   0        0        0     2426 2023-07-26 16:21:09.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/exceptions.py
+-rw-rw-rw-   0        0        0    13427 2023-07-26 16:21:08.000000 selenium_driverless-1.2.4/src/selenium_driverless/pycdp/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.782577 selenium_driverless-1.2.4/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5771 2023-07-26 08:58:02.000000 selenium_driverless-1.2.4/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.788628 selenium_driverless-1.2.4/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1374 2023-07-26 16:34:36.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.4/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.791627 selenium_driverless-1.2.4/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-07-25 22:04:49.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.4/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.793627 selenium_driverless-1.2.4/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.4/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.4/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    45692 2023-07-26 15:56:46.000000 selenium_driverless-1.2.4/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.701063 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3870 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3718 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 16:36:10.000000 selenium_driverless-1.2.4/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 16:36:10.794627 selenium_driverless-1.2.4/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.4/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2.2/LICENSE.md` & `selenium_driverless-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/PKG-INFO` & `selenium_driverless-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.2.2
+Version: 1.2.4
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -53,15 +53,15 @@
 #### with asyncio
 ```python
 from selenium_driverless import webdriver
 import asyncio
 
 
 async def main():
-    options = webdriver.Options()
+    options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
         await driver.get('http://nowsecure.nl#relax')
         await driver.implicitly_wait(3)
 
         title = await driver.title
         url = await driver.current_url
         source = await driver.page_source
@@ -73,15 +73,15 @@
 
 #### synchronous
 asyncified, might be buggy
 
 ```python
 from selenium_driverless.sync import webdriver
 
-options = webdriver.Options()
+options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
     url = driver.current_url
     source = driver.page_source
@@ -93,14 +93,15 @@
 Please feel free to open an issue or fork!
 
 ## Todo
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
+- [ ] remove pycdp dependency -_-
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.2.2/README.md` & `selenium_driverless-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #### with asyncio
 ```python
 from selenium_driverless import webdriver
 import asyncio
 
 
 async def main():
-    options = webdriver.Options()
+    options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
         await driver.get('http://nowsecure.nl#relax')
         await driver.implicitly_wait(3)
 
         title = await driver.title
         url = await driver.current_url
         source = await driver.page_source
@@ -43,15 +43,15 @@
 
 #### synchronous
 asyncified, might be buggy
 
 ```python
 from selenium_driverless.sync import webdriver
 
-options = webdriver.Options()
+options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
     url = driver.current_url
     source = driver.page_source
@@ -63,14 +63,15 @@
 Please feel free to open an issue or fork!
 
 ## Todo
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
+- [ ] remove pycdp dependency -_-
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.2.2/build_upload.md` & `selenium_driverless-1.2.4/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/setup.py` & `selenium_driverless-1.2.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 import setuptools
 
-requirements = ['selenium~=4.6', "chrome-devtools-protocol"]
+requirements = ['selenium~=4.6']
+
+# pycdp-requirements
+requirements.extend([
+    "aiohttp~=3.8.5",
+    "aiosignal~=1.3.1",
+    "async-timeout~=4.0.2",
+    "attrs~=23.1.0",
+    "charset-normalizer~=3.2.0",
+    "deprecated~=1.2.14",
+    "frozenlist~=1.4.0",
+    "idna~=3.4",
+    "inflection~=0.5.1",
+    "multidict~=6.0.4",
+    "wrapt~=1.15.0",
+    "yarl~=1.9.2",
+])
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_driverless',
     author='Aurin Aegerter',
```

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2.4/src/selenium_driverless/scripts/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2.4/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2.4/src/selenium_driverless/scripts/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/sync/alert.py` & `selenium_driverless-1.2.4/src/selenium_driverless/sync/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/sync/executor.py` & `selenium_driverless-1.2.4/src/selenium_driverless/sync/executor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/sync/switch_to.py` & `selenium_driverless-1.2.4/src/selenium_driverless/sync/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/sync/webdriver.py` & `selenium_driverless-1.2.4/src/selenium_driverless/sync/webdriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from selenium_driverless.scripts.options import Options
+from selenium_driverless.scripts.options import Options as ChromeOptions
 import asyncio
 from selenium_driverless.webdriver import Chrome as AsyncDriver
 import inspect
 
 
 class Chrome(AsyncDriver):
-    def __init__(self, options: Options = None, loop: asyncio.AbstractEventLoop = None):
+    def __init__(self, options: ChromeOptions = None, loop: asyncio.AbstractEventLoop = None):
         super().__init__(options=options)
         if not loop:
             loop = asyncio.new_event_loop()
         self._loop = loop
         self.start_session()
 
     def __enter__(self):
```

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/sync/webelement.py` & `selenium_driverless-1.2.4/src/selenium_driverless/sync/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.2.4/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/types/by.py` & `selenium_driverless-1.2.4/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.2.4/src/selenium_driverless/types/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2.4/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2.4/src/selenium_driverless/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from base64 import urlsafe_b64encode
 from contextlib import asynccontextmanager
 from importlib import import_module
 from typing import List
 from typing import Optional
 from typing import Union
 
-from pyparsing import Char
 from selenium.common.exceptions import InvalidArgumentException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.print_page_options import PrintOptions
 from selenium.webdriver.common.virtual_authenticator import Credential
 from selenium.webdriver.common.virtual_authenticator import VirtualAuthenticatorOptions
 from selenium.webdriver.common.virtual_authenticator import (
     required_virtual_authenticator,
@@ -174,16 +173,16 @@
          - capabilities - a capabilities dict to start the session with.
         """
         await self.start_client()
         if not capabilities:
             capabilities = self._capabilities
         del self._capabilities
         from selenium_driverless.utils.utils import IS_POSIX, read
-        from pycdp.asyncio import connect_cdp
-        from pycdp import cdp
+        from selenium_driverless.pycdp.asyncio import connect_cdp
+        from selenium_driverless.pycdp.cdp.target import get_targets
 
         if self._loop:
             self._switch_to = SyncSwitchTo(driver=self, loop=self._loop)
 
         if not self._options.debugger_address:
             from selenium_driverless.utils.utils import random_port
             port = random_port("localhost")
@@ -202,15 +201,15 @@
         if self._options.debugger_address.split(":")[1] == "0":
             path = self._options.user_data_dir + "/DevToolsActivePort"
             while not os.path.isfile(path):
                 await self.implicitly_wait(0.1)
             self._options.debugger_address = "localhost:" + read(path, sel_root=False).split("\n")[0]
         self._conn = await connect_cdp(f'http://{self._options.debugger_address}')
         self.browser_pid = browser.pid
-        targets = await self._conn.execute(cdp.target.get_targets())
+        targets = await self._conn.execute(get_targets())
         for target in targets:
             if target.type_ == "page":
                 target_id = target.target_id
                 break
         # noinspection PyUnboundLocalVariable
         self.session = await self._conn.connect_session(target_id)
         self._global_this = await RemoteObject(driver=self, js="globalThis", check_existence=False)
@@ -227,22 +226,22 @@
         """
         if driver_command or params:
             raise NotImplementedError("chrome not started with chromedriver")
         return await self.session.execute(cmd=cmd)
 
     async def get(self, url: str, referrer: str = None) -> None:
         """Loads a web page in the current browser session."""
-        from pycdp import cdp
+        from selenium_driverless.pycdp.cdp.page import DomContentEventFired
         await self.execute_cdp_cmd("Page.enable")
         args = {"url": url}
         if referrer:
             args["referrer"] = referrer
 
         async def get(_url: str):
-            with self.session.safe_wait_for(cdp.page.DomContentEventFired) as navigation:
+            with self.session.safe_wait_for(DomContentEventFired) as navigation:
                 await self.execute_cdp_cmd("Page.navigate", args)
                 await navigation
 
         try:
             await asyncio.wait_for(get(url), self._page_load_timeout)
         except asyncio.exceptions.TimeoutError:
             raise TimeoutError(f"page didn't load within timeout of {self._page_load_timeout}")
```

### Comparing `selenium_driverless-1.2.2/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2.4/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.2.2
+Version: 1.2.4
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -53,15 +53,15 @@
 #### with asyncio
 ```python
 from selenium_driverless import webdriver
 import asyncio
 
 
 async def main():
-    options = webdriver.Options()
+    options = webdriver.ChromeOptions()
     async with webdriver.Chrome(options=options) as driver:
         await driver.get('http://nowsecure.nl#relax')
         await driver.implicitly_wait(3)
 
         title = await driver.title
         url = await driver.current_url
         source = await driver.page_source
@@ -73,15 +73,15 @@
 
 #### synchronous
 asyncified, might be buggy
 
 ```python
 from selenium_driverless.sync import webdriver
 
-options = webdriver.Options()
+options = webdriver.ChromeOptions()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
     url = driver.current_url
     source = driver.page_source
@@ -93,14 +93,15 @@
 Please feel free to open an issue or fork!
 
 ## Todo
 - protocoll
   - [ ] add cdp event handler
 - [x] sync
   - [ ] move sync to threaded for allowing event_handlers
+- [ ] remove pycdp dependency -_-
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.2.2/tests/test_driverless.py` & `selenium_driverless-1.2.4/tests/test_driverless.py`

 * *Files identical despite different names*

