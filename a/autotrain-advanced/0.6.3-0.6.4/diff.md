# Comparing `tmp/autotrain-advanced-0.6.3.tar.gz` & `tmp/autotrain-advanced-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.6.3.tar", last modified: Wed Jul 26 08:37:35 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.6.4.tar", last modified: Wed Jul 26 08:58:23 2023, max compression
```

## Comparing `autotrain-advanced-0.6.3.tar` & `autotrain-advanced-0.6.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.3/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.3/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.3/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.476866 autotrain-advanced-0.6.3/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 08:37:24.000000 autotrain-advanced-0.6.3/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.3/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.3/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12932 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/cli/run_setup.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.3/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.3/src/autotrain/help.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/infer/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/infer/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/infer/text_generation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.3/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-26 05:47:13.000000 autotrain-advanced-0.6.3/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.3/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8186 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.3/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.3/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/clm.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/datasets.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9584 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/main.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/params.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.3/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:37:35.480866 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 08:37:35.000000 autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.4/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.6.4/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      439 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.4/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      818 2023-07-26 08:58:18.000000 autotrain-advanced-0.6.4/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.6.4/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-07-26 04:15:21.000000 autotrain-advanced-0.6.4/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1162 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13184 2023-07-26 08:58:09.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14842 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2506 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/cli/run_setup.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.6.4/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12419 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.4/src/autotrain/help.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/infer/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/infer/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1885 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/infer/text_generation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.6.4/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-07-26 05:47:13.000000 autotrain-advanced-0.6.4/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.082335 autotrain-advanced-0.6.4/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.6.4/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8186 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.6.4/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.6.4/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10768 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/clm.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9089 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/datasets.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34289 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9584 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/main.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3793 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/params.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    21169 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    13139 2023-07-26 08:37:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5756 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8221 2023-07-24 09:22:18.000000 autotrain-advanced-0.6.4/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-26 08:58:23.086335 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1613 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2097 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-26 08:58:23.000000 autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.6.3/LICENSE` & `autotrain-advanced-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/PKG-INFO` & `autotrain-advanced-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.3/setup.py` & `autotrain-advanced-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/__init__.py` & `autotrain-advanced-0.6.4/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # pylint: enable=line-too-long
 import os
 
 
 # ignore bnb warnings
 os.environ["BITSANDBYTES_NOWELCOME"] = "1"
 # os.environ["HF_HUB_DISABLE_PROGRESS_BARS"] = "1"
-__version__ = "0.6.3"
+__version__ = "0.6.4"
```

### Comparing `autotrain-advanced-0.6.3/src/autotrain/app.py` & `autotrain-advanced-0.6.4/src/autotrain/app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.6.4/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.6.4/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/cli/run_dreambooth.py` & `autotrain-advanced-0.6.4/src/autotrain/cli/run_dreambooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import glob
 import os
 from argparse import ArgumentParser
 
 from loguru import logger
 
 from autotrain.cli import BaseAutoTrainCommand
-from autotrain.trainers.dreambooth import train as train_dreambooth
-from autotrain.trainers.dreambooth.params import DreamBoothTrainingParams
-from autotrain.trainers.dreambooth.utils import VALID_IMAGE_EXTENSIONS, XL_MODELS
+
+try:
+    from autotrain.trainers.dreambooth import train as train_dreambooth
+    from autotrain.trainers.dreambooth.params import DreamBoothTrainingParams
+    from autotrain.trainers.dreambooth.utils import VALID_IMAGE_EXTENSIONS, XL_MODELS
+except ImportError:
+    logger.warning(
+        "❌ Some DreamBooth components are missing! Please run `autotrain setup` to install it. Ignore this warning if you are not using DreamBooth or running `autotrain setup` already."
+    )
 
 
 def count_images(directory):
     files_grabbed = []
     for files in VALID_IMAGE_EXTENSIONS:
         files_grabbed.extend(glob.glob(os.path.join(directory, "*" + files)))
     return len(files_grabbed)
```

### Comparing `autotrain-advanced-0.6.3/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.6.4/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/cli/run_setup.py` & `autotrain-advanced-0.6.4/src/autotrain/cli/run_setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/dataset.py` & `autotrain-advanced-0.6.4/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/help.py` & `autotrain-advanced-0.6.4/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/infer/text_generation.py` & `autotrain-advanced-0.6.4/src/autotrain/infer/text_generation.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/params.py` & `autotrain-advanced-0.6.4/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.6.4/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.6.4/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.6.4/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.6.4/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/project.py` & `autotrain-advanced-0.6.4/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/tasks.py` & `autotrain-advanced-0.6.4/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/datasets.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/datasets.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/dreambooth_deprecated.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/main.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/main.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/params.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/trainer.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/dreambooth/utils.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/dreambooth/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.6.4/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain/utils.py` & `autotrain-advanced-0.6.4/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.6.3/src/autotrain_advanced.egg-info/requires.txt` & `autotrain-advanced-0.6.4/src/autotrain_advanced.egg-info/requires.txt`

 * *Files identical despite different names*

