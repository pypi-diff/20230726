# Comparing `tmp/remotemanager-0.9.4.tar.gz` & `tmp/remotemanager-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.4.tar", last modified: Tue Jul 25 13:05:14 2023, max compression
+gzip compressed data, was "remotemanager-0.9.5.tar", last modified: Wed Jul 26 10:32:40 2023, max compression
```

## Comparing `remotemanager-0.9.4.tar` & `remotemanager-0.9.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-25 13:05:14.306562 remotemanager-0.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-25 12:11:06.000000 remotemanager-0.9.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.4/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.4/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.4/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.4/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    54208 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10077 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.4/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    22571 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:05.000000 remotemanager-0.9.4/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.4/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.4/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.4/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.4/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.4/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.4/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.4/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.4/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.4/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.4/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.4/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.4/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:05:14.306562 remotemanager-0.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-26 10:32:40.943266 remotemanager-0.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-25 14:08:53.000000 remotemanager-0.9.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.935266 remotemanager-0.9.5/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-25 14:08:53.000000 remotemanager-0.9.5/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.5/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.5/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.5/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.5/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    54656 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.5/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    23093 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:05.000000 remotemanager-0.9.5/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.5/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.5/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.5/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.5/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.5/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.5/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.5/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.5/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.5/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.5/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.5/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.5/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.935266 remotemanager-0.9.5/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 10:32:40.943266 remotemanager-0.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.5/setup.py
```

### Comparing `remotemanager-0.9.4/LICENSE` & `remotemanager-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/PKG-INFO` & `remotemanager-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.4
+Version: 0.9.5
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.4/README.md` & `remotemanager-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/pyproject.toml` & `remotemanager-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.4"
+current_version = "0.9.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.4/remotemanager/connection/cmd.py` & `remotemanager-0.9.5/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/computers/base.py` & `remotemanager-0.9.5/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/computers/example.py` & `remotemanager-0.9.5/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/computers/options.py` & `remotemanager-0.9.5/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.5/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/testing_object.py` & `remotemanager-0.9.5/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/connection/url.py` & `remotemanager-0.9.5/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/dataset/dataset.py` & `remotemanager-0.9.5/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             optional name for this dataset. Will be used for runscripts
         extra_files_send(list, str):
             extra files to send with this run
         extra_files_recv(list, str):
             extra files to retrieve with this run
         skip (bool):
             skip dataset creation if possible. Defaults True
+        extra:
+            extra text to insert into the runner jobscripts
         global_run_args:
             any further (unchanging) arguments to be passed to the runner(s)
     """
 
     _do_not_package = ["_database"]
 
     # DEV NOTE: arguments must be None for computer-url override to function
@@ -71,14 +73,15 @@
         name: str = None,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         verbose: int = None,
         add_newline: bool = True,
         block_reinit: bool = None,
         skip: bool = True,
+        extra: str = None,
         **global_run_args,
     ):
         self._verbose = Verbosity(verbose)
 
         self._logger.info("dataset initialised")
 
         self._function = Function(function)
@@ -87,14 +90,15 @@
         if " " in global_run_args.get("remote_dir", ""):
             raise ValueError(f"Space character detected in remote_dir")
         if " " in global_run_args.get("run_dir", ""):
             raise ValueError(f"Space character detected in run_dir")
         if " " in os.path.abspath(global_run_args.get("local_dir", "")):
             raise ValueError(f"Space character detected in local_dir")
         self._global_run_args.update(global_run_args)
+        self._global_run_extra = extra
 
         # dataset uuid is equal to Function uuid for now
         self._name = name or "dataset"
         self._uuid = generate_uuid(self._function.uuid + self.name)
         self._logger.info(f"uuid is {self.uuid}")
 
         self._script = script or ""
@@ -469,14 +473,15 @@
         dependency_call: bool = False,
         verbose: int = None,
         quiet: bool = False,
         skip: bool = True,
         force: bool = False,
         lazy: bool = False,
         chain_run_args: bool = True,
+        extra: str = None,
         **run_args,
     ):
         """
         Serialise arguments for later runner construction
 
         Args:
             args (dict):
@@ -527,22 +532,22 @@
                 extra_files_recv=extra_files_recv,  # noqa: E251
                 verbose=verbose,
                 quiet=quiet,
                 skip=skip,
                 force=force,
                 lazy=lazy,
                 run_args=run_args,
+                extra=extra,
             )
 
         # first grab global arguments and update them with explicit args
         run_arguments = {k: v for k, v in self._global_run_args.items()}
         run_arguments.update(run_args)
 
         extra_files_send = ensure_list(extra_files_send) + self._extra_files["send"]
-
         extra_files_recv = ensure_list(extra_files_recv) + self._extra_files["recv"]
 
         rnum = len(self.runners)
         if name is not None:
             run_arguments["name"] = name
             r_id = name
 
@@ -557,14 +562,15 @@
             arguments=args,
             dbfile=self.dbfile,
             parent=self,
             self_id=r_id,
             extra_files_send=extra_files_send,
             extra_files_recv=extra_files_recv,
             verbose=verbose,
+            extra=extra,
             **run_arguments,
         )
 
         tmp.result_extension = self.serialiser.extension
 
         if force or not skip:
             self._runs[r_id] = tmp
@@ -1224,27 +1230,30 @@
     def run(
         self,
         force: bool = False,
         dry_run: bool = False,
         quiet: bool = False,
         avoid_nodes: bool = False,
         uuids: list = None,
+        extra: str = "",
         **run_args,
     ):
         """
         Run the functions
 
         Args:
             force (bool):
                 force all runs to go through, ignoring checks
             dry_run (bool):
                 create files, but do not run
             avoid_nodes (bool):
                 if True, will attempt to avoid running on avoid_nodes using a standard
                 'bash' submission
+            extra:
+                extra text to add to runner jobscripts
             run_args:
                 any arguments to pass to the runners during this run.
                 will override any "global" arguments set at Dataset init
         """
         self.avoid_runtime()
         runtime = int(time.time())
         self._logger.runtime(f"#### Dataset run called at {runtime}")
@@ -1259,15 +1268,15 @@
             raise RuntimeError(localwinerror)
 
         if self.dependency:
             self._logger.runtime(
                 f"dataset {self} is a part of a dependency "
                 f"chain, calling from there"
             )
-            self.dependency.run(dry_run=dry_run, **run_args)
+            self.dependency.run(dry_run=dry_run, extra=extra, **run_args)
             Quiet.state = False
             return
 
         if uuids is not None:
             self._logger.runtime(f"running only runners {format_iterable(uuids)}")
 
         # first step is to handle the writing of the scripts to the local dir
@@ -1278,15 +1287,19 @@
         asynchronous = True  # should always be updated in the loop
         for runner in self.runners:
             if uuids is not None and runner.uuid not in uuids:
                 self._logger.runtime(f"skipping {runner} (uuid {runner.short_uuid})")
                 continue
 
             ready = runner.stage(
-                python=self.url.python, avoid_nodes=avoid_nodes, **run_args
+                python=self.url.python,
+                avoid_nodes=avoid_nodes,
+                global_extra=self._global_run_extra,
+                extra=extra,
+                **run_args,
             )
 
             if not ready:
                 continue
 
             self.transport.queue_for_push(runner.jobscript)
             self.transport.queue_for_push(runner.runfile)
```

### Comparing `remotemanager-0.9.4/remotemanager/dataset/dependency.py` & `remotemanager-0.9.5/remotemanager/dataset/dependency.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     def finish_append(self) -> None:
         for ds in self.ds_list:
             ds.finish_append(dependency_call=True)
 
     def run(
         self,
         dry_run: bool = False,
+        extra: str = None,
         **run_args,
     ):
         self._logger.info("dependency internal run call")
 
         ds_store = {}
         for ds in self.ds_list:
             ds_store[ds] = len(ds.runners)
@@ -210,25 +211,33 @@
             o.write("\n\n### serialiser functions ###")
             o.write(first.serialiser.dumpfunc())
             o.write("\n")
             o.write(first.serialiser.loadfunc())
 
         first.transport.queue_for_push(first.repofile)
 
+        # grab all global extra content from the datasets
+        global_extra = []
+        for ds in ds_store:
+            if ds._global_run_extra is not None:
+                global_extra.append(ds._global_run_extra)
+
         # and now a master script to kick off the chains
         # we need the export for ALL datasets
         master_content = []
 
         for ds in ds_store:
             # reuse the store as a list of runner uuids for runners_to_update
             ds_store[ds] = []
             for runner in ds.runners:
                 ready = runner.stage(
                     python=ds.url.python,
                     repo=f"${first.main_dir_env}/{first.repofile.name}",
+                    global_extra="\n".join(global_extra),
+                    extra=extra,
                     **run_args,
                 )
                 if not ready:
                     continue
 
                 # we only need the runlines for the first dataset, since the chaining
                 # is handled by the jobscripts
```

### Comparing `remotemanager-0.9.4/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.5/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/dataset/runner.py` & `remotemanager-0.9.5/remotemanager/dataset/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,22 @@
         arguments: dict,
         dbfile: str,
         parent,
         self_id: str,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         verbose: int = None,
+        extra: str = None,
         **run_args,
     ):
         self._verbose = Verbosity(verbose)
 
         self._run_args_base = self._set_defaults(run_args)
         self._run_args_temp = copy.deepcopy(self._run_args_base)
+        self.extra = extra
 
         self._extra_files_base = {
             "send": extra_files_send if extra_files_send is not None else [],
             "recv": extra_files_recv if extra_files_recv is not None else [],
         }
         self._extra_files_temp = copy.deepcopy(self._extra_files_base)
 
@@ -450,14 +452,16 @@
     def stage(
         self,
         extra_files_send: list = None,
         extra_files_recv: list = None,
         python: str = "python",
         avoid_nodes: bool = False,
         repo: str = None,
+        global_extra: str = None,
+        extra: str = None,
         **run_args,
     ) -> bool:
         """
         Prepare this runner for a run by creating files in the local dir
 
         Args:
             extra_files_send:
@@ -530,14 +534,22 @@
         self.runfile.write("\n".join(runscript))
 
         # jobscript writing
         # initialise script with whatever the parent url needs
         tmp = []
         if not avoid_nodes:
             tmp.append(self.parent._script_sub(**self._run_args_temp))
+
+        if global_extra is not None:
+            tmp.append(global_extra)
+        if self.extra is not None:
+            tmp.append(self.extra)
+        if extra is not None:
+            tmp.append(extra)
+
         if self.run_path != self.remote_dir:
             self._logger.debug("run dir is separate to remote dir, appending extras")
             submit = (
                 f"export {dir_env_name}=$1\n"
                 f"pydir=$PWD\n"
                 f"cd {self.run_dir} && "
                 f"{python} ${{pydir}}/{self.runfile.name} 2>> {errorpath}"
@@ -589,25 +601,33 @@
                 self._logger.warning("skipping already submitted run")
                 return False
 
         self._logger.important("running")
         return True
 
     @property
-    def is_finished(self):
+    def is_finished(self) -> bool:
         self._logger.runtime(
             f"checking is_finished for {self}. Current state: {self.state}"
         )
         if self.state >= "completed":
             return True
 
         self._logger.runtime("Not marked completed, returning False")
         return False
 
-    def read_local_files(self):
+    @property
+    def is_success(self) -> bool:
+        return self.state.success
+
+    @property
+    def is_failed(self) -> bool:
+        return not self.state.success
+
+    def read_local_files(self) -> None:
         satisfied = False
         success = False
         if self.state == "reset":
             self._logger.runtime("runner is in a reset state, ignoring file read")
             return
 
         if os.path.isfile(self.resultfile.local):
@@ -673,15 +693,15 @@
 
         Args:
             error:
                 run error string
         """
         self._error = error
 
-    def clear_result(self, wipe: bool = True):
+    def clear_result(self, wipe: bool = True) -> None:
         """
         Clear the results properties and set the state to "reset", which blocks some
         functions until the runner is rerun
 
         Args:
             wipe:
                 Additionally deletes the local files if True. Default True
@@ -708,15 +728,15 @@
 
             if os.path.isfile(self.errorfile.local):
                 os.remove(self.errorfile.local)
                 self._logger.info("deleted error file")
 
         self.state = "reset"
 
-    def run(self, *args, **kwargs):
+    def run(self, *args, **kwargs) -> None:
         """
         Run a single runner. See Dataset.run() for args.
 
         This function is inefficient and should not be used in a general workflow
         """
         self._logger.runtime(f"solo running runner {self}")
         self.parent.run(uuids=[self.uuid], *args, **kwargs)
```

### Comparing `remotemanager-0.9.4/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.5/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/jupyter/magic.py` & `remotemanager-0.9.5/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/logging/__init__.py` & `remotemanager-0.9.5/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/logging/log.py` & `remotemanager-0.9.5/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/logging/utils.py` & `remotemanager-0.9.5/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/logging/verbosity.py` & `remotemanager-0.9.5/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.5/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/serialisation/serial.py` & `remotemanager-0.9.5/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.5/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.5/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/storage/database.py` & `remotemanager-0.9.5/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/storage/function.py` & `remotemanager-0.9.5/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.5/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.5/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.5/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/transport/cp.py` & `remotemanager-0.9.5/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/transport/rsync.py` & `remotemanager-0.9.5/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/transport/scp.py` & `remotemanager-0.9.5/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/transport/transport.py` & `remotemanager-0.9.5/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/utils/__init__.py` & `remotemanager-0.9.5/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/utils/flags.py` & `remotemanager-0.9.5/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager/utils/version.py` & `remotemanager-0.9.5/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.4/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.5/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.4
+Version: 0.9.5
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.4/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.5/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

