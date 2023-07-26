# Comparing `tmp/micrologai-1.3.1.tar.gz` & `tmp/micrologai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologai-1.3.1.tar", last modified: Wed Jul 26 08:17:05 2023, max compression
+gzip compressed data, was "micrologai-1.3.2.tar", last modified: Wed Jul 26 09:45:55 2023, max compression
```

## Comparing `micrologai-1.3.1.tar` & `micrologai-1.3.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.442721 micrologai-1.3.1/
--rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.1/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.1/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 08:17:05.446925 micrologai-1.3.1/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)    10207 2023-07-26 08:16:40.000000 micrologai-1.3.1/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.808576 micrologai-1.3.1/dashboard/
--rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    11727 2023-07-26 07:42:00.000000 micrologai-1.3.1/dashboard/canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.1/dashboard/colors.py
--rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     8238 2023-07-19 15:09:18.000000 micrologai-1.3.1/dashboard/design.py
--rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/dialog.py
--rw-r--r--   0 laffra     (501) staff       (20)    26036 2023-07-25 12:33:02.000000 micrologai-1.3.1/dashboard/index.html
--rw-r--r--   0 laffra     (501) staff       (20)    12322 2023-07-26 07:43:07.000000 micrologai-1.3.1/dashboard/main.py
--rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/markdown.py
--rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.1/dashboard/profiler.py
--rw-r--r--   0 laffra     (501) staff       (20)     2209 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/tips.py
--rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/treeview.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.839363 micrologai-1.3.1/dashboard/views/
--rw-r--r--   0 laffra     (501) staff       (20)     2030 2023-07-25 13:02:17.000000 micrologai-1.3.1/dashboard/views/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    15757 2023-07-25 12:57:55.000000 micrologai-1.3.1/dashboard/views/call.py
--rw-r--r--   0 laffra     (501) staff       (20)     4455 2023-07-25 12:55:41.000000 micrologai-1.3.1/dashboard/views/marker.py
--rw-r--r--   0 laffra     (501) staff       (20)     4579 2023-07-25 12:55:32.000000 micrologai-1.3.1/dashboard/views/status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/views/timeline.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.932722 micrologai-1.3.1/examples/
--rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.1/examples/binaryTrees.py
--rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.1/examples/books.json
--rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.1/examples/bookstore.py
--rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.1/examples/dataframes.py
--rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.1/examples/example.py
--rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.1/examples/files.py
--rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.1/examples/go.py
--rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.1/examples/helloworld.py
--rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.1/examples/memory.py
--rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.1/examples/modules.py
--rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.1/examples/runall.sh
--rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.1/examples/startstop.py
--rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.1/examples/threads.py
--rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.1/examples/treemap.ipynb
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.994934 micrologai-1.3.1/microlog/
--rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-26 07:44:34.000000 micrologai-1.3.1/microlog/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.1/microlog/api.py
--rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.1/microlog/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.1/microlog/explain.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.177801 micrologai-1.3.1/microlog/images/
--rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.1/microlog/images/anomaly.png
--rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.1/microlog/images/apple-touch-icon.png
--rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.1/microlog/images/chatgpt.png
--rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.1/microlog/images/design-go.png
--rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/dialog.png
--rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/error-log.png
--rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.1/microlog/images/favicon-16x16.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.1/microlog/images/favicon-32x32.png
--rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.1/microlog/images/fd-leak.png
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.334321 micrologai-1.3.1/microlog/images/icons/
--rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.1/microlog/images/icons/asyncio.png
--rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.1/microlog/images/icons/dataclasses.png
--rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.1/microlog/images/icons/email.png
--rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.1/microlog/images/icons/google.png
--rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.1/microlog/images/icons/guppy.png
--rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.1/microlog/images/icons/http.png
--rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.1/microlog/images/icons/jupyter.png
--rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.1/microlog/images/icons/matplotlib.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.1/microlog/images/icons/microlog.png
--rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.1/microlog/images/icons/networkx.png
--rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.1/microlog/images/icons/numpy.png
--rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.1/microlog/images/icons/pandas.png
--rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.1/microlog/images/icons/pyparsing.png
--rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.1/microlog/images/icons/pytest.png
--rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.1/microlog/images/icons/python.png
--rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.1/microlog/images/icons/re.png
--rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.1/microlog/images/icons/squarify.png
--rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.1/microlog/images/icons/ssl.png
--rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.1/microlog/images/icons/tornado.png
--rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.1/microlog/images/icons/urllib.png
--rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.1/microlog/images/icons/wsgi.png
--rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.1/microlog/images/icons/zmq.png
--rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.1/microlog/images/log.png
--rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.1/microlog/images/logo-bing.png
--rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.1/microlog/images/logo-brave.png
--rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.1/microlog/images/logo-duckduckgo.png
--rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.1/microlog/images/logo-google.png
--rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.1/microlog/images/logo-hackernews.png
--rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.1/microlog/images/logo-sourcegraph.png
--rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.1/microlog/images/logo-stackoverflow.png
--rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.1/microlog/images/logo-twitter.png
--rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.1/microlog/images/markdown.png
--rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.1/microlog/images/memory-leak.png
--rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.1/microlog/images/overview.png
--rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.1/microlog/images/spinner.png
--rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/status.png
--rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.1/microlog/images/tips.png
--rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.1/microlog/images/zoomedin.png
--rw-r--r--   0 laffra     (501) staff       (20)     4873 2023-07-24 11:05:10.000000 micrologai-1.3.1/microlog/log.py
--rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.1/microlog/models.py
--rw-r--r--   0 laffra     (501) staff       (20)     6238 2023-07-24 12:56:21.000000 micrologai-1.3.1/microlog/server.py
--rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.1/microlog/sitecustomize.py
--rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.1/microlog/tracer.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.375231 micrologai-1.3.1/micrologai.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     2789 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/entry_points.txt
--rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-26 07:44:28.000000 micrologai-1.3.1/pyproject.toml
--rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-26 08:17:05.455852 micrologai-1.3.1/setup.cfg
--rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-26 07:44:29.000000 micrologai-1.3.1/setup.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.437653 micrologai-1.3.1/tests/
--rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.1/tests/test_call_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.1/tests/test_canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.1/tests/test_log.py
--rw-r--r--   0 laffra     (501) staff       (20)     1832 2023-07-04 08:31:09.000000 micrologai-1.3.1/tests/test_marker_view.py
--rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.1/tests/test_print.py
--rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.1/tests/test_status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.1/tests/test_status_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.1/tests/test_tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.364992 micrologai-1.3.2/
+-rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.2/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.2/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 09:45:55.367812 micrologai-1.3.2/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)    10207 2023-07-26 08:16:40.000000 micrologai-1.3.2/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.723538 micrologai-1.3.2/dashboard/
+-rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    11820 2023-07-26 08:52:27.000000 micrologai-1.3.2/dashboard/canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.2/dashboard/colors.py
+-rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     8238 2023-07-19 15:09:18.000000 micrologai-1.3.2/dashboard/design.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/dialog.py
+-rw-r--r--   0 laffra     (501) staff       (20)    26036 2023-07-25 12:33:02.000000 micrologai-1.3.2/dashboard/index.html
+-rw-r--r--   0 laffra     (501) staff       (20)    12685 2023-07-26 09:27:45.000000 micrologai-1.3.2/dashboard/main.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/markdown.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.2/dashboard/profiler.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2209 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/tips.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/treeview.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.753858 micrologai-1.3.2/dashboard/views/
+-rw-r--r--   0 laffra     (501) staff       (20)     2165 2023-07-26 09:43:49.000000 micrologai-1.3.2/dashboard/views/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    15240 2023-07-26 09:28:44.000000 micrologai-1.3.2/dashboard/views/call.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4826 2023-07-26 09:30:34.000000 micrologai-1.3.2/dashboard/views/marker.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4441 2023-07-26 09:31:18.000000 micrologai-1.3.2/dashboard/views/status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.2/dashboard/views/timeline.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.849261 micrologai-1.3.2/examples/
+-rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.2/examples/binaryTrees.py
+-rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.2/examples/books.json
+-rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.2/examples/bookstore.py
+-rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.2/examples/dataframes.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.2/examples/example.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.2/examples/files.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.2/examples/go.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.2/examples/helloworld.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.2/examples/memory.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.2/examples/modules.py
+-rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.2/examples/runall.sh
+-rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.2/examples/startstop.py
+-rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.2/examples/threads.py
+-rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.2/examples/treemap.ipynb
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:54.916238 micrologai-1.3.2/microlog/
+-rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-26 09:45:34.000000 micrologai-1.3.2/microlog/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.2/microlog/api.py
+-rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.2/microlog/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.2/microlog/explain.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.087185 micrologai-1.3.2/microlog/images/
+-rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.2/microlog/images/anomaly.png
+-rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.2/microlog/images/apple-touch-icon.png
+-rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.2/microlog/images/chatgpt.png
+-rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.2/microlog/images/design-go.png
+-rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/dialog.png
+-rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/error-log.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.2/microlog/images/favicon-16x16.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.2/microlog/images/favicon-32x32.png
+-rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.2/microlog/images/fd-leak.png
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.252718 micrologai-1.3.2/microlog/images/icons/
+-rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.2/microlog/images/icons/asyncio.png
+-rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.2/microlog/images/icons/dataclasses.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.2/microlog/images/icons/email.png
+-rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.2/microlog/images/icons/google.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.2/microlog/images/icons/guppy.png
+-rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.2/microlog/images/icons/http.png
+-rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.2/microlog/images/icons/jupyter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.2/microlog/images/icons/matplotlib.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.2/microlog/images/icons/microlog.png
+-rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.2/microlog/images/icons/networkx.png
+-rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.2/microlog/images/icons/numpy.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.2/microlog/images/icons/pandas.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.2/microlog/images/icons/pyparsing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.2/microlog/images/icons/pytest.png
+-rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.2/microlog/images/icons/python.png
+-rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.2/microlog/images/icons/re.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.2/microlog/images/icons/squarify.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.2/microlog/images/icons/ssl.png
+-rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.2/microlog/images/icons/tornado.png
+-rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.2/microlog/images/icons/urllib.png
+-rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.2/microlog/images/icons/wsgi.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.2/microlog/images/icons/zmq.png
+-rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.2/microlog/images/log.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.2/microlog/images/logo-bing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.2/microlog/images/logo-brave.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.2/microlog/images/logo-duckduckgo.png
+-rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.2/microlog/images/logo-google.png
+-rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.2/microlog/images/logo-hackernews.png
+-rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.2/microlog/images/logo-sourcegraph.png
+-rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.2/microlog/images/logo-stackoverflow.png
+-rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.2/microlog/images/logo-twitter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.2/microlog/images/markdown.png
+-rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.2/microlog/images/memory-leak.png
+-rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.2/microlog/images/overview.png
+-rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.2/microlog/images/spinner.png
+-rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.2/microlog/images/status.png
+-rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.2/microlog/images/tips.png
+-rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.2/microlog/images/zoomedin.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4873 2023-07-24 11:05:10.000000 micrologai-1.3.2/microlog/log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.2/microlog/models.py
+-rw-r--r--   0 laffra     (501) staff       (20)     6238 2023-07-24 12:56:21.000000 micrologai-1.3.2/microlog/server.py
+-rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.2/microlog/sitecustomize.py
+-rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.2/microlog/tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.297272 micrologai-1.3.2/micrologai.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     2789 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/entry_points.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-26 09:45:54.000000 micrologai-1.3.2/micrologai.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-26 09:45:34.000000 micrologai-1.3.2/pyproject.toml
+-rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-26 09:45:55.375461 micrologai-1.3.2/setup.cfg
+-rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-26 09:45:34.000000 micrologai-1.3.2/setup.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 09:45:55.362493 micrologai-1.3.2/tests/
+-rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.2/tests/test_call_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.2/tests/test_canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.2/tests/test_log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1755 2023-07-26 09:43:39.000000 micrologai-1.3.2/tests/test_marker_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.2/tests/test_print.py
+-rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.2/tests/test_status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.2/tests/test_status_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.2/tests/test_tracer.py
```

### Comparing `micrologai-1.3.1/LICENSE` & `micrologai-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/PKG-INFO` & `micrologai-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.1
+Version: 1.3.2
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
```

### Comparing `micrologai-1.3.1/README.md` & `micrologai-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/canvas.py` & `micrologai-1.3.2/dashboard/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,22 @@
         self._height = float(self.canvas.attr("height") or js.jQuery("body").height())
         self.scaleX = self.scaleY = config.CANVAS_INITIAL_SCALE
         self.offsetX = config.CANVAS_INITIAL_OFFSET_X
         self.offsetY = config.CANVAS_INITIAL_OFFSET_Y
 
     @profiler.profile("Canvas.width")
     def width(self, width=0):
-        return self.canvas.attr("width", width) if width else self._width
+        if width:
+            self._width = width
+            self.canvas.attr("width", width)
+        else:
+            return self._width
 
     def height(self, height=0):
-        return self.canvas.attr("height", height) if height else self._width
+        return self.canvas.attr("height", height) if height else float(self.canvas.attr("height") or 0)
 
     @profiler.profile("Canvas.toScreenX")
     def toScreenX(self, x):
         return x * self.scaleX + self.offsetX
 
     def fromScreenX(self, x):
         return x - self.offsetX / self.scaleX
```

### Comparing `micrologai-1.3.1/dashboard/colors.py` & `micrologai-1.3.2/dashboard/colors.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/config.py` & `micrologai-1.3.2/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/design.py` & `micrologai-1.3.2/dashboard/design.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/dialog.py` & `micrologai-1.3.2/dashboard/dialog.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/index.html` & `micrologai-1.3.2/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/main.py` & `micrologai-1.3.2/dashboard/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,19 +147,30 @@
         """
 
     @profiler.profile("Flamegraph.draw")
     def draw(self):
         self.flameCanvas.clear("#DDD")
         self.timelineCanvas.clear("#DDD")
         self.hover = None
-        width = self.flameCanvas.width()
-        StatusView.drawAll(self.timelineCanvas, [view for view in self.sampleStatuses() if not view.offscreen(width)])
+        canvasScaleX = self.flameCanvas.scaleX
+        canvasOffsetX = self.flameCanvas.offsetX
+        canvasWidth = self.flameCanvas.width()
+        StatusView.drawAll(self.timelineCanvas, [
+            view for view in self.sampleStatuses()
+            if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
+        ])
         self.timeline.draw(self.timelineCanvas)
-        CallView.drawAll(self.flameCanvas, [view for view in self.calls if not view.offscreen(width)])
-        MarkerView.drawAll(self.timelineCanvas, [view for view in self.markers if not view.offscreen(width)])
+        CallView.drawAll(self.flameCanvas, [
+            view for view in self.calls
+            if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
+        ])
+        MarkerView.drawAll(self.timelineCanvas, [
+            view for view in self.markers 
+            if not view.offscreen(canvasScaleX, canvasOffsetX, canvasWidth)
+        ])
         
     def sampleStatuses(self):
         if not self.statuses: 
             return []
         statuses = [ self.statuses[0] ]
         sample = int(max(1, 1 / self.flameCanvas.scaleX / 4))
         for n in range(len(self.statuses)):
@@ -176,16 +187,17 @@
         self.mousemoveCanvas(self.timelineCanvas, self.statuses, event)
         self.mousemoveCanvas(self.timelineCanvas, self.markers, event)
     
     def mousemoveCanvas(self, canvas, views, event):
         if canvas.isDragging() or not hasattr(event.originalEvent, "offsetX"):
             return
         x, y, _, _ = canvas.absolute(event.originalEvent.offsetX, event.originalEvent.offsetY)
+        w = canvas.width()
         for view in views:
-            if view.inside(x, y):
+            if not view.offscreen(w) and view.inside(x, y):
                 if not self.hover is view:
                     if self.hover:
                         self.hover.mouseleave(x, y)
                     view.mouseenter(x, y)
                     self.hover = view
                 view.mousemove(x, y)
```

### Comparing `micrologai-1.3.1/dashboard/markdown.py` & `micrologai-1.3.2/dashboard/markdown.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/profiler.py` & `micrologai-1.3.2/dashboard/profiler.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/tips.py` & `micrologai-1.3.2/dashboard/tips.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/treeview.py` & `micrologai-1.3.2/dashboard/treeview.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/dashboard/views/__init__.py` & `micrologai-1.3.2/dashboard/views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,18 +41,14 @@
 
     def __eq__(self, other):
         return not self is other
 
     def draw(self):
         pass
 
-    def drawIfVisible(self):
-        if not self.offscreen():
-            self.draw()
-
     def mouseenter(self, x, y):
         self.canvas.css("cursor", "pointer")
 
     def mousemove(self, x, y):
         pass
 
     def click(self, x, y):
@@ -61,20 +57,30 @@
     def mouseleave(self, x, y):
         self.canvas.css("cursor", "default")
 
     def __getattr__(self, name: str):
         return getattr(self.model, name)
         
     def inside(self, x, y):
-        return not self.offscreen() and x >= self.x and x < self.x + self.w and y >= self.y and y < self.y + self.h
+        return x >= self.x and x < self.x + self.w and y >= self.y and y < self.y + self.h
         
-    def offscreen(self):
-        x = self.canvas.toScreenX(self.x)
-        w = self.canvas.toScreenDimension(self.w)
-        return w < 3 or x + w < 0 or x > self.canvas.width()
+    def offscreen(self, scaleX, offsetX, width):
+        x = self.x * scaleX + offsetX
+        w = self.w * scaleX
+        return w < 2 or x + w < 0 or x > width
+    
+    def getFullName(self):
+        return self.callSite.name
+    
+    def getShortName(self):
+        parts = self.callSite.name.split(".")
+        name = parts[-1]
+        if name == "<module>":
+            name = parts[-2] or parts[-3]
+        return name
 
     def modifyColor(self, color, offset):
         rgb_hex = [color[x:x+2] for x in [1, 3, 5]]
         new_rgb_int = [
             int(min(255, max(0, int(hex_value, 16) + offset)))
             for hex_value in rgb_hex
         ]
```

### Comparing `micrologai-1.3.1/dashboard/views/call.py` & `micrologai-1.3.2/dashboard/views/call.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,30 +144,14 @@
         if w > 0:
             self.canvas.fillRect(self.x, self.y, self.w, self.h - 1, fill)
             self.canvas.line(self.x, self.y, self.x + self.w, self.y, 1, "#DDD")
             self.canvas.line(self.x, self.y, self.x, self.y + self.h, 1, "#AAA")
         if w > self.minWidth:
             dx = self.canvas.fromScreenDimension(4)
             self.canvas.text(self.x + dx, self.y + 2, self.getLabel(), color, self.w - 2 * dx)
- 
-    def offscreen(self, canvasWidth=0):
-        canvasWidth = canvasWidth or self.canvas.width()
-        x = self.x * self.canvas.scaleX + self.canvas.offsetX
-        w = self.w * self.canvas.scaleX
-        return w < 2 or x + w < 0 or x > canvasWidth
-    
-    def getFullName(self):
-        return self.callSite.name
-    
-    def getShortName(self):
-        parts = self.callSite.name.split(".")
-        name = parts[-1]
-        if name == "<module>":
-            name = parts[-2] or parts[-3]
-        return name
 
     def click(self, x, y):
         self.showPopup(x, y)
 
     def showPopup(self, x, y):
         if self.canvas.isDragging():
             return
```

### Comparing `micrologai-1.3.1/dashboard/views/marker.py` & `micrologai-1.3.2/dashboard/views/marker.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,33 +52,45 @@
         MarkerView.instances.clear()
 
     @classmethod
     @profiler.profile("MarkerView.drawAll")
     def drawAll(cls, canvas, markers):
         for marker in markers:
             marker.draw()
+
+    def getFullName(self):
+        return self.callSite.name
+    
+    def getShortName(self):
+        parts = self.callSite.name.split(".")
+        name = parts[-1]
+        if name == "<module>":
+            name = parts[-2] or parts[-3]
+        return name
  
-    def offscreen(self, canvasWidth=0):
-        canvasWidth = canvasWidth or self.canvas.width()
-        x = self.x * self.canvas.scaleX + self.canvas.offsetX
-        w = self.w * self.canvas.scaleX
-        return w < 2 or x + w < 0 or x > canvasWidth
+    @profiler.profile("Marker.offscreen")
+    def offscreen(self, scaleX, offsetX, width):
+        self.x = self.when * config.PIXELS_PER_SECOND - self.canvas.fromScreenDimension(18)
+        self.y = 105 - self.offset[self.kind]
+        self.w = self.canvas.fromScreenDimension(36)
+        return View.offscreen(self, scaleX, offsetX, width)
     
     @profiler.profile("Marker.draw")
     def draw(self):
         self.x = self.when * config.PIXELS_PER_SECOND - self.canvas.fromScreenDimension(18)
         self.y = 105 - self.offset[self.kind]
         self.w = self.canvas.fromScreenDimension(36)
         self.canvas.image(self.x, self.y, self.w, self.h, self.image, "#666", 3)
 
     def mouseenter(self, x, y):
         View.mouseenter(self, x, y)
         self.select()
     
     def select(self):
+        self.draw()
         self.canvas.rect(self.x, self.y, self.w, self.h, color="white")
 
     def mouseleave(self, x, y):
         View.mouseleave(self, x, y)
         self.canvas.redraw()
 
     def formatStack(self, full=True):
@@ -91,15 +103,15 @@
             return f"<a href=vscode://file/{callSite.filename}:{callSite.lineno}:1>{shortFile(callSite.filename)}:{callSite.lineno}</a>\n"
         return ''.join([
               addLink(callSite)
               for callSite in self.stack
         ])
 
     def click(self, x, y):
-        self.canvas.redraw()
+        # self.canvas.redraw()
         self.select()
         formattedStack = self.formatStack()
         stack = f"""
             <h2>Callstack</h2>
             <pre>{formattedStack}</pre>
         """ if formattedStack else ""
```

### Comparing `micrologai-1.3.1/dashboard/views/status.py` & `micrologai-1.3.2/dashboard/views/status.py`

 * *Files 17% similar despite different names*

```diff
@@ -84,21 +84,19 @@
             y = round(Y - getValue(status) * (H - offset * 2) / (maxValue + 1) - 5)
             if len(points) > 2 and points[-1][1] == points[-2][1] == y:
                 points.pop()
             points.append((x, y))
         return points
 
     @profiler.profile("View.offscreen")
-    def offscreen(self, canvasWidth=0):
-        canvasWidth = canvasWidth or self.canvas.width()
-        x = self.x * self.canvas.scaleX + self.canvas.offsetX
-        w = self.w * self.canvas.scaleX
-        offset = self.canvas.scaleX * canvasWidth / 2
-        offscreen = x + w < -offset or x > canvasWidth + offset
-        return offscreen
+    def offscreen(self, scaleX, offsetX, width):
+        x = self.x * scaleX + offsetX
+        w = self.w * scaleX
+        offset = scaleX * width / 2
+        return x + w < -offset or x > width + offset
 
     def mousemove(self, x, y):
         cpu = (self.previous.cpu + self.cpu) / 2 if self.previous else self.cpu
         rows = f"""
             <tr class="header"><td>Metric</td><td>Value</td><td>Line Color</td></tr>
             <tr><td>CPU</td> <td>{round(cpu)}%</td> <td>Green</td> </tr>
             <tr><td>Module Count</td> <td>{self.moduleCount:,}</td> <td>Yellow</td></tr>
```

### Comparing `micrologai-1.3.1/dashboard/views/timeline.py` & `micrologai-1.3.2/dashboard/views/timeline.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/binaryTrees.py` & `micrologai-1.3.2/examples/binaryTrees.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/books.json` & `micrologai-1.3.2/examples/books.json`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/bookstore.py` & `micrologai-1.3.2/examples/bookstore.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/dataframes.py` & `micrologai-1.3.2/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/example.py` & `micrologai-1.3.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/files.py` & `micrologai-1.3.2/examples/files.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/go.py` & `micrologai-1.3.2/examples/go.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/helloworld.py` & `micrologai-1.3.2/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/memory.py` & `micrologai-1.3.2/examples/memory.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/modules.py` & `micrologai-1.3.2/examples/modules.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/startstop.py` & `micrologai-1.3.2/examples/startstop.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/threads.py` & `micrologai-1.3.2/examples/threads.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/examples/treemap.ipynb` & `micrologai-1.3.2/examples/treemap.ipynb`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/api.py` & `micrologai-1.3.2/microlog/api.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/config.py` & `micrologai-1.3.2/microlog/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/explain.py` & `micrologai-1.3.2/microlog/explain.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/anomaly.png` & `micrologai-1.3.2/microlog/images/anomaly.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/apple-touch-icon.png` & `micrologai-1.3.2/microlog/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/chatgpt.png` & `micrologai-1.3.2/microlog/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/design-go.png` & `micrologai-1.3.2/microlog/images/design-go.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/dialog.png` & `micrologai-1.3.2/microlog/images/dialog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/error-log.png` & `micrologai-1.3.2/microlog/images/error-log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/favicon-32x32.png` & `micrologai-1.3.2/microlog/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/fd-leak.png` & `micrologai-1.3.2/microlog/images/fd-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/asyncio.png` & `micrologai-1.3.2/microlog/images/icons/asyncio.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/dataclasses.png` & `micrologai-1.3.2/microlog/images/icons/dataclasses.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/email.png` & `micrologai-1.3.2/microlog/images/icons/email.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/google.png` & `micrologai-1.3.2/microlog/images/icons/google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/guppy.png` & `micrologai-1.3.2/microlog/images/icons/guppy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/http.png` & `micrologai-1.3.2/microlog/images/icons/http.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/jupyter.png` & `micrologai-1.3.2/microlog/images/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/matplotlib.png` & `micrologai-1.3.2/microlog/images/icons/matplotlib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/microlog.png` & `micrologai-1.3.2/microlog/images/icons/microlog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/networkx.png` & `micrologai-1.3.2/microlog/images/icons/networkx.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/numpy.png` & `micrologai-1.3.2/microlog/images/icons/numpy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/pandas.png` & `micrologai-1.3.2/microlog/images/icons/pandas.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/pyparsing.png` & `micrologai-1.3.2/microlog/images/icons/pyparsing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/pytest.png` & `micrologai-1.3.2/microlog/images/icons/pytest.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/python.png` & `micrologai-1.3.2/microlog/images/icons/python.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/re.png` & `micrologai-1.3.2/microlog/images/icons/re.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/squarify.png` & `micrologai-1.3.2/microlog/images/icons/squarify.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/ssl.png` & `micrologai-1.3.2/microlog/images/icons/ssl.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/tornado.png` & `micrologai-1.3.2/microlog/images/icons/tornado.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/urllib.png` & `micrologai-1.3.2/microlog/images/icons/urllib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/wsgi.png` & `micrologai-1.3.2/microlog/images/icons/wsgi.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/icons/zmq.png` & `micrologai-1.3.2/microlog/images/icons/zmq.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/log.png` & `micrologai-1.3.2/microlog/images/log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-bing.png` & `micrologai-1.3.2/microlog/images/logo-bing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-brave.png` & `micrologai-1.3.2/microlog/images/logo-brave.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-duckduckgo.png` & `micrologai-1.3.2/microlog/images/logo-duckduckgo.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-google.png` & `micrologai-1.3.2/microlog/images/logo-google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-hackernews.png` & `micrologai-1.3.2/microlog/images/logo-hackernews.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-sourcegraph.png` & `micrologai-1.3.2/microlog/images/logo-sourcegraph.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-stackoverflow.png` & `micrologai-1.3.2/microlog/images/logo-stackoverflow.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/logo-twitter.png` & `micrologai-1.3.2/microlog/images/logo-twitter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/markdown.png` & `micrologai-1.3.2/microlog/images/markdown.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/memory-leak.png` & `micrologai-1.3.2/microlog/images/memory-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/overview.png` & `micrologai-1.3.2/microlog/images/overview.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/status.png` & `micrologai-1.3.2/microlog/images/status.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/tips.png` & `micrologai-1.3.2/microlog/images/tips.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/images/zoomedin.png` & `micrologai-1.3.2/microlog/images/zoomedin.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/log.py` & `micrologai-1.3.2/microlog/log.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/models.py` & `micrologai-1.3.2/microlog/models.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/server.py` & `micrologai-1.3.2/microlog/server.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/sitecustomize.py` & `micrologai-1.3.2/microlog/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/microlog/tracer.py` & `micrologai-1.3.2/microlog/tracer.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/micrologai.egg-info/PKG-INFO` & `micrologai-1.3.2/micrologai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.1
+Version: 1.3.2
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
```

### Comparing `micrologai-1.3.1/micrologai.egg-info/SOURCES.txt` & `micrologai-1.3.2/micrologai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/pyproject.toml` & `micrologai-1.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micrologai"
-version = "1.3.1"
+version = "1.3.2"
 description = "A continuous profiler and logger for Python written entirely in Python"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `micrologai-1.3.1/setup.py` & `micrologai-1.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='Microlog',
     description='A continuous profiler and logger for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.1',
+    version="1.3.2",
     author='Chris Laffra',
     author_email='laffra@gmail.com',
     url='https://www.chrislaffra.org/',
     packages=setuptools.find_packages(include=[
         'microlog',
         'dashboard',
     ]),
```

### Comparing `micrologai-1.3.1/tests/test_call_view.py` & `micrologai-1.3.2/tests/test_call_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/tests/test_canvas.py` & `micrologai-1.3.2/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/tests/test_marker_view.py` & `micrologai-1.3.2/tests/test_marker_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,19 @@
         self.assertEqual(len(log.log.markers), 25)
         self.marker.draw()
         self.assertTrue(mock_image.called)
 
     @unittest.mock.patch('dashboard.canvas.Canvas.toScreenDimension', return_value=10)
     @unittest.mock.patch('dashboard.canvas.Canvas.width', return_value=1000)
     def test_offscreen_negative(self, mock_toScreenDimension, mock_width):
-        self.canvas.width = lambda: 1000
-        self.marker.x = self.canvas.fromScreenX(-25)
-        self.marker.w = self.canvas.fromScreenDimension(10)
-        self.assertTrue(self.marker.offscreen())
+        self.canvas.offsetX = -100
+        self.assertTrue(self.marker.offscreen(self.canvas.scaleX, self.canvas.offsetX, self.canvas.width()))
 
     @unittest.mock.patch('dashboard.canvas.Canvas.toScreenDimension', return_value=10)
     @unittest.mock.patch('dashboard.canvas.Canvas.width', return_value=1000)
     def test_offscreen_positive(self, mock_toScreenDimension, mock_width):
-        self.marker.x = self.canvas.fromScreenX(25)
-        self.marker.w = self.canvas.fromScreenDimension(10)
-        self.assertFalse(self.marker.offscreen())
+        self.canvas.offsetX = 2000
+        self.assertTrue(self.marker.offscreen(self.canvas.scaleX, self.canvas.offsetX, self.canvas.width()))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `micrologai-1.3.1/tests/test_print.py` & `micrologai-1.3.2/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/tests/test_status.py` & `micrologai-1.3.2/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/tests/test_status_view.py` & `micrologai-1.3.2/tests/test_status_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.1/tests/test_tracer.py` & `micrologai-1.3.2/tests/test_tracer.py`

 * *Files identical despite different names*

