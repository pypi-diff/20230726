# Comparing `tmp/autotrain-advanced-0.6.5.tar.gz` & `tmp/autotrain-advanced-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.5.tar", last modified: Wed Jul 26 11:06:32 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.6.tar", last modified: Wed Jul 26 12:32:56 2023, max compression
```

## Comparing `autotrain-advanced-0.6.5.tar` & `autotrain-advanced-0.6.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.5/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.5/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.5/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 11:06:27.000000 autotrain-advanced-0.6.5/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37577 2023-07-26 10:24:33.000000 autotrain-advanced-0.6.5/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.5/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.5/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.5/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.529616 autotrain-advanced-0.6.5/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.5/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17073 2023-07-26 10:14:13.000000 autotrain-advanced-0.6.5/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.5/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8167 2023-07-26 11:05:41.000000 autotrain-advanced-0.6.5/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.5/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.5/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/clm.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13548 2023-07-26 11:05:27.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/main.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.5/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 11:06:32.533616 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 11:06:32.000000 autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.6/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.6/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.6/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 12:32:51.000000 autotrain-advanced-0.6.6/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37577 2023-07-26 10:24:33.000000 autotrain-advanced-0.6.6/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.6/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.6/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.6/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.6/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17073 2023-07-26 10:14:13.000000 autotrain-advanced-0.6.6/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8167 2023-07-26 11:05:41.000000 autotrain-advanced-0.6.6/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.6/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.6/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13548 2023-07-26 11:05:27.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21311 2023-07-26 12:28:59.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13240 2023-07-26 12:29:40.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.5/LICENSE` & `autotrain-advanced-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/PKG-INFO` & `autotrain-advanced-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.5
+Version: 0.6.6
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.5/setup.py` & `autotrain-advanced-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/__init__.py` & `autotrain-advanced-0.6.6/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 # os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.5"
+__version__ = "0.6.6"
```

### Comparing `autotrain-advanced-0.6.5/src/autotrain/app.py` & `autotrain-advanced-0.6.6/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.6/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.6/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.6.6/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.6/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.6/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/dataset.py` & `autotrain-advanced-0.6.6/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/help.py` & `autotrain-advanced-0.6.6/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.6/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/params.py` & `autotrain-advanced-0.6.6/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.6/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.6/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.6/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.6/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/project.py` & `autotrain-advanced-0.6.6/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/tasks.py` & `autotrain-advanced-0.6.6/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/main.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/main.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,35 +278,36 @@
 
                 save_path = os.path.join(self.config.output, f"checkpoint-{self.global_step}")
                 self.accelerator.save_state(save_path)
                 logger.info(f"Saved state to {save_path}")
 
     def _get_model_pred(self, batch, channels, noisy_model_input, timesteps, bsz):
         if self.config.xl:
+            elems_to_repeat = bsz // 2 if self.config.prior_preservation else bsz
             if not self.config.train_text_encoder:
                 unet_added_conditions = {
-                    "time_ids": self.add_time_ids.repeat(bsz, 1),
-                    "text_embeds": self.unet_add_text_embeds.repeat(bsz, 1),
+                    "time_ids": self.add_time_ids.repeat(elems_to_repeat, 1),
+                    "text_embeds": self.unet_add_text_embeds.repeat(elems_to_repeat, 1),
                 }
                 model_pred = self.unet(
                     noisy_model_input,
                     timesteps,
-                    self.prompt_embeds.repeat(bsz, 1, 1),
+                    self.prompt_embeds.repeat(elems_to_repeat, 1, 1),
                     added_cond_kwargs=unet_added_conditions,
                 ).sample
             else:
-                unet_added_conditions = {"time_ids": self.add_time_ids.repeat(bsz, 1)}
+                unet_added_conditions = {"time_ids": self.add_time_ids.repeat(elems_to_repeat, 1)}
                 prompt_embeds, pooled_prompt_embeds = utils.encode_prompt_xl(
                     text_encoders=self.text_encoders,
                     tokenizers=None,
                     prompt=None,
                     text_input_ids_list=[self.tokens_one, self.tokens_two],
                 )
                 unet_added_conditions.update({"text_embeds": pooled_prompt_embeds.repeat(bsz, 1)})
-                prompt_embeds = prompt_embeds.repeat(bsz, 1, 1)
+                prompt_embeds = prompt_embeds.repeat(elems_to_repeat, 1, 1)
                 model_pred = self.unet(
                     noisy_model_input, timesteps, prompt_embeds, added_cond_kwargs=unet_added_conditions
                 ).sample
 
         else:
             if self.config.pre_compute_text_embeddings:
                 encoder_hidden_states = batch["input_ids"]
```

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from tqdm import tqdm
 from transformers import AutoTokenizer, PretrainedConfig
 
 from autotrain.trainers.dreambooth.datasets import PromptDataset
 
 
 VALID_IMAGE_EXTENSIONS = [".jpg", ".jpeg", ".png", ".JPG", ".JPEG", ".PNG"]
-XL_MODELS = ["stabilityai/stable-diffusion-xl-base-0.9"]
+XL_MODELS = [
+    "stabilityai/stable-diffusion-xl-base-1.0",
+    "stabilityai/stable-diffusion-xl-base-0.9",
+    "diffusers/stable-diffusion-xl-base-1.0",
+]
 
 
 def create_model_card(repo_id: str, base_model: str, train_text_encoder: bool, prompt: str, repo_folder: str):
     if train_text_encoder:
         text_encoder_text = "trained"
     else:
         text_encoder_text = "not trained"
```

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.6/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain/utils.py` & `autotrain-advanced-0.6.6/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.5
+Version: 0.6.6
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.5/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

