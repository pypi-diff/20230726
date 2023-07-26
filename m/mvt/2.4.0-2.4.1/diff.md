# Comparing `tmp/mvt-2.4.0.tar.gz` & `tmp/mvt-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.4.0.tar", last modified: Fri Jul 21 10:21:45 2023, max compression
+gzip compressed data, was "mvt-2.4.1.tar", last modified: Wed Jul 26 16:25:56 2023, max compression
```

## Comparing `mvt-2.4.0.tar` & `mvt-2.4.1.tar`

### file list

```diff
@@ -1,195 +1,206 @@
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.607245 mvt-2.4.0/
--rw-r--r--   0 donncha    (501) staff       (20)    17791 2022-06-22 15:39:11.000000 mvt-2.4.0/LICENSE
--rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-07-21 10:21:45.607338 mvt-2.4.0/PKG-INFO
--rw-r--r--   0 donncha    (501) staff       (20)     3711 2023-07-16 15:19:41.000000 mvt-2.4.0/README.md
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.567529 mvt-2.4.0/mvt/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.570012 mvt-2.4.0/mvt/android/
--rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    11122 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cli.py
--rw-r--r--   0 donncha    (501) staff       (20)     1031 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_adb.py
--rw-r--r--   0 donncha    (501) staff       (20)     1118 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 donncha    (501) staff       (20)     3751 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)     2622 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 donncha    (501) staff       (20)     6138 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.570301 mvt-2.4.0/mvt/android/modules/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/modules/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.574777 mvt-2.4.0/mvt/android/modules/adb/
--rw-r--r--   0 donncha    (501) staff       (20)     1290 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    12394 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     3298 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1822 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     1803 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     2803 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     2016 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 donncha    (501) staff       (20)     1659 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1781 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 donncha    (501) staff       (20)     1377 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 donncha    (501) staff       (20)     3293 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     5278 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/files.py
--rw-r--r--   0 donncha    (501) staff       (20)     2214 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     1844 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 donncha    (501) staff       (20)    12266 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     2711 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/processes.py
--rw-r--r--   0 donncha    (501) staff       (20)     1928 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 donncha    (501) staff       (20)     1413 2023-07-20 16:29:29.000000 mvt-2.4.0/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 donncha    (501) staff       (20)     3688 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/settings.py
--rw-r--r--   0 donncha    (501) staff       (20)     5637 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     3446 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.581494 mvt-2.4.0/mvt/android/modules/androidqf/
--rw-r--r--   0 donncha    (501) staff       (20)      736 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1339 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2418 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     2371 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     3249 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     3918 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     3832 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     2783 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     3040 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 donncha    (501) staff       (20)     2245 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 donncha    (501) staff       (20)     2938 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.582212 mvt-2.4.0/mvt/android/modules/backup/
--rw-r--r--   0 donncha    (501) staff       (20)      238 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2093 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/backup/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2200 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.584556 mvt-2.4.0/mvt/android/modules/bugreport/
--rw-r--r--   0 donncha    (501) staff       (20)      664 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2495 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     2459 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     3432 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     2973 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2725 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 donncha    (501) staff       (20)     2213 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     2425 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 donncha    (501) staff       (20)     2464 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     4182 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     4034 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.585711 mvt-2.4.0/mvt/android/parsers/
--rw-r--r--   0 donncha    (501) staff       (20)      492 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     7297 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/backup.py
--rw-r--r--   0 donncha    (501) staff       (20)    16326 2023-07-16 15:19:45.000000 mvt-2.4.0/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 donncha    (501) staff       (20)      689 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/getprop.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.588730 mvt-2.4.0/mvt/common/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/common/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2622 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 donncha    (501) staff       (20)     6593 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/command.py
--rw-r--r--   0 donncha    (501) staff       (20)      799 2023-07-17 16:31:28.000000 mvt-2.4.0/mvt/common/help.py
--rw-r--r--   0 donncha    (501) staff       (20)    22958 2023-07-20 17:03:04.000000 mvt-2.4.0/mvt/common/indicators.py
--rw-r--r--   0 donncha    (501) staff       (20)     2208 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/logo.py
--rw-r--r--   0 donncha    (501) staff       (20)     8515 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/module.py
--rw-r--r--   0 donncha    (501) staff       (20)     1258 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/options.py
--rw-r--r--   0 donncha    (501) staff       (20)     7545 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/updates.py
--rw-r--r--   0 donncha    (501) staff       (20)     5744 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/url.py
--rw-r--r--   0 donncha    (501) staff       (20)     6932 2023-07-16 15:19:45.000000 mvt-2.4.0/mvt/common/utils.py
--rw-r--r--   0 donncha    (501) staff       (20)      215 2023-07-21 10:17:32.000000 mvt-2.4.0/mvt/common/version.py
--rw-r--r--   0 donncha    (501) staff       (20)     1358 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/virustotal.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.589888 mvt-2.4.0/mvt/ios/
--rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    10764 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cli.py
--rw-r--r--   0 donncha    (501) staff       (20)     1224 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)     1205 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cmd_check_fs.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.590388 mvt-2.4.0/mvt/ios/data/
--rw-r--r--   0 donncha    (501) staff       (20)     3550 2023-05-21 15:40:36.000000 mvt-2.4.0/mvt/ios/data/ios_models.json
--rw-r--r--   0 donncha    (501) staff       (20)    15419 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/data/ios_versions.json
--rw-r--r--   0 donncha    (501) staff       (20)     9049 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/decrypt.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.591049 mvt-2.4.0/mvt/ios/modules/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.592479 mvt-2.4.0/mvt/ios/modules/backup/
--rw-r--r--   0 donncha    (501) staff       (20)      439 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2625 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 donncha    (501) staff       (20)     7235 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 donncha    (501) staff       (20)     6409 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 donncha    (501) staff       (20)     3862 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 donncha    (501) staff       (20)     7170 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/base.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.594942 mvt-2.4.0/mvt/ios/modules/fs/
--rw-r--r--   0 donncha    (501) staff       (20)      913 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     4859 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 donncha    (501) staff       (20)     2816 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 donncha    (501) staff       (20)     3096 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 donncha    (501) staff       (20)     3032 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 donncha    (501) staff       (20)     1749 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 donncha    (501) staff       (20)     3886 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     3958 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 donncha    (501) staff       (20)     2221 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1423 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 donncha    (501) staff       (20)     1732 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 donncha    (501) staff       (20)     1755 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 donncha    (501) staff       (20)     1486 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.600420 mvt-2.4.0/mvt/ios/modules/mixed/
--rw-r--r--   0 donncha    (501) staff       (20)     1512 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     5603 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 donncha    (501) staff       (20)     5167 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 donncha    (501) staff       (20)     2522 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 donncha    (501) staff       (20)     3430 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     3237 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     2405 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 donncha    (501) staff       (20)     3290 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     2981 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     4376 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 donncha    (501) staff       (20)    14773 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 donncha    (501) staff       (20)     5367 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 donncha    (501) staff       (20)     1480 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 donncha    (501) staff       (20)     2967 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 donncha    (501) staff       (20)     6594 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 donncha    (501) staff       (20)     5995 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     5534 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 donncha    (501) staff       (20)     5546 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     4437 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 donncha    (501) staff       (20)     7532 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 donncha    (501) staff       (20)     4854 2023-07-18 15:50:33.000000 mvt-2.4.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 donncha    (501) staff       (20)     6723 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 donncha    (501) staff       (20)     4687 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 donncha    (501) staff       (20)    11032 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/net_base.py
--rw-r--r--   0 donncha    (501) staff       (20)     1848 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/versions.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.568567 mvt-2.4.0/mvt.egg-info/
--rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/PKG-INFO
--rw-r--r--   0 donncha    (501) staff       (20)     6342 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 donncha    (501) staff       (20)        1 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 donncha    (501) staff       (20)       70 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/entry_points.txt
--rw-r--r--   0 donncha    (501) staff       (20)      210 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/requires.txt
--rw-r--r--   0 donncha    (501) staff       (20)       10 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/top_level.txt
--rw-r--r--   0 donncha    (501) staff       (20)     1740 2023-07-21 10:21:45.607706 mvt-2.4.0/setup.cfg
--rwxr-xr-x   0 donncha    (501) staff       (20)      231 2023-02-28 15:49:54.000000 mvt-2.4.0/setup.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.601951 mvt-2.4.0/tests/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.602814 mvt-2.4.0/tests/android/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/android/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2719 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android/test_backup_module.py
--rw-r--r--   0 donncha    (501) staff       (20)     2168 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android/test_backup_parser.py
--rw-r--r--   0 donncha    (501) staff       (20)     2304 2023-07-16 15:19:45.000000 mvt-2.4.0/tests/android/test_dumpsys_parser.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.604552 mvt-2.4.0/tests/android_androidqf/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/android_androidqf/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)      623 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 donncha    (501) staff       (20)      633 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 donncha    (501) staff       (20)      607 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     1385 2023-07-21 09:07:25.000000 mvt-2.4.0/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)      692 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_processes.py
--rw-r--r--   0 donncha    (501) staff       (20)      618 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_settings.py
--rw-r--r--   0 donncha    (501) staff       (20)      661 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.604813 mvt-2.4.0/tests/android_bugreport/
--rw-r--r--   0 donncha    (501) staff       (20)        0 2023-05-10 16:45:13.000000 mvt-2.4.0/tests/android_bugreport/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1838 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_bugreport/test_bugreport.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.605294 mvt-2.4.0/tests/common/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/common/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1743 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/common/test_indicators.py
--rw-r--r--   0 donncha    (501) staff       (20)     2291 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/common/test_utils.py
--rw-r--r--   0 donncha    (501) staff       (20)      725 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/conftest.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.606659 mvt-2.4.0/tests/ios_backup/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/ios_backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)      570 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 donncha    (501) staff       (20)     1132 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_calendar.py
--rw-r--r--   0 donncha    (501) staff       (20)     1124 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_datausage.py
--rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_manifest.py
--rw-r--r--   0 donncha    (501) staff       (20)     1257 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 donncha    (501) staff       (20)     1042 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     1265 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_tcc.py
--rw-r--r--   0 donncha    (501) staff       (20)      690 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.606988 mvt-2.4.0/tests/ios_fs/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/ios_fs/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1160 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 donncha    (501) staff       (20)      572 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_android_androidqf.py
--rw-r--r--   0 donncha    (501) staff       (20)      586 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_android_bugreport.py
--rw-r--r--   0 donncha    (501) staff       (20)      525 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_ios_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)      483 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_ios_versions.py
--rw-r--r--   0 donncha    (501) staff       (20)      928 2023-06-29 17:03:21.000000 mvt-2.4.0/tests/utils.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    17791 2023-04-30 16:02:50.000000 mvt-2.4.1/LICENSE
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4242 2023-07-26 16:25:56.403168 mvt-2.4.1/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3711 2023-07-10 20:46:42.000000 mvt-2.4.1/README.md
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.383168 mvt-2.4.1/mvt/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.383168 mvt-2.4.1/mvt/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/android/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.383168 mvt-2.4.1/mvt/android/artifacts/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        0 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/artifacts/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      277 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/artifacts/artifact.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1848 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/artifacts/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2197 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/artifacts/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2380 2023-07-26 11:48:32.000000 mvt-2.4.1/mvt/android/artifacts/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12482 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1031 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2256 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3987 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6138 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.383168 mvt-2.4.1/mvt/android/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/android/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.387168 mvt-2.4.1/mvt/android/modules/adb/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1290 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12949 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/adb/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3298 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1822 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1803 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2803 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2016 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1659 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1781 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1377 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3293 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5278 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1326 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1844 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    12266 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1276 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1928 2023-07-26 11:42:42.000000 mvt-2.4.1/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1413 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1715 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5637 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3446 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.387168 mvt-2.4.1/mvt/android/modules/androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      736 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1824 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2409 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2362 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3244 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3910 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3823 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1414 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1289 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1795 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3120 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.391168 mvt-2.4.1/mvt/android/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      238 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2093 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/backup/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1985 2023-07-26 11:54:04.000000 mvt-2.4.1/mvt/android/modules/backup/helpers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2200 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.391168 mvt-2.4.1/mvt/android/modules/bugreport/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      664 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2495 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2459 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3432 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2973 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2725 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2213 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2425 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1863 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4182 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4034 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.391168 mvt-2.4.1/mvt/android/parsers/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      457 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/parsers/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7297 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/android/parsers/backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    16326 2023-07-10 20:54:10.000000 mvt-2.4.1/mvt/android/parsers/dumpsys.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      682 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/android/utils.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.391168 mvt-2.4.1/mvt/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      787 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/common/artifact.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2622 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6593 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/common/command.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      963 2023-07-26 11:42:42.000000 mvt-2.4.1/mvt/common/help.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    22959 2023-07-26 13:12:47.000000 mvt-2.4.1/mvt/common/indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2208 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/common/logo.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     8515 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/common/module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1258 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/common/options.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7545 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/common/updates.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5744 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/common/url.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6932 2023-07-10 20:47:15.000000 mvt-2.4.1/mvt/common/utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      215 2023-07-26 16:19:58.000000 mvt-2.4.1/mvt/common/version.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1358 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/common/virustotal.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.395168 mvt-2.4.1/mvt/ios/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      214 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/ios/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    10764 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/cli.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1224 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1205 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/cmd_check_fs.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.395168 mvt-2.4.1/mvt/ios/data/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3550 2023-05-24 09:57:08.000000 mvt-2.4.1/mvt/ios/data/ios_models.json
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    15552 2023-07-26 11:44:41.000000 mvt-2.4.1/mvt/ios/data/ios_versions.json
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     9049 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/ios/decrypt.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.395168 mvt-2.4.1/mvt/ios/modules/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.395168 mvt-2.4.1/mvt/ios/modules/backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      439 2023-04-30 16:02:50.000000 mvt-2.4.1/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2625 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7235 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6409 2023-07-26 11:42:42.000000 mvt-2.4.1/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3862 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7170 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/base.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.395168 mvt-2.4.1/mvt/ios/modules/fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      913 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4859 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2816 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3096 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3032 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1749 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3886 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3958 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2221 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1423 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1732 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1755 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1486 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.399168 mvt-2.4.1/mvt/ios/modules/mixed/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1512 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5603 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5167 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2522 2023-07-26 11:42:50.000000 mvt-2.4.1/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3430 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3237 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2405 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3290 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2981 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4376 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    14773 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5367 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1480 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2967 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6594 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5995 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5534 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5546 2023-07-26 11:42:42.000000 mvt-2.4.1/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4437 2023-07-26 11:42:42.000000 mvt-2.4.1/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     7532 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4854 2023-07-19 08:28:03.000000 mvt-2.4.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6723 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4687 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)    11032 2023-07-17 17:46:04.000000 mvt-2.4.1/mvt/ios/modules/net_base.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1848 2023-06-08 22:15:11.000000 mvt-2.4.1/mvt/ios/versions.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.383168 mvt-2.4.1/mvt.egg-info/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     4242 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     6564 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       70 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      210 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/requires.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       10 2023-07-26 16:25:56.000000 mvt-2.4.1/mvt.egg-info/top_level.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1740 2023-07-26 16:25:56.403168 mvt-2.4.1/setup.cfg
+-rwxr-xr-x   0 etienne   (1000) etienne   (1000)      231 2023-04-30 16:02:50.000000 mvt-2.4.1/setup.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.399168 mvt-2.4.1/tests/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/__init__.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.399168 mvt-2.4.1/tests/android/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/android/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1284 2023-07-26 11:44:41.000000 mvt-2.4.1/tests/android/test_artifact_getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1167 2023-07-26 11:44:41.000000 mvt-2.4.1/tests/android/test_artifact_processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2719 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/android/test_backup_module.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2168 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/android/test_backup_parser.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2304 2023-07-10 20:53:47.000000 mvt-2.4.1/tests/android/test_dumpsys_parser.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/tests/android_androidqf/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/android_androidqf/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      808 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      818 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1720 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      792 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2178 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      851 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      803 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     3395 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/tests/android_bugreport/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        0 2023-05-24 09:57:08.000000 mvt-2.4.1/tests/android_bugreport/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1838 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/android_bugreport/test_bugreport.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/tests/common/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/common/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1743 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/common/test_indicators.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2291 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/common/test_utils.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      725 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/conftest.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/tests/ios_backup/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/ios_backup/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      570 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1132 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1124 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1007 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1257 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1042 2023-07-10 20:46:42.000000 mvt-2.4.1/tests/ios_backup/test_sms.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1265 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      690 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2023-07-26 16:25:56.403168 mvt-2.4.1/tests/ios_fs/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      192 2023-04-30 16:02:50.000000 mvt-2.4.1/tests/ios_fs/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1160 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2194 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/test_check_android_androidqf.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2520 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/test_check_android_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      586 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/test_check_android_bugreport.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      525 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/test_check_ios_backup.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      483 2023-06-08 22:15:11.000000 mvt-2.4.1/tests/test_ios_versions.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1325 2023-07-26 11:54:04.000000 mvt-2.4.1/tests/utils.py
```

### Comparing `mvt-2.4.0/LICENSE` & `mvt-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/PKG-INFO` & `mvt-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.4.0
+Version: 2.4.1
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.4.0/README.md` & `mvt-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/cli.py` & `mvt-2.4.1/mvt/android/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 import logging
 
 import click
 
 from mvt.common.cmd_check_iocs import CmdCheckIOCS
 from mvt.common.help import (
+    HELP_MSG_ANDROID_BACKUP_PASSWORD,
     HELP_MSG_FAST,
     HELP_MSG_HASHES,
     HELP_MSG_IOC,
     HELP_MSG_LIST_MODULES,
     HELP_MSG_MODULE,
+    HELP_MSG_NONINTERACTIVE,
     HELP_MSG_OUTPUT,
     HELP_MSG_SERIAL,
     HELP_MSG_VERBOSE,
 )
 from mvt.common.logo import logo
 from mvt.common.updates import IndicatorsUpdates
 from mvt.common.utils import init_logging, set_verbose_logging
@@ -26,18 +28,20 @@
 from .cmd_check_androidqf import CmdAndroidCheckAndroidQF
 from .cmd_check_backup import CmdAndroidCheckBackup
 from .cmd_check_bugreport import CmdAndroidCheckBugreport
 from .cmd_download_apks import DownloadAPKs
 from .modules.adb import ADB_MODULES
 from .modules.adb.packages import Packages
 from .modules.backup import BACKUP_MODULES
+from .modules.backup.helpers import cli_load_android_backup_password
 from .modules.bugreport import BUGREPORT_MODULES
 
 init_logging()
 log = logging.getLogger("mvt")
+
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 # ==============================================================================
 # Main
 # ==============================================================================
 @click.group(invoke_without_command=False)
@@ -121,15 +125,15 @@
 
 
 # ==============================================================================
 # Command: check-adb
 # ==============================================================================
 @cli.command(
     "check-adb",
-    help="Check an Android device over adb",
+    help="Check an Android device over ADB",
     context_settings=CONTEXT_SETTINGS,
 )
 @click.option("--serial", "-s", type=str, help=HELP_MSG_SERIAL)
 @click.option(
     "--iocs",
     "-i",
     type=click.Path(exists=True),
@@ -137,19 +141,36 @@
     default=[],
     help=HELP_MSG_IOC,
 )
 @click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
+@click.option("--non-interactive", "-n", is_flag=True, help=HELP_MSG_NONINTERACTIVE)
+@click.option("--backup-password", "-p", help=HELP_MSG_ANDROID_BACKUP_PASSWORD)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
-def check_adb(ctx, serial, iocs, output, fast, list_modules, module, verbose):
+def check_adb(
+    ctx,
+    serial,
+    iocs,
+    output,
+    fast,
+    list_modules,
+    module,
+    non_interactive,
+    backup_password,
+    verbose,
+):
     set_verbose_logging(verbose)
-    module_options = {"fast_mode": fast}
+    module_options = {
+        "fast_mode": fast,
+        "interactive": not non_interactive,
+        "backup_password": cli_load_android_backup_password(log, backup_password),
+    }
 
     cmd = CmdAndroidCheckADB(
         results_path=output,
         ioc_files=iocs,
         module_name=module,
         serial=serial,
         module_options=module_options,
@@ -230,22 +251,41 @@
     type=click.Path(exists=True),
     multiple=True,
     default=[],
     help=HELP_MSG_IOC,
 )
 @click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
+@click.option("--non-interactive", "-n", is_flag=True, help=HELP_MSG_NONINTERACTIVE)
+@click.option("--backup-password", "-p", help=HELP_MSG_ANDROID_BACKUP_PASSWORD)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
-def check_backup(ctx, iocs, output, list_modules, verbose, backup_path):
+def check_backup(
+    ctx,
+    iocs,
+    output,
+    list_modules,
+    non_interactive,
+    backup_password,
+    verbose,
+    backup_path,
+):
     set_verbose_logging(verbose)
+
     # Always generate hashes as backups are generally small.
     cmd = CmdAndroidCheckBackup(
-        target_path=backup_path, results_path=output, ioc_files=iocs, hashes=True
+        target_path=backup_path,
+        results_path=output,
+        ioc_files=iocs,
+        hashes=True,
+        module_options={
+            "interactive": not non_interactive,
+            "backup_password": cli_load_android_backup_password(log, backup_password),
+        },
     )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking Android backup at path: %s", backup_path)
@@ -275,27 +315,43 @@
     default=[],
     help=HELP_MSG_IOC,
 )
 @click.option("--output", "-o", type=click.Path(exists=False), help=HELP_MSG_OUTPUT)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
+@click.option("--non-interactive", "-n", is_flag=True, help=HELP_MSG_NONINTERACTIVE)
+@click.option("--backup-password", "-p", help=HELP_MSG_ANDROID_BACKUP_PASSWORD)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("ANDROIDQF_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_androidqf(
-    ctx, iocs, output, list_modules, module, hashes, verbose, androidqf_path
+    ctx,
+    iocs,
+    output,
+    list_modules,
+    module,
+    hashes,
+    non_interactive,
+    backup_password,
+    verbose,
+    androidqf_path,
 ):
     set_verbose_logging(verbose)
+
     cmd = CmdAndroidCheckAndroidQF(
         target_path=androidqf_path,
         results_path=output,
         ioc_files=iocs,
         module_name=module,
         hashes=hashes,
+        module_options={
+            "interactive": not non_interactive,
+            "backup_password": cli_load_android_backup_password(log, backup_password),
+        },
     )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking AndroidQF acquisition at path: %s", androidqf_path)
```

### Comparing `mvt-2.4.0/mvt/android/cmd_check_adb.py` & `mvt-2.4.1/mvt/android/cmd_check_adb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/cmd_check_androidqf.py` & `mvt-2.4.1/mvt/ios/cmd_check_fs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
 from mvt.common.command import Command
 
-from .modules.androidqf import ANDROIDQF_MODULES
+from .modules.fs import FS_MODULES
+from .modules.mixed import MIXED_MODULES
 
 log = logging.getLogger(__name__)
 
 
-class CmdAndroidCheckAndroidQF(Command):
+class CmdIOSCheckFS(Command):
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
@@ -31,9 +32,12 @@
             module_name=module_name,
             serial=serial,
             module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
-        self.name = "check-androidqf"
-        self.modules = ANDROIDQF_MODULES
+        self.name = "check-fs"
+        self.modules = FS_MODULES + MIXED_MODULES
+
+    def module_init(self, module):
+        module.is_fs_dump = True
```

### Comparing `mvt-2.4.0/mvt/android/cmd_check_backup.py` & `mvt-2.4.1/mvt/android/cmd_check_backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 import logging
 import os
 import sys
 import tarfile
 from pathlib import Path
 from typing import List, Optional
 
-from rich.prompt import Prompt
-
 from mvt.android.modules.backup.base import BackupExtraction
+from mvt.android.modules.backup.helpers import prompt_or_load_android_backup_password
 from mvt.android.parsers.backup import (
     AndroidBackupParsingError,
     InvalidBackupPassword,
     parse_ab_header,
     parse_backup_file,
 )
 from mvt.common.command import Command
@@ -68,15 +67,20 @@
             header = parse_ab_header(data)
             if not header["backup"]:
                 log.critical("Invalid backup format, file should be in .ab format")
                 sys.exit(1)
 
             password = None
             if header["encryption"] != "none":
-                password = Prompt.ask("Enter backup password", password=True)
+                password = prompt_or_load_android_backup_password(
+                    log, self.module_options
+                )
+                if not password:
+                    log.critical("No backup password provided.")
+                    sys.exit(1)
             try:
                 tardata = parse_backup_file(data, password=password)
             except InvalidBackupPassword:
                 log.critical("Invalid backup password")
                 sys.exit(1)
             except AndroidBackupParsingError as exc:
                 log.critical("Impossible to parse this backup file: %s", exc)
```

### Comparing `mvt-2.4.0/mvt/android/cmd_check_bugreport.py` & `mvt-2.4.1/mvt/android/cmd_check_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/cmd_download_apks.py` & `mvt-2.4.1/mvt/android/cmd_download_apks.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/__init__.py` & `mvt-2.4.1/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/base.py` & `mvt-2.4.1/mvt/android/modules/adb/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from adb_shell.auth.sign_pythonrsa import PythonRSASigner
 from adb_shell.exceptions import (
     AdbCommandFailureException,
     DeviceAuthError,
     UsbDeviceNotFoundError,
     UsbReadFailedError,
 )
-from rich.prompt import Prompt
 from usb1 import USBErrorAccess, USBErrorBusy
 
+from mvt.android.modules.backup.helpers import prompt_or_load_android_backup_password
 from mvt.android.parsers.backup import (
     InvalidBackupPassword,
     parse_ab_header,
     parse_backup_file,
 )
 from mvt.common.module import InsufficientPrivileges, MVTModule
 
@@ -307,14 +307,20 @@
 
     def _generate_backup(self, package_name: str) -> bytes:
         self.log.info(
             "Please check phone and accept Android backup prompt. "
             "You may need to set a backup password. \a"
         )
 
+        if self.module_options.get("backup_password", None):
+            self.log.warning(
+                "Backup password already set from command line or environment "
+                "variable. You should use the same password if enabling encryption!"
+            )
+
         # TODO: Base64 encoding as temporary fix to avoid byte-mangling over
         #       the shell transport...
         cmd = f"/system/bin/bu backup -nocompress '{package_name}' | base64"
         backup_output_b64 = self._adb_command(cmd)
         backup_output = base64.b64decode(backup_output_b64)
         header = parse_ab_header(backup_output)
 
@@ -325,15 +331,20 @@
             )
             return None
 
         if header["encryption"] == "none":
             return parse_backup_file(backup_output, password=None)
 
         for _ in range(0, 3):
-            backup_password = Prompt.ask("Enter backup password", password=True)
+            backup_password = prompt_or_load_android_backup_password(
+                self.log, self.module_options
+            )
+            if not backup_password:
+                # Fail as no backup password loaded for this encrypted backup
+                self.log.critical("No backup password provided.")
             try:
                 decrypted_backup_tar = parse_backup_file(backup_output, backup_password)
                 return decrypted_backup_tar
             except InvalidBackupPassword:
                 self.log.error("You provided the wrong password! Please try again...")
 
         self.log.error("All attempts to decrypt backup with password failed!")
```

### Comparing `mvt-2.4.0/mvt/android/modules/adb/chrome_history.py` & `mvt-2.4.1/mvt/android/modules/adb/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_full.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.4.1/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/files.py` & `mvt-2.4.1/mvt/android/modules/adb/files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/getprop.py` & `mvt-2.4.1/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from datetime import datetime, timedelta
-from typing import Optional
+from typing import Optional, Union
 
-from mvt.android.parsers import parse_getprop
+from .webkit_base import WebkitBase
 
-from .base import AndroidExtraction
+WEBKIT_LOCALSTORAGE_ROOT_PATHS = [
+    "private/var/mobile/Containers/Data/Application/*/Library/WebKit/WebsiteData/LocalStorage/",
+]
 
 
-class Getprop(AndroidExtraction):
-    """This module extracts device properties from getprop command."""
+class WebkitLocalStorage(WebkitBase):
+    """This module looks extracts records from WebKit LocalStorage folders,
+    and checks them against any provided list of suspicious domains.
+
+
+    """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -29,39 +34,22 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-        self.results = {} if not results else results
-
-    def check_indicators(self) -> None:
-        if not self.indicators:
-            return
-
-        for result in self.results:
-            ioc = self.indicators.check_android_property_name(result.get("name", ""))
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+    def serialize(self, record: dict) -> Union[dict, list]:
+        return {
+            "timestamp": record["isodate"],
+            "module": self.__class__.__name__,
+            "event": "webkit_local_storage",
+            "data": f"WebKit Local Storage folder {record['folder']} "
+            f"containing file for URL {record['url']}",
+        }
 
     def run(self) -> None:
-        self._adb_connect()
-        output = self._adb_command("getprop")
-        self._adb_disconnect()
-
-        self.results = parse_getprop(output)
-
-        # Alert if phone is outdated.
-        for entry in self.results:
-            if entry.get("name", "") != "ro.build.version.security_patch":
-                continue
-            patch_date = datetime.strptime(entry["value"], "%Y-%m-%d")
-            if (datetime.now() - patch_date) > timedelta(days=6 * 30):
-                self.log.warning(
-                    "This phone has not received security updates "
-                    "for more than six months (last update: %s)",
-                    entry["value"],
-                )
-
-        self.log.info("Extracted %d Android system properties", len(self.results))
+        self._process_webkit_folder(WEBKIT_LOCALSTORAGE_ROOT_PATHS)
+        self.log.info(
+            "Extracted a total of %d records from WebKit Local Storages",
+            len(self.results),
+        )
```

### Comparing `mvt-2.4.0/mvt/android/modules/adb/logcat.py` & `mvt-2.4.1/mvt/android/modules/adb/logcat.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/packages.py` & `mvt-2.4.1/mvt/android/modules/adb/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/processes.py` & `mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional
+from typing import Optional, Union
 
-from .base import AndroidExtraction
+from mvt.android.parsers import parse_dumpsys_appops
 
+from .base import AndroidQFModule
 
-class Processes(AndroidExtraction):
-    """This module extracts details on running processes."""
 
+class DumpsysAppops(AndroidQFModule):
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
@@ -26,65 +26,69 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-    def check_indicators(self) -> None:
-        if not self.indicators:
-            return
-
-        for result in self.results:
-            proc_name = result.get("proc_name", "")
-            if not proc_name:
+    def serialize(self, record: dict) -> Union[dict, list]:
+        records = []
+        for perm in record["permissions"]:
+            if "entries" not in perm:
                 continue
 
-            # Skipping this process because of false positives.
-            if result["proc_name"] == "gatekeeperd":
-                continue
+            for entry in perm["entries"]:
+                if "timestamp" in entry:
+                    records.append(
+                        {
+                            "timestamp": entry["timestamp"],
+                            "module": self.__class__.__name__,
+                            "event": entry["access"],
+                            "data": f"{record['package_name']} access to "
+                            f"{perm['name']} : {entry['access']}",
+                        }
+                    )
 
-            ioc = self.indicators.check_app_id(proc_name)
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
-                continue
+        return records
 
-            ioc = self.indicators.check_process(proc_name)
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+    def check_indicators(self) -> None:
+        for result in self.results:
+            if self.indicators:
+                ioc = self.indicators.check_app_id(result.get("package_name"))
+                if ioc:
+                    result["matched_indicator"] = ioc
+                    self.detected.append(result)
+                    continue
+
+            for perm in result["permissions"]:
+                if (
+                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
+                    and perm["access"] == "allow"
+                ):
+                    self.log.info(
+                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
+                        result["package_name"],
+                    )
 
     def run(self) -> None:
-        self._adb_connect()
-
-        output = self._adb_command("ps -A")
+        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
+        if not dumpsys_file:
+            return
 
-        for line in output.splitlines()[1:]:
-            line = line.strip()
-            if line == "":
+        lines = []
+        in_package = False
+        data = self._get_file_content(dumpsys_file[0])
+        for line in data.decode("utf-8").split("\n"):
+            if line.startswith("DUMP OF SERVICE appops:"):
+                in_package = True
                 continue
 
-            fields = line.split()
-            proc = {
-                "user": fields[0],
-                "pid": fields[1],
-                "parent_pid": fields[2],
-                "vsize": fields[3],
-                "rss": fields[4],
-            }
-
-            # Sometimes WCHAN is empty, so we need to re-align output fields.
-            if len(fields) == 8:
-                proc["wchan"] = ""
-                proc["pc"] = fields[5]
-                proc["name"] = fields[7]
-            elif len(fields) == 9:
-                proc["wchan"] = fields[5]
-                proc["pc"] = fields[6]
-                proc["name"] = fields[8]
-
-            self.results.append(proc)
+            if in_package:
+                if line.startswith(
+                    "-------------------------------------------------------------------------------"
+                ):  # pylint: disable=line-too-long
+                    break
 
-        self._adb_disconnect()
+                lines.append(line.rstrip())
 
-        self.log.info("Extracted records on a total of %d processes", len(self.results))
+        self.results = parse_dumpsys_appops("\n".join(lines))
+        self.log.info("Identified %d applications in AppOps Manager", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/adb/root_binaries.py` & `mvt-2.4.1/mvt/android/modules/adb/root_binaries.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/selinux_status.py` & `mvt-2.4.1/mvt/android/modules/adb/selinux_status.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/sms.py` & `mvt-2.4.1/mvt/android/modules/adb/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/adb/whatsapp.py` & `mvt-2.4.1/mvt/android/modules/adb/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/__init__.py` & `mvt-2.4.1/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/base.py` & `mvt-2.4.1/mvt/android/modules/androidqf/processes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
-import fnmatch
 import logging
-import os
-from typing import Any, Dict, List, Optional, Union
+from typing import Optional
 
-from mvt.common.module import MVTModule
+from mvt.android.artifacts.processes import Processes as ProcessesArtifact
 
+from .base import AndroidQFModule
 
-class AndroidQFModule(MVTModule):
-    """This class provides a base for all Android Data analysis modules."""
+
+class Processes(ProcessesArtifact, AndroidQFModule):
+    """This module analyse running processes"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
-        results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None,
+        results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-        self._path = target_path
-        self._files = []
-
-        for root, dirs, files in os.walk(target_path):
-            for name in files:
-                self._files.append(os.path.join(root, name))
+    def run(self) -> None:
+        ps_files = self._get_files_by_pattern("*/ps.txt")
+        if not ps_files:
+            return
 
-    def _get_files_by_pattern(self, pattern):
-        return fnmatch.filter(self._files, pattern)
+        self.parse(self._get_file_content(ps_files[0]).decode("utf-8"))
+        self.log.info("Identified %d running processes", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,29 +45,29 @@
     def run(self) -> None:
         dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
         if not dumpsys_file:
             return
 
         lines = []
         in_accessibility = False
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.strip().startswith("DUMP OF SERVICE accessibility:"):
-                    in_accessibility = True
-                    continue
-
-                if not in_accessibility:
-                    continue
-
-                if line.strip().startswith(
-                    "-------------------------------------------------------------------------------"
-                ):  # pylint: disable=line-too-long
-                    break
+        data = self._get_file_content(dumpsys_file[0])
+        for line in data.decode("utf-8").split("\n"):
+            if line.strip().startswith("DUMP OF SERVICE accessibility:"):
+                in_accessibility = True
+                continue
+
+            if not in_accessibility:
+                continue
+
+            if line.strip().startswith(
+                "-------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
 
-                lines.append(line.rstrip())
+            lines.append(line.rstrip())
 
         self.results = parse_dumpsys_accessibility("\n".join(lines))
 
         for result in self.results:
             self.log.info(
                 'Found installed accessibility service "%s"', result.get("service")
             )
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,26 +48,26 @@
     def run(self) -> None:
         dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
         if not dumpsys_file:
             return
 
         lines = []
         in_package = False
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.strip() == "DUMP OF SERVICE package:":
-                    in_package = True
-                    continue
-
-                if not in_package:
-                    continue
-
-                if line.strip().startswith(
-                    "------------------------------------------------------------------------------"
-                ):  # pylint: disable=line-too-long
-                    break
+        data = self._get_file_content(dumpsys_file[0])
+        for line in data.decode("utf-8").split("\n"):
+            if line.strip() == "DUMP OF SERVICE package:":
+                in_package = True
+                continue
+
+            if not in_package:
+                continue
+
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
 
-                lines.append(line.rstrip())
+            lines.append(line.rstrip())
 
         self.results = parse_dumpsys_activity_resolver_table("\n".join(lines))
 
         self.log.info("Extracted activities for %d intents", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.4.1/mvt/android/modules/bugreport/accessibility.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional, Union
+from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_appops
+from mvt.android.parsers import parse_dumpsys_accessibility
 
-from .base import AndroidQFModule
+from .base import BugReportModule
 
 
-class DumpsysAppops(AndroidQFModule):
+class Accessibility(BugReportModule):
+    """This module extracts stats on accessibility."""
+
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
@@ -26,69 +28,53 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-    def serialize(self, record: dict) -> Union[dict, list]:
-        records = []
-        for perm in record["permissions"]:
-            if "entries" not in perm:
-                continue
-
-            for entry in perm["entries"]:
-                if "timestamp" in entry:
-                    records.append(
-                        {
-                            "timestamp": entry["timestamp"],
-                            "module": self.__class__.__name__,
-                            "event": entry["access"],
-                            "data": f"{record['package_name']} access to "
-                            f"{perm['name']} : {entry['access']}",
-                        }
-                    )
-
-        return records
-
     def check_indicators(self) -> None:
+        if not self.indicators:
+            return
+
         for result in self.results:
-            if self.indicators:
-                ioc = self.indicators.check_app_id(result.get("package_name"))
-                if ioc:
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
-                    continue
-
-            for perm in result["permissions"]:
-                if (
-                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
-                    and perm["access"] == "allow"
-                ):
-                    self.log.info(
-                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
-                        result["package_name"],
-                    )
+            ioc = self.indicators.check_app_id(result["package_name"])
+            if ioc:
+                result["matched_indicator"] = ioc
+                self.detected.append(result)
+                continue
 
     def run(self) -> None:
-        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
-        if not dumpsys_file:
+        content = self._get_dumpstate_file()
+        if not content:
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
-        in_package = False
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.startswith("DUMP OF SERVICE appops:"):
-                    in_package = True
-                    continue
-
-                if in_package:
-                    if line.startswith(
-                        "-------------------------------------------------------------------------------"
-                    ):  # pylint: disable=line-too-long
-                        break
+        in_accessibility = False
+        for line in content.decode(errors="ignore").splitlines():
+            if line.strip() == "DUMP OF SERVICE accessibility:":
+                in_accessibility = True
+                continue
+
+            if not in_accessibility:
+                continue
+
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
 
-                    lines.append(line.rstrip())
+            lines.append(line)
 
-        self.results = parse_dumpsys_appops("\n".join(lines))
-        self.log.info("Identified %d applications in AppOps Manager", len(self.results))
+        self.results = parse_dumpsys_accessibility("\n".join(lines))
+        for result in self.results:
+            self.log.info(
+                'Found installed accessibility service "%s"', result.get("service")
+            )
+
+        self.log.info(
+            "Identified a total of %d accessibility services", len(self.results)
+        )
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,21 +74,20 @@
 
     def run(self) -> None:
         dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
         if len(dumpsys_file) != 1:
             self.log.info("Dumpsys file not found")
             return
 
-        with open(dumpsys_file[0]) as handle:
-            data = handle.read().split("\n")
+        data = self._get_file_content(dumpsys_file[0])
 
         package = []
         in_service = False
         in_package_list = False
-        for line in data:
+        for line in data.decode("utf-8").split("\n"):
             if line.strip().startswith("DUMP OF SERVICE package:"):
                 in_service = True
                 continue
 
             if in_service and line.startswith("Packages:"):
                 in_package_list = True
                 continue
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.4.1/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,26 +82,26 @@
     def run(self) -> None:
         dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
         if not dumpsys_file:
             return
 
         in_receivers = False
         lines = []
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.strip() == "DUMP OF SERVICE package:":
-                    in_receivers = True
-                    continue
-
-                if not in_receivers:
-                    continue
-
-                if line.strip().startswith(
-                    "------------------------------------------------------------------------------"
-                ):  # pylint: disable=line-too-long
-                    break
+        data = self._get_file_content(dumpsys_file[0])
+        for line in data.decode("utf-8").split("\n"):
+            if line.strip() == "DUMP OF SERVICE package:":
+                in_receivers = True
+                continue
+
+            if not in_receivers:
+                continue
+
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
 
-                lines.append(line.rstrip())
+            lines.append(line.rstrip())
 
         self.results = parse_dumpsys_receiver_resolver_table("\n".join(lines))
 
         self.log.info("Extracted receivers for %d intents", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/processes.py` & `mvt-2.4.1/mvt/ios/modules/fs/filesystem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional
+import os
+from typing import Optional, Union
 
-from .base import AndroidQFModule
+from mvt.common.utils import convert_unix_to_iso
 
+from ..base import IOSExtraction
 
-class Processes(AndroidQFModule):
-    """This module analyse running processes"""
+
+class Filesystem(IOSExtraction):
+    """This module extracts creation and modification date of files from a
+    full file-system dump.
+    """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -26,74 +31,62 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
+    def serialize(self, record: dict) -> Union[dict, list]:
+        return {
+            "timestamp": record["modified"],
+            "module": self.__class__.__name__,
+            "event": "entry_modified",
+            "data": record["path"],
+        }
+
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            proc_name = result.get("proc_name", "")
-            if not proc_name:
+            if "path" not in result:
                 continue
 
-            # Skipping this process because of false positives.
-            if result["proc_name"] == "gatekeeperd":
-                continue
-
-            ioc = self.indicators.check_app_id(proc_name)
+            ioc = self.indicators.check_file_path(result["path"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
+
+            # If we are instructed to run fast, we skip the rest.
+            if self.module_options.get("fast_mode", None):
                 continue
 
-            ioc = self.indicators.check_process(proc_name)
+            ioc = self.indicators.check_file_path_process(result["path"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
-    def _parse_ps(self, data):
-        for line in data.split("\n")[1:]:
-            proc = line.split()
-
-            # Sometimes WCHAN is empty.
-            if len(proc) == 8:
-                proc = proc[:5] + [""] + proc[5:]
-
-            # Sometimes there is the security label.
-            if proc[0].startswith("u:r"):
-                label = proc[0]
-                proc = proc[1:]
-            else:
-                label = ""
-
-            # Sometimes there is no WCHAN.
-            if len(proc) < 9:
-                proc = proc[:5] + [""] + proc[5:]
-
-            self.results.append(
-                {
-                    "user": proc[0],
-                    "pid": int(proc[1]),
-                    "ppid": int(proc[2]),
-                    "virtual_memory_size": int(proc[3]),
-                    "resident_set_size": int(proc[4]),
-                    "wchan": proc[5],
-                    "aprocress": proc[6],
-                    "stat": proc[7],
-                    "proc_name": proc[8].strip("[]"),
-                    "label": label,
-                }
-            )
-
     def run(self) -> None:
-        ps_files = self._get_files_by_pattern("*/ps.txt")
-        if not ps_files:
-            return
-
-        with open(ps_files[0]) as handle:
-            self._parse_ps(handle.read())
-
-        self.log.info("Identified %d running processes", len(self.results))
+        for root, dirs, files in os.walk(self.target_path):
+            for dir_name in dirs:
+                try:
+                    dir_path = os.path.join(root, dir_name)
+                    result = {
+                        "path": os.path.relpath(dir_path, self.target_path),
+                        "modified": convert_unix_to_iso(os.stat(dir_path).st_mtime),
+                    }
+                except Exception:
+                    continue
+                else:
+                    self.results.append(result)
+
+            for file_name in files:
+                try:
+                    file_path = os.path.join(root, file_name)
+                    result = {
+                        "path": os.path.relpath(file_path, self.target_path),
+                        "modified": convert_unix_to_iso(os.stat(file_path).st_mtime),
+                    }
+                except Exception:
+                    continue
+                else:
+                    self.results.append(result)
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/settings.py` & `mvt-2.4.1/mvt/android/modules/adb/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from mvt.android.modules.adb.settings import ANDROID_DANGEROUS_SETTINGS
+from mvt.android.artifacts.settings import Settings as SettingsArtifact
 
-from .base import AndroidQFModule
+from .base import AndroidExtraction
 
 
-class Settings(AndroidQFModule):
-    """This module analyse setting files"""
+class Settings(SettingsArtifact, AndroidExtraction):
+    """This module extracts Android system settings."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -27,41 +27,32 @@
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
-        self.results = {}
+
+        self.results = {} if not results else results
 
     def run(self) -> None:
-        for setting_file in self._get_files_by_pattern("*/settings_*.txt"):
-            namespace = setting_file[setting_file.rfind("_") + 1 : -4]
+        self._adb_connect()
+
+        for namespace in ["system", "secure", "global"]:
+            out = self._adb_command(f"cmd settings list {namespace}")
+            if not out:
+                continue
 
             self.results[namespace] = {}
 
-            with open(setting_file) as handle:
-                for line in handle:
-                    line = line.strip()
-                    try:
-                        key, value = line.split("=", 1)
-                    except ValueError:
-                        continue
-
-                    try:
-                        self.results[namespace][key] = value
-                    except IndexError:
-                        continue
-
-                    for danger in ANDROID_DANGEROUS_SETTINGS:
-                        if danger["key"] == key and danger["safe_value"] != value:
-                            self.log.warning(
-                                'Found suspicious setting "%s = %s" (%s)',
-                                key,
-                                value,
-                                danger["description"],
-                            )
-                            break
+            for line in out.splitlines():
+                line = line.strip()
+                if line == "":
+                    continue
+
+                fields = line.split("=", 1)
+                try:
+                    self.results[namespace][fields[0]] = fields[1]
+                except IndexError:
+                    continue
 
-        self.log.info(
-            "Identified %d settings", sum([len(val) for val in self.results.values()])
-        )
+        self._adb_disconnect()
```

### Comparing `mvt-2.4.0/mvt/android/modules/androidqf/sms.py` & `mvt-2.4.1/mvt/android/modules/androidqf/sms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1
 
-import getpass
 import logging
 from typing import Optional
 
+from mvt.android.modules.backup.helpers import prompt_or_load_android_backup_password
 from mvt.android.parsers.backup import (
     AndroidBackupParsingError,
     InvalidBackupPassword,
     parse_ab_header,
     parse_backup_file,
     parse_tar_for_sms,
 )
@@ -54,15 +54,21 @@
         header = parse_ab_header(data)
         if not header["backup"]:
             self.log.critical("Invalid backup format, backup.ab was not analysed")
             return
 
         password = None
         if header["encryption"] != "none":
-            password = getpass.getpass(prompt="Backup Password: ", stream=None)
+            password = prompt_or_load_android_backup_password(
+                self.log, self.module_options
+            )
+            if not password:
+                self.log.critical("No backup password provided.")
+                return
+
         try:
             tardata = parse_backup_file(data, password=password)
         except InvalidBackupPassword:
             self.log.critical("Invalid backup password")
             return
         except AndroidBackupParsingError:
             self.log.critical(
@@ -86,12 +92,9 @@
 
     def run(self) -> None:
         files = self._get_files_by_pattern("*/backup.ab")
         if not files:
             self.log.info("No backup data found")
             return
 
-        with open(files[0], "rb") as handle:
-            data = handle.read()
-
-        self.parse_backup(data)
+        self.parse_backup(self._get_file_content(files[0]))
         self.log.info("Identified %d SMS in backup data", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/backup/base.py` & `mvt-2.4.1/mvt/android/modules/backup/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/backup/sms.py` & `mvt-2.4.1/mvt/android/modules/backup/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/__init__.py` & `mvt-2.4.1/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.4.1/mvt/android/modules/bugreport/battery_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_accessibility
+from mvt.android.parsers import parse_dumpsys_battery_history
 
 from .base import BugReportModule
 
 
-class Accessibility(BugReportModule):
-    """This module extracts stats on accessibility."""
+class BatteryHistory(BugReportModule):
+    """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -49,32 +49,27 @@
             self.log.error(
                 "Unable to find dumpstate file. "
                 "Did you provide a valid bug report archive?"
             )
             return
 
         lines = []
-        in_accessibility = False
+        in_history = False
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE accessibility:":
-                in_accessibility = True
+            if line.strip().startswith("Battery History "):
+                lines.append(line)
+                in_history = True
                 continue
 
-            if not in_accessibility:
+            if not in_history:
                 continue
 
-            if line.strip().startswith(
-                "------------------------------------------------------------------------------"
-            ):  # pylint: disable=line-too-long
+            if line.strip() == "":
                 break
 
             lines.append(line)
 
-        self.results = parse_dumpsys_accessibility("\n".join(lines))
-        for result in self.results:
-            self.log.info(
-                'Found installed accessibility service "%s"', result.get("service")
-            )
+        self.results = parse_dumpsys_battery_history("\n".join(lines))
 
         self.log.info(
-            "Identified a total of %d accessibility services", len(self.results)
+            "Extracted a total of %d battery history records", len(self.results)
         )
```

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/activities.py` & `mvt-2.4.1/mvt/android/modules/bugreport/activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/appops.py` & `mvt-2.4.1/mvt/android/modules/bugreport/appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/base.py` & `mvt-2.4.1/mvt/android/modules/bugreport/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.4.1/mvt/android/modules/bugreport/battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.4.1/mvt/common/cmd_check_iocs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
+import os
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_battery_history
+from mvt.common.command import Command
+from mvt.common.utils import exec_or_profile
 
-from .base import BugReportModule
+log = logging.getLogger(__name__)
 
 
-class BatteryHistory(BugReportModule):
-    """This module extracts records from battery daily updates."""
-
+class CmdCheckIOCS(Command):
     def __init__(
         self,
-        file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
+        ioc_files: Optional[list] = None,
+        module_name: Optional[str] = None,
+        serial: Optional[str] = None,
         module_options: Optional[dict] = None,
-        log: logging.Logger = logging.getLogger(__name__),
-        results: Optional[list] = None,
     ) -> None:
         super().__init__(
-            file_path=file_path,
             target_path=target_path,
             results_path=results_path,
+            ioc_files=ioc_files,
+            module_name=module_name,
+            serial=serial,
             module_options=module_options,
             log=log,
-            results=results,
         )
 
-    def check_indicators(self) -> None:
-        if not self.indicators:
-            return
-
-        for result in self.results:
-            ioc = self.indicators.check_app_id(result["package_name"])
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
-                continue
+        self.name = "check-iocs"
 
     def run(self) -> None:
-        content = self._get_dumpstate_file()
-        if not content:
-            self.log.error(
-                "Unable to find dumpstate file. "
-                "Did you provide a valid bug report archive?"
+        assert self.target_path is not None
+        all_modules = []
+        for entry in self.modules:
+            if entry not in all_modules:
+                all_modules.append(entry)
+
+        log.info("Checking stored results against provided indicators...")
+
+        total_detections = 0
+        for file_name in os.listdir(self.target_path):
+            name_only, _ = os.path.splitext(file_name)
+            file_path = os.path.join(self.target_path, file_name)
+
+            for iocs_module in all_modules:
+                if self.module_name and iocs_module.__name__ != self.module_name:
+                    continue
+
+                if iocs_module().get_slug() != name_only:
+                    continue
+
+                log.info(
+                    'Loading results from "%s" with module %s',
+                    file_name,
+                    iocs_module.__name__,
+                )
+
+                m = iocs_module.from_json(
+                    file_path, log=logging.getLogger(iocs_module.__module__)
+                )
+                if self.iocs.total_ioc_count > 0:
+                    m.indicators = self.iocs
+                    m.indicators.log = m.log
+
+                try:
+                    exec_or_profile("m.check_indicators()", globals(), locals())
+                except NotImplementedError:
+                    continue
+                else:
+                    total_detections += len(m.detected)
+
+        if total_detections > 0:
+            log.warning(
+                "The check of the results produced %d detections!", total_detections
             )
-            return
-
-        lines = []
-        in_history = False
-        for line in content.decode(errors="ignore").splitlines():
-            if line.strip().startswith("Battery History "):
-                lines.append(line)
-                in_history = True
-                continue
-
-            if not in_history:
-                continue
-
-            if line.strip() == "":
-                break
-
-            lines.append(line)
-
-        self.results = parse_dumpsys_battery_history("\n".join(lines))
-
-        self.log.info(
-            "Extracted a total of %d battery history records", len(self.results)
-        )
```

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.4.1/mvt/android/modules/bugreport/dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/getprop.py` & `mvt-2.4.1/mvt/ios/modules/mixed/chrome_history.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from datetime import datetime, timedelta
-from typing import Optional
+import sqlite3
+from typing import Optional, Union
 
-from mvt.android.parsers import parse_getprop
+from mvt.common.utils import convert_chrometime_to_datetime, convert_datetime_to_iso
 
-from .base import BugReportModule
+from ..base import IOSExtraction
 
+CHROME_HISTORY_BACKUP_IDS = [
+    "faf971ce92c3ac508c018dce1bef2a8b8e9838f1",
+]
+# TODO: Confirm Chrome database path.
+CHROME_HISTORY_ROOT_PATHS = [
+    "private/var/mobile/Containers/Data/Application/*/Library/Application Support/Google/Chrome/Default/History",  # pylint: disable=line-too-long
+]
 
-class Getprop(BugReportModule):
-    """This module extracts device properties from getprop command."""
+
+class ChromeHistory(IOSExtraction):
+    """This module extracts all Chome visits."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -29,49 +37,67 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-        self.results = {} if not results else results
+    def serialize(self, record: dict) -> Union[dict, list]:
+        return {
+            "timestamp": record["isodate"],
+            "module": self.__class__.__name__,
+            "event": "visit",
+            "data": f"{record['id']} - {record['url']} "
+            f"(visit ID: {record['visit_id']}, "
+            f"redirect source: {record['redirect_source']})",
+        }
 
-    def run(self) -> None:
-        content = self._get_dumpstate_file()
-        if not content:
-            self.log.error(
-                "Unable to find dumpstate file. "
-                "Did you provide a valid bug report archive?"
-            )
+    def check_indicators(self) -> None:
+        if not self.indicators:
             return
 
-        lines = []
-        in_getprop = False
+        for result in self.results:
+            ioc = self.indicators.check_domain(result["url"])
+            if ioc:
+                result["matched_indicator"] = ioc
+                self.detected.append(result)
+
+    def run(self) -> None:
+        self._find_ios_database(
+            backup_ids=CHROME_HISTORY_BACKUP_IDS, root_paths=CHROME_HISTORY_ROOT_PATHS
+        )
+        self.log.info("Found Chrome history database at path: %s", self.file_path)
+
+        conn = sqlite3.connect(self.file_path)
+        cur = conn.cursor()
+        cur.execute(
+            """
+            SELECT
+                urls.id,
+                urls.url,
+                visits.id,
+                visits.visit_time,
+                visits.from_visit
+            FROM urls
+            JOIN visits ON visits.url = urls.id
+            ORDER BY visits.visit_time;
+        """
+        )
+
+        for item in cur:
+            self.results.append(
+                {
+                    "id": item[0],
+                    "url": item[1],
+                    "visit_id": item[2],
+                    "timestamp": item[3],
+                    "isodate": convert_datetime_to_iso(
+                        convert_chrometime_to_datetime(item[3])
+                    ),
+                    "redirect_source": item[4],
+                }
+            )
 
-        for line in content.decode(errors="ignore").splitlines():
-            if line.strip().startswith("------ SYSTEM PROPERTIES"):
-                in_getprop = True
-                continue
-
-            if not in_getprop:
-                continue
-
-            if line.strip() == "------":
-                break
-
-            lines.append(line)
-
-        self.results = parse_getprop("\n".join(lines))
-
-        # Alert if phone is outdated.
-        for entry in self.results:
-            if entry["name"] == "ro.build.version.security_patch":
-                security_patch = entry["value"]
-                patch_date = datetime.strptime(security_patch, "%Y-%m-%d")
-                if (datetime.now() - patch_date) > timedelta(days=6 * 30):
-                    self.log.warning(
-                        "This phone has not received security updates "
-                        "for more than six months (last update: %s)",
-                        security_patch,
-                    )
+        cur.close()
+        conn.close()
 
-        self.log.info("Extracted %d Android system properties", len(self.results))
+        self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/packages.py` & `mvt-2.4.1/mvt/android/modules/bugreport/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/modules/bugreport/receivers.py` & `mvt-2.4.1/mvt/android/modules/bugreport/receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/parsers/backup.py` & `mvt-2.4.1/mvt/android/parsers/backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/android/parsers/dumpsys.py` & `mvt-2.4.1/mvt/android/parsers/dumpsys.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/cmd_check_iocs.py` & `mvt-2.4.1/mvt/android/modules/androidqf/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,56 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import os
 from typing import Optional
 
-from mvt.common.command import Command
-from mvt.common.utils import exec_or_profile
+from mvt.android.artifacts.settings import Settings as SettingsArtifact
 
-log = logging.getLogger(__name__)
+from .base import AndroidQFModule
 
 
-class CmdCheckIOCS(Command):
+class Settings(SettingsArtifact, AndroidQFModule):
+    """This module analyse setting files"""
+
     def __init__(
         self,
+        file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        ioc_files: Optional[list] = None,
-        module_name: Optional[str] = None,
-        serial: Optional[str] = None,
         module_options: Optional[dict] = None,
+        log: logging.Logger = logging.getLogger(__name__),
+        results: Optional[list] = None,
     ) -> None:
         super().__init__(
+            file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            ioc_files=ioc_files,
-            module_name=module_name,
-            serial=serial,
             module_options=module_options,
             log=log,
+            results=results,
         )
-
-        self.name = "check-iocs"
+        self.results = {}
 
     def run(self) -> None:
-        assert self.target_path is not None
-        all_modules = []
-        for entry in self.modules:
-            if entry not in all_modules:
-                all_modules.append(entry)
-
-        log.info("Checking stored results against provided indicators...")
-
-        total_detections = 0
-        for file_name in os.listdir(self.target_path):
-            name_only, _ = os.path.splitext(file_name)
-            file_path = os.path.join(self.target_path, file_name)
-
-            for iocs_module in all_modules:
-                if self.module_name and iocs_module.__name__ != self.module_name:
-                    continue
+        for setting_file in self._get_files_by_pattern("*/settings_*.txt"):
+            namespace = setting_file[setting_file.rfind("_") + 1 : -4]
 
-                if iocs_module().get_slug() != name_only:
+            self.results[namespace] = {}
+            data = self._get_file_content(setting_file)
+            for line in data.decode("utf-8").split("\n"):
+                line = line.strip()
+                try:
+                    key, value = line.split("=", 1)
+                except ValueError:
                     continue
 
-                log.info(
-                    'Loading results from "%s" with module %s',
-                    file_name,
-                    iocs_module.__name__,
-                )
-
-                m = iocs_module.from_json(
-                    file_path, log=logging.getLogger(iocs_module.__module__)
-                )
-                if self.iocs.total_ioc_count > 0:
-                    m.indicators = self.iocs
-                    m.indicators.log = m.log
-
                 try:
-                    exec_or_profile("m.check_indicators()", globals(), locals())
-                except NotImplementedError:
+                    self.results[namespace][key] = value
+                except IndexError:
                     continue
-                else:
-                    total_detections += len(m.detected)
 
-        if total_detections > 0:
-            log.warning(
-                "The check of the results produced %d detections!", total_detections
-            )
+        self.log.info(
+            "Identified %d settings", sum([len(val) for val in self.results.values()])
+        )
```

### Comparing `mvt-2.4.0/mvt/common/command.py` & `mvt-2.4.1/mvt/common/command.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/help.py` & `mvt-2.4.1/mvt/common/help.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,12 +5,14 @@
 
 # Help messages of repeating options.
 HELP_MSG_OUTPUT = "Specify a path to a folder where you want to store JSON results"
 HELP_MSG_IOC = "Path to indicators file (can be invoked multiple time)"
 HELP_MSG_FAST = "Avoid running time/resource consuming features"
 HELP_MSG_LIST_MODULES = "Print list of available modules and exit"
 HELP_MSG_MODULE = "Name of a single module you would like to run instead of all"
+HELP_MSG_NONINTERACTIVE = "Don't ask interactive questions during processing"
+HELP_MSG_ANDROID_BACKUP_PASSWORD = "The backup password to use for an Android backup"
 HELP_MSG_HASHES = "Generate hashes of all the files analyzed"
 HELP_MSG_VERBOSE = "Verbose mode"
 
 # Android-specific.
 HELP_MSG_SERIAL = "Specify a device serial number or HOST:PORT connection string"
```

### Comparing `mvt-2.4.0/mvt/common/indicators.py` & `mvt-2.4.1/mvt/common/indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             # got from the relationship.
             for collection in collections:
                 if collection["id"] == malware_id:
                     self._process_indicator(indicator, collection)
                     break
 
         for coll in collections:
-            self.log.info(
+            self.log.debug(
                 'Extracted %d indicators for collection with name "%s"',
                 coll["count"],
                 coll["name"],
             )
 
         self.ioc_collections.extend(collections)
```

### Comparing `mvt-2.4.0/mvt/common/logo.py` & `mvt-2.4.1/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/module.py` & `mvt-2.4.1/mvt/common/module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/options.py` & `mvt-2.4.1/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/updates.py` & `mvt-2.4.1/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/url.py` & `mvt-2.4.1/mvt/common/url.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/utils.py` & `mvt-2.4.1/mvt/common/utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/common/virustotal.py` & `mvt-2.4.1/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/cli.py` & `mvt-2.4.1/mvt/ios/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/cmd_check_backup.py` & `mvt-2.4.1/mvt/ios/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/cmd_check_fs.py` & `mvt-2.4.1/mvt/android/modules/adb/processes.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from mvt.common.command import Command
+from mvt.android.artifacts.processes import Processes as ProcessesArtifact
 
-from .modules.fs import FS_MODULES
-from .modules.mixed import MIXED_MODULES
+from .base import AndroidExtraction
 
-log = logging.getLogger(__name__)
 
+class Processes(ProcessesArtifact, AndroidExtraction):
+    """This module extracts details on running processes."""
 
-class CmdIOSCheckFS(Command):
     def __init__(
         self,
+        file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        ioc_files: Optional[list] = None,
-        module_name: Optional[str] = None,
-        serial: Optional[str] = None,
         module_options: Optional[dict] = None,
-        hashes: bool = False,
+        log: logging.Logger = logging.getLogger(__name__),
+        results: Optional[list] = None,
     ) -> None:
         super().__init__(
+            file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            ioc_files=ioc_files,
-            module_name=module_name,
-            serial=serial,
             module_options=module_options,
-            hashes=hashes,
             log=log,
+            results=results,
         )
 
-        self.name = "check-fs"
-        self.modules = FS_MODULES + MIXED_MODULES
+    def run(self) -> None:
+        self._adb_connect()
 
-    def module_init(self, module):
-        module.is_fs_dump = True
+        output = self._adb_command("ps -A")
+        self.parse(output)
+        self._adb_disconnect()
+
+        self.log.info("Extracted records on a total of %d processes", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/ios/data/ios_models.json` & `mvt-2.4.1/mvt/ios/data/ios_models.json`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/data/ios_versions.json` & `mvt-2.4.1/mvt/ios/data/ios_versions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9914529914529915%*

 * *Differences: {'insert': "[(218, OrderedDict([('version', '15.7.8'), ('build', '19H364')])), (233, "*

 * *           "OrderedDict([('version', '16.6'), ('build', '20G75')]))]"}*

```diff
@@ -868,14 +868,18 @@
         "version": "15.7.6"
     },
     {
         "build": "19H357",
         "version": "15.7.7"
     },
     {
+        "build": "19H364",
+        "version": "15.7.8"
+    },
+    {
         "build": "20A362",
         "version": "16.0"
     },
     {
         "build": "20A371",
         "version": "16.0.1"
     },
@@ -923,9 +927,13 @@
         "beta": null,
         "build": "20F66",
         "version": "16.5"
     },
     {
         "build": "20F75",
         "version": "16.5.1"
+    },
+    {
+        "build": "20G75",
+        "version": "16.6"
     }
 ]
```

### Comparing `mvt-2.4.0/mvt/ios/decrypt.py` & `mvt-2.4.1/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/backup/backup_info.py` & `mvt-2.4.1/mvt/ios/modules/backup/backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.4.1/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/backup/manifest.py` & `mvt-2.4.1/mvt/ios/modules/backup/manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/backup/profile_events.py` & `mvt-2.4.1/mvt/ios/modules/backup/profile_events.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/base.py` & `mvt-2.4.1/mvt/ios/modules/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/__init__.py` & `mvt-2.4.1/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/analytics.py` & `mvt-2.4.1/mvt/ios/modules/fs/analytics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.4.1/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/cache_files.py` & `mvt-2.4.1/mvt/ios/modules/fs/cache_files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/filesystem.py` & `mvt-2.4.1/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import os
+import plistlib
 from typing import Optional, Union
 
-from mvt.common.utils import convert_unix_to_iso
+from mvt.common.utils import convert_datetime_to_iso
 
 from ..base import IOSExtraction
 
+OSANALYTICS_ADDAILY_BACKUP_IDS = [
+    "f65b5fafc69bbd3c60be019c6e938e146825fa83",
+]
+OSANALYTICS_ADDAILY_ROOT_PATHS = [
+    "private/var/mobile/Library/Preferences/com.apple.osanalytics.addaily.plist",
+]
 
-class Filesystem(IOSExtraction):
-    """This module extracts creation and modification date of files from a
-    full file-system dump.
-    """
+
+class OSAnalyticsADDaily(IOSExtraction):
+    """Extract network usage information by process,
+    from com.apple.osanalytics.addaily.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -33,60 +39,54 @@
             module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
-            "timestamp": record["modified"],
+            "timestamp": record["ts"],
             "module": self.__class__.__name__,
-            "event": "entry_modified",
-            "data": record["path"],
+            "event": "osanalytics_addaily",
+            "data": f"{record['package']} WIFI IN: {record['wifi_in']}, "
+            f"WIFI OUT: {record['wifi_out']} - "
+            f"WWAN IN: {record['wwan_in']}, "
+            f"WWAN OUT: {record['wwan_out']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            if "path" not in result:
-                continue
-
-            ioc = self.indicators.check_file_path(result["path"])
+            ioc = self.indicators.check_process(result["package"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
-            # If we are instructed to run fast, we skip the rest.
-            if self.module_options.get("fast_mode", None):
-                continue
+    def run(self) -> None:
+        self._find_ios_database(
+            backup_ids=OSANALYTICS_ADDAILY_BACKUP_IDS,
+            root_paths=OSANALYTICS_ADDAILY_ROOT_PATHS,
+        )
+        self.log.info(
+            "Found com.apple.osanalytics.addaily plist at path: %s", self.file_path
+        )
 
-            ioc = self.indicators.check_file_path_process(result["path"])
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+        with open(self.file_path, "rb") as handle:
+            file_plist = plistlib.load(handle)
 
-    def run(self) -> None:
-        for root, dirs, files in os.walk(self.target_path):
-            for dir_name in dirs:
-                try:
-                    dir_path = os.path.join(root, dir_name)
-                    result = {
-                        "path": os.path.relpath(dir_path, self.target_path),
-                        "modified": convert_unix_to_iso(os.stat(dir_path).st_mtime),
-                    }
-                except Exception:
-                    continue
-                else:
-                    self.results.append(result)
-
-            for file_name in files:
-                try:
-                    file_path = os.path.join(root, file_name)
-                    result = {
-                        "path": os.path.relpath(file_path, self.target_path),
-                        "modified": convert_unix_to_iso(os.stat(file_path).st_mtime),
-                    }
-                except Exception:
-                    continue
-                else:
-                    self.results.append(result)
+        for app, values in file_plist.get("netUsageBaseline", {}).items():
+            self.results.append(
+                {
+                    "package": app,
+                    "ts": convert_datetime_to_iso(values[0]),
+                    "wifi_in": values[1],
+                    "wifi_out": values[2],
+                    "wwan_in": values[3],
+                    "wwan_out": values[4],
+                }
+            )
+
+        self.log.info(
+            "Extracted a total of %d com.apple.osanalytics.addaily entries",
+            len(self.results),
+        )
```

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.4.1/mvt/ios/modules/fs/net_netusage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.4.1/mvt/ios/modules/fs/safari_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.4.1/mvt/ios/modules/fs/shutdownlog.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/version_history.py` & `mvt-2.4.1/mvt/ios/modules/fs/version_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.4.1/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.4.1/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.4.1/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional, Union
+from typing import Optional
 
 from .webkit_base import WebkitBase
 
-WEBKIT_LOCALSTORAGE_ROOT_PATHS = [
-    "private/var/mobile/Containers/Data/Application/*/Library/WebKit/WebsiteData/LocalStorage/",
+WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS = [
+    "private/var/mobile/Containers/Data/Application/*/SystemData/com.apple.SafariViewService/Library/WebKit/WebsiteData/",  # pylint: disable=line-too-long
 ]
 
 
-class WebkitLocalStorage(WebkitBase):
+class WebkitSafariViewService(WebkitBase):
     """This module looks extracts records from WebKit LocalStorage folders,
     and checks them against any provided list of suspicious domains.
 
 
     """
 
     def __init__(
@@ -34,22 +34,13 @@
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
 
-    def serialize(self, record: dict) -> Union[dict, list]:
-        return {
-            "timestamp": record["isodate"],
-            "module": self.__class__.__name__,
-            "event": "webkit_local_storage",
-            "data": f"WebKit Local Storage folder {record['folder']} "
-            f"containing file for URL {record['url']}",
-        }
-
     def run(self) -> None:
-        self._process_webkit_folder(WEBKIT_LOCALSTORAGE_ROOT_PATHS)
+        self._process_webkit_folder(WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS)
         self.log.info(
-            "Extracted a total of %d records from WebKit Local Storages",
+            "Extracted a total of %d records from WebKit SafariViewService WebsiteData",
             len(self.results),
         )
```

### Comparing `mvt-2.4.0/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.4.1/mvt/android/modules/androidqf/getprop.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from .webkit_base import WebkitBase
+from mvt.android.artifacts.getprop import GetProp as GetPropArtifact
 
-WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS = [
-    "private/var/mobile/Containers/Data/Application/*/SystemData/com.apple.SafariViewService/Library/WebKit/WebsiteData/",  # pylint: disable=line-too-long
-]
+from .base import AndroidQFModule
 
 
-class WebkitSafariViewService(WebkitBase):
-    """This module looks extracts records from WebKit LocalStorage folders,
-    and checks them against any provided list of suspicious domains.
-
-
-    """
+class Getprop(GetPropArtifact, AndroidQFModule):
+    """This module extracts data from get properties."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -33,14 +27,19 @@
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
             module_options=module_options,
             log=log,
             results=results,
         )
+        self.results = []
 
     def run(self) -> None:
-        self._process_webkit_folder(WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS)
-        self.log.info(
-            "Extracted a total of %d records from WebKit SafariViewService WebsiteData",
-            len(self.results),
-        )
+        getprop_files = self._get_files_by_pattern("*/getprop.txt")
+        if not getprop_files:
+            self.log.info("getprop.txt file not found")
+            return
+
+        data = self._get_file_content(getprop_files[0]).decode("utf-8")
+
+        self.parse(data)
+        self.log.info("Extracted a total of %d properties", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/__init__.py` & `mvt-2.4.1/mvt/ios/modules/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/applications.py` & `mvt-2.4.1/mvt/ios/modules/mixed/applications.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/calendar.py` & `mvt-2.4.1/mvt/ios/modules/mixed/calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/calls.py` & `mvt-2.4.1/mvt/ios/modules/mixed/calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import sqlite3
-from typing import Union, Optional
+from typing import Optional, Union
 
 from mvt.common.utils import convert_mactime_to_iso
 
 from ..base import IOSExtraction
 
 CALLS_BACKUP_IDS = [
     "5a4935c78a5255723f707230a451d79c540d2741",
```

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.4.1/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.4.1/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import sqlite3
 from typing import Optional, Union
 
-from mvt.common.utils import convert_chrometime_to_datetime, convert_datetime_to_iso
+from mvt.common.utils import convert_unix_to_iso
 
 from ..base import IOSExtraction
 
-CHROME_HISTORY_BACKUP_IDS = [
-    "faf971ce92c3ac508c018dce1bef2a8b8e9838f1",
+FIREFOX_HISTORY_BACKUP_IDS = [
+    "2e57c396a35b0d1bcbc624725002d98bd61d142b",
 ]
-# TODO: Confirm Chrome database path.
-CHROME_HISTORY_ROOT_PATHS = [
-    "private/var/mobile/Containers/Data/Application/*/Library/Application Support/Google/Chrome/Default/History",  # pylint: disable=line-too-long
+FIREFOX_HISTORY_ROOT_PATHS = [
+    "private/var/mobile/profile.profile/browser.db",
 ]
 
 
-class ChromeHistory(IOSExtraction):
-    """This module extracts all Chome visits."""
+class FirefoxFavicon(IOSExtraction):
+    """This module extracts all Firefox favicon"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -41,63 +40,68 @@
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
-            "event": "visit",
-            "data": f"{record['id']} - {record['url']} "
-            f"(visit ID: {record['visit_id']}, "
-            f"redirect source: {record['redirect_source']})",
+            "event": "firefox_history",
+            "data": f"Firefox favicon {record['url']} "
+            f"when visiting {record['history_url']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            ioc = self.indicators.check_domain(result["url"])
+            ioc = self.indicators.check_domain(result.get("url", ""))
+            if not ioc:
+                ioc = self.indicators.check_domain(result.get("history_url", ""))
+
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
         self._find_ios_database(
-            backup_ids=CHROME_HISTORY_BACKUP_IDS, root_paths=CHROME_HISTORY_ROOT_PATHS
+            backup_ids=FIREFOX_HISTORY_BACKUP_IDS, root_paths=FIREFOX_HISTORY_ROOT_PATHS
         )
-        self.log.info("Found Chrome history database at path: %s", self.file_path)
+        self.log.info("Found Firefox favicon database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
         cur.execute(
             """
             SELECT
-                urls.id,
-                urls.url,
-                visits.id,
-                visits.visit_time,
-                visits.from_visit
-            FROM urls
-            JOIN visits ON visits.url = urls.id
-            ORDER BY visits.visit_time;
+                favicons.id,
+                favicons.url,
+                favicons.width,
+                favicons.height,
+                favicons.type,
+                favicons.date,
+                history.id,
+                history.url
+            FROM favicons
+            INNER JOIN favicon_sites ON favicon_sites.faviconID = favicons.id
+            INNER JOIN history ON favicon_sites.siteID = history.id;
         """
         )
 
         for item in cur:
             self.results.append(
                 {
                     "id": item[0],
                     "url": item[1],
-                    "visit_id": item[2],
-                    "timestamp": item[3],
-                    "isodate": convert_datetime_to_iso(
-                        convert_chrometime_to_datetime(item[3])
-                    ),
-                    "redirect_source": item[4],
+                    "width": item[2],
+                    "height": item[3],
+                    "type": item[4],
+                    "isodate": convert_unix_to_iso(item[5]),
+                    "history_id": item[6],
+                    "history_url": item[7],
                 }
             )
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/contacts.py` & `mvt-2.4.1/mvt/ios/modules/mixed/contacts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.4.1/mvt/ios/modules/mixed/firefox_history.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,16 +15,20 @@
     "2e57c396a35b0d1bcbc624725002d98bd61d142b",
 ]
 FIREFOX_HISTORY_ROOT_PATHS = [
     "private/var/mobile/profile.profile/browser.db",
 ]
 
 
-class FirefoxFavicon(IOSExtraction):
-    """This module extracts all Firefox favicon"""
+class FirefoxHistory(IOSExtraction):
+    """This module extracts all Firefox visits and tries to detect potential
+    network injection attacks.
+
+
+    """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         module_options: Optional[dict] = None,
@@ -41,67 +45,58 @@
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
             "module": self.__class__.__name__,
             "event": "firefox_history",
-            "data": f"Firefox favicon {record['url']} "
-            f"when visiting {record['history_url']}",
+            "data": f"Firefox visit with ID {record['id']} to URL: {record['url']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            ioc = self.indicators.check_domain(result.get("url", ""))
-            if not ioc:
-                ioc = self.indicators.check_domain(result.get("history_url", ""))
-
+            ioc = self.indicators.check_domain(result["url"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def run(self) -> None:
         self._find_ios_database(
             backup_ids=FIREFOX_HISTORY_BACKUP_IDS, root_paths=FIREFOX_HISTORY_ROOT_PATHS
         )
-        self.log.info("Found Firefox favicon database at path: %s", self.file_path)
+        self.log.info("Found Firefox history database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
         cur.execute(
             """
             SELECT
-                favicons.id,
-                favicons.url,
-                favicons.width,
-                favicons.height,
-                favicons.type,
-                favicons.date,
-                history.id,
-                history.url
-            FROM favicons
-            INNER JOIN favicon_sites ON favicon_sites.faviconID = favicons.id
-            INNER JOIN history ON favicon_sites.siteID = history.id;
+                visits.id,
+                visits.date/1000000,
+                history.url,
+                history.title,
+                visits.is_local,
+                visits.type
+            FROM visits, history
+            WHERE visits.siteID = history.id;
         """
         )
 
-        for item in cur:
+        for row in cur:
             self.results.append(
                 {
-                    "id": item[0],
-                    "url": item[1],
-                    "width": item[2],
-                    "height": item[3],
-                    "type": item[4],
-                    "isodate": convert_unix_to_iso(item[5]),
-                    "history_id": item[6],
-                    "history_url": item[7],
+                    "id": row[0],
+                    "isodate": convert_unix_to_iso(row[1]),
+                    "url": row[2],
+                    "title": row[3],
+                    "i1000000s_local": row[4],
+                    "type": row[5],
                 }
             )
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d history items", len(self.results))
```

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.4.1/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.4.1/mvt/ios/modules/mixed/interactionc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/locationd.py` & `mvt-2.4.1/mvt/ios/modules/mixed/locationd.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.4.1/mvt/ios/modules/mixed/net_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.4.1/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.4.1/mvt/ios/modules/mixed/safari_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.4.1/mvt/ios/modules/mixed/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/sms.py` & `mvt-2.4.1/mvt/ios/modules/mixed/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.4.1/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/tcc.py` & `mvt-2.4.1/mvt/ios/modules/mixed/tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.4.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.4.1/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.4.1/mvt/ios/modules/mixed/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/modules/net_base.py` & `mvt-2.4.1/mvt/ios/modules/net_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt/ios/versions.py` & `mvt-2.4.1/mvt/ios/versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/mvt.egg-info/PKG-INFO` & `mvt-2.4.1/mvt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.4.0
+Version: 2.4.1
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.4.0/mvt.egg-info/SOURCES.txt` & `mvt-2.4.1/mvt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 ./mvt/android/__init__.py
 ./mvt/android/cli.py
 ./mvt/android/cmd_check_adb.py
 ./mvt/android/cmd_check_androidqf.py
 ./mvt/android/cmd_check_backup.py
 ./mvt/android/cmd_check_bugreport.py
 ./mvt/android/cmd_download_apks.py
+./mvt/android/utils.py
+./mvt/android/artifacts/__init__.py
+./mvt/android/artifacts/artifact.py
+./mvt/android/artifacts/getprop.py
+./mvt/android/artifacts/processes.py
+./mvt/android/artifacts/settings.py
 ./mvt/android/modules/__init__.py
 ./mvt/android/modules/adb/__init__.py
 ./mvt/android/modules/adb/base.py
 ./mvt/android/modules/adb/chrome_history.py
 ./mvt/android/modules/adb/dumpsys_accessibility.py
 ./mvt/android/modules/adb/dumpsys_activities.py
 ./mvt/android/modules/adb/dumpsys_appops.py
@@ -47,14 +53,15 @@
 ./mvt/android/modules/androidqf/dumpsys_receivers.py
 ./mvt/android/modules/androidqf/getprop.py
 ./mvt/android/modules/androidqf/processes.py
 ./mvt/android/modules/androidqf/settings.py
 ./mvt/android/modules/androidqf/sms.py
 ./mvt/android/modules/backup/__init__.py
 ./mvt/android/modules/backup/base.py
+./mvt/android/modules/backup/helpers.py
 ./mvt/android/modules/backup/sms.py
 ./mvt/android/modules/bugreport/__init__.py
 ./mvt/android/modules/bugreport/accessibility.py
 ./mvt/android/modules/bugreport/activities.py
 ./mvt/android/modules/bugreport/appops.py
 ./mvt/android/modules/bugreport/base.py
 ./mvt/android/modules/bugreport/battery_daily.py
@@ -62,16 +69,16 @@
 ./mvt/android/modules/bugreport/dbinfo.py
 ./mvt/android/modules/bugreport/getprop.py
 ./mvt/android/modules/bugreport/packages.py
 ./mvt/android/modules/bugreport/receivers.py
 ./mvt/android/parsers/__init__.py
 ./mvt/android/parsers/backup.py
 ./mvt/android/parsers/dumpsys.py
-./mvt/android/parsers/getprop.py
 ./mvt/common/__init__.py
+./mvt/common/artifact.py
 ./mvt/common/cmd_check_iocs.py
 ./mvt/common/command.py
 ./mvt/common/help.py
 ./mvt/common/indicators.py
 ./mvt/common/logo.py
 ./mvt/common/module.py
 ./mvt/common/options.py
@@ -131,19 +138,22 @@
 ./mvt/ios/modules/mixed/tcc.py
 ./mvt/ios/modules/mixed/webkit_resource_load_statistics.py
 ./mvt/ios/modules/mixed/webkit_session_resource_log.py
 ./mvt/ios/modules/mixed/whatsapp.py
 ./tests/__init__.py
 ./tests/conftest.py
 ./tests/test_check_android_androidqf.py
+./tests/test_check_android_backup.py
 ./tests/test_check_android_bugreport.py
 ./tests/test_check_ios_backup.py
 ./tests/test_ios_versions.py
 ./tests/utils.py
 ./tests/android/__init__.py
+./tests/android/test_artifact_getprop.py
+./tests/android/test_artifact_processes.py
 ./tests/android/test_backup_module.py
 ./tests/android/test_backup_parser.py
 ./tests/android/test_dumpsys_parser.py
 ./tests/android_androidqf/__init__.py
 ./tests/android_androidqf/test_dumpsysaccessbility.py
 ./tests/android_androidqf/test_dumpsysappops.py
 ./tests/android_androidqf/test_dumpsyspackages.py
@@ -163,12 +173,8 @@
 ./tests/ios_backup/test_datausage.py
 ./tests/ios_backup/test_manifest.py
 ./tests/ios_backup/test_safari_browserstate.py
 ./tests/ios_backup/test_sms.py
 ./tests/ios_backup/test_tcc.py
 ./tests/ios_backup/test_webkit_resource_load_statistics.py
 ./tests/ios_fs/__init__.py
-./tests/ios_fs/test_filesystem.py
-tests/test_check_android_androidqf.py
-tests/test_check_android_bugreport.py
-tests/test_check_ios_backup.py
-tests/test_ios_versions.py
+./tests/ios_fs/test_filesystem.py
```

### Comparing `mvt-2.4.0/setup.cfg` & `mvt-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/android/test_backup_module.py` & `mvt-2.4.1/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/android/test_backup_parser.py` & `mvt-2.4.1/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/android/test_dumpsys_parser.py` & `mvt-2.4.1/tests/android/test_dumpsys_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.4.1/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
-from mvt.android.modules.androidqf.dumpsys_appops import DumpsysAppops
+from pathlib import Path
+
+from mvt.android.modules.androidqf.dumpsys_accessibility import DumpsysAccessibility
 from mvt.common.module import run_module
 
-from ..utils import get_android_androidqf
+from ..utils import get_android_androidqf, list_files
 
 
-class TestDumpsysAppOpsModule:
+class TestDumpsysAccessibilityModule:
     def test_parsing(self):
         data_path = get_android_androidqf()
-        m = DumpsysAppops(target_path=data_path)
+        m = DumpsysAccessibility(target_path=data_path)
+        files = list_files(data_path)
+        parent_path = Path(data_path).absolute().parent.as_posix()
+        m.from_folder(parent_path, files)
         run_module(m)
-        assert len(m.results) == 12
-        assert len(m.timeline) == 16
+        assert len(m.results) == 4
         assert len(m.detected) == 0
```

### Comparing `mvt-2.4.0/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.4.1/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
+from pathlib import Path
 
 from mvt.android.modules.androidqf.dumpsys_packages import DumpsysPackages
 from mvt.common.indicators import Indicators
 from mvt.common.module import run_module
 
-from ..utils import get_android_androidqf
+from ..utils import get_android_androidqf, list_files
 
 
 class TestDumpsysPackagesModule:
     def test_parsing(self):
         data_path = get_android_androidqf()
         m = DumpsysPackages(target_path=data_path)
+        files = list_files(data_path)
+        parent_path = Path(data_path).absolute().parent.as_posix()
+        m.from_folder(parent_path, files)
         run_module(m)
         assert len(m.results) == 2
         assert len(m.detected) == 0
         assert len(m.timeline) == 6
         assert (
             m.results[0]["package_name"]
             == "com.samsung.android.provider.filterprovider"
         )
 
     def test_detection_pkgname(self, indicator_file):
         data_path = get_android_androidqf()
         m = DumpsysPackages(target_path=data_path)
+        files = list_files(data_path)
+        parent_path = Path(data_path).absolute().parent.as_posix()
+        m.from_folder(parent_path, files)
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         ind.ioc_collections[0]["app_ids"].append("com.sec.android.app.DataCreate")
         m.indicators = ind
         run_module(m)
         assert len(m.results) == 2
         assert len(m.detected) == 1
```

### Comparing `mvt-2.4.0/tests/android_androidqf/test_getprop.py` & `mvt-2.4.1/tests/ios_fs/test_filesystem.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import os
 
-from mvt.android.modules.androidqf.getprop import Getprop
 from mvt.common.indicators import Indicators
 from mvt.common.module import run_module
+from mvt.ios.modules.fs.filesystem import Filesystem
 
-from ..utils import get_artifact_folder
+from ..utils import get_ios_backup_folder
 
 
-class TestAndroidqfGetpropAnalysis:
-    def test_androidqf_getprop(self):
-        m = Getprop(
-            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
-        )
+class TestFilesystem:
+    def test_filesystem(self):
+        m = Filesystem(target_path=get_ios_backup_folder())
         run_module(m)
-        assert len(m.results) == 10
-        assert m.results[0]["name"] == "dalvik.vm.appimageformat"
-        assert m.results[0]["value"] == "lz4"
-        assert len(m.timeline) == 0
+        assert len(m.results) == 14
+        assert len(m.timeline) == 14
         assert len(m.detected) == 0
 
-    def test_androidqf_getprop_detection(self, indicator_file):
-        m = Getprop(
-            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
-        )
+    def test_detection(self, indicator_file):
+        m = Filesystem(target_path=get_ios_backup_folder())
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
-        ind.ioc_collections[0]["android_property_names"].append("dalvik.vm.heapmaxfree")
+        # Adds a filename that exist in the folder
+        ind.ioc_collections[0]["processes"].append(
+            "64d0019cb3d46bfc8cce545a8ba54b93e7ea9347"
+        )
         m.indicators = ind
         run_module(m)
-        assert len(m.results) == 10
+        assert len(m.results) == 14
+        assert len(m.timeline) == 14
         assert len(m.detected) == 1
-        assert m.detected[0]["name"] == "dalvik.vm.heapmaxfree"
```

### Comparing `mvt-2.4.0/tests/android_androidqf/test_processes.py` & `mvt-2.4.1/tests/android_androidqf/test_processes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import os
+from pathlib import Path
 
 from mvt.android.modules.androidqf.processes import Processes
 from mvt.common.module import run_module
 
-from ..utils import get_artifact_folder
+from ..utils import get_android_androidqf, list_files
 
 
 class TestAndroidqfProcessesAnalysis:
     def test_androidqf_processes(self):
-        m = Processes(
-            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
-        )
+        data_path = get_android_androidqf()
+        m = Processes(target_path=data_path, log=logging)
+        files = list_files(data_path)
+        parent_path = Path(data_path).absolute().parent.as_posix()
+        m.from_folder(parent_path, files)
         run_module(m)
         assert len(m.results) == 15
         assert len(m.timeline) == 0
         assert len(m.detected) == 0
```

### Comparing `mvt-2.4.0/tests/android_androidqf/test_sms.py` & `mvt-2.4.1/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
-import logging
-import os
+from pathlib import Path
 
-from mvt.android.modules.androidqf.sms import SMS
+from mvt.android.modules.androidqf.dumpsys_receivers import DumpsysReceivers
 from mvt.common.module import run_module
 
-from ..utils import get_artifact_folder
+from ..utils import get_android_androidqf, list_files
 
 
-class TestAndroidqfSMSAnalysis:
-    def test_androidqf_sms(self):
-        m = SMS(
-            target_path=os.path.join(get_artifact_folder(), "androidqf"), log=logging
-        )
+class TestDumpsysReceiversModule:
+    def test_parsing(self):
+        data_path = get_android_androidqf()
+        m = DumpsysReceivers(target_path=data_path)
+        files = list_files(data_path)
+        parent_path = Path(data_path).absolute().parent.as_posix()
+        m.from_folder(parent_path, files)
         run_module(m)
-        assert len(m.results) == 2
-        assert len(m.timeline) == 0
+        assert len(m.results) == 4
         assert len(m.detected) == 0
```

### Comparing `mvt-2.4.0/tests/android_bugreport/test_bugreport.py` & `mvt-2.4.1/tests/android_bugreport/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/common/test_indicators.py` & `mvt-2.4.1/tests/common/test_indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/common/test_utils.py` & `mvt-2.4.1/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/conftest.py` & `mvt-2.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_backup_info.py` & `mvt-2.4.1/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_calendar.py` & `mvt-2.4.1/tests/ios_backup/test_calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_datausage.py` & `mvt-2.4.1/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_manifest.py` & `mvt-2.4.1/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.4.1/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_sms.py` & `mvt-2.4.1/tests/ios_backup/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_tcc.py` & `mvt-2.4.1/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.4.1/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/test_check_android_bugreport.py` & `mvt-2.4.1/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/test_check_ios_backup.py` & `mvt-2.4.1/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.4.0/tests/utils.py` & `mvt-2.4.1/tests/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import os
+from pathlib import Path
 
 
 def get_artifact(fname):
     """
     Return the artifact path in the artifact folder
     """
     fpath = os.path.join(get_artifact_folder(), fname)
@@ -30,7 +31,19 @@
 
 def get_android_androidqf():
     return os.path.join(os.path.dirname(__file__), "artifacts", "androidqf")
 
 
 def get_indicator_file():
     print("PYTEST env", os.getenv("PYTEST_CURRENT_TEST"))
+
+
+def list_files(path: str):
+    files = []
+    parent_path = Path(path).absolute().parent.as_posix()
+    target_abs_path = os.path.abspath(path)
+    for root, subdirs, subfiles in os.walk(target_abs_path):
+        for fname in subfiles:
+            file_path = os.path.relpath(os.path.join(root, fname), parent_path)
+            files.append(file_path)
+
+    return files
```

