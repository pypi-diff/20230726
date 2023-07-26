# Comparing `tmp/autotrain-advanced-0.6.4.tar.gz` & `tmp/autotrain-advanced-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.4.tar", last modified: Wed Jul 26 08:58:23 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.5.tar", last modified: Wed Jul 26 11:06:32 2023, max compression
```

## Comparing `autotrain-advanced-0.6.4.tar` & `autotrain-advanced-0.6.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.4/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.4/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.4/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 08:58:18.000000 autotrain-advanced-0.6.4/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.4/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.4/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13184 2023-07-26 08:58:09.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.4/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.4/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.4/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-26 05:47:13.000000 autotrain-advanced-0.6.4/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8186 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.4/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.4/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/clm.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9584 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/main.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.5/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.5/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.5/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 11:06:27.000000 autotrain-advanced-0.6.5/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37577 2023-07-26 10:24:33.000000 autotrain-advanced-0.6.5/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.5/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.5/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.5/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.5/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17073 2023-07-26 10:14:13.000000 autotrain-advanced-0.6.5/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8167 2023-07-26 11:05:41.000000 autotrain-advanced-0.6.5/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.5/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.5/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13548 2023-07-26 11:05:27.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.4/LICENSE` & `autotrain-advanced-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/PKG-INFO` & `autotrain-advanced-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.4
+Version: 0.6.5
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.4/setup.py` & `autotrain-advanced-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/__init__.py` & `autotrain-advanced-0.6.5/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 # os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.4"
+__version__ = "0.6.5"
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain/app.py` & `autotrain-advanced-0.6.5/src/autotrain/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -714,34 +714,19 @@
                                 visible=False,
                                 interactive=True,
                                 elem_id="lora_dropout",
                             )
                         with gr.Row():
                             db_num_steps = gr.Number(
                                 label="Num Steps",
-                                value=1000,
+                                value=500,
                                 visible=False,
                                 interactive=True,
                                 elem_id="num_steps",
                             )
-                            db_prior_preservation = gr.Dropdown(
-                                label="Prior Preservation",
-                                choices=["True", "False"],
-                                value="True",
-                                visible=False,
-                                interactive=True,
-                                elem_id="prior_preservation",
-                            )
-                            db_text_encoder_steps_percentage = gr.Number(
-                                label="Text Encoder Steps Percentage",
-                                value=0.1,
-                                visible=False,
-                                interactive=True,
-                                elem_id="text_encoder_steps_percentage",
-                            )
                         with gr.Row():
                             optimizer = gr.Dropdown(
                                 label="Optimizer",
                                 choices=["adamw_torch", "adamw_hf", "sgd", "adafactor", "adagrad"],
                                 value="adamw_torch",
                                 visible=False,
                                 interactive=True,
@@ -802,17 +787,15 @@
             lora_alpha,
             lora_dropout,
             optimizer,
             scheduler,
             percentage_warmup_steps,
             weight_decay,
             db_num_steps,
-            db_prior_preservation,
             image_size,
-            db_text_encoder_steps_percentage,
         ]
 
         def _update_params(params_data):
             _task = params_data[task_type]
             _task = APP_TASKS_MAPPING[_task]
             params = Params(
                 task=_task,
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.5/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.5/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.6.5/src/autotrain/cli/run_dreambooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from argparse import ArgumentParser
 
 from loguru import logger
 
 from autotrain.cli import BaseAutoTrainCommand
 
+
 try:
     from autotrain.trainers.dreambooth import train as train_dreambooth
     from autotrain.trainers.dreambooth.params import DreamBoothTrainingParams
     from autotrain.trainers.dreambooth.utils import VALID_IMAGE_EXTENSIONS, XL_MODELS
 except ImportError:
     logger.warning(
         "❌ Some DreamBooth components are missing! Please run `autotrain setup` to install it. Ignore this warning if you are not using DreamBooth or running `autotrain setup` already."
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.5/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.5/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/dataset.py` & `autotrain-advanced-0.6.5/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/help.py` & `autotrain-advanced-0.6.5/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.5/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/params.py` & `autotrain-advanced-0.6.5/src/autotrain/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,16 +346,14 @@
         if self.param_choice == "manual":
             return {
                 "hub_model": HubModel,
                 "image_size": ImageSize,
                 "learning_rate": LearningRate,
                 "train_batch_size": TrainBatchSize,
                 "num_steps": DBNumSteps,
-                "text_encoder_steps_percentage": DBTextEncoderStepsPercentage,
-                "prior_preservation": DBPriorPreservation,
             }
         if self.param_choice == "autotrain":
             if self.model_choice == "hub_model":
                 return {
                     "hub_model": HubModel,
                     "image_size": ImageSize,
                     "num_models": NumModels,
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.5/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.5/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.5/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.5/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/project.py` & `autotrain-advanced-0.6.5/src/autotrain/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             elif "num_models" not in self.job_params[0] and "source_language" in self.job_params[0]:
                 raise ValueError("❌ Please specify num_models in job_params when using AutoTrain model")
         else:
             self.language = "unk"
             self.max_models = len(self.job_params)
 
     def create_local(self, payload):
-        from autotrain.trainers.dreambooth import train_dreambooth_deprecated as train_dreambooth
+        from autotrain.trainers.dreambooth import train_ui as train_dreambooth
         from autotrain.trainers.image_classification import train as train_image_classification
         from autotrain.trainers.lm_trainer import train as train_lm
         from autotrain.trainers.text_classification import train as train_text_classification
 
         # check if training tracker file exists in /tmp/
         if os.path.exists(os.path.join("/tmp", "training")):
             raise ValueError("❌ Another training job is already running in this workspace.")
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain/tasks.py` & `autotrain-advanced-0.6.5/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.5/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain/utils.py` & `autotrain-advanced-0.6.5/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.4
+Version: 0.6.5
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 tqdm==4.62.1
 werkzeug==2.3.6
 huggingface_hub>=0.14.1
 triton==2.0.0.post1
 requests==2.31.0
 gradio==3.37.0
 einops==0.6.1
+invisible-watermark==0.2.0
 tensorboard
 peft
 trl
 tiktoken
 transformers
 accelerate
 diffusers
@@ -52,14 +53,15 @@
 tqdm==4.62.1
 werkzeug==2.3.6
 huggingface_hub>=0.14.1
 triton==2.0.0.post1
 requests==2.31.0
 gradio==3.37.0
 einops==0.6.1
+invisible-watermark==0.2.0
 tensorboard
 peft
 trl
 tiktoken
 transformers
 accelerate
 diffusers
@@ -90,14 +92,15 @@
 tqdm==4.62.1
 werkzeug==2.3.6
 huggingface_hub>=0.14.1
 triton==2.0.0.post1
 requests==2.31.0
 gradio==3.37.0
 einops==0.6.1
+invisible-watermark==0.2.0
 tensorboard
 peft
 trl
 tiktoken
 transformers
 accelerate
 diffusers
@@ -129,14 +132,15 @@
 tqdm==4.62.1
 werkzeug==2.3.6
 huggingface_hub>=0.14.1
 triton==2.0.0.post1
 requests==2.31.0
 gradio==3.37.0
 einops==0.6.1
+invisible-watermark==0.2.0
 tensorboard
 peft
 trl
 tiktoken
 transformers
 accelerate
 diffusers
```

