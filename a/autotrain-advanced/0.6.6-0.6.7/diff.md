# Comparing `tmp/autotrain-advanced-0.6.6.tar.gz` & `tmp/autotrain-advanced-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.6.tar", last modified: Wed Jul 26 12:32:56 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.7.tar", last modified: Wed Jul 26 14:29:10 2023, max compression
```

## Comparing `autotrain-advanced-0.6.6.tar` & `autotrain-advanced-0.6.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.6/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.6/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.6/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 12:32:51.000000 autotrain-advanced-0.6.6/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37577 2023-07-26 10:24:33.000000 autotrain-advanced-0.6.6/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.6/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.6/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.6/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.685778 autotrain-advanced-0.6.6/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.6/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17073 2023-07-26 10:14:13.000000 autotrain-advanced-0.6.6/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.6/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8167 2023-07-26 11:05:41.000000 autotrain-advanced-0.6.6/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.6/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.6/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/clm.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13548 2023-07-26 11:05:27.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/main.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21311 2023-07-26 12:28:59.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13240 2023-07-26 12:29:40.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.6/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 12:32:56.689777 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 12:32:56.000000 autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.979177 autotrain-advanced-0.6.7/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.7/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 14:29:10.979177 autotrain-advanced-0.6.7/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.7/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 14:29:10.979177 autotrain-advanced-0.6.7/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.7/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 14:29:07.000000 autotrain-advanced-0.6.7/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    37577 2023-07-26 10:24:33.000000 autotrain-advanced-0.6.7/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.7/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.7/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.7/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13185 2023-07-26 08:58:57.000000 autotrain-advanced-0.6.7/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2618 2023-07-26 14:01:59.000000 autotrain-advanced-0.6.7/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.7/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.7/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.7/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17232 2023-07-26 14:08:33.000000 autotrain-advanced-0.6.7/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.7/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.7/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.7/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.7/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.7/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8237 2023-07-26 14:21:44.000000 autotrain-advanced-0.6.7/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.7/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.7/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.975177 autotrain-advanced-0.6.7/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.979177 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       63 2023-07-26 10:40:44.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 10:30:14.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13667 2023-07-26 14:28:19.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21311 2023-07-26 12:28:59.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13240 2023-07-26 12:29:40.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.7/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 14:29:10.979177 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2205 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 14:29:10.000000 autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.6/LICENSE` & `autotrain-advanced-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/PKG-INFO` & `autotrain-advanced-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.6
+Version: 0.6.7
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.6/setup.py` & `autotrain-advanced-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/__init__.py` & `autotrain-advanced-0.6.7/src/autotrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 # os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.6"
+__version__ = "0.6.7"
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain/app.py` & `autotrain-advanced-0.6.7/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.7/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.7/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.6.7/src/autotrain/cli/run_dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.7/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.7/src/autotrain/cli/run_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,33 +25,33 @@
         run_setup_parser.set_defaults(func=run_app_command_factory)
 
     def __init__(self, update_torch: bool):
         self.update_torch = update_torch
 
     def run(self):
         # install latest transformers
-        cmd = "pip install git+https://github.com/huggingface/transformers.git"
+        cmd = "pip uninstall -y transformers && pip install git+https://github.com/huggingface/transformers.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest transformers@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest transformers")
 
-        cmd = "pip install git+https://github.com/huggingface/peft.git"
+        cmd = "pip uninstall -y peft && pip install git+https://github.com/huggingface/peft.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest peft@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest peft")
 
-        cmd = "pip install git+https://github.com/huggingface/diffusers.git"
+        cmd = "pip uninstall -y diffusers && pip install git+https://github.com/huggingface/diffusers.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest diffusers@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest diffusers")
 
-        cmd = "pip install git+https://github.com/lvwerra/trl.git"
+        cmd = "pip uninstall -y trl && pip install git+https://github.com/lvwerra/trl.git"
         pipe = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         logger.info("Installing latest trl@main")
         _, _ = pipe.communicate()
         logger.info("Successfully installed latest trl")
 
         if self.update_torch:
             cmd = "pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118"
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain/dataset.py` & `autotrain-advanced-0.6.7/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/help.py` & `autotrain-advanced-0.6.7/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.7/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/params.py` & `autotrain-advanced-0.6.7/src/autotrain/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     task: Literal["dreambooth"]
     num_steps: int = Field(1500, title="Number of steps")
     image_size: int = Field(512, title="Image size")
     text_encoder_steps_percentage: int = Field(30, title="Text encoder steps percentage")
     prior_preservation: bool = Field(False, title="Prior preservation")
     learning_rate: float = Field(2e-6, title="Learning rate")
     train_batch_size: int = Field(1, title="Training batch size")
+    gradient_accumulation_steps: int = Field(1, title="Gradient accumulation steps")
 
 
 class ImageBinaryClassificationParams(BaseModel):
     task: Literal["image_binary_classification"]
     learning_rate: float = Field(3e-5, title="Learning rate")
     num_train_epochs: int = Field(3, title="Number of training epochs")
     train_batch_size: int = Field(8, title="Training batch size")
@@ -346,14 +347,15 @@
         if self.param_choice == "manual":
             return {
                 "hub_model": HubModel,
                 "image_size": ImageSize,
                 "learning_rate": LearningRate,
                 "train_batch_size": TrainBatchSize,
                 "num_steps": DBNumSteps,
+                "gradient_accumulation_steps": GradientAccumulationSteps,
             }
         if self.param_choice == "autotrain":
             if self.model_choice == "hub_model":
                 return {
                     "hub_model": HubModel,
                     "image_size": ImageSize,
                     "num_models": NumModels,
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.7/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.7/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.7/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.7/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/project.py` & `autotrain-advanced-0.6.7/src/autotrain/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
                 "autotrain": True if self.param_choice == "autotrain" else False,
                 "language": language,
                 "max_models": self.max_models,
                 "hub_model": self.hub_model,
                 "params": self.job_params,
             },
         }
+        logger.info(f"🚀 Creating project with payload: {payload}")
 
         if local is True:
             return self.create_local(payload=payload)
 
         logger.info(f"🚀 Creating project with payload: {payload}")
         json_resp = http_post(path="/projects/create", payload=payload, token=self.token).json()
         proj_name = json_resp["proj_name"]
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain/tasks.py` & `autotrain-advanced-0.6.7/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/main.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,15 +290,15 @@
             img.save(os.path.join(processed_data_path, processed_filename), format="JPEG", quality=100)
     return concept_prompts
 
 
 @at_utils.job_watcher
 def train_ui(co2_tracker, payload, huggingface_token, model_path):
     data_repo_path = f"{payload['username']}/autotrain-data-{payload['proj_name']}"
-    data_path = "output/data"
+    data_path = "/tmp/data"
     data_repo = at_utils.clone_hf_repo(
         local_dir=data_path,
         repo_url="https://huggingface.co/datasets/" + data_repo_path,
         token=huggingface_token,
     )
     data_repo.git_pull()
 
@@ -306,15 +306,17 @@
     job_config["model_name"] = payload["config"]["hub_model"]
 
     model_name = job_config["model_name"]
     # device = job_config.get("device", "cuda")
     del job_config["model_name"]
     if "device" in job_config:
         del job_config["device"]
+    logger.info(f"job_config: {job_config}")
     job_config = DreamboothParams(**job_config)
+    logger.info(f"job_config: {job_config}")
 
     logger.info("Create model repo")
     project_name = payload["proj_name"]
     repo_name = f"autotrain-{project_name}"
     repo_user = payload["username"]
 
     # print contents of data_path folder
@@ -335,15 +337,15 @@
         model=model_name,
         image_path=os.path.join(data_path, "processed_data"),
         output=model_path,
         seed=42,
         resolution=job_config.image_size,
         fp16=True,
         batch_size=job_config.train_batch_size,
-        gradient_accumulation_steps=1,
+        gradient_accumulation=job_config.gradient_accumulation_steps,
         use_8bit_adam=True,
         lr=job_config.learning_rate,
         scheduler="constant",
         warmup_steps=0,
         num_steps=job_config.num_steps,
         revision=None,
         push_to_hub=True,
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.7/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain/utils.py` & `autotrain-advanced-0.6.7/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.6
+Version: 0.6.7
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.6/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.7/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

