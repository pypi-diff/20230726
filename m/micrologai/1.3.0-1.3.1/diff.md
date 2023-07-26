# Comparing `tmp/micrologai-1.3.0.tar.gz` & `tmp/micrologai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologai-1.3.0.tar", last modified: Wed Jul 19 14:53:33 2023, max compression
+gzip compressed data, was "micrologai-1.3.1.tar", last modified: Wed Jul 26 08:17:05 2023, max compression
```

## Comparing `micrologai-1.3.0.tar` & `micrologai-1.3.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.727920 micrologai-1.3.0/
--rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.0/LICENSE
--rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.0/MANIFEST.in
--rw-r--r--   0 laffra     (501) staff       (20)    53507 2023-07-19 14:53:33.730585 micrologai-1.3.0/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)    17867 2023-07-19 14:53:08.000000 micrologai-1.3.0/README.md
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.147562 micrologai-1.3.0/dashboard/
--rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    11639 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      810 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/colors.py
--rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     8238 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/design.py
--rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/dialog.py
--rw-r--r--   0 laffra     (501) staff       (20)    25768 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/index.html
--rw-r--r--   0 laffra     (501) staff       (20)    12115 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/main.py
--rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/markdown.py
--rw-r--r--   0 laffra     (501) staff       (20)     1710 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/profiler.py
--rw-r--r--   0 laffra     (501) staff       (20)     2209 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/tips.py
--rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/treeview.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.180956 micrologai-1.3.0/dashboard/views/
--rw-r--r--   0 laffra     (501) staff       (20)     1960 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/views/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)    15665 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/views/call.py
--rw-r--r--   0 laffra     (501) staff       (20)     4410 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/views/marker.py
--rw-r--r--   0 laffra     (501) staff       (20)     4534 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/views/status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.0/dashboard/views/timeline.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.272411 micrologai-1.3.0/examples/
--rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.0/examples/binaryTrees.py
--rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.0/examples/books.json
--rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.0/examples/bookstore.py
--rw-r--r--   0 laffra     (501) staff       (20)      998 2023-06-16 15:47:16.000000 micrologai-1.3.0/examples/dataframes.py
--rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-04-22 08:58:25.000000 micrologai-1.3.0/examples/example.py
--rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.0/examples/files.py
--rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-04-22 09:38:55.000000 micrologai-1.3.0/examples/go.py
--rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.0/examples/helloworld.py
--rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.0/examples/memory.py
--rw-r--r--   0 laffra     (501) staff       (20)      577 2023-07-12 16:18:40.000000 micrologai-1.3.0/examples/modules.py
--rwxr-xr-x   0 laffra     (501) staff       (20)      412 2023-07-09 20:45:30.000000 micrologai-1.3.0/examples/runall.sh
--rw-r--r--   0 laffra     (501) staff       (20)      799 2023-07-04 08:45:39.000000 micrologai-1.3.0/examples/startstop.py
--rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.0/examples/threads.py
--rw-r--r--   0 laffra     (501) staff       (20)    96592 2023-07-12 16:16:24.000000 micrologai-1.3.0/examples/treemap.ipynb
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.328015 micrologai-1.3.0/microlog/
--rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-19 14:37:59.000000 micrologai-1.3.0/microlog/__init__.py
--rw-r--r--   0 laffra     (501) staff       (20)     2914 2023-07-19 12:56:01.000000 micrologai-1.3.0/microlog/api.py
--rw-r--r--   0 laffra     (501) staff       (20)      798 2023-07-19 12:56:01.000000 micrologai-1.3.0/microlog/config.py
--rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.0/microlog/explain.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.496643 micrologai-1.3.0/microlog/images/
--rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.0/microlog/images/anomaly.png
--rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.0/microlog/images/apple-touch-icon.png
--rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.0/microlog/images/chatgpt.png
--rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.0/microlog/images/design-go.png
--rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.0/microlog/images/dialog.png
--rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.0/microlog/images/error-log.png
--rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.0/microlog/images/favicon-16x16.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.0/microlog/images/favicon-32x32.png
--rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.0/microlog/images/fd-leak.png
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.640817 micrologai-1.3.0/microlog/images/icons/
--rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.0/microlog/images/icons/asyncio.png
--rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.0/microlog/images/icons/dataclasses.png
--rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.0/microlog/images/icons/email.png
--rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.0/microlog/images/icons/google.png
--rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.0/microlog/images/icons/guppy.png
--rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.0/microlog/images/icons/http.png
--rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.0/microlog/images/icons/jupyter.png
--rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.0/microlog/images/icons/matplotlib.png
--rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.0/microlog/images/icons/microlog.png
--rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.0/microlog/images/icons/networkx.png
--rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.0/microlog/images/icons/numpy.png
--rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.0/microlog/images/icons/pandas.png
--rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.0/microlog/images/icons/pyparsing.png
--rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.0/microlog/images/icons/pytest.png
--rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.0/microlog/images/icons/python.png
--rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.0/microlog/images/icons/re.png
--rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.0/microlog/images/icons/squarify.png
--rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.0/microlog/images/icons/ssl.png
--rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.0/microlog/images/icons/tornado.png
--rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.0/microlog/images/icons/urllib.png
--rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.0/microlog/images/icons/wsgi.png
--rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.0/microlog/images/icons/zmq.png
--rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.0/microlog/images/log.png
--rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.0/microlog/images/logo-bing.png
--rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.0/microlog/images/logo-brave.png
--rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.0/microlog/images/logo-duckduckgo.png
--rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.0/microlog/images/logo-google.png
--rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.0/microlog/images/logo-hackernews.png
--rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.0/microlog/images/logo-sourcegraph.png
--rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.0/microlog/images/logo-stackoverflow.png
--rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.0/microlog/images/logo-twitter.png
--rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.0/microlog/images/markdown.png
--rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.0/microlog/images/memory-leak.png
--rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.0/microlog/images/overview.png
--rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.0/microlog/images/spinner.png
--rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.0/microlog/images/status.png
--rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.0/microlog/images/tips.png
--rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.0/microlog/images/zoomedin.png
--rw-r--r--   0 laffra     (501) staff       (20)     5426 2023-07-19 12:59:46.000000 micrologai-1.3.0/microlog/log.py
--rw-r--r--   0 laffra     (501) staff       (20)     9778 2023-07-19 12:56:01.000000 micrologai-1.3.0/microlog/models.py
--rw-r--r--   0 laffra     (501) staff       (20)     6112 2023-07-19 13:37:43.000000 micrologai-1.3.0/microlog/server.py
--rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.0/microlog/sitecustomize.py
--rw-r--r--   0 laffra     (501) staff       (20)    17142 2023-07-19 12:56:01.000000 micrologai-1.3.0/microlog/tracer.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.676938 micrologai-1.3.0/micrologai.egg-info/
--rw-r--r--   0 laffra     (501) staff       (20)    53507 2023-07-19 14:53:32.000000 micrologai-1.3.0/micrologai.egg-info/PKG-INFO
--rw-r--r--   0 laffra     (501) staff       (20)     2789 2023-07-19 14:53:33.000000 micrologai-1.3.0/micrologai.egg-info/SOURCES.txt
--rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-19 14:53:32.000000 micrologai-1.3.0/micrologai.egg-info/dependency_links.txt
--rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-19 14:53:32.000000 micrologai-1.3.0/micrologai.egg-info/entry_points.txt
--rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-19 14:53:33.000000 micrologai-1.3.0/micrologai.egg-info/requires.txt
--rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-19 14:53:33.000000 micrologai-1.3.0/micrologai.egg-info/top_level.txt
--rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-19 14:51:16.000000 micrologai-1.3.0/pyproject.toml
--rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-19 14:53:33.737317 micrologai-1.3.0/setup.cfg
--rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-19 14:37:56.000000 micrologai-1.3.0/setup.py
-drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-19 14:53:33.725348 micrologai-1.3.0/tests/
--rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.0/tests/test_call_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.0/tests/test_canvas.py
--rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.0/tests/test_log.py
--rw-r--r--   0 laffra     (501) staff       (20)     1832 2023-07-04 08:31:09.000000 micrologai-1.3.0/tests/test_marker_view.py
--rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.0/tests/test_print.py
--rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.0/tests/test_status.py
--rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.0/tests/test_status_view.py
--rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.0/tests/test_tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.442721 micrologai-1.3.1/
+-rw-r--r--   0 laffra     (501) staff       (20)    30607 2023-07-05 22:06:54.000000 micrologai-1.3.1/LICENSE
+-rw-r--r--   0 laffra     (501) staff       (20)      213 2023-07-19 13:43:23.000000 micrologai-1.3.1/MANIFEST.in
+-rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 08:17:05.446925 micrologai-1.3.1/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)    10207 2023-07-26 08:16:40.000000 micrologai-1.3.1/README.md
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.808576 micrologai-1.3.1/dashboard/
+-rw-r--r--   0 laffra     (501) staff       (20)       75 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    11727 2023-07-26 07:42:00.000000 micrologai-1.3.1/dashboard/canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      864 2023-07-25 13:00:57.000000 micrologai-1.3.1/dashboard/colors.py
+-rw-r--r--   0 laffra     (501) staff       (20)      699 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     8238 2023-07-19 15:09:18.000000 micrologai-1.3.1/dashboard/design.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1854 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/dialog.py
+-rw-r--r--   0 laffra     (501) staff       (20)    26036 2023-07-25 12:33:02.000000 micrologai-1.3.1/dashboard/index.html
+-rw-r--r--   0 laffra     (501) staff       (20)    12322 2023-07-26 07:43:07.000000 micrologai-1.3.1/dashboard/main.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1800 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/markdown.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1799 2023-07-25 13:09:32.000000 micrologai-1.3.1/dashboard/profiler.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2209 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/tips.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4245 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/treeview.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.839363 micrologai-1.3.1/dashboard/views/
+-rw-r--r--   0 laffra     (501) staff       (20)     2030 2023-07-25 13:02:17.000000 micrologai-1.3.1/dashboard/views/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)    15757 2023-07-25 12:57:55.000000 micrologai-1.3.1/dashboard/views/call.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4455 2023-07-25 12:55:41.000000 micrologai-1.3.1/dashboard/views/marker.py
+-rw-r--r--   0 laffra     (501) staff       (20)     4579 2023-07-25 12:55:32.000000 micrologai-1.3.1/dashboard/views/status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2152 2023-07-19 12:55:56.000000 micrologai-1.3.1/dashboard/views/timeline.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.932722 micrologai-1.3.1/examples/
+-rw-r--r--   0 laffra     (501) staff       (20)     1758 2023-06-08 14:12:55.000000 micrologai-1.3.1/examples/binaryTrees.py
+-rw-r--r--   0 laffra     (501) staff       (20)    24814 2023-04-22 19:02:44.000000 micrologai-1.3.1/examples/books.json
+-rw-r--r--   0 laffra     (501) staff       (20)     2213 2023-07-08 19:41:25.000000 micrologai-1.3.1/examples/bookstore.py
+-rw-r--r--   0 laffra     (501) staff       (20)      998 2023-07-24 09:17:39.000000 micrologai-1.3.1/examples/dataframes.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1417 2023-07-24 08:53:57.000000 micrologai-1.3.1/examples/example.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1021 2023-07-12 07:42:28.000000 micrologai-1.3.1/examples/files.py
+-rw-r--r--   0 laffra     (501) staff       (20)    13859 2023-07-25 12:36:42.000000 micrologai-1.3.1/examples/go.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1857 2023-06-15 09:37:09.000000 micrologai-1.3.1/examples/helloworld.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1127 2023-07-08 12:02:09.000000 micrologai-1.3.1/examples/memory.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1178 2023-07-24 10:45:34.000000 micrologai-1.3.1/examples/modules.py
+-rwxr-xr-x   0 laffra     (501) staff       (20)      410 2023-07-24 11:06:15.000000 micrologai-1.3.1/examples/runall.sh
+-rw-r--r--   0 laffra     (501) staff       (20)      913 2023-07-24 13:11:27.000000 micrologai-1.3.1/examples/startstop.py
+-rw-r--r--   0 laffra     (501) staff       (20)      631 2023-06-08 16:27:45.000000 micrologai-1.3.1/examples/threads.py
+-rw-r--r--   0 laffra     (501) staff       (20)    93813 2023-07-24 11:09:29.000000 micrologai-1.3.1/examples/treemap.ipynb
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:04.994934 micrologai-1.3.1/microlog/
+-rw-r--r--   0 laffra     (501) staff       (20)      302 2023-07-26 07:44:34.000000 micrologai-1.3.1/microlog/__init__.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2798 2023-07-24 11:03:18.000000 micrologai-1.3.1/microlog/api.py
+-rw-r--r--   0 laffra     (501) staff       (20)      769 2023-07-24 11:11:41.000000 micrologai-1.3.1/microlog/config.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3431 2023-07-19 12:56:01.000000 micrologai-1.3.1/microlog/explain.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.177801 micrologai-1.3.1/microlog/images/
+-rw-r--r--   0 laffra     (501) staff       (20)   292932 2023-07-12 16:09:27.000000 micrologai-1.3.1/microlog/images/anomaly.png
+-rw-rw-r--   0 laffra     (501) staff       (20)     7246 2023-04-21 09:21:45.000000 micrologai-1.3.1/microlog/images/apple-touch-icon.png
+-rw-r--r--   0 laffra     (501) staff       (20)    91386 2023-07-12 16:45:27.000000 micrologai-1.3.1/microlog/images/chatgpt.png
+-rw-r--r--   0 laffra     (501) staff       (20)   218816 2023-07-12 16:24:41.000000 micrologai-1.3.1/microlog/images/design-go.png
+-rw-r--r--   0 laffra     (501) staff       (20)   222723 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/dialog.png
+-rw-r--r--   0 laffra     (501) staff       (20)   227072 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/error-log.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      423 2023-04-21 09:21:34.000000 micrologai-1.3.1/microlog/images/favicon-16x16.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-21 09:21:34.000000 micrologai-1.3.1/microlog/images/favicon-32x32.png
+-rw-r--r--   0 laffra     (501) staff       (20)   160359 2023-07-12 16:32:21.000000 micrologai-1.3.1/microlog/images/fd-leak.png
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.334321 micrologai-1.3.1/microlog/images/icons/
+-rw-r--r--   0 laffra     (501) staff       (20)    14969 2023-04-25 09:23:09.000000 micrologai-1.3.1/microlog/images/icons/asyncio.png
+-rw-r--r--   0 laffra     (501) staff       (20)    31709 2023-04-25 10:02:27.000000 micrologai-1.3.1/microlog/images/icons/dataclasses.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23729 2023-04-27 10:35:43.000000 micrologai-1.3.1/microlog/images/icons/email.png
+-rw-r--r--   0 laffra     (501) staff       (20)   204541 2023-04-27 10:32:24.000000 micrologai-1.3.1/microlog/images/icons/google.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1533 2023-04-25 10:35:56.000000 micrologai-1.3.1/microlog/images/icons/guppy.png
+-rw-r--r--   0 laffra     (501) staff       (20)   129197 2023-04-25 10:51:41.000000 micrologai-1.3.1/microlog/images/icons/http.png
+-rw-r--r--   0 laffra     (501) staff       (20)    37752 2023-04-24 18:36:39.000000 micrologai-1.3.1/microlog/images/icons/jupyter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   198202 2023-04-24 18:31:13.000000 micrologai-1.3.1/microlog/images/icons/matplotlib.png
+-rw-rw-r--   0 laffra     (501) staff       (20)      830 2023-04-24 18:23:52.000000 micrologai-1.3.1/microlog/images/icons/microlog.png
+-rw-r--r--   0 laffra     (501) staff       (20)    17540 2023-04-24 18:44:11.000000 micrologai-1.3.1/microlog/images/icons/networkx.png
+-rw-r--r--   0 laffra     (501) staff       (20)    29693 2023-04-24 18:19:33.000000 micrologai-1.3.1/microlog/images/icons/numpy.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4625 2023-04-24 18:22:51.000000 micrologai-1.3.1/microlog/images/icons/pandas.png
+-rw-r--r--   0 laffra     (501) staff       (20)     1532 2023-04-25 09:29:26.000000 micrologai-1.3.1/microlog/images/icons/pyparsing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     7209 2023-04-25 09:59:48.000000 micrologai-1.3.1/microlog/images/icons/pytest.png
+-rw-r--r--   0 laffra     (501) staff       (20)    24301 2023-04-24 18:42:54.000000 micrologai-1.3.1/microlog/images/icons/python.png
+-rw-r--r--   0 laffra     (501) staff       (20)    26832 2023-04-25 10:30:25.000000 micrologai-1.3.1/microlog/images/icons/re.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4223 2023-04-25 09:54:17.000000 micrologai-1.3.1/microlog/images/icons/squarify.png
+-rw-r--r--   0 laffra     (501) staff       (20)    23401 2023-04-25 10:49:22.000000 micrologai-1.3.1/microlog/images/icons/ssl.png
+-rw-r--r--   0 laffra     (501) staff       (20)    73176 2023-04-24 18:34:02.000000 micrologai-1.3.1/microlog/images/icons/tornado.png
+-rw-r--r--   0 laffra     (501) staff       (20)      694 2023-04-25 10:42:25.000000 micrologai-1.3.1/microlog/images/icons/urllib.png
+-rw-r--r--   0 laffra     (501) staff       (20)    63526 2023-04-27 10:38:44.000000 micrologai-1.3.1/microlog/images/icons/wsgi.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9088 2023-04-25 09:25:52.000000 micrologai-1.3.1/microlog/images/icons/zmq.png
+-rw-r--r--   0 laffra     (501) staff       (20)   158577 2023-07-12 16:28:13.000000 micrologai-1.3.1/microlog/images/log.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39070 2023-07-08 10:22:16.000000 micrologai-1.3.1/microlog/images/logo-bing.png
+-rw-r--r--   0 laffra     (501) staff       (20)     9392 2023-07-08 10:09:42.000000 micrologai-1.3.1/microlog/images/logo-brave.png
+-rw-r--r--   0 laffra     (501) staff       (20)    39117 2023-07-08 10:21:00.000000 micrologai-1.3.1/microlog/images/logo-duckduckgo.png
+-rw-r--r--   0 laffra     (501) staff       (20)    55096 2023-07-08 10:06:59.000000 micrologai-1.3.1/microlog/images/logo-google.png
+-rw-r--r--   0 laffra     (501) staff       (20)    11762 2023-07-08 10:24:53.000000 micrologai-1.3.1/microlog/images/logo-hackernews.png
+-rw-r--r--   0 laffra     (501) staff       (20)    10721 2023-07-08 10:22:58.000000 micrologai-1.3.1/microlog/images/logo-sourcegraph.png
+-rw-r--r--   0 laffra     (501) staff       (20)    20187 2023-07-08 10:25:37.000000 micrologai-1.3.1/microlog/images/logo-stackoverflow.png
+-rw-r--r--   0 laffra     (501) staff       (20)    95279 2023-07-08 10:25:22.000000 micrologai-1.3.1/microlog/images/logo-twitter.png
+-rw-r--r--   0 laffra     (501) staff       (20)   241629 2023-04-11 09:10:24.000000 micrologai-1.3.1/microlog/images/markdown.png
+-rw-r--r--   0 laffra     (501) staff       (20)   171389 2023-07-12 16:38:49.000000 micrologai-1.3.1/microlog/images/memory-leak.png
+-rw-r--r--   0 laffra     (501) staff       (20)   184418 2023-07-12 10:42:50.000000 micrologai-1.3.1/microlog/images/overview.png
+-rw-r--r--   0 laffra     (501) staff       (20)      262 2023-05-03 09:04:18.000000 micrologai-1.3.1/microlog/images/spinner.png
+-rw-r--r--   0 laffra     (501) staff       (20)    68422 2023-04-10 13:38:11.000000 micrologai-1.3.1/microlog/images/status.png
+-rw-r--r--   0 laffra     (501) staff       (20)   122085 2023-07-12 16:48:20.000000 micrologai-1.3.1/microlog/images/tips.png
+-rw-r--r--   0 laffra     (501) staff       (20)   187519 2023-07-12 10:57:11.000000 micrologai-1.3.1/microlog/images/zoomedin.png
+-rw-r--r--   0 laffra     (501) staff       (20)     4873 2023-07-24 11:05:10.000000 micrologai-1.3.1/microlog/log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     9743 2023-07-24 10:08:40.000000 micrologai-1.3.1/microlog/models.py
+-rw-r--r--   0 laffra     (501) staff       (20)     6238 2023-07-24 12:56:21.000000 micrologai-1.3.1/microlog/server.py
+-rw-r--r--   0 laffra     (501) staff       (20)      538 2023-07-19 13:49:13.000000 micrologai-1.3.1/microlog/sitecustomize.py
+-rw-r--r--   0 laffra     (501) staff       (20)    17190 2023-07-24 10:07:20.000000 micrologai-1.3.1/microlog/tracer.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.375231 micrologai-1.3.1/micrologai.egg-info/
+-rw-r--r--   0 laffra     (501) staff       (20)    45847 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/PKG-INFO
+-rw-r--r--   0 laffra     (501) staff       (20)     2789 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/SOURCES.txt
+-rw-r--r--   0 laffra     (501) staff       (20)        1 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/dependency_links.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       48 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/entry_points.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       41 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/requires.txt
+-rw-r--r--   0 laffra     (501) staff       (20)       19 2023-07-26 08:17:04.000000 micrologai-1.3.1/micrologai.egg-info/top_level.txt
+-rw-r--r--   0 laffra     (501) staff       (20)      893 2023-07-26 07:44:28.000000 micrologai-1.3.1/pyproject.toml
+-rw-r--r--   0 laffra     (501) staff       (20)       79 2023-07-26 08:17:05.455852 micrologai-1.3.1/setup.cfg
+-rw-r--r--   0 laffra     (501) staff       (20)     1560 2023-07-26 07:44:29.000000 micrologai-1.3.1/setup.py
+drwxr-xr-x   0 laffra     (501) staff       (20)        0 2023-07-26 08:17:05.437653 micrologai-1.3.1/tests/
+-rw-r--r--   0 laffra     (501) staff       (20)     1970 2023-07-03 09:26:47.000000 micrologai-1.3.1/tests/test_call_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1326 2023-06-25 13:55:44.000000 micrologai-1.3.1/tests/test_canvas.py
+-rw-r--r--   0 laffra     (501) staff       (20)      318 2023-06-21 13:19:34.000000 micrologai-1.3.1/tests/test_log.py
+-rw-r--r--   0 laffra     (501) staff       (20)     1832 2023-07-04 08:31:09.000000 micrologai-1.3.1/tests/test_marker_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)      920 2023-06-21 12:59:07.000000 micrologai-1.3.1/tests/test_print.py
+-rw-r--r--   0 laffra     (501) staff       (20)      727 2023-07-02 20:31:07.000000 micrologai-1.3.1/tests/test_status.py
+-rw-r--r--   0 laffra     (501) staff       (20)     2071 2023-07-02 20:45:33.000000 micrologai-1.3.1/tests/test_status_view.py
+-rw-r--r--   0 laffra     (501) staff       (20)     3265 2023-07-02 20:24:48.000000 micrologai-1.3.1/tests/test_tracer.py
```

### Comparing `micrologai-1.3.0/LICENSE` & `micrologai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/PKG-INFO` & `micrologai-1.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.0
+Version: 1.3.1
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -569,261 +569,78 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # microlog.ai
 
-_Microlog_ is a continuous profiler and logger for the Python language.
-Logs and performance profiles are collected and analyzed.
-_Microlog_ explains application behavior using interactive graphs.
-It summarizes and explains the code using AI.
-
-_Microlog_ makes understanding complex applications easy, reducing support costs
+_Microlog_ is a continuous profiler and logger for the Python language that
+explains application behavior using interactive graphs and AI. 
+It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
+_Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
+It saves logs and performance profiles on the local file system. The logs are
+compressed exceptionally well, resulting in a remarkably low 0.5MB per hour of recording.
+
+This project is written in 100% Python. The recorder is a Python module that uses a separate thread to sample 
+performance and record logs. The UI is written in Python as well, rendered in the browser by Python code using
+PyScript. As a result, the identical Python classes encode _and_ decode the recordings, avoiding the need
+for cumbersome cross-language data modeling. 
+
+_Microlog_ is open source, with an available commercial license. We welcome extensions to _Microlog_ from
+the Python performance community, such as 
+recording of special events, new optimizations related to PyScript,
+or centralization of recordings into central storage systems, using `rsync`, `scp`, or `Google Drive`.
+
 # Installing microlog.ai
 
 To install _Microlog_ from pypi run:
-```
-python3 -m pip install microlog
+```console
+pip install micrologai
 ```
 
 To install _Microlog_ globally using a `sitecustomize.py`, run:
 
-```
-  git clone https://github.com/micrologai/microlog
-  cd micrologai/microlog
-  python3 setup.py install
+```console
+git3 clone https://github.com/micrologai/microlog
+cd micrologai/microlog
+python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, 
-any time a Python process runs using the same runtime you used to setup _Microlog_, it will automatically trigger _Microlog_ to generate a recording. 
+If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
 
 To use microlog manually, use:
-```
-  import microlog
-
-  with microlog.enabled():
-      # run any Python code
-```
-
-To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
-
-```
-  sh examples/runall.sh
-```
-
-This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
-
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
-```
-
-This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
-you can start it as follows:
-
-```
-  python3 microlog/server.py
-```
-
-# The Microlog.ai UI 
-
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
-
-The main elements of the UI are:
-
- - `Log list`, at the left, showing currently available logs on the local machine.
- - `Timeline`, the starting point for analysis of your application:
-    - `Status`, providing insights into CPU, memory, and I/O.
-    - `Timescale`, with ticks for second elapsed since start.
-    - `Flamegraph`, showing the result of the continuous profiler. 
- - `Design`, showing a graphical rendering of the structure of the application.
- - `Log`, listing all print and logging output and statistics in a chronological order.
- - `Explanation`, giving a human language description of your code, using OpenAIs' ChatGPT.
- - `Tips`, linking to best practices and tips for the modules used in your code.
-
-
-## Timeline Navigation and Zoom
-
-Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
-
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
-
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
-
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
-
-## Timeline Anomaly Detection
-
-When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
-
-Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
-
-![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
-
-## Timeline Detecting expensive I/O or Starved Processes
-
-The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
-Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
-
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
-
-## Timeline Integrating Profiling with Logging
-
-Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
-
-![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
-
-## Formatting Logs with Markdown
-
-Log entries can be formatted using Markdown to make it easier to show important information to the reader.
-
-![Using markdown for log entries](https://github.com/micrologai/microlog/raw/main/microlog/images/markdown.png)
-
-# Logging 
-
-_Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
-added to the _Microlog_ event log.  
-
-Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
-
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
-
-   import logging
-   logger = logging.Logger("Microlog Demo")
-
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
-   
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
-```
-
-# Design
-
-The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
-Here is an example for `examples\go.py`:
+import microlog
 
-![Microlog's innovative design graph](https://github.com/micrologai/microlog/raw/main/microlog/images/design-go.png)
-
-# Log
-
-The log tab contains a chronological listing of all print and logging output, statistics, and analysis performed by _Microlog_ in a more traditional linear log style:
-
-![Microlog's traditional log, with a twist](https://github.com/micrologai/microlog/raw/main/microlog/images/log.png)
-
-The links shown in lightblue directly take you to the source file where the print took place. This makes it extremely easy to figure out what code prints what exactly. For the `files.py` example, the log shows that this program leaked one file descriptor. That same report is also shown in the timeline when you click at the warning icon at the end of the run. 
-The popup also shows a link to the source location where the file was opened:
-
-![Detecting leaked file descriptors](https://github.com/micrologai/microlog/raw/main/microlog/images/fd-leak.png)
-
-## Log - Memory Leaks
-
-In addition to checking for leaked file descriptors, _Microlog_ aims to detect memory leaks. Those objects that were
-allocated but cannot be garbage-collected as they are either reachable from a module or are involed in a reference cycle that
-cannot be broken. The following report shows the top-10 offenders for the `dataframes.py` example, that uses Pandas dataframes.
-
-![Detecting memory leaks](https://github.com/micrologai/microlog/raw/main/microlog/images/memory-leak.png)
-
-# Explanation
-
-The explanation tab shows a human-language explanation provided by OpenAI's `ChatGPT` to explain the design and implementation behind the application being monitored by _Microlog_. This analysis is not performed on the source code, but on a condensed call graph generated from the performance log that was recorded by _Microlog_. Here is an example of the what `ChatGPT` thinks of
-our `examples\go.py` execution:
-
-![ChatGPT's simple explanation of complex Python code](https://github.com/micrologai/microlog/raw/main/microlog/images/chatgpt.png)
-
-# Tips
-
-To discover best practices, performance tips, or tutorials for modules being used by the application, _Microlog_ offers quick
-links to general information sources, such as search engines and Q&A sites:
-
-![Tips make you a better Python developer](https://github.com/micrologai/microlog/raw/main/microlog/images/tips.png)
-
-
-# Developer Notes
-
-## Run all unit tests
-
-```
-python3 -m unittest discover tests
+with microlog.enabled():
+    # run any Python code
 ```
 
+To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
-## Upload new version to PyPi
-
-First build the package into a source distribution and a Python wheel:
-```
-python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
-```
-
-Then verify whether the build works for pypi:
-```
-twine check dist/*
-```
-
-Then upload to the pypi test environment:
-```
-twine upload --repository pypitest dist/*
-```
-
-```
-twine upload dist/*
-```
-
-# License
-
-
-
-## Run all examples
-
-```
+```console
 sh examples/runall.sh
 ```
 
-# License
-
-_Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
-
-
-
-To give you an idea of the features, of _Microlog_, run all the examples:
-
-```
-  sh examples/runall.sh
-```
-
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
+```console
+📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
 The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
 you can start it as follows:
 
-```
-  python3 microlog/server.py
+```console
+python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
 To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
@@ -843,35 +660,35 @@
 
 ## Timeline Navigation and Zoom
 
 Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
 
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
+In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scroll wheel on the mouse.
 
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
+In addition, we clicked on a method call in the flame graph, which is now highlighted in red. A moveable popup dialog shows details about the method, such as the average CPU during the call. A CPU percentage below 100% means the process is involved
+in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), async or thread synchronization, or other system-level event handling using `select` or event handlers. 
 
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
+A low CPU typically indicates a bottleneck and warrants in-depth investigation.
 
 ## Timeline Anomaly Detection
 
 When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
 
 Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
 
 ![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
 
 ## Timeline Detecting expensive I/O or Starved Processes
 
 The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
 Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
 
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
+![Microlog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
 
 ## Timeline Integrating Profiling with Logging
 
 Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
 
 ![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
 
@@ -885,29 +702,29 @@
 
 _Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
 added to the _Microlog_ event log.  
 
 Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
 
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
+print("Add a log entry to microlog with an info marker...")
+print("... or as an error marker.", stream=sys.stderr)
 
-   import logging
-   logger = logging.Logger("Microlog Demo")
+import logging
+logger = logging.Logger("Microlog Demo")
 
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
+logger.info("Add a log entry to microlog with an info marker...")
+logger.debug("... or a bug marker...")
+logger.warning("... or a warning marker...")
+logger.error("... or an error marker.")
    
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
+microlog.info("Add something to the log explicitly...")
+microlog.warning("... as a warning...")
+microlog.debug("... as a debug message...")
+microlog.error("... as an error.")
 ```
 
 # Design
 
 The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
 Here is an example for `examples\go.py`:
 
@@ -955,41 +772,30 @@
 python3 -m unittest discover tests
 ```
 
 
 ## Upload new version to PyPi
 
 First build the package into a source distribution and a Python wheel:
-```
+```console
 python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
+python3 -m build
 ```
 
 Then verify whether the build works for pypi:
-```
+```console
 twine check dist/*
 ```
 
 Then upload to the pypi test environment:
-```
+```console
 twine upload --repository pypitest dist/*
 ```
 
-If that looks fine, upload to the real pypi environment:
-```
+Finally, if the pypi test upload appears to work fine, run:
+```console
 twine upload dist/*
 ```
 
 # License
 
-
-
-## Run all examples
-
-```
-sh examples/runall.sh
-```
-
-# License
-
 _Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
```

### Comparing `micrologai-1.3.0/README.md` & `micrologai-1.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,256 +1,73 @@
 # microlog.ai
 
-_Microlog_ is a continuous profiler and logger for the Python language.
-Logs and performance profiles are collected and analyzed.
-_Microlog_ explains application behavior using interactive graphs.
-It summarizes and explains the code using AI.
-
-_Microlog_ makes understanding complex applications easy, reducing support costs
+_Microlog_ is a continuous profiler and logger for the Python language that
+explains application behavior using interactive graphs and AI. 
+It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
+_Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
+It saves logs and performance profiles on the local file system. The logs are
+compressed exceptionally well, resulting in a remarkably low 0.5MB per hour of recording.
+
+This project is written in 100% Python. The recorder is a Python module that uses a separate thread to sample 
+performance and record logs. The UI is written in Python as well, rendered in the browser by Python code using
+PyScript. As a result, the identical Python classes encode _and_ decode the recordings, avoiding the need
+for cumbersome cross-language data modeling. 
+
+_Microlog_ is open source, with an available commercial license. We welcome extensions to _Microlog_ from
+the Python performance community, such as 
+recording of special events, new optimizations related to PyScript,
+or centralization of recordings into central storage systems, using `rsync`, `scp`, or `Google Drive`.
+
 # Installing microlog.ai
 
 To install _Microlog_ from pypi run:
-```
-python3 -m pip install microlog
+```console
+pip install micrologai
 ```
 
 To install _Microlog_ globally using a `sitecustomize.py`, run:
 
-```
-  git clone https://github.com/micrologai/microlog
-  cd micrologai/microlog
-  python3 setup.py install
+```console
+git3 clone https://github.com/micrologai/microlog
+cd micrologai/microlog
+python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, 
-any time a Python process runs using the same runtime you used to setup _Microlog_, it will automatically trigger _Microlog_ to generate a recording. 
+If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
 
 To use microlog manually, use:
-```
-  import microlog
-
-  with microlog.enabled():
-      # run any Python code
-```
-
-To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
-
-```
-  sh examples/runall.sh
-```
-
-This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
-
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
-```
-
-This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
-you can start it as follows:
-
-```
-  python3 microlog/server.py
-```
-
-# The Microlog.ai UI 
-
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
-
-The main elements of the UI are:
-
- - `Log list`, at the left, showing currently available logs on the local machine.
- - `Timeline`, the starting point for analysis of your application:
-    - `Status`, providing insights into CPU, memory, and I/O.
-    - `Timescale`, with ticks for second elapsed since start.
-    - `Flamegraph`, showing the result of the continuous profiler. 
- - `Design`, showing a graphical rendering of the structure of the application.
- - `Log`, listing all print and logging output and statistics in a chronological order.
- - `Explanation`, giving a human language description of your code, using OpenAIs' ChatGPT.
- - `Tips`, linking to best practices and tips for the modules used in your code.
-
-
-## Timeline Navigation and Zoom
-
-Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
-
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
-
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
-
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
-
-## Timeline Anomaly Detection
-
-When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
-
-Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
-
-![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
-
-## Timeline Detecting expensive I/O or Starved Processes
-
-The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
-Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
-
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
-
-## Timeline Integrating Profiling with Logging
-
-Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
-
-![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
-
-## Formatting Logs with Markdown
-
-Log entries can be formatted using Markdown to make it easier to show important information to the reader.
-
-![Using markdown for log entries](https://github.com/micrologai/microlog/raw/main/microlog/images/markdown.png)
-
-# Logging 
-
-_Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
-added to the _Microlog_ event log.  
-
-Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
-
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
-
-   import logging
-   logger = logging.Logger("Microlog Demo")
-
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
-   
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
-```
-
-# Design
-
-The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
-Here is an example for `examples\go.py`:
+import microlog
 
-![Microlog's innovative design graph](https://github.com/micrologai/microlog/raw/main/microlog/images/design-go.png)
-
-# Log
-
-The log tab contains a chronological listing of all print and logging output, statistics, and analysis performed by _Microlog_ in a more traditional linear log style:
-
-![Microlog's traditional log, with a twist](https://github.com/micrologai/microlog/raw/main/microlog/images/log.png)
-
-The links shown in lightblue directly take you to the source file where the print took place. This makes it extremely easy to figure out what code prints what exactly. For the `files.py` example, the log shows that this program leaked one file descriptor. That same report is also shown in the timeline when you click at the warning icon at the end of the run. 
-The popup also shows a link to the source location where the file was opened:
-
-![Detecting leaked file descriptors](https://github.com/micrologai/microlog/raw/main/microlog/images/fd-leak.png)
-
-## Log - Memory Leaks
-
-In addition to checking for leaked file descriptors, _Microlog_ aims to detect memory leaks. Those objects that were
-allocated but cannot be garbage-collected as they are either reachable from a module or are involed in a reference cycle that
-cannot be broken. The following report shows the top-10 offenders for the `dataframes.py` example, that uses Pandas dataframes.
-
-![Detecting memory leaks](https://github.com/micrologai/microlog/raw/main/microlog/images/memory-leak.png)
-
-# Explanation
-
-The explanation tab shows a human-language explanation provided by OpenAI's `ChatGPT` to explain the design and implementation behind the application being monitored by _Microlog_. This analysis is not performed on the source code, but on a condensed call graph generated from the performance log that was recorded by _Microlog_. Here is an example of the what `ChatGPT` thinks of
-our `examples\go.py` execution:
-
-![ChatGPT's simple explanation of complex Python code](https://github.com/micrologai/microlog/raw/main/microlog/images/chatgpt.png)
-
-# Tips
-
-To discover best practices, performance tips, or tutorials for modules being used by the application, _Microlog_ offers quick
-links to general information sources, such as search engines and Q&A sites:
-
-![Tips make you a better Python developer](https://github.com/micrologai/microlog/raw/main/microlog/images/tips.png)
-
-
-# Developer Notes
-
-## Run all unit tests
-
-```
-python3 -m unittest discover tests
+with microlog.enabled():
+    # run any Python code
 ```
 
+To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
-## Upload new version to PyPi
-
-First build the package into a source distribution and a Python wheel:
-```
-python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
-```
-
-Then verify whether the build works for pypi:
-```
-twine check dist/*
-```
-
-Then upload to the pypi test environment:
-```
-twine upload --repository pypitest dist/*
-```
-
-```
-twine upload dist/*
-```
-
-# License
-
-
-
-## Run all examples
-
-```
+```console
 sh examples/runall.sh
 ```
 
-# License
-
-_Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
-
-
-
-To give you an idea of the features, of _Microlog_, run all the examples:
-
-```
-  sh examples/runall.sh
-```
-
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
+```console
+📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
 The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
 you can start it as follows:
 
-```
-  python3 microlog/server.py
+```console
+python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
 To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
@@ -270,35 +87,35 @@
 
 ## Timeline Navigation and Zoom
 
 Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
 
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
+In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scroll wheel on the mouse.
 
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
+In addition, we clicked on a method call in the flame graph, which is now highlighted in red. A moveable popup dialog shows details about the method, such as the average CPU during the call. A CPU percentage below 100% means the process is involved
+in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), async or thread synchronization, or other system-level event handling using `select` or event handlers. 
 
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
+A low CPU typically indicates a bottleneck and warrants in-depth investigation.
 
 ## Timeline Anomaly Detection
 
 When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
 
 Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
 
 ![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
 
 ## Timeline Detecting expensive I/O or Starved Processes
 
 The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
 Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
 
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
+![Microlog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
 
 ## Timeline Integrating Profiling with Logging
 
 Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
 
 ![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
 
@@ -312,29 +129,29 @@
 
 _Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
 added to the _Microlog_ event log.  
 
 Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
 
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
+print("Add a log entry to microlog with an info marker...")
+print("... or as an error marker.", stream=sys.stderr)
 
-   import logging
-   logger = logging.Logger("Microlog Demo")
+import logging
+logger = logging.Logger("Microlog Demo")
 
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
+logger.info("Add a log entry to microlog with an info marker...")
+logger.debug("... or a bug marker...")
+logger.warning("... or a warning marker...")
+logger.error("... or an error marker.")
    
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
+microlog.info("Add something to the log explicitly...")
+microlog.warning("... as a warning...")
+microlog.debug("... as a debug message...")
+microlog.error("... as an error.")
 ```
 
 # Design
 
 The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
 Here is an example for `examples\go.py`:
 
@@ -382,41 +199,30 @@
 python3 -m unittest discover tests
 ```
 
 
 ## Upload new version to PyPi
 
 First build the package into a source distribution and a Python wheel:
-```
+```console
 python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
+python3 -m build
 ```
 
 Then verify whether the build works for pypi:
-```
+```console
 twine check dist/*
 ```
 
 Then upload to the pypi test environment:
-```
+```console
 twine upload --repository pypitest dist/*
 ```
 
-If that looks fine, upload to the real pypi environment:
-```
+Finally, if the pypi test upload appears to work fine, run:
+```console
 twine upload dist/*
 ```
 
 # License
 
-
-
-## Run all examples
-
-```
-sh examples/runall.sh
-```
-
-# License
-
 _Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
```

### Comparing `micrologai-1.3.0/dashboard/canvas.py` & `micrologai-1.3.1/dashboard/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
 import itertools
-import math
+import json
 import js # type: ignore
+import math
 import pyodide # type: ignore
 
 import dashboard.profiler as profiler
 from dashboard import config
 
 jquery = js.jQuery
 
@@ -68,15 +69,15 @@
     def drag(self, dx, dy, event=None):
         if not self.fixedX:
             self.offsetX = self.offsetX + dx
         if not self.fixedY:
             self.offsetY = min(21, self.offsetY + dy)
         if event and self.dragCallback:
             self.dragCallback(dx, dy)
-        self.redraw()
+            self.redraw()
 
     def mouseleave(self, event):
         self.dragX = 0
         self.dragY = 0
 
     def mouseup(self, event):
         self.dragX = 0
@@ -103,15 +104,15 @@
             self.offsetX = x - (scaleFactor * (x - self.offsetX))
         if not self.fixedScaleY:
             self.offsetY = y - (scaleFactor * (y - self.offsetY))
         self.scaleX = config.CANVAS_INITIAL_SCALE if self.fixedScaleX else scaleFactor * self.scaleX
         self.scaleY = config.CANVAS_INITIAL_SCALE if self.fixedScaleY else scaleFactor * self.scaleY
         if event and self.zoomCallback:
             self.zoomCallback(x, y, scaleFactor)
-        self.redraw()
+            self.redraw()
     
     def reset(self):
         self._width = float(self.canvas.attr("width") or js.jQuery("body").width())
         self._height = float(self.canvas.attr("height") or js.jQuery("body").height())
         self.scaleX = self.scaleY = config.CANVAS_INITIAL_SCALE
         self.offsetX = config.CANVAS_INITIAL_OFFSET_X
         self.offsetY = config.CANVAS_INITIAL_OFFSET_Y
@@ -187,57 +188,57 @@
 
     @profiler.profile("Canvas.polygon")
     def polygon(self, points, lineWidth=1, color="black"):
         coordinates = itertools.chain.from_iterable([
             (x * self.scaleX + self.offsetX, y * self.scaleY + self.offsetY)
             for x, y in points
         ])
-        return js.optimizedDrawPolygon(self.context, lineWidth, color, *coordinates)
+        return js.optimizedDrawPolygon(self.context, color, lineWidth, json.dumps(list(coordinates)))
 
     @profiler.profile("Canvas.rects")
     def fillRects(self, rects):
         coordinates = itertools.chain.from_iterable([
             (
                 math.ceil(x * self.scaleX + self.offsetX),
                 math.ceil(y * self.scaleY + self.offsetY),
                 math.ceil(w * self.scaleX),
                 math.ceil(h * self.scaleY),
                 color
             )
             for x, y, w, h, color in rects
         ])
-        return js.optimizedFillRects(self.context, *coordinates)
+        return js.optimizedFillRects(self.context, json.dumps(list(coordinates)))
 
     @profiler.profile("Canvas.lines")
     def lines(self, lines, width, color):
         coordinates = itertools.chain.from_iterable([
             (
                 x1 * self.scaleX + self.offsetX,
                 y1 * self.scaleY + self.offsetY,
                 x2 * self.scaleX + self.offsetX,
                 y2 * self.scaleY + self.offsetY,
             )
             for x1, y1, x2, y2, in lines
         ])
-        return js.optimizedDrawLines(self.context, width, color, *coordinates)
+        return js.optimizedDrawLines(self.context, width, color, json.dumps(list(coordinates)))
 
     @profiler.profile("Canvas.texts")
     def texts(self, texts, font):
         coordinates = itertools.chain.from_iterable([
             (
                 x * self.scaleX + self.offsetX,
                 y * self.scaleY + self.offsetY,
                 text,
                 color,
                 w * self.scaleX,
             )
             for x, y, text, color, w in texts
         ])
         self.setFont(font)
-        return js.optimizedDrawTexts(self.context, *coordinates)
+        return js.optimizedDrawTexts(self.context, json.dumps(list(coordinates)))
 
     @profiler.profile("Canvas.rect")
     def rect(self, x:float, y:float, w:float, h:float, lineWidth=1, color="white"):
         x = math.ceil(x * self.scaleX + self.offsetX)
         y = math.ceil(y * self.scaleY + self.offsetY)
         w = math.ceil(w * self.scaleX)
         h = math.ceil(h * self.scaleY)
```

### Comparing `micrologai-1.3.0/dashboard/colors.py` & `micrologai-1.3.1/dashboard/colors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # Microlog. Copyright (c) 2023 laffra, dcharbon. All rights reserved.
 #
 
-import random
+from dashboard import profiler
 
 colors = {}
 
 CANDY = [
     "#e09550", "#e2d165", "#e0bb5a", "#dab5fc", "#e4664e",
     "#4da2f7", "#4da2f7", "#4eb28e", "#dab5fc", "#dab5fc",
 ]
@@ -26,11 +26,12 @@
     try:
         ordinals = ord(name[0]) + ord(name[round(len(name) / 2)]) + ord(name[-1])
         return ordinals % len(palette)
     except:
         return 0
 
 
+@profiler.profile("colors.getColor")
 def getColor(name, palette=PASTEL):
     if not name in colors:
         colors[name] = palette[index(name)]
     return colors[name]
```

### Comparing `micrologai-1.3.0/dashboard/config.py` & `micrologai-1.3.1/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/design.py` & `micrologai-1.3.1/dashboard/design.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/dialog.py` & `micrologai-1.3.1/dashboard/dialog.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/index.html` & `micrologai-1.3.1/dashboard/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width,initial-scale=1" />
     <title>Microlog</title>
     <script src="https://code.jquery.com/jquery-3.6.0.js"></script>
     <script src="https://code.jquery.com/ui/1.13.2/jquery-ui.js"></script>
-    <script defer src="https://pyscript.net/latest/pyscript.js"></script>
+    <script defer src="https://pyscript.net/releases/2023.05.1/pyscript.js"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/vis/4.21.0/vis.min.js"></script>
     <link rel="stylesheet" href="https://code.jquery.com/ui/1.13.2/themes/base/jquery-ui.css">
-    <link rel="stylesheet" href="https://pyscript.net/latest/pyscript.css" />
+    <link rel="stylesheet" href="https://pyscript.net/releases/2023.05.1/pyscript.css" />
     <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
 </head>
 <style>
     body {
         margin: 0;
         background: black;
     }
@@ -521,65 +521,65 @@
         ]
     </py-config>
     <script>
         $(".tabs").tabs()
 
         object = () => { }
 
-        function optimizedDrawPolygon() {
-            const context = arguments[0]
+        function optimizedDrawPolygon(context, color, lineWidth, coordinatesJson) {
+            const coordinates = JSON.parse(coordinatesJson)
             context.beginPath()
-            context.strokeStyle = arguments[2]
-            context.lineWidth = arguments[1]
-            var n = 3
-            context.moveTo(arguments[n], arguments[n + 1])
-            for (; n < arguments.length; n += 2) {
-                x = arguments[n]
-                y = arguments[n + 1]
+            context.strokeStyle = color
+            context.lineWidth = lineWidth
+            var n = 0
+            context.moveTo(coordinates[n], coordinates[n + 1])
+            for (; n < coordinates.length; n += 2) {
+                x = coordinates[n]
+                y = coordinates[n + 1]
                 context.lineTo(x, y)
             }
             context.stroke()
         }
 
-        function optimizedFillRects() {
-            const context = arguments[0]
+        function optimizedFillRects(context, coordinatesJson) {
+            const coordinates = JSON.parse(coordinatesJson)
             context.beginPath()
-            for (var n = 1; n < arguments.length; n += 5) {
-                x = arguments[n]
-                y = arguments[n + 1]
-                w = arguments[n + 2]
-                h = arguments[n + 3]
-                context.fillStyle = arguments[n + 4]
+            for (var n = 0; n < coordinates.length; n += 5) {
+                x = coordinates[n]
+                y = coordinates[n + 1]
+                w = coordinates[n + 2]
+                h = coordinates[n + 3]
+                context.fillStyle = coordinates[n + 4]
                 context.fillRect(x, y, w, h)
             }
         }
 
-        function optimizedDrawTexts() {
-            const context = arguments[0]
+        function optimizedDrawTexts(context, coordinatesJson) {
+            const coordinates = JSON.parse(coordinatesJson)
             context.beginPath()
             context.strokeStyle = "red"
-            for (var n = 1; n < arguments.length; n += 5) {
-                x = arguments[n]
-                y = arguments[n + 1]
-                text = arguments[n + 2]
-                color = arguments[n + 3]
-                w = arguments[n + 4]
+            for (var n = 0; n < coordinates.length; n += 5) {
+                x = coordinates[n]
+                y = coordinates[n + 1]
+                text = coordinates[n + 2]
+                color = coordinates[n + 3]
+                w = coordinates[n + 4]
                 context.fillStyle = color
                 context.fillText(text, x, y, w)
             }
         }
 
-        function optimizedDrawLines() {
-            const context = arguments[0]
-            context.lineWidth = arguments[1]
-            context.strokeStyle = arguments[2]
-            for (var n = 3; n < arguments.length; n += 4) {
+        function optimizedDrawLines(context, lineWidth, strokeStyle, coordinatesJson) {
+            const coordinates = JSON.parse(coordinatesJson)
+            context.lineWidth = lineWidth
+            context.strokeStyle = strokeStyle
+            for (var n = 0; n < coordinates.length; n += 4) {
                 context.beginPath()
-                context.moveTo(arguments[n], arguments[n + 1])
-                context.lineTo(arguments[n + 2], arguments[n + 3])
+                context.moveTo(coordinates[n], coordinates[n + 1])
+                context.lineTo(coordinates[n + 2], coordinates[n + 3])
                 context.stroke()
             }
         }
         
         function getUrlParameter(name) {
             const queryString = window.location.search;
             const urlParams = new URLSearchParams(queryString);
```

### Comparing `micrologai-1.3.0/dashboard/main.py` & `micrologai-1.3.1/dashboard/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,48 +78,55 @@
         self.currentTab = ui.newTab.text()
         self.redraw()
 
     def reset(self):
         self.timelineCanvas.reset()
         self.flameCanvas.reset()
 
-    @profiler.report("Flamegraph.load")
-    def load(self, log):
+    @profiler.profile("Flamegraph.convertLog")
+    def convertLog(self, log):
         self.calls = [ CallView(self.flameCanvas, model) for model in log.log.calls ]
         self.statuses = [ StatusView(self.timelineCanvas, model) for model in log.log.statuses ]
         self.markers = [ MarkerView(self.timelineCanvas, model) for model in log.log.markers ]
-        self.design = Design(self.calls)
-        self.tips = Tips(self.calls)
+
+    @profiler.profile("Flamegraph.showStatus")
+    def showStatus(self, logEntries, index):
+        if self.statuses and index < len(self.statuses):
+            logEntries.append((self.statuses[index].when, str(self.statuses[index]), ""))
+
+    @profiler.report("Flamegraph.load")
+    def load(self, log):
+        self.convertLog(log)
         statusIndex = 0
         logEntries = []
-        def showStatus(index):
-            if self.statuses and index < len(self.statuses):
-                logEntries.append((self.statuses[index].when, str(self.statuses[index]), ""))
-        showStatus(0)
+        self.showStatus(logEntries, 0)
         for marker in self.markers:
             while self.statuses[statusIndex].when < marker.when and statusIndex < len(self.statuses) - 1:
                 statusIndex += 1
             logEntries.append((marker.when, markdown.toHTML(marker.message), marker.formatStack(full=False)))
-            showStatus(statusIndex)
+            self.showStatus(logEntries, statusIndex)
         self.addLogEntries(logEntries)
-        showStatus(-1)
+        self.showStatus(logEntries, -1)
         self.hover = None
         js.jQuery(self.flameElementId).empty()
         js.jQuery(self.timelineElementId).empty()
    
-    @profiler.report("Redrawing the whole flame graph.")
+    @profiler.report("Redrawing the whole UI.")
     def redraw(self, event=None):
         if self.currentTab == "Timeline":
             self.draw()
             debug("Draw", profiler.getTime("Flamegraph.draw"))
         elif self.currentTab == "Design":
             js.jQuery("#debug").html("")
+            self.design = Design(self.calls)
             self.design.draw()
         elif self.currentTab == "Explanation":
             explain(getLogFromUrl())
+        elif self.currentTab == "Tips":
+            self.tips = Tips(self.calls)
         if event:
             self.mousemove(event) 
 
     @profiler.profile("Adding log entries.")
     def addLogEntries(self, logEntries):
         js.jQuery("#tabs-log").html(f"""
             <table>
@@ -262,17 +269,17 @@
     if not any(logList):
         js.jQuery(".logs").empty().append(js.jQuery("<span>").css("color", "pink").text("No matching logs found")),
         return
     def tree():
         return defaultdict(tree)
     logs = tree()
     for log in [log for log in reversed(logList) if log]:
-        application, version, name = log.split("/")
+        application, name = log.split("/")
         if application != "-":
-            logs[application][version][name.replace(".log", "")]
+            logs[application][name.replace(".log", "")]
     TreeView(
         js.jQuery(".logs").empty(),
         logs,
         getLogFromUrl(),
         lambda path: showLog(path),
         lambda path, doneHandler: deleteLog(path, doneHandler),
         refreshLogs
@@ -281,26 +288,26 @@
 
 flamegraph = Flamegraph("#flameCanvas", "#timelineCanvas")
 
 
 def showFlamegraph(data):
     log.log.load(data)
     js.jQuery("#debug").html("")
-    debug("Load", profiler.getTime("Flamegraph.load"))
     flamegraph.load(log)
     flamegraph.redraw()
 
 
 def debug(label: str, value=None) -> None:
     if value == None:
         message = label
     else:
         val = f"{value:.3f}" if isinstance(value, float) else value
         message = f"{label}: {val}<br>"
     js.jQuery("#debug").html(message + js.jQuery("#debug").html())
+    js.console.log(message)
     
 
 def refreshLogs(event=None):
     js.setTimeout(pyodide.ffi.create_proxy(lambda: showAllLogs()), 1)
 
 
 def setupLogHandlers():
```

### Comparing `micrologai-1.3.0/dashboard/markdown.py` & `micrologai-1.3.1/dashboard/markdown.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/profiler.py` & `micrologai-1.3.1/dashboard/profiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,18 +32,20 @@
     
 def generateReport(explanation, duration):
     print("-" * 55)
     print(explanation, f"{duration:.3}s")
     print("-" * 55)
     print("Operation                       Calls  Time")
     print("-" * 55)
-    for key in profiler.profileCount:
-        count = profiler.profileCount[key]
-        total = profiler.profileTime[key]
-        print(f"{key:30s} {count:6d} {total:6.3f}s")
+    results = sorted([
+        (key, profiler.profileCount[key], profiler.profileTime[key])
+        for key in profiler.profileCount
+    ], key=lambda item: -item[-1])
+    for key, count, duration in results:
+        print(f"{key:30s} {count:6d} {duration:6.3f}s")
     print("-" * 55)
 
 
 def profile(name):
     def decorator(function):
         def inner(*args, **argv):
             try:
```

### Comparing `micrologai-1.3.0/dashboard/tips.py` & `micrologai-1.3.1/dashboard/tips.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/treeview.py` & `micrologai-1.3.1/dashboard/treeview.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/dashboard/views/__init__.py` & `micrologai-1.3.1/dashboard/views/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import collections
 import js # type: ignore
 from typing import List
 import microlog.api as api
 from dashboard import canvas
 from dashboard import config
+from dashboard import profiler
 from dashboard.dialog import dialog
 from dashboard.views.timeline import Timeline
 
 def sanitize(text):
     return text.replace("<", "&lt;").replace("\\n", "<br>")
 
 
@@ -25,14 +26,15 @@
     model: Model = None
     canvas: canvas.Canvas
     x: float
     y: float
     w: float
     h: float
 
+    @profiler.profile("View.__init__")
     def __init__(self, canvas, model):
         self.canvas = canvas
         self.model = model
         self.x = self.when * config.PIXELS_PER_SECOND
         self.y = 0
         self.w = self.duration * config.PIXELS_PER_SECOND
         self.h = 0
```

### Comparing `micrologai-1.3.0/dashboard/views/call.py` & `micrologai-1.3.1/dashboard/views/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     model = Call
     threadIndex = defaultdict(lambda: len(CallView.threadIndex))
     showThreads = set()
     instances = []
     minWidth = 3
     selected = None
 
+    @profiler.profile("CallView.__init__")
     def __init__(self, canvas: canvas.Canvas, model: dict):
         View.__init__(self, canvas, model)
         self.h = config.LINE_HEIGHT
         self.y = self.depth * config.LINE_HEIGHT + 200 * self.getThreadIndex(self.canvas, self.threadId)
         self.color = colors.getColor(self.callSite.name)
         self.index = len(CallView.instances)
         CallView.instances.append(self)
@@ -54,14 +55,15 @@
     def reset(cls):
         CallView.instances.clear()
         CallView.selected = None
         cls.threadIndex = defaultdict(lambda: len(CallView.threadIndex))
         js.jQuery(".thread-selector").remove()
 
     @classmethod
+    @profiler.profile("CallView.getThreadIndex")
     def getThreadIndex(cls, canvas, threadId):
         if not threadId in cls.threadIndex:
             cls.showThreads.add(threadId)
             def redraw(event):
                 if threadId in cls.showThreads:
                     cls.showThreads.remove(threadId)
                 else:
```

### Comparing `micrologai-1.3.0/dashboard/views/marker.py` & `micrologai-1.3.1/dashboard/views/marker.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         api.config.EVENT_KIND_INFO:  0,
         api.config.EVENT_KIND_ERROR: 24,
         api.config.EVENT_KIND_WARN:  48,
         api.config.EVENT_KIND_DEBUG: 72,
     }
     instances = []
 
+    @profiler.profile("StatusView.__init__")
     def __init__(self, canvas, model):
         View.__init__(self, canvas, model)
         self.image = self.images[self.kind]
         self.x = self.when * config.PIXELS_PER_SECOND - self.canvas.fromScreenDimension(18)
         self.w = self.canvas.fromScreenDimension(36)
         self.h = self.canvas.fromScreenDimension(36)
         self.index = len(MarkerView.instances)
```

### Comparing `micrologai-1.3.0/dashboard/views/status.py` & `micrologai-1.3.1/dashboard/views/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from microlog.models import toGB
 from dashboard import profiler
 
 class StatusView(View):
     model = Status
     instances = []
     
+    @profiler.profile("StatusView.__init__")
     def __init__(self, canvas: canvas.Canvas, model):
         View.__init__(self, canvas, model)
         self.h = config.STATS_HEIGHT
         self.previous = None
         StatusView.instances.append(self)
 
     @classmethod
```

### Comparing `micrologai-1.3.0/dashboard/views/timeline.py` & `micrologai-1.3.1/dashboard/views/timeline.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/binaryTrees.py` & `micrologai-1.3.1/examples/binaryTrees.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/books.json` & `micrologai-1.3.1/examples/books.json`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/bookstore.py` & `micrologai-1.3.1/examples/bookstore.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/dataframes.py` & `micrologai-1.3.1/examples/dataframes.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/example.py` & `micrologai-1.3.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/files.py` & `micrologai-1.3.1/examples/files.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/go.py` & `micrologai-1.3.1/examples/go.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/helloworld.py` & `micrologai-1.3.1/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/memory.py` & `micrologai-1.3.1/examples/memory.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/startstop.py` & `micrologai-1.3.1/examples/startstop.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,33 +3,40 @@
 #
 # A Microlog example that uses start and stop
 # 
 
 import microlog
 import time
 
+
+time.sleep(0.5)
+print("This code is recorded when Microlog is set up in sitecustomize.py")
+time.sleep(0.5)
+
 #
 # Microlog can be enabled/disabled using start/stop calls.
 #
 microlog.start("examples.startstop-1")
 
-print("this statement is recorded by Microlog in log 1")
-time.sleep(0.5) # code in here is being recorded
+time.sleep(0.5)
+print("This code is recorded by Microlog in startstop-1")
+time.sleep(0.5)
 
 microlog.stop()
 
 #
 # Microlog is re-entrant and allows multiple start/stop sessions.
 # Logs are only generated when Microlog is enabled.
 #
 print("This statement is not recorded by Microlog")
 
 
 #
 # A new session can be created using a context manager. 
 #
 with microlog.enabled("examples.startstop-2"):
-    print("this statement is recorded by Microlog in log 2")
+    time.sleep(0.5)
+    print("This code is recorded by Microlog in startstop-2")
     time.sleep(0.5) 
 
 
 print("This statement is not recorded by Microlog")
```

### Comparing `micrologai-1.3.0/examples/threads.py` & `micrologai-1.3.1/examples/threads.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/examples/treemap.ipynb` & `micrologai-1.3.1/examples/treemap.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974893162393162%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['📈 Microlog ··· 2.2s ··· 4.1KB ··· ipykernel_launcher "*

 * *            "··· http://127.0.0.1:4000/log/ipykernel_launcher/0.0.0/2023_07_24_13_09_18 🚀\\n']}}}, "*

 * *            "1: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAAgMAAAGbCAYAAABZBpPkAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAfwElEQVR4nO3deXSU5f338c9khQRCgLCEJWE3QKGxqCBI8RAoUKD+UJbqoyQsWhD7A59TUORXl […]*

```diff
@@ -5,22 +5,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/Users/laffra/microlog/logs/ipykernel_launcher/0.0.0/2023_07_12_18_16_17.log\n",
-                        "------------------------------------------------------------------------------------------\n",
-                        "Microlog Statistics for ipykernel_launcher:\n",
-                        "------------------------------------------------------------------------------------------\n",
-                        "- log size:    4,430 bytes\n",
-                        "- report URL:  http://127.0.0.1:4000/log/ipykernel_launcher/0.0.0/2023_07_12_18_16_17\n",
-                        "- duration:    1.164s\n",
-                        "------------------------------------------------------------------------------------------\n"
+                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 2.2s \u00b7\u00b7\u00b7 4.1KB \u00b7\u00b7\u00b7 ipykernel_launcher \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/ipykernel_launcher/0.0.0/2023_07_24_13_09_18 \ud83d\ude80\n"
                     ]
                 }
             ],
             "source": [
                 "\n",
                 "import microlog\n",
                 "microlog.start(\"Treemap-Jupyter-Notebook\")"
@@ -29,15 +22,15 @@
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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9JKmTZumnTt3Kj09XZMnT9bYsWNVp06dQm8FnO/s2bPq16+fcnNz9eabbyokJMS7befOndqyZUup/16AS0UMwG92797tfWIvOPmsNApeuU+ZMqXYSw4LLucqEBgYWOR+Ba/cKlasqNWrVysjI0PvvPOOli9frjfeeEM33nij3nvvvWLvf7FKmsflOPcVt/Tjz2nAgAHFhlN8fLx331atWunZZ58tcr/zn+SL+z5K+v5yc3PVpUsXHT58WA899JBiY2MVHh6urKwspaSk+O2kuIEDB2rRokVat26dWrVqpaVLl2r48OHFhmBRPB6PmjdvrubNm6tHjx5q1qyZ0tLSSoyBUaNG6aOPPtKKFStUv359n215eXnq0qWLHnzwwSLvWxA2wOUiBuAXeXl5SklJUUREhEaOHKknnnhCffr00a233urdp7gP0mnatKmk/CXfm266qczmFBAQoKSkJCUlJenZZ5/VE088oTFjxigjI6PI40RHR0uS/v3vfxfatn37dkVFRfmsCpS3GjVqqHLlysrNzS3x59S0aVNt3rxZSUlJV/QDjLZu3aodO3Zo3rx5GjhwoHf8/fffL3L/vLw87d692+dJb8eOHZJUqk/z27Vrl5xzPt9TUffv1q2batSoobS0NLVr1045OTm68847L+Zb89GkSRNVrVpVe/fuveB+CxYs0HPPPafnnntOnTt3LrS9adOmOnHiRJn+OweKwjkD8Itnn31W69at04wZM5SamqoOHTronnvu8bkKoeCJ9OjRoz73TUxMVNOmTfX0008X+QlvBw8evOj5HD58uNBYwarD+ZfWFahTp44SEhI0b948nzlu27ZN7733nm6++eaLnkdZCgwM1G233aYlS5Zo27Zthbaf+3Pq16+fsrKyNHPmzEL7nTp1SidPniyzOUm+KyHOOT3//PPF3ufFF1/02ffFF19UUFCQkpKSSjzet99+q7/97W/er48fP65XXnlFCQkJql27tne8QoUKuv3227Vw4ULNnTtXrVq18q6aXMjHH39c5M9m/fr1OnToUJFvIRXYtm2bhg4dqgEDBui+++4rcp9+/frpo48+Unp6eqFtR48e1dmzZ0ucI1AarAygzC1btkzbt28vNN6hQwc1adJEmZmZeuyxx5SSkqJevXpJyv8o44SEBA0fPlwLFy6UlP+qKDIyUtOnT1flypUVHh6udu3aqXHjxpo1a5a6d++uli1batCgQapXr56ysrKUkZGhiIgIvf322xc154kTJ2r16tXq0aOHoqOjdeDAAU2bNk3169fX9ddfX+z9pkyZou7du+u6667TkCFDvJcWVqlSRePHj7+oOVwJTz75pDIyMtSuXTvdddddatGihQ4fPqyNGzdqxYoV3gi68847tXDhQg0bNkwZGRnq2LGjcnNztX37di1cuFDp6ell8kFSsbGxatq0qf70pz8pKytLERERWrJkSaFzBwqEhoZq+fLlSk5OVrt27bRs2TK98847euSRR4p9H/1czZs315AhQ7RhwwbVqlVLs2fP1v79+zVnzpxC+w4cOFB//vOflZGRUepLPefPn6+0tDTdcsstSkxMVHBwsDIzMzV79myFhob6fE7F+QYNGiRJ+vWvf61XX33VZ1vB/yujRo3S0qVL1bNnT6WkpCgxMVEnT57U1q1btXjxYn311VeKiooq1VyBC/LTVQz4BbrQpYX64ZK8s2fPurZt27r69esXuvzq+eefd5LcG2+84R176623XIsWLVyFChUKXdb36aefultvvdVVr17dhYSEuOjoaNevXz+3cuVK7z4Fl/SdfxlawVwLLnlbuXKl6927t6tbt64LDg52devWdbfffrvPJV1FXVronHMrVqxwHTt2dBUrVnQRERGuV69e7vPPP/fZp7TzKI3iLi0cMWJEkfvv37/fjRgxwjVo0MAFBQW52rVru6SkJDdjxgyf/U6fPu0mT57sWrZs6UJCQlzVqlVdYmKimzBhgjt27NgFj1Xws5kyZYrPeEZGhpPkFi1a5B37/PPP3U033eQqVarkoqKi3F133eU2b95c6GebnJzswsPD3RdffOF+85vfuLCwMFerVi03btw4l5ubW+LPKTo62vXo0cOlp6e7+Ph4FxIS4mJjY33mcr6WLVu6gIAA980335T4+M45t2XLFjdq1Cj3q1/9ylWrVs1VqFDB1alTx/Xt29dt3LjRZ9/zLy0suPSxuP9XCnz33Xdu9OjRLiYmxgUHB7uoqCjXoUMH9/TTT7vTp0+Xap5ASTzOlcGZSwBQxlJSUrR48eJy/WU/rVu3VrVq1Qp9OibwS8c5AwAg6V//+pc2bdrkc2IjYAXnDAAwbdu2bfrkk0/0zDPPqE6dOurfv7+/pwSUO1YGAJi2ePFiDRo0SGfOnNHr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",
+                        "image/png": "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7dpVLVu21KJFizRgwAB17NhRo0aNUtOmTZWdna2srCzFxMTorbfeuqg5p6ena/369Ro4cKASExN17NgxzZ8/X82aNdNNN91U7uMee+wxDRgwQDfeeKPGjBnju7SwTp06mjlz5kXN4Up45JFHlJWVpa5du+ruu+9Whw4ddPLkSW3evFlr1671RdBdd92l5cuXa9y4ccrKylKPHj1UXFysXbt2afny5crMzKySL5JKSkpS69at9atf/UrZ2dmKiYnRypUrA84dKFWjRg2tWbNGqamp6tq1q1avXq23335bDz30ULmfo5+rXbt2GjNmjD755BM1atRIL774oo4eParFixcHbDty5Ej99re/VVZWVqUv9Vy2bJkyMjI0ZMgQdenSRREREdq5c6defPFF1ahRw+97Ks43atQoSdKPf/xjvfTSS373lf6/MnnyZK1atUqDBg1SWlqaunTpovz8fG3fvl2vv/66Dhw4oLi4uErNFbigIF3FgKvQhS4t1L8uySsqKnLXX3+9a9asWcDlV08//bST5F577TXf2Jtvvuk6dOjgwsLCAi7r++yzz9ytt97q6tev7yIjI11iYqIbPny4e++993zblF7Sd/5laKVzLb3k7b333nO33HKLa9KkiYuIiHBNmjRxt99+u98lXWVdWuicc2vXrnU9evRwNWvWdDExMW7w4MHuiy++8NumsvOojPIuLZwwYUKZ2x89etRNmDDBNW/e3IWHh7vGjRu7lJQUt2DBAr/tCgsL3dy5c13Hjh1dZGSkq1u3ruvSpYubNWuWO3369AWPVfrcPPbYY37jWVlZTpJbsWKFb+yLL75wffr0cbVq1XJxcXHu7rvvdlu3bg14blNTU110dLT78ssv3U9+8hMXFRXlGjVq5GbMmOGKi4srfJ4SExPdwIEDXWZmpuvcubOLjIx0SUlJfnM5X8eOHV1ISIj76quvKty/c85t27bNTZ482f3oRz9y9erVc2FhYS4+Pt4NGzbMbd682W/b8y8tLL30sbz/V0p98803burUqa5NmzYuIiLCxcXFue7du7vHH3/cFRYWVmqeQEU8zlXBmUsAUMXS0tL0+uuvV+s/9nPttdeqXr16Ad+OCVztOGcAACT97W9/05YtW/xObASs4JwBAKbt2LFDn376qZ544gnFx8drxIgRwZ4SUO1YGQBg2uuvv65Ro0bp7Nmz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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -96,15 +89,15 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAkIAAAHkCAYAAADSCkBuAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABJDElEQVR4nO3dd3wVVd7H8e9NgTTCpYUEAqGGopCoNAEJhJUuRRFccEEpiuCuZXVFxQf1QRHL7sqiwkpfUUqkNwVEVjaISAkEgQChhBIJCwmGIKTM84ebebgkQHAT7iXn83698oI7c2bmd+eE5MuZmXMdlmVZAgAAMJCXuwsAAABwF4IQAAAwFkEIAAAYiyAEAACMRRACAADGIggBAABjEYQAAICxCEIAAMBYBCEAAGAsghBwi/r666/lcDj06quvuruUYuNwONS+fXu3Hb9WrVqqVauWy7KZM2fK4XBo5syZbqkpn7vPzZUOHz4sh8OhRx55xN2lFImn9CM8D0EItxSHw3Hdr6+//vpX7/+RRx6Rw+HQ4cOHi61mk+SHs8u/AgICFBYWpnbt2un555/X9u3bS+TYt9ov5isVFsJwdbm5ufr4448VExOjihUrytfXVyEhIWratKmGDRumpUuXurtE3CJ83F0A8GuMHTv2qutM+WXSokUL7dmzR5UrV3Z3KQVERETYgeTSpUtKS0vTtm3b9O677+rdd9/VgAEDNGXKFAUFBblst2fPHgUEBLih4l+sW7fObce+HnefG0+Sm5urHj16aPXq1XI6nerevbvCw8N16dIl7d69W59++qn27t2rnj172tv06dNHrVq1UlhYmBsrhyciCOGWVJouB/1aAQEBatiwobvLKFStWrUK7aMdO3Zo0KBB+vTTT3XmzBmtWrXKZb2730/dunXdevxrcfe58SSfffaZVq9eraioKG3YsEHly5d3WZ+VlaXNmze7LCtfvnyBdoDEpTGUYocOHZLT6VTFihV15MgRl3Xnz59Xo0aN5O3tbV9KczgcmjVrliSpdu3a9qWdK0eYzpw5oxdffFGNGjWSv7+/ypcvr44dO+rLL78sUMPl9yWsX79e7du3V7ly5RQcHKzu3btrz549Bbb58ccf9dxzz6lBgwYKDAyU0+lUgwYN9Mgjjyg5Odlud617hPbv369BgwapevXqKlOmjKpVq6ZBgwZp//79Bdq++uqr9iXFuLg4tWjRQgEBAapYsaIeeughHT9+/Hqnusiio6O1du1aValSRatXr9bixYtd1hd2H8xPP/2k//3f/9Xtt9+u4OBglStXTnXr1lX//v21detW+z3Url1bkjRr1iyXS3P594Rcfr6+++47de/eXRUrVnS5FHq9y1MrVqxQ69atFRgYqAoVKqhv376FntP27dvL4XAUuo8r71XJr+vIkSM6cuSIS+2XX+a72j1CGRkZevHFF9WgQQP5+fmpQoUK6ty5s9auXVug7eXnYMeOHerevbucTqcCAgIUExOj+Pj4q773a9m7d6969+6tihUrKjAwUG3bti3w72HKlClyOBx67bXXCt1HamqqfH191aRJk+seL7/ORx55pNBwExAQoA4dOrgsK+weofxL4Vf7Kux74bPPPlOHDh3kdDrl5+enRo0aady4cbp48eJ164ZnYkQIpVbt2rU1depUPfjggxowYIA2bNggH59fvuVHjhypvXv36tVXX7V/uYwdO1aLFy9WQkKCnnrqKTmdTkmy/5SkI0eOqH379jp8+LDuuecedenSRefPn9fy5cvVpUsXTZkyRcOHDy9Qy/Lly7VkyRJ17dpVI0aM0A8//KCVK1dqy5Yt+uGHH+zLW1lZWWrTpo0OHjyoe++9V/fdd58sy9KRI0e0ZMkS9e3bV3Xq1Lnm+96yZYt+85vf6KefflLPnj3VuHFj7d27V5988omWLFmitWvXqnnz5gW2+/DDD7V06VL17NlTMTEx2rx5s+bNm6eEhATt2LFDZcuW/RW9UFBISIgef/xxjRs3TnPmzFHv3r2v2tayLHXp0kXx8fG6++67NWzYMPn4+OjYsWNav3697rnnHt11111q37690tPT9f777ysqKspln9HR0S773LRpk8aPH6+2bdtqyJAhOn36tMqUKXPduhcuXKhVq1apT58+at++vXbs2KHPP/9c69evV3x8vBo0aPCrzketWrU0duxY/fWvf5UkPf3001et/Urp6elq06aNfvjhBzVv3lxPP/20Tp8+rfnz56tTp0766KOP9PjjjxfY7vvvv9fbb79tn9OjR4/q888/V8eOHbVjx44bei+HDh3S3XffrSZNmujxxx/XyZMnNW/ePHXt2lWffvqp+vfvL0kaOHCg/vSnP2natGkaM2aMvL29XfYzffp05eTkFFrvlSpVqiRJSkpKKnKdhendu3ehYWfXrl1auHBhgUuRQ4YM0YwZMxQeHq4HHnhATqdT3377rV555RWtW7dOa9assX/G4BZiAbcQSZYka+zYsYV+jR8/vsA2TzzxhCXJGj16tGVZljVz5kxLktWhQwcrNzfXpe3gwYMtSdahQ4cKPX5MTIzlcDiszz77zGX52bNnraioKMvPz89KTU21l8+YMcOSZHl7e1tr16512Wb06NGWJGvChAn2sqVLl1qSrKeffrrAsS9evGidO3fOfr1+/Xr7XOTLy8uzGjZsaEmyPvnkE5ft586da0myGjRo4PK+x44da0myypUrZ+3cudNlm9/+9reWJGvevHmFno8r5dcUExNzzXZr1661JFk1a9Z0WX7ltjt37rQkWb179y6wj9zcXOvMmTP260OHDlmSrMGDB1+zNknW5MmTC20TERFhRUREuCzL70NJ1rJly1zW/fWvf7UkWbGxsS7LY2JirKv9eM3f34wZM6577MsVdl4fe+wxS5L12GOPWXl5efbypKQkKzg42CpTpozL9/Ll5+DK40+ePNmSZD3xxBNXreFy+edbkvXcc8+5rNuyZYvl4+NjOZ1OKyMjw14+atSoQs9jXl6eVbt2bSsgIMBKT0+/7rG3bdtm+fr6Wg6Hw3r44Yetzz//3Dp8+PA1t7naeb9SSkqKVb16dcvPz8/atGlTge379OljZWVluWyT/2/or3/963Vrh+chCOGWkv+D92pf5cuXL7DNhQsXrKioKMvhcFh/+9vfrMDAQKtKlSrWiRMnCrS9VhDasWOHJcnq27dvobUtXrzYkmR98MEH9rL8H54DBw4s0D45OdmSZD3wwAP2svwg9OKLL173XBQWhDZu3GhJsu6+++5Ct2nbtq0lydqwYYO9LP+H+Msvv1yg/VdffWVJsv74xz9et57La7peENqzZ48lyfL393dZfrUg9Nvf/va6xy5qEIqOjr7qPq4VhK4MO5ZlWTk5OVbdunUtSS6/iG9GELp48aIVEBBgBQUFWf/+978LtB8zZowlyXrttdfsZfnnoE2bNgXaX7p0yfLx8bHuuuuuq9ZwufzzXb58eZeAni//39LMmTPtZYmJiZYkq0ePHi5tV69ebUmyHn300SId27Isa968eVZoaKjLv/+KFStavXv3tpYuXVqgfVGC0Llz56ymTZtaDofDWrBggcu66Oho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VatWTWlpaVqyZImys7Pte4akX/7X3rJlS33zzTcaOHCgIiMj5e3trZ49e6pp06b/9Xu677771KdPH/Xp00f16tXTjh07tGrVKlWsWFEffvihS9tHH31U77zzjsaPH6+EhAQ1btxYSUlJ9jxEn3/+eYH9d+zYUVu2bFGXLl3Url07lS1bVlFRUbrvvvuuWtNbb72lb775RpMmTdKWLVvUoUMHex6hn376SZMmTbInmiwp7dq109SpU7V582a1adPGnkcoLy9PU6ZMUXBwcIFtatasqe7du9v/9m70stjmzZv1/vvvKzQ0VG3btrXf46FDh7RixQpduHBBvXr1crnhuTBDhw7Vzz//rJYtWxYIrdIv91Llz+s0ZMgQbd26VR9++KHq1q2rzp07q2bNmjpz5owOHTqkf/7zn3r00UeL9H0ND3OTn1ID/iu6zuPzuuzx2IkTJ1qSrJ49exa6rz59+liSrD//+c8uy9977z2rYcOGVpkyZSxJBR5pPnfunPXGG29Yd955pxUYGGj5+flZtWrVsrp162ZNmTLFyszMtNte75FdXfFI9A8//GA988wz1l133WVVrlzZKlOmjBUREWE98MAD1r/+9S+XbQt7fD7f3r17rYcfftgKDQ21fHx8rNDQUGvgwIHW3r17C7TNf3x+/fr1BdZd75H0K10+T03+l5+fnxUaGmrdc8891nPPPWdt3779qttfeT5SUlKsF1980WrdurVVtWpVq0yZMlb16tWtLl26WCtXriyw/f79+60ePXpYFStWtBwOh8u5v9b5ynetx+dnzJhhLVu2zGrVqpUVEBBglS9f3rr//vutffv2FbqvxMREq2vXrlZQUJAVGBhoxcTEWF9//fVVvycyMzOtESNGWNWrV7e8vb0LnPcrz02+s2fPWn/605+sevXqWWXKlLHKly9v/eY3v7G++OKLAm2vdw6u9wj/5S7/3vjhhx+snj17Wk6n0/L397dat25trV69+prb50830axZsyId73JHjx61Jk2aZPXu3duKjIy0ypUrZ/n6+lqhoaFW165drX/84x8F5ggr7LxHRERc82dJYedi2bJlVvfu3a0qVapYvr6+VtWqVa3mzZtbL7/8srVnz54bfi9wP4dlcXcXAODmevXVV/Xaa69p6tSpGjp0qLvLgcEIQgCAm+qnn35S/fr1lZ2drZSUlOve+waU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4sWLat++vbtLAwAAblbqg1Dr1q117tw5zZ8/X+np6apVq5ZeeumlQi+NlVa+vr7q27dvqbzsd6uhLzwHfeFZ6A/PYVpfOCxTLgICAABcoVTfIwQAAHAtBCEAAGAsghAAADAWQQgAABiLIAQAAIxV6h+fB4B8eXl5Sk1NtT+H8HKNGzd2U1UA3IkgBMAISUlJmjhxotLS0gpdP2/evJtcEQBPwDxCpdiJEye0atUqHT9+XJJUvXp1de3aVdWqVXNzZWaZP3++OnTooCpV+MRod3r++ecVFhamfv36qUKFCnI4HC7rAwIC3FSZuaZPn67Q0FB169bNZfnq1auVmpqqRx55xD2FGSYvL09ff/21du3aVeho6dixY91U2c3BPUKl1Lfffqs//vGPSk5OVkREhCIiInTo0CH98Y9/1Lfffuvu8oyyZcsW/f73v9frr7+ujRs3Kjs7290lGSk1NVUDBgxQeHi4AgMDFRAQ4PKFm2/z5s1q2LBhgeWRkZH8nLqJZsyYoRkzZigvL081atSwf2fkf5V2XBorpebMmaPevXurf//+Lsvnz5+vOXPmqFWrVm6qzDzvvPOODh06pPXr12vGjBmaNm2aWrdurQ4dOqhevXruLs8Y9erVU2pqqkJDQ91dCv4jMzOz0BAaEBCgn376yQ0VmSk+Pl7PPPOM7rzzTneX4hYEoVLq7NmziomJKbD8nnvu0dKlS91Qkdlq166t2rVra9CgQdq6davWr1+vV155RdWrV1dsbKzat2/PqEQJ69q1q2bPnq309HTVrFlT3t7eLutN+J+vpwkNDdWOHTvUpUsXl+Xbt29XSEiIm6oyj4+Pj9H/QSAIlVK33Xab9uzZU+Cbe+/evWrUqJGbqoIk5ebmKjc3V5IUGBio1atXa968eXr88cfVunVrN1dXer333nuSpI8++qjQ9dwsffN1795d06dP17lz53T77bdLknbt2qXly5dr8ODBbq7OHD169NDKlSs1dOjQAvfOmYCbpUuR77//3v77mTNnNH/+fN19992qX7++JGn//v369ttv9eCDD6pTp07uKtNIycnJWr9+vf71r3/J19dX7dq1U8eOHe2gumrVKi1cuFAff/yxmystva72tFg+bmZ3jy+//FILFy7U2bNnJf3SDw8++GChI9ooPu+++67L68TERAUFBSk8PFw+Pq5jJM8999zN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uxQAvwITKgLAf8Hb21ve3t7uLgPAr8SIEICb4syZM5o7d662b9+u8+fPKzQ0VD169FBsbKwuXbqkP/3pT5Kkt99+2x5dyczM1LPPPquQkBC9/vrr+uijj7Rhw4YC+84fHcrLy9OqVau0bt06/fjjjwoICFDz5s01YMAABQUF2e1HjRqlGjVqqHfv3po1a5aOHj2qChUq6MEHH1RMTIzdLicnR4sWLdI333yjf//73ypbtqyqV6+uBx98UE2bNrWPHRcX5zJClZubq0WLFmnDhg3697//rQoVKqhNmzZ68MEH5evre8N1ACg5jAgBKHHp6el6+eWXJUmdO3dWcHCwduzYocmTJ+vChQvq3r27Ro0apVdeeUWfffaZBg8eLEmaOnWqsrKyNHLkSHl5eenee+/V2bNntXPnTj355JMFjvP3v/9dGzZsUPv27dW1a1edOnVKq1ev1qFDh/S///u/8vH5/x95qampeu+99xQbG6uYmBitX79eH374oerUqaMaNWpIkhYsWKDFixcrNjZW9erV04ULF3Tw4EElJyfbQagwkydP1oYNG9SqVSv16NFD+/fv1+LFi3X8+HE9//zzLm2LUgeAkkMQAlDi5s6dq7y8PL377rsqV66cJKlTp07661//qgULFujee+9V/fr11bNnTy1ZskQtWrRQRkaG4uPj9cgjj6hatWqSpMjISIWFhWnnzp1q166dyzH27t2rr776Sn/4wx/Utm1be/ltt92mN998U99++63L8hMnTui1115To0aNJEmtW7fWE088ofXr19sfSrxt2zbdcccdevzxx4v8Xg8fPqwNGzYoNjZWI0aMkPRL+CtfvryWLVumxMRE3X777TdUB4CSw1NjAEqUZVnavHmz7rrrLlmWpXPnztlf0dHRysrKUnJysiSpX79+qlGjhj744ANNnTpVjRs3VteuXYt0nE2bNikgIEBNmzZ1OUadOnXk5+enxMREl/bh4eF2+JCk4OBgVatWTadOnbKXBQYGKiUlRSdPnizy+92+fbskqUePHi7L77vvPkm/hKsbrQNAyWFECECJOnfunM6fP6+1a9dq7dq1V20jST4+PnriiSf04osvytfXVyNHjpTD4SjScVJTU5WVlaVhw4Zd8xj5KleuXKBNYGCgzp8/b7/u16+f3nnnHT311FOqUaOGoqOj1a5dO0VERFy1jrS0NDkcDoWGhrosdzqdCgwM1OnTp2+4DgAlhyAEoETlP49xzz33XPUG4MuDRUJCgiQpOztbJ0+eVEhISJGOk5eXp/Lly+v3v/99oeuDg4NdXnt5FT4gfvnzI40bN9bf/vY3bdmyRQkJCfrqq6+0YsUKDR8+XB07drxmPUUNcEWpA0DJIQgBKFHBwcHy9/dXXl7eNW8wlqQjR44oLi5O7du315EjRzR58mS99957CggIsNtcLWBUrVpVu3btUsOGDYt1Tp+goCB16NBBHTp00M8//6yxY8dqwYIFVw1CVapUkWVZOnnypMLDw+3l6enpOn/+fKEjQADch3uEAJQoLy8vtWzZUps3b9bRo0cLrM+/ZJWTk6MPP/xQFSpU0KOPPqqRI0cqIyNDM2fOdGlftmxZSSpw6ah169bKy8tTXFxcgWPk5ub+qktNP/30k8trPz8/Va1aVdnZ2Vfd5o477pAkrVy50mX58uXLJUl33nnnDdcBoOQwIgSgxA0YMEC7d+/Wyy+/rI4dOyo8PFyZmZlKTk7Wrl27NGPGDC1cuFCHDx/WK6+8In9/f0VERKhv376aO3euWrVqZQeIOnXqSJJmzJihqKgoeXl5qU2bNmrcuLF+85vfaPHixTpy5IiaNm0qb29vpaamatOmTXr00UfVqlWrG6r72WefVePGjVWnTh0FBQXp4MGD2rx5szp37nzVbWrVqqWYmBitXbtW58+fV+PGjXXgwAFt2LBBzZs3d3liDID7EYQAlDin06k333xTcXFx2rx5s7744guVK1dONWrU0MCBA5WcnKxFixapc+fOLkGhd+/e2rJli6ZMmaI///nPCgwMVMuWLdWlSxfFx8frm2++kWVZatOmjSTpscceU506dbR27Vp99tln8vb2VpUqVXTPPfeoQYMGN1x3165d9f3332vnzp3Kzs5WlSpV1L9/f/Xs2fOa240YMUJVq1bV119/re+++05Op1O9e/fWgw8+eMM1AChZzCwNAACMxT1CAADAWAQhAABgLIIQAAAwFkEIAAAYiyAEAACMRRACAADGIggBAABjEYQAAICxCEIAAMBYBCEAAGAsghAAADAWQQgAABjr/wAvOZBDy9EfcAAAAABJRU5ErkJggg==",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjkAAAHkCAYAAADcoz4BAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABEwklEQVR4nO3deVxWdd7/8ffFomwioiIqiltolkLllpoglhumWJYz2mhptmjdLTNNVnab3TZm5czUWOnkfmepkUuu5YKODm65oJiKigsuJE6CIqYs5/eHP67bS0DBxOviy+v5ePDQ65zvOedznS/C2+8553vZLMuyBAAAYBg3ZxcAAABQFgg5AADASIQcAABgJEIOAAAwEiEHAAAYiZADAACMRMgBAABGIuQAAAAjEXIAAICRCDmAi1q7dq1sNpveeecdZ5dyy9hsNkVFRTnt+A0aNFCDBg0cls2YMUM2m00zZsxwSk0FnH1urnXkyBHZbDY9+eSTzi6lRFylH+FaCDlwKTab7YZfa9euven9P/nkk7LZbDpy5Mgtq7kiKQheV3/5+Piodu3a6tSpk1577TXt2LGjTI5d3n7pXquogIXi5eXl6YsvvlBkZKQCAwPl6empoKAgtWzZUk8//bS+++47Z5eIcsDD2QUARRk9enSx6yrKL4o2bdpo7969qlGjhrNLKSQ0NNQeNi5fvqz09HRt375dH330kT766CMNGDBAkydPlp+fn8N2e/fulY+PjxMqvmL16tVOO/aNOPvcuJK8vDz16tVLK1asUEBAgGJiYhQSEqLLly9rz549+uqrr7Rv3z717t3bvk3fvn3Vrl071a5d24mVw9UQcuCSTLpEc7N8fHzUrFkzZ5dRpAYNGhTZRzt37tSgQYP01Vdf6ZdfftHy5csd1jv7/TRu3Nipx78eZ58bV/L1119rxYoVCg8P17p161S1alWH9dnZ2dq8ebPDsqpVqxZqB3C5CuXW4cOHFRAQoMDAQB09etRh3YULF3TnnXfK3d3dfnnLZrNp5syZkqSGDRvaL7dcOzL0yy+/6I033tCdd94pb29vVa1aVV26dNEPP/xQqIar7wOIj49XVFSUqlSpIn9/f8XExGjv3r2Ftvn555/1pz/9SU2bNpWvr68CAgLUtGlTPfnkk0pJSbG3u949OQcOHNCgQYNUt25dVapUSXXq1NGgQYN04MCBQm3feecd+2W+uLg4tWnTRj4+PgoMDNTvfvc7nThx4kanusQiIiK0atUq1axZUytWrNDChQsd1hd138n58+f1P//zP7r77rvl7++vKlWqqHHjxurfv7+2bdtmfw8NGzaUJM2cOdPhclnBPRhXn68tW7YoJiZGgYGBDpcnb3TJaOnSpWrfvr18fX1VrVo19evXr8hzGhUVJZvNVuQ+rr03pKCuo0eP6ujRow61X33prbh7cjIzM/XGG2+oadOm8vLyUrVq1dStWzetWrWqUNurz8HOnTsVExOjgIAA+fj4KDIyUgkJCcW+9+vZt2+fYmNjFRgYKF9fX3Xs2LHQv4fJkyfLZrNpzJgxRe4jLS1Nnp6eatGixQ2PV1Dnk08+WWRw8fHxUefOnR2WFXVPTsHl6eK+ivpe+Prrr9W5c2cFBATIy8tLd955p8aOHatLly7dsG64HkZyUG41bNhQU6ZM0WOPPaYBAwZo3bp18vC48i09fPhw7du3T++88479F8fo0aO1cOFCJSYm6qWXXlJAQIAk2f+UpKNHjyoqKkpHjhzRAw88oO7du+vChQtasmSJunfvrsmTJ2vYsGGFalmyZIkWLVqkHj166LnnntNPP/2kZcuWaevWrfrpp5/sl5yys7PVoUMHHTp0SA899JAefvhhWZalo0ePatGiRerXr58aNWp03fe9detWPfjggzp//rx69+6t5s2ba9++ffryyy+1aNEirVq1Sq1bty603WeffabvvvtOvXv3VmRkpDZv3qy5c+cqMTFRO3fuVOXKlW+iFwoLCgrSs88+q7Fjx2r27NmKjY0ttq1lWerevbsSEhJ0//336+mnn5aHh4eOHz+u+Ph4PfDAA7rvvvsUFRWljIwMffzxxwoPD3fYZ0REhMM+N27cqHHjxqljx44aMmSIzpw5o0qVKt2w7vnz52v58uXq27evoqKitHPnTn377beKj49XQkKCmjZtelPno0GDBho9erT+/ve/S5JefvnlYmu/VkZGhjp06KCffvpJrVu31ssvv6wzZ85o3rx56tq1qz7//HM9++yzhbb78ccf9cEHH9jP6bFjx/Ttt9+qS5cu2rlzZ6ney+HDh3X//ferRYsWevbZZ3Xq1CnNnTtXPXr00FdffaX+/ftLkgYOHKg///nPmjp1qkaNGiV3d3eH/UybNk25ublF1nut6tWrS5KS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T0/XokWLlJOTY79HR7ryv+22bdtq/fr1GjhwoMLCwuTu7q7evXurZcuWv/k9Pfzww+rbt6/69u2rJk2aaOfOnVq+fLkCAwP12WefObR96qmn9OGHH2rcuHFKTExU8+bNlZycbJ9n59tvvy20/y5dumjr1q3q3r27OnXqpMqVKys8PFwPP/xwsTW9//77Wr9+vSZOnKitW7eqc+fO9nlyzp8/r4kTJ9onSSwrnTp10pQpU7R582Z16NDBPk9Ofn6+Jk+eLH9//0Lb1K9fXzExMfZ/e6W9VLV582Z9/PHHCg4OVseOHe3v8fDhw1q6dKkuXryoPn36ONw8XJShQ4fq119/Vdu2bQsFUunKvUsF8xYNGTJE27Zt02effabGjRurW7duql+/vn755RcdPnxY//rXv/TUU0+V6PsaLuQ2P80FXJdu8Ai5rnpE9JNPPrEkWb179y5yX3379rUkWX/9618dlk+YMMFq1qyZValSJUtSocd6z507Z7333nvWvffea/n6+lpeXl5WgwYNrJ49e1qTJ0+2srKy7G1v9Niqrnks+KeffrJeeeUV67777rNq1KhhVapUyQoNDbUeffRR69///rfDtkU9Ql5g37591hNPPGEFBwdbHh4eVnBwsDVw4EBr3759hdoWPEIeHx9faN2NHsu+1tXzsBR8eXl5WcHBwdYDDzxg/elPf7J27NhR7PbXno/U1FTrjTfesNq3b2/VqlXLqlSpklW3bl2re/fu1rJlywptf+DAAatXr15WYGCgZbPZHM799c5Xges9Qj59+nRr8eLFVrt27SwfHx+ratWq1iOPPGLt37+/yH0lJSVZPXr0sPz8/CxfX18rMjLSWrt2bbHfE1lZWdZzzz1n1a1b13J3dy903q89NwXOnj1r/fnPf7aaNGliVapUyapatar14IMPWt9//32htjc6Bzd6jP1qV39v/PTTT1bv3r2tgIAAy9vb22rfvr21YsWK625fMOVCq1atSnS8qx07dsyaOHGiFRsba4WFhVlVqlSxPD09reDgYKtHjx7W//7v/xaaA6uo8x4aGnrdnyVFnYvFixdbMTExVs2aNS1PT0+rVq1aVuvWra233nrL2rt3b6nfC5zLZlncSQUAuLXeeecdjRkzRlOmTNHQoUOdXQ4qKEIOAOCWOn/+vO644w7l5OQoNTWVT1eH03BPDgDglli6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Z968eercubNq1uTTg53ltddeU+3atfX444+rWrVqstlsDut9fHycVFnFNW3aNAUHB6tnz54Oy1esWKG0tDQ9+eSTzimsAsrPz9fatWu1e/fuIkc6R48e7aTKyh735JRDmzZt0h//+EelpKQoNDRUoaGhOnz4sP74xz9q06ZNzi6vwtm6datefPFFvfvuu9qwYUO5/2T78igtLU0DBgxQSEiIfH195ePj4/CF22/z5s1q1qxZoeVhYWH8nLrNpk+frunTpys/P1/16tWz/94o+DIZl6vKodmzZys2Nlb9+/d3WD5v3jzNnj1b7dq1c1JlFdOHH36ow4cPKz4+XtOnT9fUqVPVvn17de7cWU2aNHF2eRVCkyZNlJaWpuDgYGeXgv8vKyuryIDp4+Oj8+fPO6GiiishIUGvvPKK7r33XmeXctsRcsqhs2fPKjIystDyBx54QN99950TKkLDhg3VsGFDDRo0SNu2bVN8fLzefvtt1a1bV9HR0YqKimJEoQz16NFDs2bNUkZGhurXry93d3eH9ab/b9UVBQcHa+fOnerevbvD8h07digoKMhJVVVMHh4eFfY/AISccuiuu+7S3r17C33T7tu3T3feeaeTqkKBvLw85eXlSZJ8fX21YsUKzZ07V88++6zat2/v5OrMNGHCBEnS559/XuR6bjy+/WJiYjRt2jSdO3dOd999tyRp9+7dWrJkiQYPHuzk6iqWXr16admyZRo6dGih+9VMx43H5cSPP/5o//svv/yiefPm6f7779cdd9whSTpw4IA2bdqkxx57TF27dnVWmRVWSkqK4uPj9e9//1uenp7q1KmTunTpYg+iy5cv1/z58/XFF184uVIzFfdUVQFuCneOH374QfPnz9fZs2clXemHxx57rMiRaNxaH330kcPrpKQk+fn5KSQkRB4ejuMbf/rTn25nabcVIaecuPb+m+vhf6231x//+EedPHlSLVu2VJcuXdSqVSu5uTne03/u3DkNGzaMvkGFdO7cOVWqVEleXl7OLqXC+Oyzz0rcdvjw4WVYiXMRcoDfKC4uTtHR0QoMDFTBP6eKNiTsCtLS0rRs2TKHaRV69uxZYe9FcDamVnAdly9fVn5+vj1knj59Wlu3blXdunUVERHh3OLKGCEHuAXWrFmjpUuX6tSpU5Kk2rVrq2fPnurSpYuTK6sYdu7cqQ8++EANGjRQ06ZNJUn79+/X0aNH9frrr6tly5ZOrrDiee2115SamqrmzZsrOjpabdu2laenp7PLqpDGjh2rNm3aqGvXrrpw4YJefvlleXh46Ny5cxo8eLDRtzhw43E5tXv37mIndjJ56NEVzZ07V0uWLFGPHj0UFhYm6coMvDNnztSZM2dKdakRN+err75STEyMBg4c6LB89uzZmj17NiHHCZhawXUcPnzYfrP3pk2bFBAQoPHjx2vz5s2aN28eIQeu5ZtvvlFcXJwaN26sgIAALo042Q8//KBnn31WHTt2tC9r1aqV6tevr+nTpxNyboMTJ07olVdeKbS8c+fOWrZsmRMqgsTUCq7i0qVL8vb2liQlJiaqTZs2cnNz0x133HHDm/bLO0JOObRy5UqNGDFCnTp1cnYp0JVHxhs3blxoeaNGjeyPkqNs+fv768iRI6pdu7bD8iNHjsjf399JVeFqTK3gPMHBwdqyZYvatGmjxMRE9erVS9KVG8ILwo+pCDnlUG5urv2yCJyvU6dO+uGHHwrN/bFq1SqH0R2UnS5duuif//ynfv75Z4d7chYtWqSYmBgnV1dxFTW1wtChQx2mVpg+fTohp4z169dPH3/8sWbOnKkWLVrYf38kJiaqYcOGTq6ubHHjcTn05ZdfysvLS/369XN2KdCVDyJct26datSo4TBv0ZkzZxQZGekw+y6ToJUNy7K0dOlSLVmyxD4nS7Vq1dS7d2/16NGDS7pOwNQKriUjI0Nnz55VaGiovR8OHjwob29v1a1b18nVlR1CTjk0ffp0/etf/1L9+vUVGhpaaAp7fpHeXmPGjClxW5M/7ddVXLx4UZKMH4Z3dUytAFdAyCmHbvRLlV+kqGguX74sy7JUuXJlSVdmQN6yZYtCQkIUHh7u5OoqLqZWgLMRcgCUexV5HhBXVdzUCitWrFBMTAxPHeK2cLtxE7ia+Ph4Xb582dllAC7j8OHD9g+nLZgH5NNPP9ULL7yg5cuXO7m6iqlgaoUBAwaoVatWatWqlQYMGKBnnnlGP/zwg7PLQwVByCmHvvrqKw0bNkyff/659u/f7+xyAKeryPOAuCqmVoArIOSUQ5MmTdKIESN0/vx5vfPOO3r55Ze1cOFCZWRkOLs0wCkK5gE5c+aMEhMT7ffhVIR5QFxVwdQK12JqBdxO3JNTzmVkZGj9+vVat26dTpw4oYiICEVHR+u+++4r9LgmYKpNmzbp448/Vn5+vu6++269/fbbkqQFCxZo7969evPNN51cYcXD1ApwBYQcAxw4cEDx8fFat26dAgICdOHCBfn6+mr48OG66667nF0ecFsUzAPSoEED+6PKBw8elI+Pj+rUqePk6ioeplaAKyDklFMZGRn617/+pbVr1+rnn39W69atFR0drZYtW+rXX39VXFycEhIS9Nlnnzm7VKBMfPTRRxo+fLh8fHz00UcfXbetl5eXQkJC1LVrVz4rCahA+FiHcuj9999XYmKi6tSpoy5duigyMlJ+fn729V5eXnr44Ye1ePFiJ1YJlC0fHx/7iM2NgktOTo5Wrlyp/fv36/XXX78d5QFwAYzklEOff/65unTpct3Pr7IsS2fOnFHNmjVvY2WA6zp+/LjeeOMN/e///q+zSwFwmxByAFQI+fn5OnbsmBo0aODsUgDcJoSccmr37t1aunSpTpw4IUmqW7euevbsqZYtWzq5MgAAXAMhpxz6/vvvNWPGDLVt29Z+yerAgQPatGmTBg8erO7duzu5QgAAnI8bj8uhBQsWFBlmmjZtqgULFhByAAAQMx6XSxcuXFBERESh5eHh4crOzr79BQEA4IIIOeVQq1attGXLlkLLt27dqvvuu88JFQEA4Hq4J6cc+vbbb7V48WI1bdrU4Z6c/fv3q1evXg6f1dOzZ09nlQkAgFMRcsqhESNGlKidzWbTxIkTy7gaAABcEyEHAAAYiaeryomZM2eqf//+8vLy0syZM4ttZ7PZNGjQoNtYGQAAromQU04cOXJEeXl59r8DAIDr43IVAAAwEo+QAwAAIxFyAACAkQg5AADASIQcAABgJEIOABRj3rx5evzxx51dBoCbRMgB4DK2b9+uefPmObsMAIbgEXIALmPq1Kn6/vvvXSbo5OXlKS8vT5UqVXJ2KQBuApMBAkAx3N3d5e7u7uwyANwkRnIA/Ga//PKL5syZox07dujChQsKDg5Wr169FB0drcuXL+vPf/6zJOmDDz6wj4pkZWXp1VdfVVBQkN599119/vnnWrduXaF9F4zq5Ofna/ny5Vq9erV+/vln+fj4qHXr1howYID8/Pzs7UeMGKF69eopNjZWM2fO1LFjx1StWjU99thjioyMtLfLzc3VggULtH79ev3nP/9R5cqVVbduXT322GNq2bKl/dhxcXEO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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -124,15 +117,15 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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Pic7O1sjRoy4uob/fzab7ZrqryQpKUlvvPGGEhIS9P7771/Vc/bt22fdhygnJ6feAFi7fzt37lTPnj2varsxMTGaP3++PB6PPv/8c73//vt6+eWX9bvf/U41NTX6/e9/f/U7BhiEj88D+Fpat26tLl266Pjx49apqC/btGmTJFmfbLqcXr16SZK2bNmi6urqOvOXfqRcku644w5J0ocffnitbTe41q1bS7ryacRaDodDw4YNU3l5uf7+97/rG9/4Rr11/83+2Ww2de/eXT/4wQ+0fv16SbrqlSrARAQhAF9bRkaGPB6Pfvazn3mFmNLSUmsFIiMj44rbiImJ0T333KNDhw5p7ty5XnPZ2dl1rg+SpJEjR6pLly56+eWXlZOTU+928/LyVFlZea27VMehQ4c0Z86cej9m7/F4NGvWLEnSXXfddcXtnDt3TiNGjFBRUZHmzZt32XsSSdITTzyhsLAwzZgxQ1u3bq0zX1NT4xUQ9+zZU++KWu0Yd7gGLo9TYwC+tqeeekpr1qxRdna2kpOTlZ6ersrKSi1dulSnTp3S//t//0/9+/f/yu28/PLLuvPOO/XjH/9Y69atU3JysgoLC7VixQrdd999WrVqlVe93W7X8uXLNWTIEA0bNkz9+vVTSkqKgoODVVxcrG3btqmoqEglJSX/dQhwuVz60Y9+pJ/97GdKTU3VrbfeqtatW+vUqVN6//33VVRUpIiICD333HNX3M6cOXP08ccfKz4+/rIXeT/++OOKi4tTu3bttGzZMo0ePVp33HGHBg8erO7du8tms6m4uFh5eXn617/+pXPnzkmS1q9fr5/97Ge68847lZiYqIiICB07dkzZ2dlq1qyZfvazn/1XvwPAnxGEAHxtzZs31/r16/X888/r7bff1p///GcFBgYqOTlZL774or773e9e1Xa6du2qjz/+WNOmTdOGDRu0efNm9ezZU++8844cDkedICRJPXv21M6dO/X8889r9erV+tvf/qZmzZopKipKvXr10owZM+p87cXX0a1bN61YsULr1q3Txx9/rCVLluj06dMKDg5WQkKCfvWrX+lHP/qROnTocMXt1K5OFRUVacaMGfXWDBw40LrT9eDBg7Vr1y796U9/0nvvvacPP/xQzZs3V3R0tAYNGqQHHnjAet6QIUN09OhR/eMf/1B2drbKysoUFRWle+65R08+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+HGNGjVK//M//6MWLVro2Wef1datW6/L7wJAw2BFCMANIy4uTt///vetx+Xl5dq0aZMeffRRSdKMGTPUvHlzaz4tLU2zZs3Su+++q7S0NK9tnThxQjNnzlRiYqIkKSYmRrNmzdK8efP04osvqn379pKkkJAQ/fWvf9XevXvVvXt3SdLChQvVvn17/eEPf5DdbpckDRkyRL/5zW/01ltvqU+fPo33SwDQoFgRAnDDuOeee7weJyUl6d///rcqKyslySsEVVZWqqysTN/4xjf0xRdfWDW1YmJirBAkSV27dpUk3XrrrVYIkqSEhARJ0hdffCHpYvjKz8/XnXfeqbNnz6qsrExlZWX697//reTkZJWUlOj06dMNuNcAGhMrQgBuGF8OKNLF1RpJqqioUHBwsPbt26elS5eqoKBA58+f96qtrKxUcHDwZbdVO9euXbt6xysqKiRdPKXm8Xi0ZMkSLVmypN4+XS6X2rZte627B8AHCEIAbhiX+4Zwj8ejkydP6ve//72io6P12GOPqV27dgoMDNRnn32md9991+sanytt60qvIcnazn333afk5OR6ayMjI69qfwD4HkEIgF/Yvn27qqqq9POf/9xrtWfPnj0N+jo33XSTJCkgIEA9e/Zs0G0DuP64RgiAX6hdyalduZEung7bvHlzg75OmzZt1L17d23YsEFnzpypM19WVtagrwegcbEiBMAvJCcnKzAwUJmZmfr2t7+tc+fOaePGjQoNDa03sPw3xo8fr1//+td66qmnNHjwYEVERMjlcqmgoECnT5/Ws88+26CvB6DxsCIEwC9ER0frySeflM1m0xtvvKH169fr29/+ttLT0xv8tWJiYjR79mz16tVLmzdv1vz587V+/XrZbDY98MADDf56ABqPzfPldWQAAACDsCIEAACMRRACAADGIggBAABjEYQAAICxCEIAAMBYBCEAAGAsghAAADAWQQgAABiLIAQAAIxFEAIAAMYiCAEAAGMRhAAAgLEIQgAAwFj/H+fTCDlY2AUEAAAAAElFTkSuQmCC",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAkIAAAIUCAYAAAD2cEPqAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAABBzElEQVR4nO3deViU1/3//9cIo4KI4EKAoCAiwRoF06iJ2Gi0iYjGJUtjYz4xQb1q1W5p+q1tbVNbTaVpNmv6iU20xiwfRatBDRqXaBoDqcbEBaMi4oKKcajOUMCFgfn94Y+7GUGjKTg45/m4Lq8w55w59/sm91y+PPcyNo/H4xEAAICBmvm6AAAAAF8hCAEAAGMRhAAAgLEIQgAAwFgEIQAAYCyCEAAAMBZBCAAAGIsgBAAAjEUQAgAAxiIIAbhuDh8+LJvNpscff/yq37Nw4ULZbDYtXLiw0epqDDabTQMHDvR1GQC+AkEIQB02m+2Kf260UNIQtm3bprFjxyo2NlYtWrRQaGiounTpovvuu09//OMfVVFR4esSAXwNgb4uAEDT9fTTT9fbnpKScn0L8bE333xT48aNk8fj0aBBgzR69GgFBQXpyJEj2rJli1avXq37779fCQkJ1nv27t2r4OBgH1YN4GoQhABc1m9/+1tfl+BzlZWVmjJlimw2m9atW6fBgwfXGZObm6v27dt7tSUlJV2vEgH8Fzg1BuC/cv78ec2ePVs9evRQcHCwQkND9a1vfUtZWVnXNE9hYaEeeughhYeHq1WrVurXr5/efffdK77n2LFjmjp1quLj49WiRQu1a9dOI0aM0LZt2+qM/e1vfyubzabNmzfr7bffVt++fRUSEqK4uLgrbiM/P19lZWW69dZb6w1BktSvXz+FhYV5tV16jdDmzZu/8pTj5s2bvebYt2+fHn/8cXXs2FHNmzfXTTfdpEceeUT79++vU8MXX3yhp556SrfccotatWqlsLAw3XLLLXr88cdVVFR0xX0ETMaKEICv7cKFCxoyZIg++OADJSUlacqUKaqsrNSyZcv08MMPa8eOHXrmmWe+cp4DBw7ozjvv1L/+9S8NHTpUKSkpKiws1KhRozR06NB63/Ppp5/q3nvv1enTpzVkyBDdf//9Ki0t1TvvvKP+/ftrxYoVSk9Pr/O+5557TuvXr9d9992nu+++Wy6X64q1tWvXTpJ04sQJVVRUqFWrVlfxm6krLi6u3lONVVVVev7553Xu3DmvU2lr167V/fffr6qqKt13331KSEjQsWPHtHz5cr377rvatGmTbrvtNkkXV61SU1N18OBB3XPPPbrvvvvk8Xh05MgRZWdn68EHH1R8fPzXqhvwex4AuIQkjyTP008/XefP3/72N2vcM88845HkGTp0qKeqqspq/+KLLzyxsbEeSZ6PPvrIaj906JBHkmfcuHFe27vnnns8kjwvvviiV/s777xj1fLl7VZVVXm6dOniadGihWfz5s1e7zl+/LgnOjraExkZ6Tl37pzV/vTTT3skeYKDgz2ffvrpVf8uampqPL179/ZI8iQnJ3vmzp3r+fTTTz3nz5+/4vskeQYMGPCV848bN84jyfPjH//Yajt9+rQnLCzM065dO8+ePXu8xu/evdvTqlUrT69evay2lStX1pmj1vnz5z1lZWVfWQdgKoIQgDpqw0d9f778l3tCQoLHZrN59u7dW2eO1157zSPJ88QTT1ht9QWh4uJijyRP586dPW63u848AwYMqBOEagPSU089VW/9L774okeS591337XaaoNQfWHhqxw5csQzcOBAr9+D3W739OnTxzN79myPy+Wq856rCUIzZszwSPKMHDnSU11dXaf+uXPn1vu+H//4xx5JVkiqDUK/+MUvrnnfANNxagzAZXk8nsv2/fvf/1ZhYaFuvvnmei8MHjRokCTps88+u+I2avv79++vgICAOv0DBw7UBx984NWWl5cnSTpy5Ei9F3QfOHBA0sU7ty49PdanT58r1lOfTp06adOmTdq7d6/Wr1+vTz75RFu3brX+/OUvf9HmzZvVuXPnq57zrbfe0tNPP63bb79db7/9tpo1+88lm7X7t3Pnznr3r6CgwNq/b3zjGxowYIBuvvlmzZ49W59++qnS09OVmpqqlJSUen+nAP6DIATga6m9tiYqKqre/tp2p9N5VfPcdNNN9fZHRkbWafvXv/4lSVq6dOkV5y4vL7+q+a5Wt27d1K1bN+v1vn37lJGRoby8PP3kJz/RO++8c1XzfPDBB8rIyFBsbKxWr15d5zb72v179dVXrzhP7f6Fhobq448/1tNPP62VK1fqvffekyS1b99ekydP1vTp02W32692NwGjEIQAfC1t2rSRJJ08ebLe/pKSEq9xXzXPF198UW9/ffPXvic7O1sjRoy4uoL/fzab7ZrGX0lSUpLeeOMNJSQk6P3337+q9+zbt896DlFOTk69AbB2/3bu3KmePXte1bwxMTGaP3++PB6PPv/8c73//vt6+eWX9bvf/U41NTX6/e9/f/U7BhiE2+cBfC2tW7dWly5ddPz4cetU1Jdt2rRJkqw7my6nV69ekqQtW7aourq6Tv+lt5RL0h133CFJ+vDDD6+17AbXunVrSVc+jVjL4XBo2LBhKi8v19///nd94xvfqHfcf7N/NptN3bt31w9+8AOtX79ekq56pQowEUEIwNeWkZEhj8ejn/3sZ14hprS01FqByMjIuOIcMTExuueee3To0CHNnTvXqy87O7vO9UGSNHLkSHXp0kUvv/yycnJy6p03Ly9PlZWV17pLdRw6dEhz5syp9zZ7j8ejWbNmSZLuuuuuK85z7tw5jRgxQkVFRZo3b95ln0kkSU888YTCwsI0Y8YMbd26tU5/TU2NV0Dcs2dPvStqtW084Rq4PE6NAfjannrqKa1Zs0bZ2dlKTk5Wenq6KisrtXTpUp06dUr/7//9P/Xv3/8r53n55Zd155136sc//rHWrVun5ORkFRYWasWKFbrvvvu0atUqr/F2u13Lly/XkCFDNGzYMPXr108pKSkKDg5WcXGxtm3bpqKiIpWUlPzXIcDlculHP/qRfvaznyk1NVW33nqrWrdurVOnTun9999XUVGRIiIi9Nxzz11xnjlz5ujjjz9WfHz8ZS/yfvzxxxUXF6d27dpp2bJlGj16tO644w4NHjxY3bt3l81mU3FxsfLy8vSvf/1L586dkyStX79eP/vZz3TnnXcqMTFREREROnbsmLKzs9WsWTP97Gc/+69+B4A/IwgB+NqaN2+u9evX6/nnn9fbb7+tP//5zwoMDFRycrJefPFFffe7372qebp27aqPP/5Y06ZN04YNG7R582b17NlT77zzjhwOR50gJEk9e/bUzp079fzzz2v16tX629/+pmbNmikqKkq9evXSjBkz6nztxdfRrVs3rVixQuvWrdPHH3+sJUuW6PTp0woODlZCQoJ+9atf6Uc/+pE6dOhwxXlqV6eKioo0Y8aMescMHDjQetL14MGDtWvXLv3pT3/Se++9pw8//FDNmzdXdHS0Bg0apAceeMB635AhQ3T06FH94x//UHZ2tsrKyhQVFaV77rlHTz75pPr1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i4v1q1/9SsePH9eoUaP0P//zP2rRooWeffZZbd269br8LgA0DFaEANww4uLi9P3vf996XV5erk2bNunRRx+VJM2YMUPNmze3+tPS0jRr1iy9++67SktL85rrxIkTmjlzphITEyVJMTExmjVrlubNm6cXX3xR7du3lySFhITor3/9q/bu3avu3btLkhYuXKj27dvrD3/4g+x2uyRpyJAh+s1vfqO33npLffr0abxfAoAGxYoQgBvGPffc4/U6KSlJ//73v1VZWSlJXiGosrJSZWVl+sY3vqEvvvjCGlMrJibGCkGS1LVrV0nSrbfeaoUgSUpISJAkffHFF5Iuhq/8/HzdeeedOnv2rMrKylRWVqZ///vfSk5OVklJiU6fPt2Aew2gMbEiBOCG8eWAIl1crZGkiooKBQcHa9++fVq6dKkKCgp0/vx5r7GVlZUKDg6+7Fy1fe3atau3vaKiQtLFU2oej0dLlizRkiVL6q3T5XKpbdu217p7AHyAIATghnG5bwj3eDw6efKkfv/73ys6OlqPPfaY2rVrp8DAQH322Wd69913va7xudJcV9qGJGue++67T8nJyfWOjYyMvKr9AeB7BCEAfmH79u2qqqrSz3/+c6/Vnj179jTodm666SZJUkBAgHr27NmgcwO4/rhGCIBfqF3JqV25kS6eDtu8eXODbqdNmzbq3r27NmzYoDNnztTpLysra9DtAWhcrAgB8AvJyckKDAxUZmamvv3tb+vcuXPauHGjQkND6w0s/43x48fr17/+tZ566ikNHjxYERERcrlcKigo0OnTp/Xss8826PYANB5WhAD4hejoaD355JOy2Wx64403tH79en37299Wenp6g28rJiZGs2fPVq9evbR582bNnz9f69evl81m0wMPPNDg2wPQeGyeL68jAwAAGIQVIQAAYCyCEAAAMBZBCAAAGIsgBAAAjEUQAgAAxiIIAQAAYxGEAACAsQhCAADAWAQhAABgLIIQAAAwFkEIAAAYiyAEAACMRRACAADG+v8AzrIJQCiCoTwAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -154,15 +147,15 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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CCMAgEIYAQAUwggAoBBGAACFMAIAKIQRAEAhjAAACmEEAFAIIwCAQhgBABTCCACgEEYAAIUwAgAohBEAQCGMAAAKYQQAUAgjAIBCGAEAFMIIAKAQRgAAhTACACiEEQBAIYwAAAphBABQCCMAgGJYwmjXrl3ZsmVL9uzZMxy7AwCoikMKo8ceeyxXXnllLrvsslx77bV59tlnkyRdXV255ppr8p//+Z/DMiQAwEg46DB6/PHHs3LlykyZMiXnn3/+gM9NnTo1Rx99dNavX3+o8wEAjJiDDqPvf//7+eQnP5lly5bl85///H6fP/nkk7N58+ZDGg4AYCQddBi9+OKLOf3009/380ceeWS6uroOdvcAACPuoMNowoQJH/hi69deey2TJ08+2N0DAIy4gw6jOXPm5Ic//GHefvvt/T7X2dmZH/zgBznttNMOaTgAgJF00GF04YUX5vXXX891112Xf/7nf06S/OQnP8k//MM/pL29PUly3nnnDc+UAAAjoK6vr6/vYL/4pZdeyp133pkNGzYMuP+Tn/xkLr300jQ1NR3ygMPtv/7rv7J69er09fXli1/8YhYsWDDkfezYsSN79+6twHTsU1dXl5kzZ2br1q05hCUKVWH9UqvG6tptbGzMMcccM6htGw7lQCeccEJuuOGG/N///V+2bduWvr6+HHfccZk6deqh7LZi3n777axevTo33nhjJk2alGuvvTZz587NlClTqj0aADAKHHQY7dy5M0cccUQmT56cyZMnp6WlZcDnf/azn6WrqyvTp08/5CGHy7PPPpumpqYcffTRSZLW1tY8+eST+fVf//UqT5asv/e7ycQ9yVtHZN65VxzydpU6/kjsZ98+evfWpb6x74D7quS8774vyYceZ6jbD3aOShip41BZtfg41uLM48m7H5+LFn9zVMxRrXVy0KfSfu/3fi8TJkzIH//xHx8wLP793/89t99+e/7xH//xkIfcZ9OmTVmzZk02b96cXbt2ZcmSJZk7d+6AbTo6OnL//fens7Mzs2bNyiWXXNIfbY8++mg2btyYSy+9NEmyZs2aJMnZZ589pDmG+1Ta+h8uzfbpz6YvSV2SY3e2ZN6ZNx70dpU6/kjs59372Oe9+6rkvEn2O/6BZvigeT9o+8HOMRyPa7WOQ2VPR9Ti41iLM48nB3p85s/7xoifSqvkOhnKqbRDekuQKVOm5Lvf/W7uvPPO9Pb2HsquBqW7uzuzZ8/uD5v3euSRR7J69eqcd955WbFiRWbNmpXly5fnjTfeOKjj7d27N7t37+7/eOutt/o/V1dXNywf6+/97oB/WPvyzj/M6+/97kFtV6njj8R+3ruPHGBflZz3tenPHvD473ec95t3KHNV6nGt1nF8/PxjOH9P1PLjWIszj6eP93t81t3z/0bFHMO1TobikF5jtO8v0/7+7/8+L7zwQq666qqKvr6otbU1ra2t7/v5Bx54IAsWLMj8+fOTJIsWLcoTTzyRdevW5ZxzzslRRx2V119/vX/7119/fb9TgO9277335u677+6/feKJJ2bFihWDrs5BmbjngCGQid2ZOXPm0Ler1PFHYj8H2Md795X0VWze/n19yAz9x/mAeQc9V6Ue12odhwFmzJgxvDusxcexFmceT0bL4zNa5sghhlHyzmmo5ubm3HbbbbnuuuvS3t6e5ubm4ZhtSHp6evL888/nnHPO6b+vvr4+p556ap5++ukkSUtLS1566aW8/vrrmTRpUn784x/nd3/3d993n+eee24WLlzYf3tfde7YsSM9PT3DM/hbR6QuA/9BrkuStyZk69atQ9+uUscfif0cYB/v3de+/12JeQ+07wPN0H+cD5h30HNV6nGt1nFI8s7vihkzZvT/UcqwqcXHsRZnHk9Gy+NT4TkaGhpG5lTaPqecckq+9a1vZdq0afn6179elTeP7erqSm9vb6ZNmzbg/mnTpqWzszNJcthhh+XLX/5yli5dmq9+9av5whe+8IF/kdbY2JhJkyb1f0ycOLH/c319fcPyMe/cK3Lszpbse6Kv/7zquVcc1HaVOv5I7Oe9+8gB9lXJeY/b2XLA47/fcd5v3qHMVanHtVrH8fHzj+H8PVHLj2MtzjyePt7v8Zn//31lVMwxXOtkKA7pxddXXHHFgBde9/T05K/+6q/ygx/8IE1NTXn55ZeH9cXX73bBBRcMePH166+/nssuuyw33XRTTj755P7t/vZv/zabNm3KzTffPGzHrsR1jN55JX538taEQfxV2odvV6njj8R+9u2jd29S35gD7quS8777viQfepyhbj/YOSphpI4z3tXVVfZaMLX4ONbizOPJux+fixZ/s2rXMarUOhnKi6+HNYz2WbduXf7yL/8yPT09IxZGPT09ufjii3P11VcP+Eu1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dOnSTJgwIXv27El7e3t+7dd+LVOmTKn2aDBo99xzT0466aRqjwEH5aabbsoRRxxR7TEqxqk0akp9fX0mTJiQJOnp6UmSMfeePoxtW7duzSuvvJLW1tZqjwIcgGeMGFGbNm3KmjVrsnnz5uzatStLlizJ3LlzB2zT0dGR+++/P52dnZk1a1YuueSStLS09H/+zTffzDe+8Y1s3bo1F198caZOnTrS3wbj1HCs37/5m7/JxRdfnKeffnqkx2ecG471myQ33nhj6uvrc9ZZZ+U3fuM3RvJbGBGeMWJEdXd3Z/bs2bn00ksP+PlHHnkkq1evznnnnZcVK1Zk1qxZWb58ed54443+bT7ykY/klltuye23354f/ehH6ezsHKHpGe8Odf0+9thjmTlzZo4//viRHBuSDM/v32XLlmXFihW55pprcu+99+aFF14YqfFHjGeMGFGtra0feArhgQceyIIFCzJ//vwkyaJFi/LEE09k3bp1OeeccwZsO23atMyaNStPPfVUPvOZz1RybEhy6Ov3mWeeySOPPJJHH300e/bsSU9PTyZNmpTzzjtvpL4FxrHh+P179NFHJ0mOOuqotLa2ZvPmzZk1a1bFZx9JwohRo6enJ88///yAAKqvr8+pp57af9qhs7MzEyZMyMSJE7N79+789Kc/zW/91m9VaWL4ucGs34suuigXXXRRkmT9+vV58cUXRRGjwmDW7549e9LX15eJEydmz5492bBhQ04//fQqTVw5wohRo6urK729vZk2bdqA+6dNm5ZXX301SbJz585873vfS/LOi67b2trysY99bKRHhf0MZv3CaDWY9fvGG29k5cqVSZLe3t4sWLBgv9cfjQXCiJrS0tKSW265pdpjwCGbN29etUeAITnuuOPGxe9fL75m1Jg6dWrq6+v3ezF1Z2fnfv8vBkYb65daZv3+nDBi1GhoaEhzc3M2bNjQf19vb282bNiQk08+uYqTwYezfqll1u/POZXGiNqzZ0+2bdvWf3v79u3ZsmVLJk+enOnTp2fhwoVZtWpVmpub09LSkoceeijd3d1OOzAqWL/UMut3cOr6XDaYEbRx48YsXbp0v/vPPPPMLF68OMk7Fxhbs2ZNOjs7M3v27PzRH/2Rt09gVLB+qWXW7+AIIwCAwmuMAAAKYQQAUAgjAIBCGAEAFMIIAKAQRgAAhTACACiEEQBAIYwADtKqVavypS99qdpjAMPIe6UBNW39+vW54447+m/X19fnyCOPzKc+9alceOGFOfroo6s4HVBrhBEwJlxwwQU59thjs3fv3jzzzDNZv359nnrqqdx66605/PDDqz0eUCOEETAmtLa25uMf/3iSZMGCBZkyZUruu+++PP744znjjDOqPB1QK4QRMCZ94hOfyH333ZfXXnstSdLT05Pvf//7eeKJJ7Jt27b09vbmxBNPzAUXXJBTTjml/+u2b9+eP/3TP83FF1+cSZMm5b777sv//M//ZNasWbn00kvT0tLygcfdsmVLli1blhNOOCF/9md/liOOOKKi3ycwvLz4GhiTtm/fniT5yEc+kiTZvXt3/vVf/zVz5szJH/zBH+T8889PV1dXli9fni1btuz39T/60Y+yZs2afO5zn8vv//7vZ/v27bn11lvT09Pzvsd89tlns3Tp0px44om5/vrrRRHUIM8YAWPC7t2709XV1f8ao7vvvjuNjY359Kc/nSSZPHlyVq1alYaGn//aW7BgQa688so8/PDDufzyywfsb+fOnbntttsyefLkJMnxxx+fP//zP8+TTz7Zv893e+qpp/LNb34zn/jEJ9Le3p7GxsYKfrdApQgjYExYtmzZgNvHHHNMrrjiinz0ox9N8s5fq9XXv/MkeW9vb3bv3p3e3t58/OMfz+bNm/fb3+mnn94fRUnyi7/4i0nSf2ru3TZs2JAVK1bktNNOy5VXXjkgvoDa4r9eYEy49NJLM3PmzOzevTvr1q3LT3/60/2etVm/fn0eeOCBvPLKK3n77bf77z/22GP329/06dMH3N4XSW+++eaA+/fu3ZtvfetbaW5uzlVXXZXDDjtsuL4loAqEETAmtLS09P9V2ty5c3PDDTfktttuy2233ZYjjjgi//Zv/5Y77rgjv/qrv5qzzz47U6dOTX19ff7pn/7pgM8C7Xt26b36+voG3G5sbExra2see+yx/OQnPzngaTagdnjxNTDm1NfX56KLLsquXbvS0dGRJHn00Udz3HHHZcmSJfnN3/zN/NIv/VI+9alPZe/evYd8vK985Ss59dRT8xd/8RfZuHHjIe8PqB5hBIxJc+bMSUtLSx588MH87Gc/638G6N3P+DzzzDN5+umnD/lYDQ0NWbJkSVpaWrJixYo8++yzh7xPoDqEETBmnX322XnjjTeyfv36fPrTn85rr72WlStX5l/+5V/yd3/3d7n55pvT1NQ0LMc6/PDDc+211+b444/PzTffnBdffHFY9guMLGEEjFlz587Ncccdl/vvvz9nnnlmLrzwwrzwwgv567/+6zz55JO54oor0tzcPGzHmzRpUr72ta9l2rRpuemmm7Jt27Zh2zcwMur63vtKQgCAccozRgAAhTACACiEEQBAIYwAAAphBABQCCMAgEIYAQAUwggAoBBGAACFMAIAKIQRAEAhjAAACmEEAFD8/1uCGZ/iyK+jAAAAAElFTkSuQmCC",
+                        "image/png": "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2qOPPhonTpyIu+66K2/7doHH4THc/0FCvlnDFLvRsoaH5QKPFwqeJUuWxK/8yq9c8ENm8620tDSqq6ujqampN4y6u7ujqakpstnssM0BABSvQZ98fT6TJk3K+xWl29vbo6Wlpff24cOHo7m5OcrLy2Pq1KmxbNmy2Lx5c1RXV0dNTU08++yz0dHREYsXL87rHADA6JRzGD322GORyWTij//4j6OkpCQee+yxj3xOJpOJW2+9dVADnum1116LdevW9d6ur6+PiIhFixbFmjVr4uqrr462trZ44oknorW1NWbNmhX33nvvWSdkAwCcS85htGfPnshkMtHd3R0lJSWxZ8+ej3xOfy+q9FHmzZsXTzzxxAUfk81m837orKGhIRobG6OysjLq6uryum0AYOQY8MnXY5mTr4fHaDnpj7HLGqbYjZY1PCwnX3/Y22+/Hf/xH/8Rra2tcfnll8fixYtj4sSJ+do8AMCQ61cYNTQ0xHPPPRfr16/v89EfL730UnznO9/pczXo5557LjZs2DCkHxECAJBP/bry9UsvvRTTp0/vEzunTp2K73//+1FSUhK33nprbNq0KW688cY4evRoPPXUU3kfGABgqPQrjN56662YM2dOn/v27NkTbW1t8du//duxePHiuOKKK+IrX/lKLFy4MH7yk5/kdVgAgKHUrzD63//93/j4xz/e577//u//jojoc7XpiIhf+IVfiKNHjw5yPACA4dOvMDrzA1lPe+WVV2LcuHFRVVXV5/7S0tIoLR2y60cCAORdv8Kouro6nn/++Th58mRERLz55puxf//+uOqqq+Kiiy7q89i33377rHeXAABGsn69pXPdddfFPffcE1//+tfjiiuuiAMHDkRExIoVK8567Isvvhjz5s3Lz5QF5gKPADA29CuMPvGJT8S3vvWteOqpp+Lw4cMxZ86c+PKXvxzV1dV9Hrdnz564+OKLY+HChXkdtlCG4mraAMDI48rXA+DK18NjtFxxlbHLGqbYjZY13J8rX/frHCMAgNFMGAEAJMIIACARRgAAiTACAEiEEQBA4jM7cuACjwAwNgijHLjAIwCMDQ6lAQAkwggAIBFGAACJMAIASIQRAEAijAAAEmEEAJAIIwCARBgBACTCCAAg8ZEgOfBZaQAwNgijHPisNAAYGxxKAwBIhBEAQCKMAAASYQQAkAgjAIBEGAEA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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -178,62 +171,38 @@
                 "        plt.xlabel('Rank')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Import networkx\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Done. Print something to stderr.\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "print(\"Import networkx\")\n",
                 "import networkx as nx\n",
                 "\n",
                 "for n in range(100):\n",
                 "    # Sort the index\n",
                 "    df_sorted = df.sort_values(by='id')\n",
                 "\n",
                 "    G = nx.Graph()\n",
                 "    for i, row in df_sorted.iterrows():\n",
                 "        if row.parent:\n",
-                "            G.add_edge(row.id, row.parent)\n",
-                "print(\"Done. Print something to stderr.\", file=sys.stderr)"
+                "            G.add_edge(row.id, row.parent)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/Users/laffra/microlog/logs/Treemap-Jupyter-Notebook/0.0.0/2023_07_12_18_16_23.log\n",
-                        "------------------------------------------------------------------------------------------\n",
-                        "Microlog Statistics for Treemap-Jupyter-Notebook:\n",
-                        "------------------------------------------------------------------------------------------\n",
-                        "- log size:    9,660 bytes\n",
-                        "- report URL:  http://127.0.0.1:4000/log/Treemap-Jupyter-Notebook/0.0.0/2023_07_12_18_16_23\n",
-                        "- duration:    6.697s\n",
-                        "------------------------------------------------------------------------------------------\n"
+                        "\ud83d\udcc8 Microlog \u00b7\u00b7\u00b7 9.7s \u00b7\u00b7\u00b7 10.9KB \u00b7\u00b7\u00b7 Treemap-Jupyter-Notebook \u00b7\u00b7\u00b7 http://127.0.0.1:4000/log/Treemap-Jupyter-Notebook/0.0.0/2023_07_24_13_09_28 \ud83d\ude80\n"
                     ]
                 }
             ],
             "source": [
                 "microlog.stop()"
             ]
         }
```

### Comparing `micrologai-1.3.0/microlog/api.py` & `micrologai-1.3.1/microlog/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,20 +44,18 @@
     log.log.addMarker(marker)
 
 
 class _Microlog():
     def __init__(self):
         self.running = False
 
-    def start(self, application: str = "", version: str = "", environment: str = ""):
+    def start(self, application: str = ""):
         from microlog import log
         self.stop()
         config.application = application
-        config.version = version
-        config.environment = environment
         log.start()
         self.startTracer()
         self.logEnvironment()
         self.running = True
 
     def logEnvironment(self):
         from microlog import debug
```

### Comparing `micrologai-1.3.0/microlog/config.py` & `micrologai-1.3.1/microlog/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,12 +35,10 @@
 sampleDelay: float = float(os.environ.get("MICROLOG_SAMPLE_DELAY", 0.1))
 
 IGNORE_MODULES = [
     "microlog.api",
     "microlog.tracer",
     "microlog.microlog",
     "microlog",
-    "importlib"
 ] 
 
-application = ""
-version = ""
+application = ""
```

### Comparing `micrologai-1.3.0/microlog/explain.py` & `micrologai-1.3.1/microlog/explain.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/anomaly.png` & `micrologai-1.3.1/microlog/images/anomaly.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/apple-touch-icon.png` & `micrologai-1.3.1/microlog/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/chatgpt.png` & `micrologai-1.3.1/microlog/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/design-go.png` & `micrologai-1.3.1/microlog/images/design-go.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/dialog.png` & `micrologai-1.3.1/microlog/images/dialog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/error-log.png` & `micrologai-1.3.1/microlog/images/error-log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/favicon-32x32.png` & `micrologai-1.3.1/microlog/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/fd-leak.png` & `micrologai-1.3.1/microlog/images/fd-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/asyncio.png` & `micrologai-1.3.1/microlog/images/icons/asyncio.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/dataclasses.png` & `micrologai-1.3.1/microlog/images/icons/dataclasses.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/email.png` & `micrologai-1.3.1/microlog/images/icons/email.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/google.png` & `micrologai-1.3.1/microlog/images/icons/google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/guppy.png` & `micrologai-1.3.1/microlog/images/icons/guppy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/http.png` & `micrologai-1.3.1/microlog/images/icons/http.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/jupyter.png` & `micrologai-1.3.1/microlog/images/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/matplotlib.png` & `micrologai-1.3.1/microlog/images/icons/matplotlib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/microlog.png` & `micrologai-1.3.1/microlog/images/icons/microlog.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/networkx.png` & `micrologai-1.3.1/microlog/images/icons/networkx.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/numpy.png` & `micrologai-1.3.1/microlog/images/icons/numpy.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/pandas.png` & `micrologai-1.3.1/microlog/images/icons/pandas.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/pyparsing.png` & `micrologai-1.3.1/microlog/images/icons/pyparsing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/pytest.png` & `micrologai-1.3.1/microlog/images/icons/pytest.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/python.png` & `micrologai-1.3.1/microlog/images/icons/python.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/re.png` & `micrologai-1.3.1/microlog/images/icons/re.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/squarify.png` & `micrologai-1.3.1/microlog/images/icons/squarify.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/ssl.png` & `micrologai-1.3.1/microlog/images/icons/ssl.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/tornado.png` & `micrologai-1.3.1/microlog/images/icons/tornado.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/urllib.png` & `micrologai-1.3.1/microlog/images/icons/urllib.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/wsgi.png` & `micrologai-1.3.1/microlog/images/icons/wsgi.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/icons/zmq.png` & `micrologai-1.3.1/microlog/images/icons/zmq.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/log.png` & `micrologai-1.3.1/microlog/images/log.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-bing.png` & `micrologai-1.3.1/microlog/images/logo-bing.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-brave.png` & `micrologai-1.3.1/microlog/images/logo-brave.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-duckduckgo.png` & `micrologai-1.3.1/microlog/images/logo-duckduckgo.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-google.png` & `micrologai-1.3.1/microlog/images/logo-google.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-hackernews.png` & `micrologai-1.3.1/microlog/images/logo-hackernews.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-sourcegraph.png` & `micrologai-1.3.1/microlog/images/logo-sourcegraph.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-stackoverflow.png` & `micrologai-1.3.1/microlog/images/logo-stackoverflow.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/logo-twitter.png` & `micrologai-1.3.1/microlog/images/logo-twitter.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/markdown.png` & `micrologai-1.3.1/microlog/images/markdown.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/memory-leak.png` & `micrologai-1.3.1/microlog/images/memory-leak.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/overview.png` & `micrologai-1.3.1/microlog/images/overview.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/status.png` & `micrologai-1.3.1/microlog/images/status.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/tips.png` & `micrologai-1.3.1/microlog/images/tips.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/images/zoomedin.png` & `micrologai-1.3.1/microlog/images/zoomedin.png`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/log.py` & `micrologai-1.3.1/microlog/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import defaultdict
 import datetime
 import os
 import re
 import sys
 import time
 import bz2
+import traceback;
 
 from microlog import config
 from microlog.models import Call
 from microlog.models import CallSite
 from microlog.models import Stack
 from microlog.models import Status
 from microlog.models import toGB
@@ -22,23 +23,26 @@
 debug = False
 
 class Log():
     def __init__(self):
         self.start()
 
     def start(self):
+        self.running = True
         self.calls = []
         self.markers = []
         self.statuses = []
         self.begin = time.perf_counter()
 
     def now(self):
         return time.perf_counter() - self.begin
 
     def addCall(self, call: Call):
+        if not self.running: 
+            return
         self.calls.append(call)
 
     def addStatus(self, status: Status):
         self.statuses.append(status)
 
     def addMarker(self, marker: Marker):
         self.markers.append(marker)
@@ -86,14 +90,15 @@
                 self.calls.append(Call.load(line, callSites))
             elif kind == config.EVENT_KIND_STATUS:
                 self.statuses.append(Status.load(line, symbols))
             elif kind == config.EVENT_KIND_MARKER:
                 self.markers.append(Marker.load(line, symbols, stacks))
 
     def stop(self):
+        self.running = False
         if not getApplication():
             return
         uncompressed = bytes(self.save(), encoding="utf-8")
         identifier = getIdentifier()
         path = getLogPath(identifier)
         if debug:
             with open(path.replace(".zip",""), "w") as fd:
@@ -104,15 +109,15 @@
         if not verbose:
             return
         if "VSCODE_CWD" in os.environ and not "ipykernel" in sys.modules:
             return
         self.showDetails(path, identifier)
     
     def showDetails(self, path, identifier):
-        application, version, _ = identifier.split("/")
+        application, _ = identifier.split("/")
         duration = self.now()
         sys.stdout.write(f"📈 Microlog ··· {duration:.1f}s ··· {toGB(os.stat(path).st_size)} ··· {application} ··· {f'http://127.0.0.1:4000/log/{identifier}'} 🚀\n")
 
 log = Log()
 
 
 def start():
@@ -128,40 +133,17 @@
     if config.application:
          return config.application
     name = sys.argv[0] if sys.argv[0] != "-c" else sys.argv[1] if sys.argv[0] == "-m" else "python"
     name = "-".join(name.split("/")[-3:])
     name = name.replace("python-site-packages-", "").replace(".py", "")
     return name
 
-
-def getVersion():
-    from microlog import config
-    if config.version:
-         return config.version
-    path = os.path.abspath(sys.argv[0])
-    while path != "/":
-        setup = os.path.join(path, "setup.py")
-        if os.path.exists(setup):
-            import ast
-            with open(setup) as fd:
-                tree = ast.parse(fd.read())
-                for line in ast.dump(tree, indent=4).split("\n"):
-                    if re.search("value='[0-9.]*'", line):
-                        return re.sub(r".*value='([0-9.]*)'.*", r"\1", line)
-        path = os.path.dirname(path)
-    return "0.0.0"
-
-
-def getEnvironment():
-    return "dev"
-
-
 def getIdentifier():
     date = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
-    return f"{getApplication()}/{getVersion()}/{date}"
+    return f"{getApplication()}/{date}"
 
 
 def getLogPath(identifier):
     import appdata
     paths = appdata.AppDataPaths('microlog')
     if paths.require_setup:
         paths.setup()
```

### Comparing `micrologai-1.3.0/microlog/models.py` & `micrologai-1.3.1/microlog/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         name = frame.f_code.co_name
         if self.ignore(module):
             return None
         return CallSite(filename, lineno, f"{module}.{clazz}.{name}")
         
     def ignore(self, module):
         from microlog import config
-        return module in config.IGNORE_MODULES or module.startswith("importlib.")
+        return module in config.IGNORE_MODULES
 
     def __iter__(self):
         return iter(self.callSites)
 
     def __len__(self):
         return len(self.callSites)
```

### Comparing `micrologai-1.3.0/microlog/server.py` & `micrologai-1.3.1/microlog/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,27 @@
                 import urllib
                 query = urllib.parse.urlparse(self.path).query
                 query_components = dict(qc.split("=") for qc in query.split("&"))
                 filter = query_components["filter"]
                 logs = []
                 for root, dirs, files in os.walk(paths.logs_path, topdown=False):
                     for name in sorted([file for file in files if file.endswith(".zip")]):
-                        application, version = root.split("/")[-2:]
+                        application = root.split("/")[-1]
                         if name.endswith(".zip") and filter in root:
-                            logs.append(f"{application}/{version}/{name[:-4]}\n")
+                            logs.append(f"{application}/{name[:-4]}\n")
                 return self.sendData("text/html", bytes("\n".join(logs), encoding="utf-8"))
 
             if self.path.startswith("/zip/"):
                 name = f"{self.path[5:]}.log.zip".replace("%20", " ")
                 return self.sendData("application/microlog", self.readLog(name))
 
             if self.path.startswith("/delete/"):
                 name = f"{self.path[8:]}.log.zip".replace("%20", " ")
+                if name.startswith("logs/"):
+                    name = name[5:]
                 path = os.path.join(paths.logs_path, name)
                 os.remove(path)
                 return self.sendData("text/html", bytes("OK", encoding="utf-8"))
 
             if self.path.startswith("/explain/"):
                 import explain
                 name = f"{self.path[9:]}.log.zip".replace("%20", " ")
@@ -87,14 +89,16 @@
         except Exception as e:
             logging.error(e)
             import traceback
             traceback.print_exc()
             return str(e)
 
     def readLog(self, name):
+        if name.startswith("logs/"):
+            name = name[5:]
         path = os.path.join(paths.logs_path, name)
         with open(path, "rb") as fd:
             compressed = fd.read()
         return bz2.decompress(compressed)
         
     def sendData(self, kind, data):
         self.send_response(200)
```

### Comparing `micrologai-1.3.0/microlog/sitecustomize.py` & `micrologai-1.3.1/microlog/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/microlog/tracer.py` & `micrologai-1.3.1/microlog/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,16 @@
     def sample(self, function=None) -> None:
         """
         Samples all threads.
 
         Parameters:
         - function: The function to add to the current stack trace, when using a decorator.
         """
+        if not self.running:
+            return
         from microlog import log
         when = log.log.now()
         frames = sys._current_frames()
         for threadId, frame in frames.items():
             if threadId != self.ident:
                 self.merge(threadId, self.getStack(when, threadId, frame, function))
         for threadId in list(self.stacks.keys()):
```

### Comparing `micrologai-1.3.0/micrologai.egg-info/PKG-INFO` & `micrologai-1.3.1/micrologai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrologai
-Version: 1.3.0
+Version: 1.3.1
 Summary: A continuous profiler and logger for Python written entirely in Python
 Home-page: https://www.chrislaffra.org/
 Author: Chris Laffra
 Author-email: Chris Laffra <chris@chrislaffra.com>
 License:                      Server Side Public License
                              VERSION 1, OCTOBER 16, 2018
         
@@ -569,261 +569,78 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # microlog.ai
 
-_Microlog_ is a continuous profiler and logger for the Python language.
-Logs and performance profiles are collected and analyzed.
-_Microlog_ explains application behavior using interactive graphs.
-It summarizes and explains the code using AI.
-
-_Microlog_ makes understanding complex applications easy, reducing support costs
+_Microlog_ is a continuous profiler and logger for the Python language that
+explains application behavior using interactive graphs and AI. 
+It makes understanding complex applications easy, reducing support costs
 and shortening production problems, increasing application quality, and minimizing outages.
 
+_Microlog_ has extremely low runtime overhead (~1%) and exceptionally fast rendering (~20ms).
+It saves logs and performance profiles on the local file system. The logs are
+compressed exceptionally well, resulting in a remarkably low 0.5MB per hour of recording.
+
+This project is written in 100% Python. The recorder is a Python module that uses a separate thread to sample 
+performance and record logs. The UI is written in Python as well, rendered in the browser by Python code using
+PyScript. As a result, the identical Python classes encode _and_ decode the recordings, avoiding the need
+for cumbersome cross-language data modeling. 
+
+_Microlog_ is open source, with an available commercial license. We welcome extensions to _Microlog_ from
+the Python performance community, such as 
+recording of special events, new optimizations related to PyScript,
+or centralization of recordings into central storage systems, using `rsync`, `scp`, or `Google Drive`.
+
 # Installing microlog.ai
 
 To install _Microlog_ from pypi run:
-```
-python3 -m pip install microlog
+```console
+pip install micrologai
 ```
 
 To install _Microlog_ globally using a `sitecustomize.py`, run:
 
-```
-  git clone https://github.com/micrologai/microlog
-  cd micrologai/microlog
-  python3 setup.py install
+```console
+git3 clone https://github.com/micrologai/microlog
+cd micrologai/microlog
+python3 setup.py install
 ```
 
 # How to use microlog.ai
 
-If you used the setup command shown above, 
-any time a Python process runs using the same runtime you used to setup _Microlog_, it will automatically trigger _Microlog_ to generate a recording. 
+If you used the setup command shown above, _Microlog_ is enabled for all Python processes running on that Python VM. 
 
 To use microlog manually, use:
-```
-  import microlog
-
-  with microlog.enabled():
-      # run any Python code
-```
-
-To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
-
-```
-  sh examples/runall.sh
-```
-
-This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
-
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
-```
-
-This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
-The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
-you can start it as follows:
-
-```
-  python3 microlog/server.py
-```
-
-# The Microlog.ai UI 
-
-To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
-
-The main elements of the UI are:
-
- - `Log list`, at the left, showing currently available logs on the local machine.
- - `Timeline`, the starting point for analysis of your application:
-    - `Status`, providing insights into CPU, memory, and I/O.
-    - `Timescale`, with ticks for second elapsed since start.
-    - `Flamegraph`, showing the result of the continuous profiler. 
- - `Design`, showing a graphical rendering of the structure of the application.
- - `Log`, listing all print and logging output and statistics in a chronological order.
- - `Explanation`, giving a human language description of your code, using OpenAIs' ChatGPT.
- - `Tips`, linking to best practices and tips for the modules used in your code.
-
-
-## Timeline Navigation and Zoom
-
-Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
-
-![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
-
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
-
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
-
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
-
-## Timeline Anomaly Detection
-
-When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
-
-Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
-
-![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
-
-## Timeline Detecting expensive I/O or Starved Processes
-
-The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
-Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
-
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
-
-## Timeline Integrating Profiling with Logging
-
-Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
-
-![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
-
-## Formatting Logs with Markdown
-
-Log entries can be formatted using Markdown to make it easier to show important information to the reader.
-
-![Using markdown for log entries](https://github.com/micrologai/microlog/raw/main/microlog/images/markdown.png)
-
-# Logging 
-
-_Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
-added to the _Microlog_ event log.  
-
-Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
-
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
-
-   import logging
-   logger = logging.Logger("Microlog Demo")
-
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
-   
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
-```
-
-# Design
-
-The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
-Here is an example for `examples\go.py`:
+import microlog
 
-![Microlog's innovative design graph](https://github.com/micrologai/microlog/raw/main/microlog/images/design-go.png)
-
-# Log
-
-The log tab contains a chronological listing of all print and logging output, statistics, and analysis performed by _Microlog_ in a more traditional linear log style:
-
-![Microlog's traditional log, with a twist](https://github.com/micrologai/microlog/raw/main/microlog/images/log.png)
-
-The links shown in lightblue directly take you to the source file where the print took place. This makes it extremely easy to figure out what code prints what exactly. For the `files.py` example, the log shows that this program leaked one file descriptor. That same report is also shown in the timeline when you click at the warning icon at the end of the run. 
-The popup also shows a link to the source location where the file was opened:
-
-![Detecting leaked file descriptors](https://github.com/micrologai/microlog/raw/main/microlog/images/fd-leak.png)
-
-## Log - Memory Leaks
-
-In addition to checking for leaked file descriptors, _Microlog_ aims to detect memory leaks. Those objects that were
-allocated but cannot be garbage-collected as they are either reachable from a module or are involed in a reference cycle that
-cannot be broken. The following report shows the top-10 offenders for the `dataframes.py` example, that uses Pandas dataframes.
-
-![Detecting memory leaks](https://github.com/micrologai/microlog/raw/main/microlog/images/memory-leak.png)
-
-# Explanation
-
-The explanation tab shows a human-language explanation provided by OpenAI's `ChatGPT` to explain the design and implementation behind the application being monitored by _Microlog_. This analysis is not performed on the source code, but on a condensed call graph generated from the performance log that was recorded by _Microlog_. Here is an example of the what `ChatGPT` thinks of
-our `examples\go.py` execution:
-
-![ChatGPT's simple explanation of complex Python code](https://github.com/micrologai/microlog/raw/main/microlog/images/chatgpt.png)
-
-# Tips
-
-To discover best practices, performance tips, or tutorials for modules being used by the application, _Microlog_ offers quick
-links to general information sources, such as search engines and Q&A sites:
-
-![Tips make you a better Python developer](https://github.com/micrologai/microlog/raw/main/microlog/images/tips.png)
-
-
-# Developer Notes
-
-## Run all unit tests
-
-```
-python3 -m unittest discover tests
+with microlog.enabled():
+    # run any Python code
 ```
 
+To give you an idea of the features of _Microlog_, you could run all the examples. This does assume you set up microlog globally. In that case, run:
 
-## Upload new version to PyPi
-
-First build the package into a source distribution and a Python wheel:
-```
-python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
-```
-
-Then verify whether the build works for pypi:
-```
-twine check dist/*
-```
-
-Then upload to the pypi test environment:
-```
-twine upload --repository pypitest dist/*
-```
-
-```
-twine upload dist/*
-```
-
-# License
-
-
-
-## Run all examples
-
-```
+```console
 sh examples/runall.sh
 ```
 
-# License
-
-_Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
-
-
-
-To give you an idea of the features, of _Microlog_, run all the examples:
-
-```
-  sh examples/runall.sh
-```
-
 This runs for a minute and eventually produces 13 logs. You will see lines appear looking like this:
 
-```
-📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/0.1.1/2023_07_12_10_24_53 🚀
+```console
+📈 Microlog ··· 26.3s ··· 4.6KB ··· examples-memory ··· http://127.0.0.1:4000/log/examples-memory/2023_07_12_10_24_53 🚀
 ```
 
 This shows how long the app ran, the size of the (compressed) log, its name, and a URL to view the result.
 The report URL is rendered by the _Microlog_ server implemented in `microlog/server.py`.  If it is not yet running,
 you can start it as follows:
 
-```
-  python3 microlog/server.py
+```console
+python3 microlog/server.py
 ```
 
 # The Microlog.ai UI 
 
 To describe the UI features of _Microlog_, we will look at the output of the `examples\memory.py` example:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/overview.png)
@@ -843,35 +660,35 @@
 
 ## Timeline Navigation and Zoom
 
 Using the mouse, the dashboard can be panned and zoomed. More details will be shown when zoomed in deeper:
 
 ![Example run of microlog](https://github.com/micrologai/microlog/raw/main/microlog/images/zoomedin.png)
 
-In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scrollwheel on the mouse.
+In the above example, we panned the flame graph by grabbing it with the mouse and zoomed in using the scroll wheel on the mouse.
 
-In addition, we clicked on a method call in the flame graph, which is now highlight in red. A moveable popup dialog shows details about the method, such as average CPU during the call. A CPU percentage below 100% means the process is involved
-in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), or async or thread synchronization, or other system level event handling using `select` or event handlers. 
+In addition, we clicked on a method call in the flame graph, which is now highlighted in red. A moveable popup dialog shows details about the method, such as the average CPU during the call. A CPU percentage below 100% means the process is involved
+in reading or writing files on the local disk, loading or sending data over sockets, loading new modules (requiring disk I/O), async or thread synchronization, or other system-level event handling using `select` or event handlers. 
 
-Low CPU typically indicates a bottleneck and warrants in-depth investigation.
+A low CPU typically indicates a bottleneck and warrants in-depth investigation.
 
 ## Timeline Anomaly Detection
 
 When a method is selected in the flame graph, the popup shows information about similar calls detected in the same run, showing when they ran and how long they ran. _Microlog_ also uses anomaly detection to highlight methods you may want to investigate in more detail. In the screenshot below, the average call duration is 1 second, and four calls were more than 50% over the average. 
 
 Automatic anomaly detection, call stack analysis, and process health indicators offered by _Microlog_ allow you to debug performance/quality issues quickly.
 
 ![Anomaly detection in the Microlog UI](https://github.com/micrologai/microlog/raw/main/microlog/images/anomaly.png)
 
 ## Timeline Detecting expensive I/O or Starved Processes
 
 The top bar shows general statistics for the process, such as CPU and number of modules loaded over time. 
 Note that a low CPU in the top bar tends to indicate I/O took place at that moment.
 
-![Mircolog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
+![Microlog's status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/status.png)
 
 ## Timeline Integrating Profiling with Logging
 
 Log entries are shown as visual markers in the top bar. Because _Microlog_ shows log entries on the timeline, analyzing problems becomes much easier than with normal logs. No more scrolling page after page to find a stack trace. With _Microlog_, they appear as easy-to-see stop signs:
 
 ![Log entries in the status bar](https://github.com/micrologai/microlog/raw/main/microlog/images/error-log.png)
 
@@ -885,29 +702,29 @@
 
 _Microlog_ detects calls to `print` and `logging`. Those calls are automatically intercepted
 added to the _Microlog_ event log.  
 
 Manual log entries can be inserted into Microlog using `info`, `warn`, `debug`, and `error`:
 
 ```python
-   print("Add a log entry to microlog with an info marker...")
-   print("... or as an error marker.", stream=sys.stderr)
+print("Add a log entry to microlog with an info marker...")
+print("... or as an error marker.", stream=sys.stderr)
 
-   import logging
-   logger = logging.Logger("Microlog Demo")
+import logging
+logger = logging.Logger("Microlog Demo")
 
-   logger.info("Add a log entry to microlog with an info marker...")
-   logger.debug("... or a bug marker...")
-   logger.warning("... or a warning marker...")
-   logger.error("... or an error marker.")
+logger.info("Add a log entry to microlog with an info marker...")
+logger.debug("... or a bug marker...")
+logger.warning("... or a warning marker...")
+logger.error("... or an error marker.")
    
-   microlog.info("Add something to the log explicitly...")
-   microlog.warning("... as a warning...")
-   microlog.debug("... as a debug message...")
-   microlog.error("... as an error.")
+microlog.info("Add something to the log explicitly...")
+microlog.warning("... as a warning...")
+microlog.debug("... as a debug message...")
+microlog.error("... as an error.")
 ```
 
 # Design
 
 The Design tab analyzes the runtime call graph and draws a structural diagram of the underlying design of your application.
 Here is an example for `examples\go.py`:
 
@@ -955,41 +772,30 @@
 python3 -m unittest discover tests
 ```
 
 
 ## Upload new version to PyPi
 
 First build the package into a source distribution and a Python wheel:
-```
+```console
 python3 -m pip install --user --upgrade setuptools wheel twine build
-python3 -m build --sdist
-python3 -m build --wheel
+python3 -m build
 ```
 
 Then verify whether the build works for pypi:
-```
+```console
 twine check dist/*
 ```
 
 Then upload to the pypi test environment:
-```
+```console
 twine upload --repository pypitest dist/*
 ```
 
-If that looks fine, upload to the real pypi environment:
-```
+Finally, if the pypi test upload appears to work fine, run:
+```console
 twine upload dist/*
 ```
 
 # License
 
-
-
-## Run all examples
-
-```
-sh examples/runall.sh
-```
-
-# License
-
 _Microlog_ is released under version 1 of the [Server Side Public License (SSPL)](LICENSE).
```

### Comparing `micrologai-1.3.0/micrologai.egg-info/SOURCES.txt` & `micrologai-1.3.1/micrologai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/pyproject.toml` & `micrologai-1.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micrologai"
-version = "1.3.0"
+version = "1.3.1"
 description = "A continuous profiler and logger for Python written entirely in Python"
 readme = "README.md"
 authors = [{ name = "Chris Laffra", email = "chris@chrislaffra.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `micrologai-1.3.0/setup.py` & `micrologai-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='Microlog',
     description='A continuous profiler and logger for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.3.0',
+    version='1.3.1',
     author='Chris Laffra',
     author_email='laffra@gmail.com',
     url='https://www.chrislaffra.org/',
     packages=setuptools.find_packages(include=[
         'microlog',
         'dashboard',
     ]),
```

### Comparing `micrologai-1.3.0/tests/test_call_view.py` & `micrologai-1.3.1/tests/test_call_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_canvas.py` & `micrologai-1.3.1/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_marker_view.py` & `micrologai-1.3.1/tests/test_marker_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_print.py` & `micrologai-1.3.1/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_status.py` & `micrologai-1.3.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_status_view.py` & `micrologai-1.3.1/tests/test_status_view.py`

 * *Files identical despite different names*

### Comparing `micrologai-1.3.0/tests/test_tracer.py` & `micrologai-1.3.1/tests/test_tracer.py`

 * *Files identical despite different names*

