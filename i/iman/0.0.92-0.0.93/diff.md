# Comparing `tmp/iman-0.0.92.tar.gz` & `tmp/iman-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iman-0.0.92.tar", last modified: Wed Jul 26 07:09:08 2023, max compression
+gzip compressed data, was "dist\iman-0.0.93.tar", last modified: Wed Jul 26 07:13:34 2023, max compression
```

## Comparing `iman-0.0.92.tar` & `iman-0.0.93.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/
--rw-rw-rw-   0        0        0     6943 2023-07-26 07:09:08.000000 iman-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0     6569 2023-07-26 07:08:42.000000 iman-0.0.92/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/
--rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.92/iman/AUG.py
--rw-rw-rw-   0        0        0    17907 2023-07-26 05:34:14.000000 iman-0.0.92/iman/Audio.py
--rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.92/iman/Boors.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/Features/
--rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.92/iman/Features/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/Features/mfcc/
--rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.92/iman/Features/mfcc/LS.py
--rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.92/iman/Features/mfcc/SB.py
--rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.92/iman/Features/mfcc/__init__.py
--rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.92/iman/Features/mfcc/getmfcc_from_librosa.py
--rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.92/iman/Features/mfcc/sb_mfcc_class.py
--rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.92/iman/Image.py
--rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.92/iman/Report.py
--rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.92/iman/Text.py
--rw-rw-rw-   0        0        0     4478 2023-07-22 04:52:36.000000 iman-0.0.92/iman/__init__.py
--rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.92/iman/examples.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/examples_folder/
--rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.92/iman/examples_folder/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.92/iman/examples_folder/age.py
--rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.92/iman/examples_folder/ffmpeg.py
--rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.92/iman/examples_folder/flask.py
--rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.92/iman/examples_folder/gpu_allocate_tf.py
--rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.92/iman/examples_folder/graphviz_chart.py
--rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.92/iman/examples_folder/parallel.py
--rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.92/iman/examples_folder/post_by_python.py
--rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.92/iman/examples_folder/pyworldd.py
--rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.92/iman/examples_folder/queue_worker.py
--rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.92/iman/examples_folder/save_docx.py
--rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.92/iman/examples_folder/stft_test.py
--rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.92/iman/examples_folder/threading_example.py
--rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.92/iman/examples_folder/wikipedia.py
--rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.92/iman/gpu_info.py
--rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.92/iman/info.py
--rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.92/iman/matlab.py
--rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.92/iman/metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/num2fa/
--rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.92/iman/num2fa/__init__.py
--rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.92/iman/num2fa/__main__.py
--rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.92/iman/par.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/pyctcdecode/
--rw-rw-rw-   0        0        0      265 2023-07-11 05:28:53.000000 iman-0.0.92/iman/pyctcdecode/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-07-11 05:28:53.000000 iman-0.0.92/iman/pyctcdecode/alphabet.py
--rw-rw-rw-   0        0        0      617 2023-07-11 05:28:53.000000 iman-0.0.92/iman/pyctcdecode/constants.py
--rw-rw-rw-   0        0        0    29784 2023-07-19 12:40:28.000000 iman-0.0.92/iman/pyctcdecode/decoder.py
--rw-rw-rw-   0        0        0    11420 2023-07-11 05:28:53.000000 iman-0.0.92/iman/pyctcdecode/language_model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/sad_tf/
--rw-rw-rw-   0        0        0      101 2023-07-23 07:12:34.000000 iman-0.0.92/iman/sad_tf/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-07-17 06:10:42.000000 iman-0.0.92/iman/sad_tf/export_funcs.py
--rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.92/iman/sad_tf/features.py
--rw-rw-rw-   0        0        0    18972 2023-07-23 07:08:02.000000 iman-0.0.92/iman/sad_tf/segmenter.py
--rw-rw-rw-   0        0        0    20025 2023-07-23 08:03:31.000000 iman-0.0.92/iman/sad_tf/segmentero.py
--rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.92/iman/sad_tf/sidekit_mfcc.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_tf/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.92/iman/sad_tf/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_tf/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/sad_torch_mfcc/
--rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.92/iman/sad_torch_mfcc/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.92/iman/sad_torch_mfcc/export_funcs.py
--rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.92/iman/sad_torch_mfcc/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.92/iman/sad_torch_mfcc/sad_model.py
--rw-rw-rw-   0        0        0    19324 2023-07-22 04:57:05.000000 iman-0.0.92/iman/sad_torch_mfcc/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_torch_mfcc/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.92/iman/sad_torch_mfcc/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_torch_mfcc/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/
--rw-rw-rw-   0        0        0       36 2023-07-26 06:11:13.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/__init__.py
--rw-rw-rw-   0        0        0      631 2023-07-26 06:41:32.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/sad_model.py
--rw-rw-rw-   0        0        0    10284 2023-07-26 07:04:45.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.92/iman/sad_torch_mfcc_speaker/viterbi_utils.py
--rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.92/iman/tsne.py
--rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.92/iman/web.py
--rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.92/iman/xvector.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:09:08.000000 iman-0.0.92/iman.egg-info/
--rw-rw-rw-   0        0        0     6943 2023-07-26 07:09:07.000000 iman-0.0.92/iman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2067 2023-07-26 07:09:07.000000 iman-0.0.92/iman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:09:07.000000 iman-0.0.92/iman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-26 07:09:07.000000 iman-0.0.92/iman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 07:09:07.000000 iman-0.0.92/iman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 07:09:08.000000 iman-0.0.92/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-07-26 07:08:58.000000 iman-0.0.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/
+-rw-rw-rw-   0        0        0     6963 2023-07-26 07:13:34.000000 iman-0.0.93/PKG-INFO
+-rw-rw-rw-   0        0        0     6589 2023-07-26 07:11:54.000000 iman-0.0.93/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/
+-rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.93/iman/AUG.py
+-rw-rw-rw-   0        0        0    17907 2023-07-26 05:34:14.000000 iman-0.0.93/iman/Audio.py
+-rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.93/iman/Boors.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/Features/
+-rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.93/iman/Features/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/Features/mfcc/
+-rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.93/iman/Features/mfcc/LS.py
+-rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.93/iman/Features/mfcc/SB.py
+-rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.93/iman/Features/mfcc/__init__.py
+-rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.93/iman/Features/mfcc/getmfcc_from_librosa.py
+-rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.93/iman/Features/mfcc/sb_mfcc_class.py
+-rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.93/iman/Image.py
+-rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.93/iman/Report.py
+-rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.93/iman/Text.py
+-rw-rw-rw-   0        0        0     4478 2023-07-22 04:52:36.000000 iman-0.0.93/iman/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.93/iman/examples.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/examples_folder/
+-rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.93/iman/examples_folder/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.93/iman/examples_folder/age.py
+-rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.93/iman/examples_folder/ffmpeg.py
+-rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.93/iman/examples_folder/flask.py
+-rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.93/iman/examples_folder/gpu_allocate_tf.py
+-rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.93/iman/examples_folder/graphviz_chart.py
+-rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.93/iman/examples_folder/parallel.py
+-rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.93/iman/examples_folder/post_by_python.py
+-rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.93/iman/examples_folder/pyworldd.py
+-rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.93/iman/examples_folder/queue_worker.py
+-rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.93/iman/examples_folder/save_docx.py
+-rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.93/iman/examples_folder/stft_test.py
+-rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.93/iman/examples_folder/threading_example.py
+-rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.93/iman/examples_folder/wikipedia.py
+-rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.93/iman/gpu_info.py
+-rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.93/iman/info.py
+-rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.93/iman/matlab.py
+-rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.93/iman/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/num2fa/
+-rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.93/iman/num2fa/__init__.py
+-rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.93/iman/num2fa/__main__.py
+-rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.93/iman/par.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/pyctcdecode/
+-rw-rw-rw-   0        0        0      265 2023-07-11 05:28:53.000000 iman-0.0.93/iman/pyctcdecode/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-07-11 05:28:53.000000 iman-0.0.93/iman/pyctcdecode/alphabet.py
+-rw-rw-rw-   0        0        0      617 2023-07-11 05:28:53.000000 iman-0.0.93/iman/pyctcdecode/constants.py
+-rw-rw-rw-   0        0        0    29784 2023-07-19 12:40:28.000000 iman-0.0.93/iman/pyctcdecode/decoder.py
+-rw-rw-rw-   0        0        0    11420 2023-07-11 05:28:53.000000 iman-0.0.93/iman/pyctcdecode/language_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/sad_tf/
+-rw-rw-rw-   0        0        0      101 2023-07-23 07:12:34.000000 iman-0.0.93/iman/sad_tf/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-07-17 06:10:42.000000 iman-0.0.93/iman/sad_tf/export_funcs.py
+-rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.93/iman/sad_tf/features.py
+-rw-rw-rw-   0        0        0    18972 2023-07-23 07:08:02.000000 iman-0.0.93/iman/sad_tf/segmenter.py
+-rw-rw-rw-   0        0        0    20025 2023-07-23 08:03:31.000000 iman-0.0.93/iman/sad_tf/segmentero.py
+-rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.93/iman/sad_tf/sidekit_mfcc.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_tf/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.93/iman/sad_tf/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_tf/viterbi_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/sad_torch_mfcc/
+-rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.93/iman/sad_torch_mfcc/__init__.py
+-rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.93/iman/sad_torch_mfcc/export_funcs.py
+-rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.93/iman/sad_torch_mfcc/features.py
+-rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.93/iman/sad_torch_mfcc/sad_model.py
+-rw-rw-rw-   0        0        0    19324 2023-07-22 04:57:05.000000 iman-0.0.93/iman/sad_torch_mfcc/segmenter.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_torch_mfcc/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.93/iman/sad_torch_mfcc/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_torch_mfcc/viterbi_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/
+-rw-rw-rw-   0        0        0       36 2023-07-26 06:11:13.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-07-26 06:41:32.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/features.py
+-rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/sad_model.py
+-rw-rw-rw-   0        0        0    10232 2023-07-26 07:10:07.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/segmenter.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.93/iman/sad_torch_mfcc_speaker/viterbi_utils.py
+-rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.93/iman/tsne.py
+-rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.93/iman/web.py
+-rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.93/iman/xvector.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/
+-rw-rw-rw-   0        0        0     6963 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2067 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 07:13:34.000000 iman-0.0.93/iman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:13:34.000000 iman-0.0.93/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-07-26 07:10:19.000000 iman-0.0.93/setup.py
```

### Comparing `iman-0.0.92/PKG-INFO` & `iman-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.92
+Version: 0.0.93
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
@@ -216,14 +216,15 @@
 wav_speech , wav_noise = filter_sig(isig , wav , sr) ``Get Speech and Noise Parts of file - Do when complete_output=False``
 
 from sad_tf.segmentero import Segmenter ``to use onnx models - need to install onnxruntime``
 
 from iman.sad_torch_mfcc_speaker import *
 ================================================
 seg = Segmenter(batch_size, vad_type=['sad'|'vad'] , sr=8000 , model_path="c:\\sad_model_pytorch.pth" , max_time=120 , tq=1,ffmpeg_path='c:\\ffmpeg.exe', device='cuda')  ``TORCH - max_time in second to split fea output``
+mfcc = seg(fname) 
 
 from iman import Report   ``Tensorboard Writer``
 ==================================================
 r=Report.rep(log_dir=None)
 
 r.WS(_type , _name , value , itr)  ``Add_scalar``
```

### Comparing `iman-0.0.92/README.rst` & `iman-0.0.93/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 wav_speech , wav_noise = filter_sig(isig , wav , sr) ``Get Speech and Noise Parts of file - Do when complete_output=False``
 
 from sad_tf.segmentero import Segmenter ``to use onnx models - need to install onnxruntime``
 
 from iman.sad_torch_mfcc_speaker import *
 ================================================
 seg = Segmenter(batch_size, vad_type=['sad'|'vad'] , sr=8000 , model_path="c:\\sad_model_pytorch.pth" , max_time=120 , tq=1,ffmpeg_path='c:\\ffmpeg.exe', device='cuda')  ``TORCH - max_time in second to split fea output``
+mfcc = seg(fname) 
 
 from iman import Report   ``Tensorboard Writer``
 ==================================================
 r=Report.rep(log_dir=None)
 
 r.WS(_type , _name , value , itr)  ``Add_scalar``
```

### Comparing `iman-0.0.92/iman/AUG.py` & `iman-0.0.93/iman/AUG.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Audio.py` & `iman-0.0.93/iman/Audio.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Features/mfcc/LS.py` & `iman-0.0.93/iman/Features/mfcc/LS.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Features/mfcc/SB.py` & `iman-0.0.93/iman/Features/mfcc/SB.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Features/mfcc/getmfcc_from_librosa.py` & `iman-0.0.93/iman/Features/mfcc/getmfcc_from_librosa.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Features/mfcc/sb_mfcc_class.py` & `iman-0.0.93/iman/Features/mfcc/sb_mfcc_class.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Image.py` & `iman-0.0.93/iman/Image.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Report.py` & `iman-0.0.93/iman/Report.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/Text.py` & `iman-0.0.93/iman/Text.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/__init__.py` & `iman-0.0.93/iman/__init__.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/examples.py` & `iman-0.0.93/iman/examples.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/examples_folder/age.py` & `iman-0.0.93/iman/examples_folder/age.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/examples_folder/pyworldd.py` & `iman-0.0.93/iman/examples_folder/pyworldd.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/examples_folder/save_docx.py` & `iman-0.0.93/iman/examples_folder/save_docx.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/gpu_info.py` & `iman-0.0.93/iman/gpu_info.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/info.py` & `iman-0.0.93/iman/info.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/metrics.py` & `iman-0.0.93/iman/metrics.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/num2fa/__init__.py` & `iman-0.0.93/iman/num2fa/__init__.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/pyctcdecode/alphabet.py` & `iman-0.0.93/iman/pyctcdecode/alphabet.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/pyctcdecode/constants.py` & `iman-0.0.93/iman/pyctcdecode/constants.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/pyctcdecode/decoder.py` & `iman-0.0.93/iman/pyctcdecode/decoder.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/pyctcdecode/language_model.py` & `iman-0.0.93/iman/pyctcdecode/language_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/export_funcs.py` & `iman-0.0.93/iman/sad_tf/export_funcs.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/features.py` & `iman-0.0.93/iman/sad_tf/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/segmenter.py` & `iman-0.0.93/iman/sad_tf/segmenter.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/segmentero.py` & `iman-0.0.93/iman/sad_tf/segmentero.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/sidekit_mfcc.py` & `iman-0.0.93/iman/sad_tf/sidekit_mfcc.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/thread_returning.py` & `iman-0.0.93/iman/sad_tf/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/viterbi.py` & `iman-0.0.93/iman/sad_tf/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_tf/viterbi_utils.py` & `iman-0.0.93/iman/sad_tf/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/export_funcs.py` & `iman-0.0.93/iman/sad_torch_mfcc/export_funcs.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/features.py` & `iman-0.0.93/iman/sad_torch_mfcc/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/sad_model.py` & `iman-0.0.93/iman/sad_torch_mfcc/sad_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/segmenter.py` & `iman-0.0.93/iman/sad_torch_mfcc/segmenter.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/thread_returning.py` & `iman-0.0.93/iman/sad_torch_mfcc/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/viterbi.py` & `iman-0.0.93/iman/sad_torch_mfcc/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc/viterbi_utils.py` & `iman-0.0.93/iman/sad_torch_mfcc/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/features.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/sad_model.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/sad_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/segmenter.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/segmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,17 +273,15 @@
                  break
 
               if start_sec is None:
                   start_sec = 0
               
               speech_len , isii = self.segment_feats(mspec, loge, start_sec)
              
-              print(isii)
               spee = spee + speech_len
-              print(spee)
               
               if (spee >=  self.max_time):
                   p = just_filter(isii , mspec.squeeze() , sr = self.sample_rate )
                   if (p!=[]):
                     last_mfcc.append(p)
                   return torch.cat(last_mfcc)[0:max_frame,:]
               else:
```

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/thread_returning.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/viterbi.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/sad_torch_mfcc_speaker/viterbi_utils.py` & `iman-0.0.93/iman/sad_torch_mfcc_speaker/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/web.py` & `iman-0.0.93/iman/web.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman/xvector.py` & `iman-0.0.93/iman/xvector.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/iman.egg-info/PKG-INFO` & `iman-0.0.93/iman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.92
+Version: 0.0.93
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
@@ -216,14 +216,15 @@
 wav_speech , wav_noise = filter_sig(isig , wav , sr) ``Get Speech and Noise Parts of file - Do when complete_output=False``
 
 from sad_tf.segmentero import Segmenter ``to use onnx models - need to install onnxruntime``
 
 from iman.sad_torch_mfcc_speaker import *
 ================================================
 seg = Segmenter(batch_size, vad_type=['sad'|'vad'] , sr=8000 , model_path="c:\\sad_model_pytorch.pth" , max_time=120 , tq=1,ffmpeg_path='c:\\ffmpeg.exe', device='cuda')  ``TORCH - max_time in second to split fea output``
+mfcc = seg(fname) 
 
 from iman import Report   ``Tensorboard Writer``
 ==================================================
 r=Report.rep(log_dir=None)
 
 r.WS(_type , _name , value , itr)  ``Add_scalar``
```

### Comparing `iman-0.0.92/iman.egg-info/SOURCES.txt` & `iman-0.0.93/iman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iman-0.0.92/setup.py` & `iman-0.0.93/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
         # the name must match the folder name 'verysimplemodule'
         name="iman", 
-        version='0.0.92',
+        version='0.0.93',
         author="Iman Sarraf",
         author_email="imansarraf@gmail.com",
         description='Python package for daily Tasks',
         long_description=read('README.rst'),
         packages=find_packages(),
         
         # add any additional packages that
```

