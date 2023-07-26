# Comparing `tmp/autotrain-advanced-0.6.2.tar.gz` & `tmp/autotrain-advanced-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.2.tar", last modified: Fri Jul 21 11:05:10 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.3.tar", last modified: Wed Jul 26 08:37:35 2023, max compression
```

## Comparing `autotrain-advanced-0.6.2.tar` & `autotrain-advanced-0.6.3.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.2/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.2/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.2/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      816 2023-07-21 11:05:06.000000 autotrain-advanced-0.6.2/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.2/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.6.2/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1033 2023-07-19 10:07:30.000000 autotrain-advanced-0.6.2/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-20 12:00:11.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2178 2023-07-19 10:23:02.000000 autotrain-advanced-0.6.2/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.2/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-19 10:21:07.000000 autotrain-advanced-0.6.2/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.2/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.444928 autotrain-advanced-0.6.2/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-20 09:08:58.000000 autotrain-advanced-0.6.2/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-20 12:00:25.000000 autotrain-advanced-0.6.2/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.2/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.2/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.2/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.2/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.2/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-21 11:04:59.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-07-18 10:31:20.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-19 09:53:41.000000 autotrain-advanced-0.6.2/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-19 10:14:57.000000 autotrain-advanced-0.6.2/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-21 11:05:10.448928 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1325 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-21 11:05:10.000000 autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.3/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.3/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.3/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.476866 autotrain-advanced-0.6.3/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 08:37:24.000000 autotrain-advanced-0.6.3/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.3/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.3/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12932 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.3/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.3/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.3/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-26 05:47:13.000000 autotrain-advanced-0.6.3/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8186 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.3/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.3/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9584 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.2/LICENSE` & `autotrain-advanced-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/PKG-INFO` & `autotrain-advanced-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.2/setup.py` & `autotrain-advanced-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/__init__.py` & `autotrain-advanced-0.6.3/src/autotrain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # Lint as: python3
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
-os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.2"
+# os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
+__version__ = "0.6.3"
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain/app.py` & `autotrain-advanced-0.6.3/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.3/src/autotrain/cli/autotrain.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 
 from .. import __version__
 from .run_app import RunAutoTrainAppCommand
+from .run_dreambooth import RunAutoTrainDreamboothCommand
 from .run_llm import RunAutoTrainLLMCommand
 from .run_setup import RunSetupCommand
 
 
 def main():
     parser = argparse.ArgumentParser(
         "AutoTrain advanced CLI",
@@ -15,14 +16,15 @@
     parser.add_argument("--version", "-v", help="Display AutoTrain version", action="store_true")
     commands_parser = parser.add_subparsers(help="commands")
 
     # Register commands
     RunAutoTrainAppCommand.register_subcommand(commands_parser)
     RunAutoTrainLLMCommand.register_subcommand(commands_parser)
     RunSetupCommand.register_subcommand(commands_parser)
+    RunAutoTrainDreamboothCommand.register_subcommand(commands_parser)
 
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         exit(0)
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.3/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.3/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.3/src/autotrain/cli/run_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
         cmd = "pip install git+https://github.com/huggingface/peft.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest peft@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest peft")
 
+        cmd = "pip install git+https://github.com/huggingface/diffusers.git"
+        pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        logger.info("Installing latest diffusers@main")
+        _, _ = pipe.communicate()
+        logger.info("Successfully installed latest diffusers")
+
         cmd = "pip install git+https://github.com/lvwerra/trl.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest trl@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest trl")
 
         if self.update_torch:
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain/dataset.py` & `autotrain-advanced-0.6.3/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/help.py` & `autotrain-advanced-0.6.3/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.3/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/params.py` & `autotrain-advanced-0.6.3/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.3/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.3/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.3/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.3/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/project.py` & `autotrain-advanced-0.6.3/src/autotrain/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             elif "num_models" not in self.job_params[0] and "source_language" in self.job_params[0]:
                 raise ValueError("❌ Please specify num_models in job_params when using AutoTrain model")
         else:
             self.language = "unk"
             self.max_models = len(self.job_params)
 
     def create_local(self, payload):
-        from autotrain.trainers.dreambooth import train as train_dreambooth
+        from autotrain.trainers.dreambooth import train_dreambooth_deprecated as train_dreambooth
         from autotrain.trainers.image_classification import train as train_image_classification
         from autotrain.trainers.lm_trainer import train as train_lm
         from autotrain.trainers.text_classification import train as train_text_classification
 
         # check if training tracker file exists in /tmp/
         if os.path.exists(os.path.join("/tmp", "training")):
             raise ValueError("❌ Another training job is already running in this workspace.")
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain/tasks.py` & `autotrain-advanced-0.6.3/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -835,18 +835,18 @@
         pretrained_model_name_or_path=model_name,
         instance_data_dir=os.path.join(data_path, "processed_data"),
         class_data_dir=None,
         output_dir=model_path,
         seed=42,
         resolution=job_config.image_size,
         mixed_precision="fp16",
-        train_batch_size=job_config.train_batch_size,
+        train_batch_size=job_config.batch_size,
         gradient_accumulation_steps=1,
         use_8bit_adam=True,
-        learning_rate=job_config.learning_rate,
+        learning_rate=job_config.lr,
         lr_scheduler="polynomial",
         lr_warmup_steps=0,
         max_train_steps=job_config.num_steps,
         gradient_checkpointing=gradient_checkpointing,
         cache_latents=cache_latents,
         revision=None,
     )
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.3/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain/utils.py` & `autotrain-advanced-0.6.3/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,18 +25,24 @@
 src/autotrain/preprocessor/dreambooth.py
 src/autotrain/preprocessor/tabular.py
 src/autotrain/preprocessor/text.py
 src/autotrain/preprocessor/vision.py
 src/autotrain/trainers/__init__.py
 src/autotrain/trainers/callbacks.py
 src/autotrain/trainers/clm.py
-src/autotrain/trainers/dreambooth.py
 src/autotrain/trainers/image_classification.py
 src/autotrain/trainers/lm_trainer.py
 src/autotrain/trainers/text_classification.py
 src/autotrain/trainers/utils.py
+src/autotrain/trainers/dreambooth/__init__.py
+src/autotrain/trainers/dreambooth/datasets.py
+src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+src/autotrain/trainers/dreambooth/main.py
+src/autotrain/trainers/dreambooth/params.py
+src/autotrain/trainers/dreambooth/trainer.py
+src/autotrain/trainers/dreambooth/utils.py
 src/autotrain_advanced.egg-info/PKG-INFO
 src/autotrain_advanced.egg-info/SOURCES.txt
 src/autotrain_advanced.egg-info/dependency_links.txt
 src/autotrain_advanced.egg-info/entry_points.txt
 src/autotrain_advanced.egg-info/requires.txt
 src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.2/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

