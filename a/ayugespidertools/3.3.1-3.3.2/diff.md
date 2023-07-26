# Comparing `tmp/ayugespidertools-3.3.1.tar.gz` & `tmp/ayugespidertools-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.3.1.tar", max compression
+gzip compressed data, was "ayugespidertools-3.3.2.tar", max compression
```

## Comparing `ayugespidertools-3.3.1.tar` & `ayugespidertools-3.3.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/LICENSE
--rw-r--r--   0        0        0    14144 2023-06-21 05:41:38.000000 ayugespidertools-3.3.1/README.md
--rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.1/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.1/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.3.1/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.1/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.3.1/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-07 02:13:50.000000 ayugespidertools-3.3.1/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6610 2023-06-07 02:13:56.000000 ayugespidertools-3.3.1/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     5265 2023-06-09 09:17:13.000000 ayugespidertools-3.3.1/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    16918 2023-06-20 02:40:39.000000 ayugespidertools-3.3.1/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13306 2023-06-07 01:56:44.000000 ayugespidertools-3.3.1/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32649 2023-06-20 01:18:52.000000 ayugespidertools-3.3.1/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     6000 2023-06-06 07:14:58.000000 ayugespidertools-3.3.1/ayugespidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3718 2023-06-07 02:14:02.000000 ayugespidertools-3.3.1/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     3577 2023-06-26 09:54:18.000000 ayugespidertools-3.3.1/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    10672 2023-06-20 02:00:17.000000 ayugespidertools-3.3.1/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3685 2023-06-07 02:14:19.000000 ayugespidertools-3.3.1/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      388 2023-06-07 02:14:26.000000 ayugespidertools-3.3.1/ayugespidertools/config.py
--rw-r--r--   0        0        0     9982 2023-06-07 02:14:34.000000 ayugespidertools-3.3.1/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7673 2023-06-07 02:14:39.000000 ayugespidertools-3.3.1/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     6383 2023-06-29 08:59:35.000000 ayugespidertools-3.3.1/ayugespidertools/items.py
--rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.1/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8542 2023-06-07 02:14:45.000000 ayugespidertools-3.3.1/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.1/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5448 2023-06-09 09:27:15.000000 ayugespidertools-3.3.1/ayugespidertools/oss.py
--rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.1/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.1/ayugespidertools/request.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 06:57:30.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/__init__.py
--rw-r--r--   0        0        0     1644 2023-06-26 09:00:55.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10562 2023-06-19 03:16:03.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     3779 2023-06-07 02:15:17.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2429 2023-06-07 02:15:24.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/__init__.py
--rw-r--r--   0        0        0     2453 2023-06-25 08:49:18.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1495 2023-06-19 09:43:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2046 2023-06-19 09:44:14.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1183 2023-06-19 09:44:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3180 2023-06-07 09:54:44.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     1779 2023-06-07 09:52:37.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0    11430 2023-06-20 02:32:25.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     3851 2023-06-19 09:45:42.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-06-16 03:09:25.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2734 2023-06-06 08:35:52.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3608 2023-06-19 09:45:59.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7944 2023-06-21 08:29:00.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.1/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.1/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     5168 2023-06-21 08:26:39.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.1/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.1/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.3.1/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3074 2023-06-29 07:47:06.000000 ayugespidertools-3.3.1/pyproject.toml
--rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 ayugespidertools-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/LICENSE
+-rw-r--r--   0        0        0     9808 2023-07-25 03:00:57.000000 ayugespidertools-3.3.2/README.md
+-rw-r--r--   0        0        0      433 2023-06-20 01:16:24.000000 ayugespidertools-3.3.2/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.3.2/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:44:00.000000 ayugespidertools-3.3.2/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.3.2/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      503 2023-07-25 06:46:03.000000 ayugespidertools-3.3.2/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3636 2023-07-18 06:55:41.000000 ayugespidertools-3.3.2/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6562 2023-07-18 06:58:54.000000 ayugespidertools-3.3.2/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     5181 2023-07-18 07:01:23.000000 ayugespidertools-3.3.2/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16320 2023-07-25 07:41:37.000000 ayugespidertools-3.3.2/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    12726 2023-07-18 07:24:16.000000 ayugespidertools-3.3.2/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32637 2023-07-18 07:24:36.000000 ayugespidertools-3.3.2/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     5980 2023-07-18 07:24:56.000000 ayugespidertools-3.3.2/ayugespidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3688 2023-07-18 08:47:02.000000 ayugespidertools-3.3.2/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     3567 2023-07-18 07:26:36.000000 ayugespidertools-3.3.2/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    17832 2023-07-25 09:12:39.000000 ayugespidertools-3.3.2/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3642 2023-07-18 07:30:17.000000 ayugespidertools-3.3.2/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      376 2023-07-25 06:28:48.000000 ayugespidertools-3.3.2/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9615 2023-07-18 07:47:21.000000 ayugespidertools-3.3.2/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7568 2023-07-25 07:44:00.000000 ayugespidertools-3.3.2/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     6254 2023-07-18 08:52:39.000000 ayugespidertools-3.3.2/ayugespidertools/items.py
+-rw-r--r--   0        0        0      752 2023-06-07 06:21:31.000000 ayugespidertools-3.3.2/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8458 2023-07-18 07:52:38.000000 ayugespidertools-3.3.2/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2023-06-07 02:14:51.000000 ayugespidertools-3.3.2/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5368 2023-07-18 07:53:41.000000 ayugespidertools-3.3.2/ayugespidertools/oss.py
+-rw-r--r--   0        0        0     1129 2023-06-21 02:34:36.000000 ayugespidertools-3.3.2/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.3.2/ayugespidertools/request.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1340 2023-07-18 07:30:35.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-18 07:30:49.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      900 2023-06-19 02:30:56.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:57:30.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-18 07:31:13.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      232 2023-06-07 06:21:21.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10391 2023-07-18 07:33:53.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3747 2023-07-18 07:34:22.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2417 2023-07-18 07:34:34.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     1154 2023-06-21 02:33:49.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 02:39:39.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2441 2023-07-18 07:34:59.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-18 07:35:17.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2044 2023-07-18 07:36:59.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1171 2023-07-18 07:37:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3093 2023-07-18 07:38:54.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     1769 2023-07-18 07:39:07.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    11172 2023-07-18 07:40:39.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     3831 2023-07-18 07:40:57.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      326 2023-07-18 07:41:07.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1696 2023-07-18 07:41:25.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2722 2023-07-18 07:41:38.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3589 2023-07-18 07:42:26.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7252 2023-07-20 09:38:27.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-18 07:43:50.000000 ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.3.2/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      820 2023-06-07 01:45:35.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.3.2/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     5148 2023-07-18 07:44:41.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1673 2023-06-20 01:20:48.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.3.2/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.3.2/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.3.2/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6910 2023-07-18 07:54:34.000000 ayugespidertools-3.3.2/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     2979 2023-07-26 02:48:20.000000 ayugespidertools-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11436 1970-01-01 00:00:00.000000 ayugespidertools-3.3.2/PKG-INFO
```

### Comparing `ayugespidertools-3.3.1/LICENSE` & `ayugespidertools-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/README.md` & `ayugespidertools-3.3.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,884 +1,613 @@
-00000000: 215b 6179 7567 6573 7069 6465 7274 6f6f  ![ayugespidertoo
-00000010: 6c73 2d6c 6f67 6f5d 2868 7474 7073 3a2f  ls-logo](https:/
-00000020: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000030: 6f6e 7465 6e74 2e63 6f6d 2f73 6865 6e67  ontent.com/sheng
-00000040: 6368 656e 7961 6e67 2f41 7975 6765 5370  chenyang/AyugeSp
-00000050: 6964 6572 546f 6f6c 732f 6d61 696e 2f61  iderTools/main/a
-00000060: 7274 776f 726b 2f61 7975 6765 7370 6964  rtwork/ayugespid
-00000070: 6572 746f 6f6c 732d 6c6f 676f 2e70 6e67  ertools-logo.png
-00000080: 290d 0a0d 0a5b 215b 4f53 4353 2053 7461  )....[![OSCS Sta
-00000090: 7475 735d 2868 7474 7073 3a2f 2f77 7777  tus](https://www
-000000a0: 2e6f 7363 7331 3032 342e 636f 6d2f 706c  .oscs1024.com/pl
-000000b0: 6174 666f 726d 2f62 6164 6765 2f41 7975  atform/badge/Ayu
-000000c0: 6765 5370 6964 6572 546f 6f6c 732e 7376  geSpiderTools.sv
-000000d0: 673f 7369 7a65 3d73 6d61 6c6c 295d 2868  g?size=small)](h
-000000e0: 7474 7073 3a2f 2f77 7777 2e6d 7572 7068  ttps://www.murph
-000000f0: 7973 6563 2e63 6f6d 2f61 6363 6570 743f  ysec.com/accept?
-00000100: 636f 6465 3d30 6563 3337 3537 3539 6165  code=0ec375759ae
-00000110: 6265 6137 6664 3236 3032 3438 3931 3062  bea7fd260248910b
-00000120: 3938 3830 3626 7479 7065 3d31 2666 726f  98806&type=1&fro
-00000130: 6d3d 3229 0d0a 215b 4769 7448 7562 5d28  m=2)..![GitHub](
-00000140: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000150: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-00000160: 6365 6e73 652f 7368 656e 6763 6865 6e79  cense/shengcheny
-00000170: 616e 672f 4179 7567 6553 7069 6465 7254  ang/AyugeSpiderT
-00000180: 6f6f 6c73 290d 0a21 5b70 7974 686f 6e5d  ools)..![python]
-00000190: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000001a0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-000001b0: 7468 6f6e 2d33 2e38 2e31 2532 422d 626c  thon-3.8.1%2B-bl
-000001c0: 7565 290d 0a21 5b47 6974 4875 6220 576f  ue)..![GitHub Wo
-000001d0: 726b 666c 6f77 2053 7461 7475 7320 2877  rkflow Status (w
-000001e0: 6974 6820 6272 616e 6368 295d 2868 7474  ith branch)](htt
-000001f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000200: 2e69 6f2f 6769 7468 7562 2f61 6374 696f  .io/github/actio
-00000210: 6e73 2f77 6f72 6b66 6c6f 772f 7374 6174  ns/workflow/stat
-00000220: 7573 2f73 6865 6e67 6368 656e 7961 6e67  us/shengchenyang
-00000230: 2f41 7975 6765 5370 6964 6572 546f 6f6c  /AyugeSpiderTool
-00000240: 732f 636f 6465 716c 2e79 6d6c 3f62 7261  s/codeql.yml?bra
-00000250: 6e63 683d 6d61 696e 290d 0a21 5b52 6561  nch=main)..![Rea
-00000260: 6420 7468 6520 446f 6373 5d28 6874 7470  d the Docs](http
-00000270: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000280: 696f 2f72 6561 6474 6865 646f 6373 2f61  io/readthedocs/a
-00000290: 7975 6765 7370 6964 6572 746f 6f6c 7329  yugespidertools)
-000002a0: 0d0a 215b 4769 7448 7562 2061 6c6c 2072  ..![GitHub all r
-000002b0: 656c 6561 7365 735d 2868 7474 7073 3a2f  eleases](https:/
-000002c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000002d0: 6769 7468 7562 2f64 6f77 6e6c 6f61 6473  github/downloads
-000002e0: 2f73 6865 6e67 6368 656e 7961 6e67 2f41  /shengchenyang/A
-000002f0: 7975 6765 5370 6964 6572 546f 6f6c 732f  yugeSpiderTools/
-00000300: 746f 7461 6c3f 6c61 6265 6c3d 7265 6c65  total?label=rele
-00000310: 6173 6573 2532 3064 6f77 6e6c 6f61 6473  ases%20downloads
-00000320: 290d 0a21 5b50 7950 4920 2d20 446f 776e  )..![PyPI - Down
-00000330: 6c6f 6164 735d 2868 7474 7073 3a2f 2f69  loads](https://i
-00000340: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000350: 7069 2f64 6d2f 4179 7567 6553 7069 6465  pi/dm/AyugeSpide
-00000360: 7254 6f6f 6c73 3f6c 6162 656c 3d70 7970  rTools?label=pyp
-00000370: 6925 3230 646f 776e 6c6f 6164 7329 0d0a  i%20downloads)..
-00000380: 0d0a 2320 4179 7567 6553 7069 6465 7254  ..# AyugeSpiderT
-00000390: 6f6f 6c73 20e5 b7a5 e585 b7e8 afb4 e698  ools ...........
-000003a0: 8e0d 0a0d 0a3e 20e4 b880 e58f a5e8 af9d  .....> .........
-000003b0: e4bb 8be7 bb8d efbc 9ae7 94a8 e4ba 8ee6  ................
-000003c0: 89a9 e5b1 9520 6053 6372 6170 7960 20e5  ..... `Scrapy` .
-000003d0: 8a9f e883 bde6 9da5 e8a7 a3e6 94be e58f  ................
-000003e0: 8ce6 898b efbc 8ce8 bf98 e586 85e7 bdae  ................
-000003f0: e4b8 80e4 ba9b e788 ace8 99ab e5bc 80e5  ................
-00000400: 8f91 e4b8 ade7 9a84 e980 9ae7 94a8 e696  ................
-00000410: b9e6 b395 e380 820d 0a0d 0a23 2320 e589  ...........## ..
-00000420: 8de8 a880 0d0a 0d0a e59c a8e4 bdbf e794  ................
-00000430: a820 6050 7974 686f 6e60 2060 5363 7261  . `Python` `Scra
-00000440: 7079 6020 e5ba 93e5 bc80 e58f 91e7 88ac  py` ............
-00000450: e899 abe6 97b6 efbc 8ce5 858d e4b8 8de4  ................
-00000460: ba86 e4bc 9ae9 878d e5a4 8de7 9a84 e4bf  ................
-00000470: aee6 94b9 e592 8ce7 bc96 e586 9920 6073  ............. `s
-00000480: 6574 7469 6e67 732e 7079 60ef bc8c 6069  ettings.py`...`i
-00000490: 7465 6d2e 7079 60ef bc8c 606d 6964 646c  tem.py`...`middl
-000004a0: 6577 6172 6573 2e70 7960 efbc 8c60 7069  ewares.py`...`pi
-000004b0: 7065 6c69 6e65 732e 7079 6020 e592 8ce4  pelines.py` ....
-000004c0: b880 e4ba 9be9 809a e794 a8e6 96b9 e6b3  ................
-000004d0: 95e6 8896 e884 9ae6 9cac efbc 8ce4 bd86  ................
-000004e0: e585 b6e5 ae9e e590 84e4 b8aa e9a1 b9e7  ................
-000004f0: 9bae e4b8 ade7 9a84 e8bf 99e4 ba9b e696  ................
-00000500: 87e4 bbb6 e586 85e5 aeb9 e5a4 a7e8 87b4  ................
-00000510: e79b b8e5 908c efbc 8ce9 82a3 e4b8 bae4  ................
-00000520: bd95 e4b8 8de6 8a8a e4bb 96e4 bbac e7bb  ................
-00000530: 9fe4 b880 e695 b4e7 9086 e59c a8e4 b880  ................
-00000540: e8b5 b7e5 91a2 e380 82e8 99bd e8af b4e5  ................
-00000550: 8faf e4bb a5e4 bdbf e794 a820 6073 6372  ........... `scr
-00000560: 6170 7960 20e7 9a84 e6a8 a1e6 9dbf e58a  apy` ...........
-00000570: 9fe8 83bd efbc 8ce4 bd86 e8bf 98e6 98af  ................
-00000580: e697 a0e6 b395 e980 82e9 858d e689 80e6  ................
-00000590: 9c89 e79a 84e5 bc80 e58f 91e5 9cba e699  ................
-000005a0: afe3 8082 0d0a 0d0a e588 9ae5 bc80 e5a7  ................
-000005b0: 8be6 8891 e4b9 9fe5 8faa e698 afe6 83b3  ................
-000005c0: e68a 8ae5 ae83 e794 a8e6 9da5 e980 82e9  ................
-000005d0: 858d 2060 4d79 7371 6c60 20e5 ad98 e582  .. `Mysql` .....
-000005e0: a8e7 9a84 e59c bae6 99af efbc 8ce5 8faf  ................
-000005f0: e4bb a5e8 87aa e58a a8e5 889b e5bb bae7  ................
-00000600: 9bb8 e585 b3e6 95b0 e68d aee5 ba93 efbc  ................
-00000610: 8ce6 95b0 e68d aee8 a1a8 efbc 8ce5 ad97  ................
-00000620: e6ae b5e6 b3a8 e987 8aef bc8c e887 aae5  ................
-00000630: 8aa8 e6b7 bbe5 8aa0 e696 b0e6 b7bb e58a  ................
-00000640: a0e7 9a84 e5ad 97e6 aeb5 efbc 8ce5 928c  ................
-00000650: e887 aae5 8aa8 e4bf aee5 a48d e5b8 b8e8  ................
-00000660: a781 efbc 88e5 ad97 e6ae b5e7 bc96 e7a0  ................
-00000670: 81ef bc8c 6044 6174 6120 746f 6f20 6c6f  ....`Data too lo
-00000680: 6e67 60ef bc8c e5ad 98e5 82a8 e5ad 97e6  ng`.............
-00000690: aeb5 e4b8 8de5 ad98 e59c a8e7 ad89 e7ad  ................
-000006a0: 89ef bc89 e79a 84e5 ad98 e582 a8e9 97ae  ................
-000006b0: e9a2 98e3 8082 e590 8ee6 9da5 e4b8 8de6  ................
-000006c0: 96ad e4bc 98e5 8c96 e592 8ce6 b7bb e58a  ................
-000006d0: a0e5 9084 e7a7 8de5 9cba e699 afef bc8c  ................
-000006e0: e4bd bfe5 be97 e788 ace8 99ab e5bc 80e5  ................
-000006f0: 8f91 e59c a8e9 809a e794 a8e5 9cba e699  ................
-00000700: afe4 b88b e587 a0e4 b98e e58f aae7 94a8  ................
-00000710: e59c a8e6 848f 2060 7370 6964 6572 6020  ...... `spider` 
-00000720: e884 9ae6 9cac e79a 84e8 a7a3 e69e 90e8  ................
-00000730: a784 e588 99e5 928c 2060 5649 5460 20e4  ........ `VIT` .
-00000740: b88b e79a 8420 602e 636f 6e66 6020 e985  ..... `.conf` ..
-00000750: 8de7 bdae e58d b3e5 8faf efbc 8ce8 84b1  ................
-00000760: e7a6 bbe6 97a0 e684 8fe4 b989 e79a 84e9  ................
-00000770: 878d e5a4 8de6 938d e4bd 9ce3 8082 0d0a  ................
-00000780: 0d0a e887 b3e4 ba8e e6ad a4e5 ba93 e581  ................
-00000790: 9ae4 ba86 e593 aae4 ba9b e58a 9fe8 83bd  ................
-000007a0: efbc 8ce5 8faa e8a6 81e4 bda0 e786 9fe6  ................
-000007b0: 8289 2060 7079 7468 6f6e 6020 e8af ade6  .. `python` ....
-000007c0: b395 e592 8c20 6073 6372 6170 7960 20e5  ..... `scrapy` .
-000007d0: ba93 efbc 8ce5 868d e7bb 93e5 9088 205b  .............. [
-000007e0: 4465 6d6f 5370 6964 6572 5d28 6874 7470  DemoSpider](http
-000007f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000800: 6865 6e67 6368 656e 7961 6e67 2f44 656d  hengchenyang/Dem
-00000810: 6f53 7069 6465 7229 20e4 b8ad e79a 84e5  oSpider) .......
-00000820: ba94 e794 a8e7 a4ba e4be 8bef bc8c e4bd  ................
-00000830: a0e5 8faf e4bb a5e5 be88 e5bf abe4 b88a  ................
-00000840: e689 8be3 8082 e585 b7e4 bd93 e79a 84e5  ................
-00000850: 8685 e5ae b9e5 928c e6b3 a8e6 848f e4ba  ................
-00000860: 8be9 a1b9 e4b9 9fe5 8faf e4bb a5e5 9ca8  ................
-00000870: 205b 4179 7567 6553 7069 6465 7254 6f6f   [AyugeSpiderToo
-00000880: 6c73 2072 6561 6474 6865 646f 6373 20e6  ls readthedocs .
-00000890: 9687 e6a1 a35d 2868 7474 7073 3a2f 2f61  .....](https://a
-000008a0: 7975 6765 7370 6964 6572 746f 6f6c 732e  yugespidertools.
-000008b0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000008c0: 6e2f 6c61 7465 7374 2f29 20e4 b8ad e69f  n/latest/) .....
-000008d0: a5e7 9c8b e380 820d 0a0d 0a23 2320 312e  ...........## 1.
-000008e0: 20e5 898d e68f 90e6 9da1 e4bb b60d 0a0d   ...............
-000008f0: 0a3e 2060 7079 7468 6f6e 2033 2e38 2e31  .> `python 3.8.1
-00000900: 2b60 20e5 8faf e4bb a5e7 9bb4 e68e a5e8  +` .............
-00000910: be93 e585 a5e4 bba5 e4b8 8be5 91bd e4bb  ................
-00000920: a4ef bc9a 0d0a 0d0a 6060 6073 6865 6c6c  ........```shell
-00000930: 0d0a 7069 7020 696e 7374 616c 6c20 6179  ..pip install ay
-00000940: 7567 6573 7069 6465 7274 6f6f 6c73 202d  ugespidertools -
-00000950: 6920 6874 7470 733a 2f2f 7079 7069 2e6f  i https://pypi.o
-00000960: 7267 2f73 696d 706c 650d 0a60 6060 0d0a  rg/simple..```..
-00000970: 0d0a e6b3 a8ef bc9a e69c ace5 ba93 e4be  ................
-00000980: 9de8 b596 e4b8 ade7 9a84 2060 7079 6d6f  .......... `pymo
-00000990: 6e67 6f60 20e7 8988 e69c ace8 a681 e59c  ngo` ...........
-000009a0: a820 605e 332e 3132 2e33 6020 28e5 8db3  . `^3.12.3` (...
-000009b0: 6033 2e31 332e 3060 20e5 8f8a e4bb a5e4  `3.13.0` .......
-000009c0: b88b 2920 e698 afe5 9ba0 e4b8 bae6 8891  ..) ............
-000009d0: e79a 8420 606d 6f6e 676f 4442 6020 e79a  ... `mongoDB` ..
-000009e0: 84e7 8988 e69c ace4 b8ba 2060 332e 3460  .......... `3.4`
-000009f0: efbc 8c60 7079 6d6f 676f 6020 e5ae 98e6  ...`pymogo` ....
-00000a00: 96b9 e4bb 8e20 6033 2e31 332e 3060 20e4  ..... `3.13.0` .
-00000a10: bba5 e590 8ee7 9a84 e789 88e6 9cac e5bc  ................
-00000a20: 80e5 a78b e4b8 8de5 868d e694 afe6 8c81  ................
-00000a30: 2060 332e 3460 20e7 8988 e69c ace4 bba5   `3.4` .........
-00000a40: e4b8 8be7 9a84 2060 4d6f 6e67 6f44 4260  ...... `MongoDB`
-00000a50: 20e6 95b0 e68d aee5 ba93 e4ba 86ef bc8c   ...............
-00000a60: e69c 9be5 91a8 e79f a5ef bc81 2a2a e4bd  ............**..
-00000a70: a0e4 b99f e58f afe4 bba5 e6a0 b9e6 8dae  ................
-00000a80: 205b 332e 335d 2823 332e 332e 2d42 7569   [3.3](#3.3.-Bui
-00000a90: 6c64 2d59 6f75 722d 4f77 6e2d 4c69 6272  ld-Your-Own-Libr
-00000aa0: 6172 7929 20e8 87aa e5ae 9ae4 b989 e5ba  ary) ...........
-00000ab0: 932a 2a0d 0a0d 0a23 2320 322e 20e4 bdbf  .**....## 2. ...
-00000ac0: e794 a8e6 96b9 e6b3 950d 0a0d 0a3e 20e9  .............> .
-00000ad0: a1b9 e79b aee4 b8bb e8a6 81e5 8c85 e590  ................
-00000ae0: abe4 b8a4 e983 a8e5 8886 efbc 9a0d 0a3e  ...............>
-00000af0: 0d0a 0d0a 2d20 e5bc 80e5 8f91 e59c bae6  ....- ..........
-00000b00: 99af e4b8 ade7 9a84 e5b7 a5e5 85b7 e5ba  ................
-00000b10: 930d 0a20 202d 20e6 af94 e5a6 8220 604d  ...  - ...... `M
-00000b20: 6f6e 676f 4442 60ef bc8c 604d 7973 716c  ongoDB`...`Mysql
-00000b30: 2073 716c 6020 e8af ade5 8fa5 e79a 84e7   sql` ..........
-00000b40: 949f e688 90ef bc8c e59b bee5 838f e5a4  ................
-00000b50: 84e7 9086 efbc 8ce6 95b0 e68d aee5 a484  ................
-00000b60: e790 86e7 9bb8 e585 b320 2e2e 2e20 2e2e  ......... ... ..
-00000b70: 2e0d 0a2d 2060 5363 7261 7079 6020 e689  ...- `Scrapy` ..
-00000b80: a9e5 b195 e58a 9fe8 83bd efbc 882a 2ae4  .............**.
-00000b90: b8bb e68e a8e5 8a9f e883 bd20 e280 9420  ........... ... 
-00000ba0: e8a7 a3e6 94be e58f 8ce6 898b 2a2a efbc  ............**..
-00000bb0: 890d 0a20 202d 20e4 bdbf e788 ace8 99ab  ...  - .........
-00000bc0: e5bc 80e5 8f91 e697 a0e9 a1bb e59c a8e6  ................
-00000bd0: 848f e695 b0e6 8dae e5ba 93e5 928c e695  ................
-00000be0: b0e6 8dae e8a1 a8e7 bb93 e69e 84ef bc8c  ................
-00000bf0: e4b8 8de7 94a8 e58e bbe7 aea1 e5b8 b8e8  ................
-00000c00: a784 2060 6974 656d 2c20 7069 7065 6c69  .. `item, pipeli
-00000c10: 6e65 7360 20e5 928c 2060 6d69 6464 6c65  nes` ... `middle
-00000c20: 7761 7265 7360 20e7 9a84 e696 87e4 bbb6  wares` .........
-00000c30: e79a 84e7 bc96 e586 99e3 8082 e586 85e7  ................
-00000c40: bdae e980 9ae7 94a8 e79a 8420 606d 6964  ........... `mid
-00000c50: 646c 6577 6172 6573 6020 e4b8 ade9 97b4  dlewares` ......
-00000c60: e4bb b6e6 96b9 e6b3 95ef bc88 e99a 8fe6  ................
-00000c70: 9cba e8af b7e6 b182 e5a4 b4ef bc8c e58a  ................
-00000c80: a8e6 8081 2fe7 8bac e4ba abe4 bba3 e790  ..../...........
-00000c90: 86e7 ad89 efbc 89ef bc8c e592 8ce5 b8b8  ................
-00000ca0: e794 a8e7 9a84 2060 7069 7065 6c69 6e65  ...... `pipeline
-00000cb0: 7360 20e6 96b9 e6b3 95ef bc88 604d 7973  s` .........`Mys
-00000cc0: 716c 60ef bc8c 604d 6f6e 676f 4442 6020  ql`...`MongoDB` 
-00000cd0: e5ad 98e5 82a8 efbc 8c60 4b61 666b 6160  .........`Kafka`
-00000ce0: efbc 8c60 5261 6262 6974 4d51 6020 e68e  ...`RabbitMQ` ..
-00000cf0: a8e9 8081 e998 9fe5 8897 e7ad 89ef bc89  ................
-00000d00: e380 820d 0a0d 0a23 2323 2032 2e31 2e20  .......### 2.1. 
-00000d10: 5363 7261 7079 20e6 89a9 e5b1 95e5 ba93  Scrapy .........
-00000d20: e59c bae6 99af 0d0a 0d0a 3e20 e5bc 80e5  ..........> ....
-00000d30: 8f91 e4ba bae5 9198 e58f aae9 9c80 e6a0  ................
-00000d40: b9e6 8dae e591 bde4 bba4 e794 9fe6 8890  ................
-00000d50: e7a4 bae4 be8b e6a8 a1e6 9dbf efbc 8ce5  ................
-00000d60: 868d e985 8de7 bdae e5b9 b6e6 bf80 e6b4  ................
-00000d70: bbe7 9bb8 e585 b3e8 aebe e7bd aee5 8db3  ................
-00000d80: e58f afef bc8c e58f afe4 bba5 e4b8 93e6  ................
-00000d90: b3a8 e4ba 8ee7 88ac e899 ab20 6073 7069  ........... `spi
-00000da0: 6465 7260 20e7 9a84 e5bc 80e5 8f91 e380  der` ...........
-00000db0: 820d 0a0d 0ae4 bdbf e794 a8e6 96b9 e6b3  ................
-00000dc0: 95e7 a4ba e4be 8b20 6047 4946 6020 e5a6  ....... `GIF` ..
-00000dd0: 82e4 b88b efbc 9a0d 0a0d 0a21 5b61 7975  ...........![ayu
-00000de0: 6765 7370 6964 6572 746f 6f6c 732e 6769  gespidertools.gi
-00000df0: 665d 2868 7474 7073 3a2f 2f72 6177 2e67  f](https://raw.g
-00000e00: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000e10: 2e63 6f6d 2f73 6865 6e67 6368 656e 7961  .com/shengchenya
-00000e20: 6e67 2f41 7975 6765 5370 6964 6572 546f  ng/AyugeSpiderTo
-00000e30: 6f6c 732f 6d61 696e 2f65 7861 6d70 6c65  ols/main/example
-00000e40: 732f 6179 7567 6573 7069 6465 7274 6f6f  s/ayugespidertoo
-00000e50: 6c73 2d75 7365 2e67 6966 290d 0a0d 0ae5  ls-use.gif).....
-00000e60: afb9 e4bb a5e4 b88a 2060 4749 4660 20e4  ........ `GIF` .
-00000e70: b8ad e79a 84e6 ada5 e9aa a4e8 bf9b e8a1  ................
-00000e80: 8ce8 a7a3 e987 8aef bc9a 0d0a 0d0a 6060  ..............``
-00000e90: 6073 6865 6c6c 0d0a 2320 e69f a5e7 9c8b  `shell..# ......
-00000ea0: e5ba 93e7 8988 e69c ac0d 0a61 7975 6765  ...........ayuge
-00000eb0: 2076 6572 7369 6f6e 0d0a 0d0a 2320 e588   version....# ..
-00000ec0: 9be5 bbba e9a1 b9e7 9bae 0d0a 6179 7567  ............ayug
-00000ed0: 6520 7374 6172 7470 726f 6a65 6374 203c  e startproject <
-00000ee0: 7072 6f6a 6563 745f 6e61 6d65 3e0d 0a0d  project_name>...
-00000ef0: 0a23 20e8 bf9b e585 a5e9 a1b9 e79b aee6  .# .............
-00000f00: a0b9 e79b aee5 bd95 0d0a 6364 203c 7072  ..........cd <pr
-00000f10: 6f6a 6563 745f 6e61 6d65 3e0d 0a0d 0a23  oject_name>....#
-00000f20: 20e6 9bbf e68d a228 e8a6 86e7 9b96 29e4   ......(......).
-00000f30: b8ba e79c 9fe5 ae9e e79a 84e9 858d e7bd  ................
-00000f40: ae20 2e63 6f6e 6620 e696 87e4 bbb6 efbc  . .conf ........
-00000f50: 9a0d 0a23 20e8 bf99 e987 8ce6 98af e4b8  ...# ...........
-00000f60: bae4 ba86 e6bc 94e7 a4ba e696 b9e4 bebf  ................
-00000f70: efbc 8ce6 ada3 e5b8 b8e6 8385 e586 b5e6  ................
-00000f80: 98af e79b b4e6 8ea5 e59c a820 5649 5420  ........... VIT 
-00000f90: e8b7 afe5 be84 e4b8 8be7 9a84 202e 636f  ............ .co
-00000fa0: 6e66 20e9 858d e7bd aee6 9687 e4bb b6e5  nf .............
-00000fb0: a1ab e4b8 8ae4 bda0 e99c 80e8 a681 e79a  ................
-00000fc0: 84e9 858d e7bd aee5 8db3 e58f af0d 0a23  ...............#
-00000fd0: 20e4 b88d e99c 80e8 a681 e79a 84e9 858d   ...............
-00000fe0: e7bd aee8 aebe e7bd aee4 b8ba e7a9 baef  ................
-00000ff0: bc8c e688 96e8 8085 e4b8 8de7 94a8 e790  ................
-00001000: 86e4 bc9a e5ae 83ef bc8c e688 96e8 8085  ................
-00001010: e588 a0e9 99a4 e5ae 83e4 b99f e58f afe4  ................
-00001020: bba5 efbc 8ce7 9c8b e4b8 aae4 baba e980  ................
-00001030: 89e6 8ba9 0d0a 6370 202f 726f 6f74 2f6d  ......cp /root/m
-00001040: 7974 656d 702f 2e63 6f6e 6620 4465 6d6f  ytemp/.conf Demo
-00001050: 5370 6964 6572 2f56 4954 2f2e 636f 6e66  Spider/VIT/.conf
-00001060: 0d0a 0d0a 2320 e794 9fe6 8890 e788 ace8  ....# ..........
-00001070: 99ab e884 9ae6 9cac 0d0a 6179 7567 6520  ..........ayuge 
-00001080: 6765 6e73 7069 6465 7220 3c73 7069 6465  genspider <spide
-00001090: 725f 6e61 6d65 3e20 3c65 7861 6d70 6c65  r_name> <example
-000010a0: 2e63 6f6d 3e0d 0a0d 0a23 20e8 bf90 e8a1  .com>....# .....
-000010b0: 8ce8 849a e69c ac0d 0a73 6372 6170 7920  .........scrapy 
-000010c0: 6372 6177 6c20 3c73 7069 6465 725f 6e61  crawl <spider_na
-000010d0: 6d65 3e0d 0a23 20e6 b3a8 efbc 9ae4 b99f  me>..# .........
-000010e0: e58f afe4 bba5 e4bd bfe7 94a8 2061 7975  ............ ayu
-000010f0: 6765 2063 7261 776c 203c 7370 6964 6572  ge crawl <spider
-00001100: 5f6e 616d 653e 0d0a 6060 600d 0a0d 0ae5  _name>..```.....
-00001110: 85b7 e4bd 93e4 bdbf e794 a8e6 96b9 e6b3  ................
-00001120: 95e8 afb7 e59c a820 5b44 656d 6f53 7069  ....... [DemoSpi
-00001130: 6465 7220 e4b9 8b20 4179 7567 6553 7069  der ... AyugeSpi
-00001140: 6465 7254 6f6f 6c73 20e5 b7a5 e585 b7e5  derTools .......
-00001150: ba94 e794 a8e7 a4ba e4be 8b5d 2868 7474  ...........](htt
-00001160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001170: 7368 656e 6763 6865 6e79 616e 672f 4465  shengchenyang/De
-00001180: 6d6f 5370 6964 6572 2920 e9a1 b9e7 9bae  moSpider) ......
-00001190: e4b8 ade6 9fa5 e79c 8bef bc8c e79b aee5  ................
-000011a0: 898d e5b7 b2e9 8082 e985 8de4 bba5 e4b8  ................
-000011b0: 8be5 9cba e699 afef bc9a 0d0a 0d0a 6060  ..............``
-000011c0: 6064 6966 660d 0a23 20e9 8787 e99b 86e6  `diff..# .......
-000011d0: 95b0 e68d aee5 ad98 e585 a520 604d 7973  ........... `Mys
-000011e0: 716c 6020 e79a 84e5 9cba e699 afef bc9a  ql` ............
-000011f0: 0d0a 2b20 3129 2e64 656d 6f5f 6f6e 653a  ..+ 1).demo_one:
-00001200: 20e9 858d e7bd aee6 a0b9 e68d aee6 9cac   ...............
-00001210: e59c b020 6073 6574 7469 6e67 7360 20e7  ... `settings` .
-00001220: 9a84 2060 4c4f 4341 4c5f 4d59 5351 4c5f  .. `LOCAL_MYSQL_
-00001230: 434f 4e46 4947 6020 e4b8 ade5 8f96 e580  CONFIG` ........
-00001240: bc0d 0a2b 2033 292e 6465 6d6f 5f74 6872  ...+ 3).demo_thr
-00001250: 6565 3a20 e985 8de7 bdae e6a0 b9e6 8dae  ee: ............
-00001260: 2060 636f 6e73 756c 6020 e79a 84e5 ba94   `consul` ......
-00001270: e794 a8e7 aea1 e790 86e4 b8ad e5bf 83e4  ................
-00001280: b8ad e58f 96e5 80bc 0d0a 2b20 3529 2e64  ..........+ 5).d
-00001290: 656d 6f5f 6669 7665 3a20 e5bc 82e6 ada5  emo_five: ......
-000012a0: e5ad 98e5 85a5 2060 4d79 7371 6c60 20e7  ...... `Mysql` .
-000012b0: 9a84 e59c bae6 99af 0d0a 0d0a 2320 e987  ............# ..
-000012c0: 87e9 9b86 e695 b0e6 8dae e5ad 98e5 85a5  ................
-000012d0: 2060 4d6f 6e67 6f44 4260 20e7 9a84 e59c   `MongoDB` .....
-000012e0: bae6 99af efbc 9a0d 0a2b 2032 292e 6465  .........+ 2).de
-000012f0: 6d6f 5f74 776f 3a20 e987 87e9 9b86 e695  mo_two: ........
-00001300: b0e6 8dae e5ad 98e5 85a5 2060 4d6f 6e67  .......... `Mong
-00001310: 6f44 4260 20e7 9a84 e59c bae6 99af efbc  oDB` ...........
-00001320: 88e9 858d e7bd aee6 a0b9 e68d aee6 9cac  ................
-00001330: e59c b020 6073 6574 7469 6e67 7360 20e7  ... `settings` .
-00001340: 9a84 2060 4c4f 4341 4c5f 4d4f 4e47 4f44  .. `LOCAL_MONGOD
-00001350: 425f 434f 4e46 4947 6020 e4b8 ade5 8f96  B_CONFIG` ......
-00001360: e580 bcef bc89 0d0a 2b20 3429 2e64 656d  ........+ 4).dem
-00001370: 6f5f 666f 7572 3a20 e987 87e9 9b86 e695  o_four: ........
-00001380: b0e6 8dae e5ad 98e5 85a5 2060 4d6f 6e67  .......... `Mong
-00001390: 6f44 4260 20e7 9a84 e59c bae6 99af efbc  oDB` ...........
-000013a0: 88e9 858d e7bd aee6 a0b9 e68d ae20 6063  ............. `c
-000013b0: 6f6e 7375 6c60 20e7 9a84 e5ba 94e7 94a8  onsul` .........
-000013c0: e7ae a1e7 9086 e4b8 ade5 bf83 e4b8 ade5  ................
-000013d0: 8f96 e580 bcef bc89 0d0a 2b20 3629 2e64  ..........+ 6).d
-000013e0: 656d 6f5f 7369 783a 20e5 bc82 e6ad a5e5  emo_six: .......
-000013f0: ad98 e585 a520 604d 6f6e 676f 4442 6020  ..... `MongoDB` 
-00001400: e79a 84e5 9cba e699 af0d 0a0d 0a23 20e5  .............# .
-00001410: b086 2060 5363 7261 7079 6020 e79a 8420  .. `Scrapy` ... 
-00001420: 6052 6571 7565 7374 60ef bc8c 6046 6f72  `Request`...`For
-00001430: 6d52 6571 7565 7374 6020 e69b bfe6 8da2  mRequest` ......
-00001440: e4b8 bae5 85b6 e5ae 83e5 b7a5 e585 b7e5  ................
-00001450: ae9e e78e b0e7 9a84 e59c bae6 99af 0d0a  ................
-00001460: 2d20 e4bb a5e4 b88a e4b8 bae4 bdbf e794  - ..............
-00001470: a820 7363 7261 7079 2052 6571 7565 7374  . scrapy Request
-00001480: 20e7 9a84 e59c bae6 99af 0d0a 2d20 3729   ...........- 7)
-00001490: 2e64 656d 6f5f 7365 7665 6e3a 2073 6372  .demo_seven: scr
-000014a0: 6170 7920 5265 7175 6573 7420 e69b bfe6  apy Request ....
-000014b0: 8da2 e4b8 ba20 7265 7175 6573 7473 20e8  ..... requests .
-000014c0: afb7 e6b1 82e7 9a84 e59c bae6 99af 28e5  ..............(.
-000014d0: b7b2 e588 a0e9 99a4 e6ad a4e5 8a9f e883  ................
-000014e0: bdef bc8c e69b b4e6 8ea8 e88d 90e4 bdbf  ................
-000014f0: e794 a820 6169 6f68 7474 7020 e696 b9e5  ... aiohttp ....
-00001500: bc8f 290d 0a0d 0a2b 2038 292e 6465 6d6f  ..)....+ 8).demo
-00001510: 5f65 6967 6874 3a20 e590 8ce6 97b6 e5ad  _eight: ........
-00001520: 98e5 85a5 204d 7973 716c 20e5 928c 204d  .... Mysql ... M
-00001530: 6f6e 676f 4442 20e7 9a84 e59c bae6 99af  ongoDB .........
-00001540: 0d0a 0d0a 2b20 3929 2e64 656d 6f5f 6169  ....+ 9).demo_ai
-00001550: 6f68 7474 705f 6578 616d 706c 653a 2073  ohttp_example: s
-00001560: 6372 6170 7920 5265 7175 6573 7420 e69b  crapy Request ..
-00001570: bfe6 8da2 e4b8 ba20 6169 6f68 7474 7020  ....... aiohttp 
-00001580: e8af b7e6 b182 e79a 84e5 9cba e699 afef  ................
-00001590: bc8c e68f 90e4 be9b e4ba 86e5 9084 e7a7  ................
-000015a0: 8de8 afb7 e6b1 82e5 9cba e699 afe7 a4ba  ................
-000015b0: e4be 8bef bc88 4745 542c 504f 5354 efbc  ......GET,POST..
-000015c0: 890d 0a2b 2031 3029 2e64 656d 6f5f 6169  ...+ 10).demo_ai
-000015d0: 6f68 7474 705f 7465 7374 3a20 7363 7261  ohttp_test: scra
-000015e0: 7079 2061 696f 6874 7470 20e5 9ca8 e585  py aiohttp .....
-000015f0: b7e4 bd93 e9a1 b9e7 9bae e4b8 ade7 9a84  ................
-00001600: e4bd bfe7 94a8 e696 b9e6 b395 e7a4 bae4  ................
-00001610: be8b 0d0a 0d0a 2b20 3131 292e 6465 6d6f  ......+ 11).demo
-00001620: 5f70 726f 7879 5f6f 6e65 3a20 e5bf abe4  _proxy_one: ....
-00001630: bba3 e790 86e5 8aa8 e680 81e9 9aa7 e981  ................
-00001640: 93e4 bba3 e790 86e7 a4ba e4be 8b0d 0a2b  ...............+
-00001650: 2031 3229 2e64 656d 6f5f 7072 6f78 795f   12).demo_proxy_
-00001660: 7477 6f3a 20e6 b58b e8af 95e5 bfab e4bb  two: ...........
-00001670: a3e7 9086 e78b ace4 baab e4bb a3e7 9086  ................
-00001680: 0d0a 0d0a 2b31 3329 2e64 656d 6f5f 4179  ....+13).demo_Ay
-00001690: 7554 7572 626f 4d79 7371 6c50 6970 656c  uTurboMysqlPipel
-000016a0: 696e 653a 206d 7973 716c 20e5 908c e6ad  ine: mysql .....
-000016b0: a5e8 bf9e e68e a5e6 b1a0 e79a 84e7 a4ba  ................
-000016c0: e4be 8b0d 0a2b 3134 292e 6465 6d6f 5f63  .....+14).demo_c
-000016d0: 7261 776c 3a20 e694 afe6 8c81 2073 6372  rawl: ...... scr
-000016e0: 6170 7920 4372 6177 6c53 7069 6465 7220  apy CrawlSpider 
-000016f0: e79a 84e7 a4ba e4be 8b0d 0a0d 0a23 20e6  .............# .
-00001700: 9cac e5ba 93e4 b8ad e7bb 99e5 87ba e694  ................
-00001710: afe6 8c81 2049 7465 6d20 4c6f 6164 6572  .... Item Loader
-00001720: 7320 e789 b9e6 80a7 e79a 84e7 a4ba e4be  s ..............
-00001730: 8b28 e696 87e6 a1a3 e59c b0e5 9d80 efbc  .(..............
-00001740: 9a68 7474 7073 3a2f 2f61 7975 6765 7370  .https://ayugesp
-00001750: 6964 6572 746f 6f6c 732e 7265 6164 7468  idertools.readth
-00001760: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001770: 7374 2f74 6f70 6963 732f 6c6f 6164 6572  st/topics/loader
-00001780: 732e 6874 6d6c 290d 0a2b 3135 292e 6465  s.html)..+15).de
-00001790: 6d6f 5f69 7465 6d5f 6c6f 6164 6572 3a20  mo_item_loader: 
-000017a0: e69c ace5 ba93 e4b8 ade4 bdbf e794 a820  ............... 
-000017b0: 4974 656d 204c 6f61 6465 7273 20e7 9a84  Item Loaders ...
-000017c0: e7a4 bae4 be8b 0d0a 2d31 3629 2e64 656d  ........-16).dem
-000017d0: 6f5f 6974 656d 5f6c 6f61 6465 725f 7477  o_item_loader_tw
-000017e0: 6f3a 20e5 b195 e7a4 bae6 9cac e5ba 93e4  o: .............
-000017f0: bdbf e794 a820 6974 656d 4c6f 6164 6572  ..... itemLoader
-00001800: 20e7 89b9 e680 a7e7 9a84 e7a4 bae4 be8b   ...............
-00001810: efbc 8ce6 ada4 e7a4 bae4 be8b e5b7 b2e5  ................
-00001820: 88a0 e999 a4ef bc8c e58f afe6 9fa5 e79c  ................
-00001830: 8be4 b88a e4b8 aa20 6465 6d6f 5f69 7465  ....... demo_ite
-00001840: 6d5f 6c6f 6164 6572 20e4 b8ad e79a 84e7  m_loader .......
-00001850: a4ba e4be 8bef bc8c e79b aee5 898d e5b7  ................
-00001860: b2e7 bb8f e58f afe4 bba5 e5be 88e6 96b9  ................
-00001870: e4be bfe7 9a84 e4bd bfe7 94a8 2049 7465  ............ Ite
-00001880: 6d20 4c6f 6164 6572 7320 e58a 9fe8 83bd  m Loaders ......
-00001890: e4ba 860d 0a0d 0a2b 3137 292e 6465 6d6f  .......+17).demo
-000018a0: 5f6d 6f6e 676f 5f61 7379 6e63 3a20 6173  _mongo_async: as
-000018b0: 796e 6369 6f20 e789 88e6 9cac e5ad 98e5  yncio ..........
-000018c0: 82a8 206d 6f6e 676f 4442 20e7 9a84 2070  .. mongoDB ... p
-000018d0: 6970 656c 696e 6573 20e7 a4ba e4be 8b0d  ipelines .......
-000018e0: 0a2b 3138 292e 6465 6d6f 5f6d 713a 20e6  .+18).demo_mq: .
-000018f0: 95b0 e68d aee5 ad98 e585 a520 7261 6262  ........... rabb
-00001900: 6974 6d71 20e7 9a84 e6a8 a1e6 9dbf e7a4  itmq ...........
-00001910: bae4 be8b 0d0a 2b31 3929 2e64 656d 6f5f  ......+19).demo_
-00001920: 6b61 666b 613a 20e6 95b0 e68d aee5 ad98  kafka: .........
-00001930: e585 a520 6b61 666b 6120 e79a 84e6 a8a1  ... kafka ......
-00001940: e69d bfe7 a4ba e4be 8b0d 0a2b 3230 292e  ...........+20).
-00001950: 6465 6d6f 5f66 696c 653a 20e4 b88b e8bd  demo_file: .....
-00001960: bde5 9bbe e789 87e7 ad89 e696 87e4 bbb6  ................
-00001970: e588 b0e6 9cac e59c b0e7 9a84 e6a8 a1e6  ................
-00001980: 9dbf e7a4 bae4 be8b 0d0a 6060 600d 0a0d  ..........```...
-00001990: 0ae6 b3a8 efbc 9ae5 85b7 e4bd 93e5 8685  ................
-000019a0: e5ae b9e5 8f8a e697 b6e6 9588 e680 a7e8  ................
-000019b0: afb7 e4bb a520 5b44 656d 6f53 7069 6465  ..... [DemoSpide
-000019c0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-000019d0: 622e 636f 6d2f 7368 656e 6763 6865 6e79  b.com/shengcheny
-000019e0: 616e 672f 4465 6d6f 5370 6964 6572 2920  ang/DemoSpider) 
-000019f0: e9a1 b9e7 9bae e4b8 ade6 8f8f e8bf b0e4  ................
-00001a00: b8ba e587 86e3 8082 0d0a 0d0a 2323 2320  ............### 
-00001a10: 322e 322e 20e5 bc80 e58f 91e5 9cba e699  2.2. ...........
-00001a20: af0d 0a0d 0a3e 20e8 bf99 e987 8ce4 b88d  .....> .........
-00001a30: e586 8de4 b880 e4b8 80e5 8897 e4b8 bee6  ................
-00001a40: 8980 e69c 89e5 8a9f e883 bdef bc8c e5a4  ................
-00001a50: a7e6 a682 e4bb 8be7 bb8d e4b8 8be5 8c85  ................
-00001a60: e590 abe7 9a84 e5a4 a7e8 87b4 e58a 9fe8  ................
-00001a70: 83bd e380 820d 0a0d 0a2d 202a 2ae6 95b0  .........- **...
-00001a80: e68d aee5 a484 e790 86e7 9bb8 e585 b33a  ...............:
-00001a90: 2a2a 20e6 af94 e5a6 82e4 b880 e4ba 9be5  ** .............
-00001aa0: ad97 e7ac a6e4 b8b2 e5a4 84e7 9086 efbc  ................
-00001ab0: 8c60 7572 6c60 20e6 8bbc e68e a5e5 a484  .`url` .........
-00001ac0: e790 86e3 8082 0d0a 2d20 2a2a e5b8 b8e7  ........- **....
-00001ad0: 94a8 e58a a0e8 a7a3 e5af 86e3 8081 e7bc  ................
-00001ae0: 96e7 a081 3a2a 2a20 6072 7361 602c 2060  ....:** `rsa`, `
-00001af0: 6d6d 3360 20e7 ad89 efbc 8ce5 85b6 e5ae  mm3` ...........
-00001b00: 9ee6 9bb4 e68e a8e8 8d90 205b 6368 6570  .......... [chep
-00001b10: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00001b20: 622e 636f 6d2f 7365 6375 7269 7365 632f  b.com/securisec/
-00001b30: 6368 6570 7929 20e5 ba93 202d 20e4 bda0  chepy) ... - ...
-00001b40: e883 bde7 94a8 205b 6963 7962 6572 6368  ...... [icyberch
-00001b50: 6566 5d28 6874 7470 733a 2f2f 6963 7962  ef](https://icyb
-00001b60: 6572 6368 6566 2e63 6f6d 2f29 20e6 b58b  erchef.com/) ...
-00001b70: e8af 95e8 b791 e980 9ae7 9a84 e58a a0e8  ................
-00001b80: a7a3 e5af 86e9 83bd e58f afe4 bba5 e794  ................
-00001b90: a8e6 ada4 e5ba 93e6 9bb4 e696 b9e4 bebf  ................
-00001ba0: e59c b0e5 ae9e e78e b0ef bc8c e4b8 a4e4  ................
-00001bb0: b889 e8a1 8ce4 bba3 e7a0 81e5 8db3 e58f  ................
-00001bc0: afe6 909e e5ae 9ae3 8082 0d0a 2d20 2a2a  ............- **
-00001bd0: 7371 6c20 e8af ade5 8fa5 e68b bce6 8ea5  sql ............
-00001be0: 3a2a 2a20 e58f aae8 83bd e581 9ae5 88b0  :** ............
-00001bf0: e69c 80e7 ae80 e58d 95e7 9a84 e980 bbe8  ................
-00001c00: be91 efbc 8ce5 a682 e69e 9ce9 9c80 e8a6  ................
-00001c10: 81e7 81b5 e6b4 bbe6 8896 e7a8 8de5 a48d  ................
-00001c20: e69d 82e7 9a84 e683 85e5 86b5 efbc 8ce8  ................
-00001c30: afb7 e58f 82e8 8083 2060 6469 7265 6374  ........ `direct
-00001c40: 7371 6c60 2c20 6070 7974 686f 6e2d 7371  sql`, `python-sq
-00001c50: 6c60 2c20 6070 7970 696b 6160 e688 9620  l`, `pypika`... 
-00001c60: 6070 796d 696c 6b60 20e7 ad89 e585 b6e5  `pymilk` .......
-00001c70: ae83 e7ac ace4 b889 e696 b9e7 b1bb e4bc  ................
-00001c80: bce5 8a9f e883 bde5 ba93 e79a 84e5 ae9e  ................
-00001c90: e78e b0e6 96b9 e6b3 95e3 8082 0d0a 2d20  ..............- 
-00001ca0: 2a2a e6bb 91e5 9d97 e59b bee7 8987 e7bc  **..............
-00001cb0: bae5 8fa3 e4bd 8de7 bdae e8af 86e5 88ab  ................
-00001cc0: e58f 8ae8 bda8 e8bf b9e7 949f e688 902a  ...............*
-00001cd0: 2a0d 0a0d 0ae6 b3a8 efbc 9a0d 0a0d 0a3e  *..............>
-00001ce0: 20e6 bb91 e59d 97e7 bcba e58f a3e8 af86   ...............
-00001cf0: e588 abe7 a4ba e4be 8bef bc8c e58f 8ce7  ................
-00001d00: bcba e58f a3e4 b99f e58f afe6 ada3 e5b8  ................
-00001d10: b8e8 af86 e588 abe3 8082 0d0a 0d0a 7c20  ..............| 
-00001d20: e8af 86e5 88ab e7bb 93e6 9e9c e5b1 95e7  ................
-00001d30: a4ba 2020 2020 2020 2020 2020 2020 2020  ..              
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001de0: 2020 7c20 e5a4 87e6 b3a8 2020 2020 2020    | ......      
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-00001e20: 7c20 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | :-------------
-00001e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
-00001ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f10: 2d2d 2d2d 2d2d 207c 0d0a 7c20 3c69 6d67  ------ |..| <img
-00001f20: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00001f30: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00001f40: 656e 742e 636f 6d2f 7368 656e 6763 6865  ent.com/shengche
-00001f50: 6e79 616e 672f 4179 7567 6553 7069 6465  nyang/AyugeSpide
-00001f60: 7254 6f6f 6c73 2f6d 6169 6e2f 6578 616d  rTools/main/exam
-00001f70: 706c 6573 2f73 6c69 6465 725f 6e6f 7463  ples/slider_notc
-00001f80: 685f 6469 7374 616e 6365 5f72 6563 6f67  h_distance_recog
-00001f90: 6e69 7465 312e 706e 6722 2061 6c74 3d22  nite1.png" alt="
-00001fa0: 736c 6964 6572 5f6e 6f74 6368 5f64 6973  slider_notch_dis
-00001fb0: 7461 6e63 655f 7265 636f 676e 6974 6531  tance_recognite1
-00001fc0: 2220 7374 796c 653d 227a 6f6f 6d3a 2032  " style="zoom: 2
-00001fd0: 3525 3b22 202f 3e20 7c20 e697 a020 2020  5%;" /> | ...   
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 7c0d 0a7c 203c 696d 6720 7372 633d    |..| <img src=
-00002020: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00002030: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00002040: 6f6d 2f73 6865 6e67 6368 656e 7961 6e67  om/shengchenyang
-00002050: 2f41 7975 6765 5370 6964 6572 546f 6f6c  /AyugeSpiderTool
-00002060: 732f 6d61 696e 2f65 7861 6d70 6c65 732f  s/main/examples/
-00002070: 736c 6964 6572 5f6e 6f74 6368 5f64 6973  slider_notch_dis
-00002080: 7461 6e63 655f 7265 636f 676e 6974 6532  tance_recognite2
-00002090: 2e70 6e67 2220 616c 743d 2273 6c69 6465  .png" alt="slide
-000020a0: 725f 6e6f 7463 685f 6469 7374 616e 6365  r_notch_distance
-000020b0: 5f72 6563 6f67 6e69 7465 3222 2073 7479  _recognite2" sty
-000020c0: 6c65 3d22 7a6f 6f6d 3a20 3235 253b 2220  le="zoom: 25%;" 
-000020d0: 2f3e 207c 20e5 8faf e4bb a5e5 b195 e7a4  /> | ...........
-000020e0: bae5 8faa e8af 86e5 88ab e6bb 91e5 9d97  ................
-000020f0: e5b0 8fe6 96b9 e59d 97e7 9a84 e7bb 93e6  ................
-00002100: 9e9c efbc 8ce5 be97 e588 b0e6 9bb4 e7b2  ................
-00002110: bee5 8786 e79a 84e5 9d90 e6a0 87e6 95b0  ................
-00002120: e68d aee3 8082 207c 0d0a 0d0a 2323 2033  ...... |....## 3
-00002130: 2e20 e8a1 a5e5 8585 0d0a 0d0a 2a2a e59c  . ..........**..
-00002140: a8e4 bdbf e794 a8e8 bf87 e7a8 8be4 b8ad  ................
-00002150: e88b a5e9 8187 e588 b0e5 9084 e7a7 8de9  ................
-00002160: 97ae e9a2 98ef bc8c e688 96e6 9c89 e4bb  ................
-00002170: bbe4 bd95 e4bc 98e5 8c96 e5bb bae8 aeae  ................
-00002180: e6ac a2e8 bf8e e68f 9020 4973 7375 6573  ......... Issues
-00002190: 2021 2a2a 0d0a 0d0a 2323 2320 332e 312e   !**....### 3.1.
-000021a0: 20e8 b791 e980 9ae6 b58b e8af 95e7 a4ba   ...............
-000021b0: e4be 8b0d 0a0d 0ae5 898d e68f 90ef bc9a  ................
-000021c0: e99c 80e8 a681 e59c a820 6074 6573 7473  ......... `tests
-000021d0: 6020 e79a 8420 6056 4954 6020 e79b aee5  ` ... `VIT` ....
-000021e0: bd95 e4b8 8be5 889b e5bb ba20 602e 636f  ........... `.co
-000021f0: 6e66 6020 e696 87e4 bbb6 efbc 8ce5 b7b2  nf` ............
-00002200: e7bb 99e5 87ba e7a4 bae4 be8b e696 87e4  ................
-00002210: bbb6 efbc 8ce8 afb7 e5a1 abe5 8699 e6b5  ................
-00002220: 8be8 af95 e689 80e9 9c80 e586 85e5 aeb9  ................
-00002230: efbc 8ce7 84b6 e590 8eef bc9a 0d0a 0d0a  ................
-00002240: 2d20 e58f afe4 bba5 e79b b4e6 8ea5 e4bd  - ..............
-00002250: bfe7 94a8 2060 746f 7860 20e6 9da5 e8bf  .... `tox` .....
-00002260: 90e8 a18c e6b5 8be8 af95 e380 820d 0a0d  ................
-00002270: 0a2d 20e6 9cac e5ba 93e4 bba5 205b 706f  .- ......... [po
-00002280: 6574 7279 5d28 6874 7470 733a 2f2f 7079  etry](https://py
-00002290: 7468 6f6e 2d70 6f65 7472 792e 6f72 672f  thon-poetry.org/
-000022a0: 646f 6373 2f29 20e5 bc80 e58f 91ef bc8c  docs/) .........
-000022b0: e982 a3e4 b988 e79b b4e6 8ea5 e696 b0e7  ................
-000022c0: 8eaf e5a2 83e4 b88b e8bf 90e8 a18c 2060  .............. `
-000022d0: 706f 6574 7279 2069 6e73 7461 6c6c 6020  poetry install` 
-000022e0: e590 8eef bc8c e689 8be5 8aa8 e8bf 90e8  ................
-000022f0: a18c e79b aee6 a087 e6b5 8be8 af95 e688  ................
-00002300: 9620 6070 7974 6573 7460 20e5 91bd e4bb  . `pytest` .....
-00002310: a4e6 9da5 e6b5 8be8 af95 e7ad 89e7 9a86  ................
-00002320: e58f afe3 8082 0d0a 2d20 e4b9 9fe5 8faf  ........- ......
-00002330: e4bb a5e4 bdbf e794 a820 606d 616b 6560  ......... `make`
-00002340: 20e5 b7a5 e585 b7ef bc8c 606d 616b 6520   .........`make 
-00002350: 7374 6172 7460 20e7 84b6 e590 8e20 606d  start` ...... `m
-00002360: 616b 6520 7465 7374 6020 e58d b3e5 8faf  ake test` ......
-00002370: e380 820d 0a0d 0ae6 b58b e8af 95e5 ae8c  ................
-00002380: e6af 95e5 908e 2060 6d61 6b65 2063 6c65  ...... `make cle
-00002390: 616e 6020 e6b8 85e7 9086 e696 87e4 bbb6  an` ............
-000023a0: e380 820d 0a0d 0a23 2323 2033 2e32 2e20  .......### 3.2. 
-000023b0: e4bd a0e5 8faf e883 bde5 9ca8 e684 8fe7  ................
-000023c0: 9a84 e4ba 8b0d 0a0d 0a3e 20e6 ada4 e9a1  .........> .....
-000023d0: b9e7 9bae e4bc 9ae6 85a2 e685 a2e4 b8b0  ................
-000023e0: e5af 8c20 6070 7974 686f 6e60 20e5 bc80  ... `python` ...
-000023f0: e58f 91e4 b8ad e79a 84e9 8187 e588 b0e7  ................
-00002400: 9a84 e980 9ae7 94a8 e696 b9e6 b395 efbc  ................
-00002410: 8ce8 afa6 e683 85e8 afb7 e8a7 8120 5b54  ............. [T
-00002420: 6f64 6f4c 6973 745d 2823 546f 646f 4c69  odoList](#TodoLi
-00002430: 7374 29e3 8082 0d0a 0d0a 312e 20e8 8ba5  st).......1. ...
-00002440: e4bd a0e8 a789 e5be 97e6 9f90 e4ba 9be5  ................
-00002450: 9cba e699 afe4 b88b e79a 84e5 8a9f e883  ................
-00002460: bde5 ae9e e78e b0e4 b88d e5a4 aae7 aca6  ................
-00002470: e590 88e4 bda0 e79a 84e9 a284 e69c 9fef  ................
-00002480: bc8c e683 b3e8 a681 e4bf aee6 94b9 e688  ................
-00002490: 96e6 b7bb e58a a0e8 87aa e5ae 9ae4 b989  ................
-000024a0: e58a 9fe8 83bd efbc 8ce6 8896 e7a7 bbe9  ................
-000024b0: 99a4 e5af b9e4 bda0 e697 a0e7 94a8 e6a8  ................
-000024c0: a1e5 9d97 e380 81e4 bfae e694 b9e5 ba93  ................
-000024d0: e590 8de7 ad89 efbc 8ce4 bda0 e58f afe4  ................
-000024e0: bba5 e887 aae8 a18c e4bf aee6 94b9 e590  ................
-000024f0: 8e20 6062 7569 6c64 60e3 8082 0d0a 322e  . `build`.....2.
-00002500: 20e6 9cac e5ba 93e4 b8bb e68e a820 6073   ............ `s
-00002510: 6372 6170 7960 20e6 89a9 e5b1 95ef bc88  crapy` .........
-00002520: e58d b3e5 a29e e5bc bae7 8988 e79a 84e8  ................
-00002530: 87aa e5ae 9ae4 b989 e6a8 a1e6 9dbf efbc  ................
-00002540: 89e7 9a84 e58a 9fe8 83bd efbc 8ce5 9ca8  ................
-00002550: e4bd bfe7 94a8 e69c ace5 ba93 e697 b6ef  ................
-00002560: bc8c e790 86e8 aeba e4b8 8ae5 b9b6 e4b8  ................
-00002570: 8de4 bc9a e5bd b1e5 938d e4bd a020 6073  ............. `s
-00002580: 6372 6170 7960 20e9 a1b9 e79b aee5 8f8a  crapy` .........
-00002590: e585 b6e5 ae83 e7bb 84e4 bbb6 efbc 8ce4  ................
-000025a0: b894 e4bd a0e4 b99f e58f afe4 bba5 e6a0  ................
-000025b0: b9e6 8dae e4b8 8ae6 9da1 e9a1 bbe7 9fa5  ................
-000025c0: e69d a5e5 a29e e5bc bae6 ada4 e5ba 93e5  ................
-000025d0: 8a9f e883 bde3 8082 e59b a0e4 b8ba e6a8  ................
-000025e0: a1e6 9dbf e58a 9fe8 83bd e5a4 a9e7 949f  ................
-000025f0: e5b0 b1e6 9c89 e58f 8ae5 85b6 e698 8ee7  ................
-00002600: a1ae e79a 84e4 bc98 e7bc bae7 82b9 efbc  ................
-00002610: 8ce6 8891 e697 a0e6 b395 e8a6 86e7 9b96  ................
-00002620: e689 80e6 9c89 e5ba 94e7 94a8 e59c bae6  ................
-00002630: 99af efbc 8c2a 2ae4 bd86 e698 afe5 ae83  .....**.........
-00002640: e79a 84e9 ab98 e695 88e7 8e87 e79a 84e7  ................
-00002650: a1ae e4bc 9ae8 a7a3 e694 bee5 8f8c e689  ................
-00002660: 8b2a 2ae3 8082 0d0a 332e 202a 2ae5 bd93  .**.....3. **...
-00002670: e784 b6ef bc8c e4bd a0e4 b99f e58f afe4  ................
-00002680: bba5 e980 89e6 8ba9 e7bb 99e6 ada4 e9a1  ................
-00002690: b9e7 9bae e581 9ae5 87ba e8b4 a1e7 8cae  ................
-000026a0: efbc 8ce6 af94 e5a6 82e5 a29e e58a a0e6  ................
-000026b0: 8896 e4bc 98e5 8c96 e69f 90e4 ba9b e58a  ................
-000026c0: 9fe8 83bd e7ad 89ef bc8c e4bd 86e5 9ca8  ................
-000026d0: e6ad a4e4 b98b e589 8de8 afb7 e68f 90e7  ................
-000026e0: 9bb8 e585 b3e7 9a84 2060 4953 5355 4553  ........ `ISSUES
-000026f0: 6020 e7bb 8fe7 a1ae e8ae a4e5 908e e586  ` ..............
-00002700: 8de5 bc80 e58f 91e5 928c e68f 90e4 baa4  ................
-00002710: 2060 5055 4c4c 2052 4551 5545 5354 5360   `PULL REQUESTS`
-00002720: efbc 8ce4 bba5 e585 8de4 b88d e5a4 aae7  ................
-00002730: aca6 e590 88e6 9cac e5ba 93e5 9cba e699  ................
-00002740: afe6 8896 e5b7 b2e5 ba9f e5bc 83e7 ad89  ................
-00002750: e58e 9fe5 9ba0 e980 a0e6 8890 e4bd a0e7  ................
-00002760: 9a84 e8b4 a1e7 8cae e6b5 aae8 b4b9 efbc  ................
-00002770: 8ce9 82a3 e5b0 b1e5 a4aa e58f afe6 839c  ................
-00002780: e4ba 86ef bc81 2a2a 0d0a 0d0a 2323 2320  ......**....### 
-00002790: 332e 332e 2042 7569 6c64 2d59 6f75 722d  3.3. Build-Your-
-000027a0: 4f77 6e2d 4c69 6272 6172 790d 0a0d 0a3e  Own-Library....>
-000027b0: 20e5 85b7 e4bd 93e5 8685 e5ae b9e8 afb7   ...............
-000027c0: e4bb a520 5b70 6f65 7472 7920 e5ae 98e6  ... [poetry ....
-000027d0: 96b9 e696 87e6 a1a3 5d28 6874 7470 733a  ........](https:
-000027e0: 2f2f 7079 7468 6f6e 2d70 6f65 7472 792e  //python-poetry.
-000027f0: 6f72 672f 646f 6373 2f29 20e4 b8ba e587  org/docs/) .....
-00002800: 86e3 8082 0d0a 0d0a e68d ae20 5b33 2e32  ........... [3.2
-00002810: 5d28 2333 2e32 2e2d e4bd a0e5 8faf e883  ](#3.2.-........
-00002820: bde5 9ca8 e684 8fe7 9a84 e4ba 8b29 20e5  .............) .
-00002830: 8faf e79f a5ef bc8c e4bd a0e5 8faf e4bb  ................
-00002840: a520 6063 6c6f 6e65 6020 e6ba 90e7 a081  . `clone` ......
-00002850: e590 8eef bc8c e4bf aee6 94b9 e4bb bbe6  ................
-00002860: 848f e696 b9e6 b395 efbc 88e6 af94 e5a6  ................
-00002870: 82e4 bda0 e79a 84e9 a1b9 e79b aee5 9cba  ................
-00002880: e699 afe4 b88b e58f afe8 83bd e99c 80e8  ................
-00002890: a681 e585 b6e5 ae83 e79a 84e6 97a5 e5bf  ................
-000028a0: 97e9 858d e7bd aee9 bb98 e8ae a4e5 80bc  ................
-000028b0: efbc 8ce6 8896 e6b7 bbe5 8aa0 e585 b6e5  ................
-000028c0: ae83 e79a 84e9 a1b9 e79b aee7 bb93 e69e  ................
-000028d0: 84e6 a8a1 e69d bfe7 ad89 efbc 89ef bc8c  ................
-000028e0: e4bf aee6 94b9 e5ae 8ce6 8890 e590 8e20  ............... 
-000028f0: 6070 6f65 7472 7920 2062 7569 6c64 6020  `poetry  build` 
-00002900: e688 9620 606d 616b 6520 6275 696c 6460  ... `make build`
-00002910: 20e5 8db3 e58f afe6 8993 e58c 85e4 bdbf   ...............
-00002920: e794 a8e3 8082 0d0a 0d0a e6af 94e5 a682  ................
-00002930: e4bd a0e5 8faf e883 bde9 9c80 e8a6 81e6  ................
-00002940: 9bb4 e696 b0e4 be9d e8b5 96e5 ba93 e4b8  ................
-00002950: ad20 6070 796d 6f6e 676f 6020 e4b8 bae6  . `pymongo` ....
-00002960: 96b0 e789 88e6 9cac 2060 782e 782e 7860  ........ `x.x.x`
-00002970: efbc 8ce9 82a3 e58f aae9 9c80 2060 706f  ............ `po
-00002980: 6574 7279 2069 6e73 7461 6c6c 6020 e5ae  etry install` ..
-00002990: 89e8 a385 e78e b0e6 9c89 e4be 9de8 b596  ................
-000029a0: e590 8eef bc8c e586 8d20 6070 6f65 7472  ......... `poetr
-000029b0: 7920 6164 6420 7079 6d6f 6e67 6f40 782e  y add pymongo@x.
-000029c0: 782e 7860 20e5 ae89 e8a3 85e7 9bae e6a0  x.x` ...........
-000029d0: 87e7 8988 e69c acef bc88 e5b0 bde9 878f  ................
-000029e0: e4b8 8de8 a681 e4bd bfe7 94a8 2060 706f  ............ `po
-000029f0: 6574 7279 2075 7064 6174 6520 7079 6d6f  etry update pymo
-00002a00: 6e67 6f60 efbc 89ef bc8c e7a1 aee5 ae9a  ngo`............
-00002a10: e6b5 8be8 af95 e6ad a3e5 b8b8 e4ba 86e5  ................
-00002a20: 8db3 e58f af20 6070 6f65 7472 7920 6275  ..... `poetry bu
-00002a30: 696c 6460 20e6 8993 e58c 85e4 bdbf e794  ild` ...........
-00002a40: a8e3 8082 0d0a 0d0a 2323 2054 6f64 6f4c  ........## TodoL
-00002a50: 6973 740d 0a0d 0a2d 205b 785d 2060 7363  ist....- [x] `sc
-00002a60: 7261 7079 6020 e79a 84e6 89a9 e5b1 95e5  rapy` ..........
-00002a70: 8a9f e883 bde5 9cba e699 af0d 0a20 202d  .............  -
-00002a80: 205b 785d 2060 7363 7261 7079 6020 e884   [x] `scrapy` ..
-00002a90: 9ae6 9cac e8bf 90e8 a18c e4bf a1e6 81af  ................
-00002aa0: e7bb 9fe8 aea1 e592 8ce9 a1b9 e79b aee4  ................
-00002ab0: be9d e8b5 96e8 a1a8 e987 87e9 9b86 e987  ................
-00002ac0: 8fe7 bb9f e8ae a1ef bc8c e58f afe7 94a8  ................
-00002ad0: e4ba 8ee6 97a5 e5bf 97e8 aeb0 e5bd 95e5  ................
-00002ae0: 928c e9a2 84e8 ada6 0d0a 2020 2d20 5b78  ..........  - [x
-00002af0: 5d20 e887 aae5 ae9a e4b9 89e6 a8a1 e69d  ] ..............
-00002b00: bfef bc8c e59c a820 6061 7975 6765 7370  ....... `ayugesp
-00002b10: 6964 6572 746f 6f6c 7320 7374 6172 7470  idertools startp
-00002b20: 726f 6a65 6374 203c 7072 6f6a 6e61 6d65  roject <projname
-00002b30: 3e60 20e5 928c 2060 6179 7567 6573 7069  >` ... `ayugespi
-00002b40: 6465 7274 6f6f 6c73 2067 656e 7370 6964  dertools genspid
-00002b50: 6572 203c 7370 6964 6572 6e61 6d65 3e60  er <spidername>`
-00002b60: 20e6 97b6 e794 9fe6 8890 e980 82e5 9088   ...............
-00002b70: e69c ace5 ba93 e79a 84e6 a8a1 e69d bfe6  ................
-00002b80: 9687 e4bb b60d 0a20 202d 205b 785d 207e  .......  - [x] ~
-00002b90: 7ee5 a29e e58a a0e6 a0b9 e68d ae20 606e  ~............ `n
-00002ba0: 6163 6f73 6020 e69d a5e8 8eb7 e58f 96e9  acos` ..........
-00002bb0: 858d e7bd aee7 9a84 e58a 9fe8 83bd 7e7e  ..............~~
-00002bc0: 202d 3e20 e694 b9e4 b8ba e5a2 9ee5 8aa0   -> ............
-00002bd0: e6a0 b9e6 8dae 2060 636f 6e73 756c 6020  ...... `consul` 
-00002be0: e69d a5e8 8eb7 e58f 96e9 858d e7bd aee7  ................
-00002bf0: 9a84 e58a 9fe8 83bd 0d0a 2020 2d20 5b78  ..........  - [x
-00002c00: 5d20 e4bb a3e7 9086 e4b8 ade9 97b4 e4bb  ] ..............
-00002c10: b6ef bc88 e78b ace4 baab e4bb a3e7 9086  ................
-00002c20: e380 81e5 8aa8 e680 81e9 9aa7 e981 93e4  ................
-00002c30: bba3 e790 86ef bc89 0d0a 2020 2d20 5b78  ..........  - [x
-00002c40: 5d20 e99a 8fe6 9cba e8af b7e6 b182 e5a4  ] ..............
-00002c50: b420 6055 4160 20e4 b8ad e997 b4e4 bbb6  . `UA` .........
-00002c60: efbc 8ce6 a0b9 e68d ae20 6066 616b 655f  ......... `fake_
-00002c70: 7573 6572 6167 656e 7460 20e4 b8ad e79a  useragent` .....
-00002c80: 84e6 9d83 e987 8de6 9da5 e99a 8fe6 9cba  ................
-00002c90: 0d0a 2020 2d20 5b78 5d20 e4bd bfe7 94a8  ..  - [x] ......
-00002ca0: e4bb a5e4 b88b e5b7 a5e5 85b7 e69d a5e6  ................
-00002cb0: 9bbf e68d a220 6073 6372 6170 7960 20e7  ..... `scrapy` .
-00002cc0: 9a84 2060 5265 7175 6573 7460 20e6 9da5  .. `Request` ...
-00002cd0: e58f 91e9 8081 e8af b7e6 b182 0d0a 2020  ..............  
-00002ce0: 2020 2d20 5b78 5d20 7e7e 6072 6571 7565    - [x] ~~`reque
-00002cf0: 7374 7360 3a20 e8bf 99e4 b8aa e4b8 8de6  sts`: ..........
-00002d00: 8ea8 e88d 90e4 bdbf e794 a8ef bc8c 6072  ..............`r
-00002d10: 6571 7565 7374 7360 20e5 908c e6ad a5e5  equests` .......
-00002d20: ba93 e4bc 9ae9 998d e4bd 8e20 6073 6372  ........... `scr
-00002d30: 6170 7960 20e8 bf90 e8a1 8ce6 9588 e78e  apy` ...........
-00002d40: 877e 7eef bc88 e5b7 b2e7 a7bb e999 a4e6  .~~.............
-00002d50: ada4 e58a 9fe8 83bd efbc 8ce6 9bb4 e68e  ................
-00002d60: a8e8 8d90 2060 6169 6f68 7474 7060 20e7  .... `aiohttp` .
-00002d70: 9a84 e696 b9e5 bc8f efbc 890d 0a20 2020  .............   
-00002d80: 202d 205b 785d 2060 6169 6f68 7474 7060   - [x] `aiohttp`
-00002d90: 3a20 e99b 86e6 8890 e5b0 8620 6073 6372  : ......... `scr
-00002da0: 6170 7920 5265 7175 6573 7460 20e6 9bbf  apy Request` ...
-00002db0: e68d a2e4 b8ba 2060 6169 6f68 7474 7060  ...... `aiohttp`
-00002dc0: 20e7 9a84 e58d 8fe7 a88b e696 b9e5 bc8f   ...............
-00002dd0: 0d0a 2020 2d20 5b78 5d20 604d 7973 716c  ..  - [x] `Mysql
-00002de0: 6020 e5ad 98e5 82a8 e79a 84e5 9cba e699  ` ..............
-00002df0: afe4 b88b e980 82e9 858d 0d0a 2020 2020  ............    
-00002e00: 2d20 5b78 5d20 e887 aae5 8aa8 e588 9be5  - [x] ..........
-00002e10: bbba 2060 4d79 7371 6c60 20e7 94a8 e688  .. `Mysql` .....
-00002e20: b7e5 9cba e699 afe4 b88b e99c 80e8 a681  ................
-00002e30: e79a 84e6 95b0 e68d aee5 ba93 e592 8ce6  ................
-00002e40: 95b0 e68d aee8 a1a8 e58f 8ae5 ad97 e6ae  ................
-00002e50: b5e6 a0bc e5bc 8fef bc8c e8bf 98e6 9c89  ................
-00002e60: e5ad 97e6 aeb5 e6b3 a8e9 878a 0d0a 2020  ..............  
-00002e70: 2d20 5b78 5d20 604d 6f6e 676f 4442 6020  - [x] `MongoDB` 
-00002e80: e5ad 98e5 82a8 e79a 84e5 9cba e699 afe4  ................
-00002e90: b88b e980 82e9 858d efbc 8ce7 bc96 e586  ................
-00002ea0: 99e9 a38e e6a0 bce4 b88e 2060 4d79 7371  .......... `Mysq
-00002eb0: 6c60 20e5 ad98 e582 a8e7 ad89 e59c bae6  l` .............
-00002ec0: 99af e4b8 8be4 b880 e887 b40d 0a20 202d  .............  -
-00002ed0: 205b 785d 2060 6173 796e 6369 6f60 20e8   [x] `asyncio` .
-00002ee0: afad e6b3 95e6 94af e68c 81e4 b88e 2060  .............. `
-00002ef0: 6173 796e 6360 20e7 acac e4b8 89e6 96b9  async` .........
-00002f00: e5ba 93e6 94af e68c 81e7 a4ba e4be 8b0d  ................
-00002f10: 0a20 2020 202d 205b 785d 2060 7370 6964  .    - [x] `spid
-00002f20: 6572 6020 e4b8 ade4 bdbf e794 a820 6061  er` ......... `a
-00002f30: 7379 6e63 696f 6020 e79a 8420 6061 696f  syncio` ... `aio
-00002f40: 6874 7470 6020 e7a4 bae4 be8b 0d0a 2020  http` ........  
-00002f50: 2020 2d20 5b78 5d20 6070 6970 656c 696e    - [x] `pipelin
-00002f60: 6560 20e4 b8ad e4bd bfe7 94a8 2060 6173  e` ......... `as
-00002f70: 796e 6369 6f60 20e7 9a84 2060 6169 6f4d  yncio` ... `aioM
-00002f80: 7973 716c 6020 e7a4 bae4 be8b 0d0a 2020  ysql` ........  
-00002f90: 2d20 5b78 5d20 e99b 86e6 8890 2060 4b61  - [x] ...... `Ka
-00002fa0: 666b 6160 efbc 8c60 5261 6262 6974 4d51  fka`...`RabbitMQ
-00002fb0: 6020 e7ad 89e6 95b0 e68d aee6 8ea8 e980  ` ..............
-00002fc0: 81e5 8a9f e883 bd0d 0a2d 205b 785d 20e5  .........- [x] .
-00002fd0: b8b8 e794 a8e5 bc80 e58f 91e5 9cba e699  ................
-00002fe0: af0d 0a20 202d 205b 785d 2060 7371 6c60  ...  - [x] `sql`
-00002ff0: 20e8 afad e58f a5e6 8bbc e68e a5ef bc8c   ...............
-00003000: e58f aae6 98af e7ae 80e5 8d95 e59c bae6  ................
-00003010: 99af efbc 8ce5 908e e7bb ade4 bc98 e58c  ................
-00003020: 96e3 8082 e5b7 b2e7 bb99 e587 bae4 bc98  ................
-00003030: e58c 96e6 96b9 e590 91ef bc8c e58f 82e8  ................
-00003040: 8083 e5ba 93e7 ad89 e4bf a1e6 81af e380  ................
-00003050: 820d 0a20 202d 205b 785d 2060 6d6f 6e67  ...  - [x] `mong
-00003060: 6f44 4260 20e8 afad e58f a5e6 8bbc e68e  oDB` ...........
-00003070: a50d 0a20 202d 205b 785d 20e6 95b0 e68d  ...  - [x] .....
-00003080: aee6 a0bc e5bc 8fe5 8c96 e5a4 84e7 9086  ................
-00003090: efbc 8ce6 af94 e5a6 82ef bc9a e58e bbe9  ................
-000030a0: 99a4 e7bd 91e9 a1b5 e6a0 87e7 adbe efbc  ................
-000030b0: 8ce5 8ebb e999 a4e6 97a0 e695 88e7 a9ba  ................
-000030c0: e6a0 bce7 ad89 0d0a 2020 2d20 5b78 5d20  ........  - [x] 
-000030d0: e5ad 97e4 bd93 e58f 8de7 88ac e8bf 98e5  ................
-000030e0: 8e9f e696 b9e6 b395 0d0a 2020 2020 2d20  ..........    - 
-000030f0: 5b78 5d20 e59f bae4 ba8e 2060 7474 6660  [x] ...... `ttf`
-00003100: efbc 8c60 776f 6666 6020 e4b9 8be7 b1bb  ...`woff` ......
-00003110: e79a 84e5 ad97 e4bd 93e6 9687 e4bb b6e6  ................
-00003120: 98a0 e5b0 84ef bc8c e688 96e7 bb93 e590  ................
-00003130: 8820 6063 7373 6020 e7ad 89e5 ae9e e78e  . `css` ........
-00003140: b00d 0a20 2020 2020 202d 205b 785d 20e5  ...      - [x] .
-00003150: 8faf e4bb a5e7 9bb4 e68e a5e5 9ca8 e5ad  ................
-00003160: 97e4 bd93 e696 87e4 bbb6 2060 786d 6c60  .......... `xml`
-00003170: 20e4 b8ad e689 bee5 88b0 e698 a0e5 b084   ...............
-00003180: e585 b3e7 b3bb e79a 84ef bc9a e4bd bfe7  ................
-00003190: 94a8 205b 666f 6e74 666f 7267 655d 2868  .. [fontforge](h
-000031a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000031b0: 6d2f 666f 6e74 666f 7267 652f 666f 6e74  m/fontforge/font
-000031c0: 666f 7267 652f 7265 6c65 6173 6573 2920  forge/releases) 
-000031d0: e5b7 a5e5 85b7 e5af bce5 87ba e698 a0e5  ................
-000031e0: b084 e58d b3e5 8faf e380 820d 0a20 2020  .............   
-000031f0: 2020 202d 205b 785d 20e6 97a0 e6b3 95e6     - [x] .......
-00003200: 89be e588 b0e6 98a0 e5b0 84e5 85b3 e7b3  ................
-00003210: bbe7 9a84 efbc 8ce5 8899 e4b8 80e8 88ac  ................
-00003220: e4bd bfe7 94a8 2060 6f63 7260 20e8 af86  ...... `ocr` ...
-00003230: e588 abef bc88 e587 86e7 a1ae e78e 87e9  ................
-00003240: 9d9e e799 bee5 8886 e799 beef bc89 efbc  ................
-00003250: 8ce9 809a e8bf 8720 6066 6f6e 7466 6f72  ....... `fontfor
-00003260: 6765 6020 e5af bce5 87ba e6af 8fe4 b8aa  ge` ............
-00003270: e698 a0e5 b084 e79a 8420 6070 6e67 60ef  ......... `png`.
-00003280: bc8c e590 8ee5 868d e980 9ae8 bf87 e590  ................
-00003290: 84e7 a78d e696 b9e5 bc8f e8af 86e5 88ab  ................
-000032a0: e380 820d 0a20 202d 205b 785d 2060 6874  .....  - [x] `ht
-000032b0: 6d6c 6020 e6a0 bce5 bc8f e8bd ac20 606d  ml` ......... `m
-000032c0: 6172 6b64 6f77 6e60 20e6 a0bc e5bc 8f0d  arkdown` .......
-000032d0: 0a20 202d 205b 785d 2060 6874 6d6c 6020  .  - [x] `html` 
-000032e0: e695 b0e6 8dae e5a4 84e7 9086 efbc 8ce5  ................
-000032f0: 8ebb e999 a4e6 a087 e7ad beef bc8c e4b8  ................
-00003300: 8de5 8faf e8a7 81e5 ad97 e7ac a6ef bc8c  ................
-00003310: e789 b9e6 ae8a e5ad 97e7 aca6 e694 b9e6  ................
-00003320: 8890 e6ad a3e5 b8b8 e698 bee7 a4ba e7ad  ................
-00003330: 89e7 ad89 e7ad 890d 0a20 202d 205b 785d  .........  - [x]
-00003340: 20e6 b7bb e58a a0e5 b8b8 e794 a8e7 9a84   ...............
-00003350: e59b bee7 8987 e9aa 8ce8 af81 e7a0 81e4  ................
-00003360: b8ad e79a 84e5 a484 e790 86e6 96b9 e6b3  ................
-00003370: 950d 0a20 2020 202d 205b 785d 20e6 bb91  ...    - [x] ...
-00003380: e59d 97e7 bcba e58f a3e8 b79d e7a6 bbe7  ................
-00003390: 9a84 e8af 86e5 88ab e696 b9e6 b395 efbc  ................
-000033a0: 88e5 a49a e7a7 8de5 ae9e e78e b0e6 96b9  ................
-000033b0: e5bc 8fef bc89 0d0a 2020 2020 2d20 5b78  ........    - [x
-000033c0: 5d20 e6a0 b9e6 8dae e6bb 91e5 9d97 e8b7  ] ..............
-000033d0: 9de7 a6bb e794 9fe6 8890 e8bd a8e8 bfb9  ................
-000033e0: e695 b0e7 bb84 e79a 84e6 96b9 e6b3 950d  ................
-000033f0: 0a20 2020 202d 205b 785d 20e8 af86 e588  .    - [x] .....
-00003400: abe7 82b9 e980 89e9 aa8c e8af 81e7 a081  ................
-00003410: e4bd 8de7 bdae e58f 8ae7 82b9 e587 bbe9  ................
-00003420: a1ba e5ba 8fef bc8c e8af 86e5 88ab e7bb  ................
-00003430: 93e6 9e9c e4b8 8de5 a4aa e5a5 bdef bc8c  ................
-00003440: e5be 85e4 bc98 e58c 960d 0a20 2020 202d  ...........    -
-00003450: 205b 785d 20e5 9bbe e789 87e4 b9b1 e5ba   [x] ...........
-00003460: 8fe6 b7b7 e6b7 86e7 9a84 e8bf 98e5 8e9f  ................
-00003470: e696 b9e6 b395 e7a4 bae4 be8b 0d0a 0d0a  ................
-00003480: 2a2a e6b3 a8ef bc9a 2a2a 0d0a 0d0a 312e  **......**....1.
-00003490: 20e7 94b1 e4ba 8e20 6073 6372 6170 7960   ...... `scrapy`
-000034a0: 20e6 89a9 e5b1 95e5 ba93 e79a 84e5 bc80   ...............
-000034b0: e6ba 90e9 a1b9 e79b aee4 bc97 e5a4 9aef  ................
-000034c0: bc8c e59c a8e4 bdbf e794 a8e6 9cac e5ba  ................
-000034d0: 93e7 9a84 e59f bae7 a180 e4b8 8ae6 89a9  ................
-000034e0: e5b1 95e5 ae83 e4bb acef bc8c e4b8 8ee4  ................
-000034f0: bdbf e794 a820 6073 6372 6170 7960 20e6  ..... `scrapy` .
-00003500: 97b6 e689 a9e5 b195 e5ae 83e4 bbac e79a  ................
-00003510: 84e7 94a8 e6b3 95e4 b880 e887 b4ef bc8c  ................
-00003520: e689 80e4 bba5 e4b8 8de5 868d e5bc 80e5  ................
-00003530: 8f91 e4b8 80e4 ba9b e585 b6e5 ae83 e5b7  ................
-00003540: a5e5 85b7 e5b7 b2e7 bb8f e68b a5e6 9c89  ................
-00003550: e4b8 94e7 a8b3 e5ae 9ae7 9a84 e58a 9fe8  ................
-00003560: 83bd efbc 8ce4 bd86 e4b9 9fe4 bc9a e5b0  ................
-00003570: bde9 878f e5bc 80e5 8f91 e4b8 80e4 ba9b  ................
-00003580: e5b8 b8e7 94a8 e4b8 94e9 809a e794 a8e7  ................
-00003590: 9a84 e696 b9e6 b395 e69d a5e6 8f90 e58d  ................
-000035a0: 87e6 9588 e78e 87e3 8082 0d0a 322e 20e5  ............2. .
-000035b0: ad97 e4bd 93e5 8f8d e788 ace9 83a8 e588  ................
-000035c0: 86e4 b88d e4bc 9ae7 bb99 e587 bae8 afa6  ................
-000035d0: e7bb 86e8 a7a3 e586 b3e7 a4ba e4be 8bef  ................
-000035e0: bc8c e4b8 8de7 aea1 e698 afe4 bdbf e794  ................
-000035f0: a820 6066 6f6e 7466 6f72 6765 60ef bc8c  . `fontforge`...
-00003600: 6066 6f6e 7454 6f6f 6c73 6020 e688 9620  `fontTools` ... 
-00003610: 606f 6372 6020 e7ad 89e5 b7a5 e585 b7ef  `ocr` ..........
-00003620: bc8c e5b7 b2e7 bb8f e884 b1e7 a6bb e69c  ................
-00003630: ace5 ba93 e79a 84e8 8c83 e59b b4e4 ba86  ................
-00003640: efbc 8ce6 8891 e4bc 9ae7 bb99 e587 bae9  ................
-00003650: 83a8 e588 86e4 be9d e8b5 96e7 9a84 e696  ................
-00003660: b9e6 b395 efbc 8ce4 bd86 e4b8 8de4 bc9a  ................
-00003670: e6b7 bbe5 8aa0 e4bb a5e4 b88a e5b7 a5e5  ................
-00003680: 85b7 e5ba 93e7 9a84 e4be 9de8 b596 e4ba  ................
-00003690: 86ef bc8c e880 8ce5 afbc e887 b4e6 9cac  ................
-000036a0: e5ba 93e4 be9d e8b5 96e8 bf87 e4ba 8ee6  ................
-000036b0: 9d82 e7b3 85e3 8082 e880 8ce4 b894 efbc  ................
-000036c0: 8ce8 8ba5 e8a6 81e5 ae9e e78e b0e9 ab98  ................
-000036d0: e58f afe7 94a8 e79a 84e5 ad97 e4bd 93e6  ................
-000036e0: 98a0 e5b0 84e4 b99f e6af 94e8 be83 e7ae  ................
-000036f0: 80e5 8d95 efbc 8ce8 afb7 e887 aae8 a18c  ................
-00003700: e5ae 9ee7 8eb0 efbc 8ce5 8faf e883 bde4  ................
-00003710: bc9a e880 83e8 9991 e696 b0e5 bc80 2060  .............. `
-00003720: 7079 7069 6020 e5ba 93e6 9da5 e5ae 9ee7  pypi` ..........
-00003730: 8eb0 e6ad a4e9 83a8 e588 86e3 8082 0d0a  ................
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0d0a 2020 2020 3c61 2068 7265 663d  ">..    <a href=
+00000020: 2268 7474 7073 3a2f 2f61 7975 6765 7370  "https://ayugesp
+00000030: 6964 6572 746f 6f6c 732e 7265 6164 7468  idertools.readth
+00000040: 6564 6f63 732e 696f 2220 7461 7267 6574  edocs.io" target
+00000050: 3d22 5f62 6c61 6e6b 2220 7265 6c3d 226e  ="_blank" rel="n
+00000060: 6f6f 7065 6e65 7220 6e6f 7265 6665 7272  oopener noreferr
+00000070: 6572 223e 0d0a 2020 2020 2020 2020 3c69  er">..        <i
+00000080: 6d67 2073 7263 3d22 2e2f 6172 7477 6f72  mg src="./artwor
+00000090: 6b2f 6179 7567 6573 7069 6465 7274 6f6f  k/ayugespidertoo
+000000a0: 6c73 2d6c 6f67 6f2e 706e 6722 2061 6c74  ls-logo.png" alt
+000000b0: 3d22 6179 7567 6573 7069 6465 7274 6f6f  ="ayugespidertoo
+000000c0: 6c73 2d6c 6f67 6f22 3e0d 0a20 2020 203c  ls-logo">..    <
+000000d0: 2f61 3e0d 0a3c 2f70 3e0d 0a3c 6872 2f3e  /a>..</p>..<hr/>
+000000e0: 0d0a 0d0a 2320 4179 7567 6553 7069 6465  ....# AyugeSpide
+000000f0: 7254 6f6f 6c73 20e4 bb8b e7bb 8d0d 0a0d  rTools .........
+00000100: 0a5b 215b 4f53 4353 2053 7461 7475 735d  .[![OSCS Status]
+00000110: 2868 7474 7073 3a2f 2f77 7777 2e6f 7363  (https://www.osc
+00000120: 7331 3032 342e 636f 6d2f 706c 6174 666f  s1024.com/platfo
+00000130: 726d 2f62 6164 6765 2f41 7975 6765 5370  rm/badge/AyugeSp
+00000140: 6964 6572 546f 6f6c 732e 7376 673f 7369  iderTools.svg?si
+00000150: 7a65 3d73 6d61 6c6c 295d 2868 7474 7073  ze=small)](https
+00000160: 3a2f 2f77 7777 2e6d 7572 7068 7973 6563  ://www.murphysec
+00000170: 2e63 6f6d 2f61 6363 6570 743f 636f 6465  .com/accept?code
+00000180: 3d30 6563 3337 3537 3539 6165 6265 6137  =0ec375759aebea7
+00000190: 6664 3236 3032 3438 3931 3062 3938 3830  fd260248910b9880
+000001a0: 3626 7479 7065 3d31 2666 726f 6d3d 3229  6&type=1&from=2)
+000001b0: 0d0a 215b 4769 7448 7562 5d28 6874 7470  ..![GitHub](http
+000001c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001d0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+000001e0: 652f 7368 656e 6763 6865 6e79 616e 672f  e/shengchenyang/
+000001f0: 4179 7567 6553 7069 6465 7254 6f6f 6c73  AyugeSpiderTools
+00000200: 290d 0a21 5b70 7974 686f 6e5d 2868 7474  )..![python](htt
+00000210: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000220: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
+00000230: 2d33 2e38 2e31 2532 422d 626c 7565 290d  -3.8.1%2B-blue).
+00000240: 0a21 5b47 6974 4875 6220 576f 726b 666c  .![GitHub Workfl
+00000250: 6f77 2053 7461 7475 7320 2877 6974 6820  ow Status (with 
+00000260: 6272 616e 6368 295d 2868 7474 7073 3a2f  branch)](https:/
+00000270: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000280: 6769 7468 7562 2f61 6374 696f 6e73 2f77  github/actions/w
+00000290: 6f72 6b66 6c6f 772f 7374 6174 7573 2f73  orkflow/status/s
+000002a0: 6865 6e67 6368 656e 7961 6e67 2f41 7975  hengchenyang/Ayu
+000002b0: 6765 5370 6964 6572 546f 6f6c 732f 636f  geSpiderTools/co
+000002c0: 6465 716c 2e79 6d6c 3f62 7261 6e63 683d  deql.yml?branch=
+000002d0: 6d61 696e 290d 0a21 5b52 6561 6420 7468  main)..![Read th
+000002e0: 6520 446f 6373 5d28 6874 7470 733a 2f2f  e Docs](https://
+000002f0: 696d 672e 7368 6965 6c64 732e 696f 2f72  img.shields.io/r
+00000300: 6561 6474 6865 646f 6373 2f61 7975 6765  eadthedocs/ayuge
+00000310: 7370 6964 6572 746f 6f6c 7329 0d0a 215b  spidertools)..![
+00000320: 4769 7448 7562 2061 6c6c 2072 656c 6561  GitHub all relea
+00000330: 7365 735d 2868 7474 7073 3a2f 2f69 6d67  ses](https://img
+00000340: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000350: 7562 2f64 6f77 6e6c 6f61 6473 2f73 6865  ub/downloads/she
+00000360: 6e67 6368 656e 7961 6e67 2f41 7975 6765  ngchenyang/Ayuge
+00000370: 5370 6964 6572 546f 6f6c 732f 746f 7461  SpiderTools/tota
+00000380: 6c3f 6c61 6265 6c3d 7265 6c65 6173 6573  l?label=releases
+00000390: 2532 3064 6f77 6e6c 6f61 6473 290d 0a21  %20downloads)..!
+000003a0: 5b50 7950 4920 2d20 446f 776e 6c6f 6164  [PyPI - Download
+000003b0: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+000003c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
+000003d0: 6d2f 4179 7567 6553 7069 6465 7254 6f6f  m/AyugeSpiderToo
+000003e0: 6c73 3f6c 6162 656c 3d70 7970 6925 3230  ls?label=pypi%20
+000003f0: 646f 776e 6c6f 6164 7329 0d0a 0d0a 2a2a  downloads)....**
+00000400: e7ae 80e4 bd93 e4b8 ade6 9687 2a2a 207c  ............** |
+00000410: 205b 456e 676c 6973 685d 282e 2f52 4541   [English](./REA
+00000420: 444d 455f 656e 2e6d 6429 0d0a 0d0a 2323  DME_en.md)....##
+00000430: 20e6 a682 e8bf b00d 0a0d 0a3e 20e4 b880   ..........> ...
+00000440: e58f a5e8 af9d e4bb 8be7 bb8d efbc 9ae7  ................
+00000450: 94a8 e4ba 8ee6 89a9 e5b1 9520 5363 7261  ........... Scra
+00000460: 7079 20e5 8a9f e883 bde6 9da5 e8a7 a3e6  py .............
+00000470: 94be e58f 8ce6 898b e380 820d 0a0d 0ae5  ................
+00000480: 9ca8 e4bd bfe7 94a8 2060 5363 7261 7079  ........ `Scrapy
+00000490: 6020 e5bc 80e5 8f91 e788 ace8 99ab e697  ` ..............
+000004a0: b6ef bc8c e585 8de4 b88d e4ba 86e4 bc9a  ................
+000004b0: e987 8de5 a48d e59c b0e7 bc96 e586 9920  ............... 
+000004c0: 6073 6574 7469 6e67 7360 efbc 8c60 6974  `settings`...`it
+000004d0: 656d 7360 efbc 8c60 6d69 6464 6c65 7761  ems`...`middlewa
+000004e0: 7265 7360 efbc 8c60 7069 7065 6c69 6e65  res`...`pipeline
+000004f0: 7360 0d0a e592 8ce4 b880 e4ba 9be9 809a  s`..............
+00000500: e794 a8e6 96b9 e6b3 95ef bc8c e4bd 86e5  ................
+00000510: 9084 e9a1 b9e7 9bae e4b8 ade7 9a84 e8bf  ................
+00000520: 99e4 ba9b e586 85e5 aeb9 e983 bde5 a4a7  ................
+00000530: e887 b4e7 9bb8 e590 8cef bc8c e982 a3e4  ................
+00000540: b8ba e4bd 95e4 b88d e68a 8ae5 ae83 e4bb  ................
+00000550: ace7 bb9f e4b8 80e6 95b4 e790 86e5 9ca8  ................
+00000560: e4b8 80e8 b5b7 e591 a2ef bc9f e688 91e4  ................
+00000570: b99f e683 b3e6 89a9 e5b1 95e4 b880 e4ba  ................
+00000580: 9be5 8a9f e883 bdef bc8c e6af 94e5 a682  ................
+00000590: e5bd 9320 6073 7069 6465 7260 0d0a e4b8  ... `spider`....
+000005a0: ade6 b7bb e58a a0e5 ad97 e6ae b5e5 908e  ................
+000005b0: efbc 8ce4 b88d e794 a8e5 868d e4bf aee6  ................
+000005c0: 94b9 e5af b9e5 ba94 e79a 8420 6069 7465  ........... `ite
+000005d0: 6d60 20e5 928c 2060 7069 7065 6c69 6e65  m` ... `pipeline
+000005e0: 7360 20e7 949a e887 b3e4 b88d e794 a8e6  s` .............
+000005f0: 898b e58a a8e4 bfae e694 b920 604d 7973  ........... `Mys
+00000600: 716c 6020 e8a1 a8e7 bb93 e69e 84ef bc8c  ql` ............
+00000610: e6ad a4e6 97b6 e4bd bfe7 94a8 2060 7363  ............ `sc
+00000620: 7261 7079 6020 e79a 84e6 a8a1 e69d bfe5  rapy` ..........
+00000630: 8a9f e883 bde5 b0b1 e4b8 8de5 a49f e4ba  ................
+00000640: 86e3 8082 0d0a 0d0a e9a1 b9e7 9bae e79a  ................
+00000650: 84e4 b8bb e697 a8e6 98af e8ae a9e5 bc80  ................
+00000660: e58f 91e8 8085 e58f aae9 9c80 e4b8 93e6  ................
+00000670: b3a8 e4ba 8e20 6073 7069 6465 7260 20e8  ..... `spider` .
+00000680: 849a e69c ace7 9a84 e7bc 96e5 8699 efbc  ................
+00000690: 8ce5 878f e5b0 91e5 bc80 e58f 91e5 928c  ................
+000006a0: e7bb b4e6 8aa4 e6b5 81e7 a88b e380 82e7  ................
+000006b0: 9086 e683 b3e7 8ab6 e680 81e4 b88b efbc  ................
+000006c0: 8ce5 8faa e99c 80e5 85b3 e6b3 a820 6073  ............. `s
+000006d0: 7069 6465 7260 0d0a e4b8 ade5 ad97 e6ae  pider`..........
+000006e0: b5e7 9a84 e8a7 a3e6 9e90 e8a7 84e5 8899  ................
+000006f0: e592 8c20 6056 4954 6020 e4b8 8be7 9a84  ... `VIT` ......
+00000700: 2060 2e63 6f6e 6660 20e9 858d e7bd aee5   `.conf` .......
+00000710: 8db3 e58f afef bc8c 2a2a e884 b1e7 a6bb  ........**......
+00000720: e697 a0e6 848f e4b9 89e7 9a84 e987 8de5  ................
+00000730: a48d e693 8de4 bd9c 2a2a e380 820d 0a0d  ........**......
+00000740: 0ae4 bba5 2060 4d79 7371 6c60 20e5 ad98  .... `Mysql` ...
+00000750: e582 a8e5 9cba e699 afe4 b8be e4be 8bef  ................
+00000760: bc9a e58f afe4 bba5 e887 aae5 8aa8 e588  ................
+00000770: 9be5 bbba e79b b8e5 85b3 e695 b0e6 8dae  ................
+00000780: e5ba 93ef bc8c e695 b0e6 8dae e8a1 a8ef  ................
+00000790: bc8c e5ad 97e6 aeb5 e6b3 a8e9 878a efbc  ................
+000007a0: 8ce8 87aa e58a a8e6 b7bb e58a a020 6073  ............. `s
+000007b0: 7069 6465 7260 0d0a e4b8 ade6 96b0 e6b7  pider`..........
+000007c0: bbe5 8aa0 e79a 84e5 ad97 e6ae b5ef bc8c  ................
+000007d0: e592 8ce8 87aa e58a a8e4 bfae e5a4 8de5  ................
+000007e0: b8b8 e8a7 81ef bc88 e5ad 97e6 aeb5 e7bc  ................
+000007f0: 96e7 a081 efbc 8c60 4461 7461 2074 6f6f  .......`Data too
+00000800: 206c 6f6e 6760 efbc 8ce5 ad98 e582 a8e5   long`..........
+00000810: ad97 e6ae b5e4 b88d e5ad 98e5 9ca8 e7ad  ................
+00000820: 89ef bc89 e79a 84e5 ad98 e582 a8e9 97ae  ................
+00000830: e9a2 98e3 8082 0d0a 0d0a 2323 20e5 ae89  ..........## ...
+00000840: e8a3 850d 0a0d 0a3e 2060 7079 7468 6f6e  .......> `python
+00000850: 2033 2e38 2e31 2b60 20e5 8faf e4bb a5e7   3.8.1+` .......
+00000860: 9bb4 e68e a5e8 be93 e585 a5e4 bba5 e4b8  ................
+00000870: 8be5 91bd e4bb a4ef bc9a 0d0a 0d0a 6060  ..............``
+00000880: 6073 6865 6c6c 0d0a 7069 7020 696e 7374  `shell..pip inst
+00000890: 616c 6c20 6179 7567 6573 7069 6465 7274  all ayugespidert
+000008a0: 6f6f 6c73 202d 6920 6874 7470 733a 2f2f  ools -i https://
+000008b0: 7079 7069 2e6f 7267 2f73 696d 706c 650d  pypi.org/simple.
+000008c0: 0a60 6060 0d0a 0d0a 2323 20e7 94a8 e6b3  .```....## .....
+000008d0: 950d 0a0d 0a3e 20e5 bc80 e58f 91e4 baba  .....> .........
+000008e0: e591 98e5 8faa e99c 80e6 a0b9 e68d aee5  ................
+000008f0: 91bd e4bb a4e7 949f e688 90e7 a4ba e4be  ................
+00000900: 8be6 a8a1 e69d bfef bc8c e586 8de9 858d  ................
+00000910: e7bd aee7 9bb8 e585 b3e8 aebe e7bd aee5  ................
+00000920: 8db3 e58f afe3 8082 0d0a 0d0a e4bd bfe7  ................
+00000930: 94a8 e696 b9e6 b395 e7a4 bae4 be8b 2060  .............. `
+00000940: 4749 4660 20e5 a682 e4b8 8bef bc9a 0d0a  GIF` ...........
+00000950: 0d0a 215b 6179 7567 6573 7069 6465 7274  ..![ayugespidert
+00000960: 6f6f 6c73 2e67 6966 5d28 2e2f 6578 616d  ools.gif](./exam
+00000970: 706c 6573 2f61 7975 6765 7370 6964 6572  ples/ayugespider
+00000980: 746f 6f6c 732d 7573 652e 6769 6629 0d0a  tools-use.gif)..
+00000990: 0d0a e5af b9e4 bba5 e4b8 8a20 6047 4946  ........... `GIF
+000009a0: 6020 e4b8 ade7 9a84 e6ad a5e9 aaa4 e8bf  ` ..............
+000009b0: 9be8 a18c e8a7 a3e9 878a efbc 9a0d 0a0d  ................
+000009c0: 0a60 6060 7368 656c 6c0d 0a23 20e6 9fa5  .```shell..# ...
+000009d0: e79c 8be5 ba93 e789 88e6 9cac 0d0a 6179  ..............ay
+000009e0: 7567 6520 7665 7273 696f 6e0d 0a0d 0a23  uge version....#
+000009f0: 20e5 889b e5bb bae9 a1b9 e79b ae0d 0a61   ..............a
+00000a00: 7975 6765 2073 7461 7274 7072 6f6a 6563  yuge startprojec
+00000a10: 7420 3c70 726f 6a65 6374 5f6e 616d 653e  t <project_name>
+00000a20: 0d0a 0d0a 2320 e8bf 9be5 85a5 e9a1 b9e7  ....# ..........
+00000a30: 9bae e6a0 b9e7 9bae e5bd 950d 0a63 6420  .............cd 
+00000a40: 3c70 726f 6a65 6374 5f6e 616d 653e 0d0a  <project_name>..
+00000a50: 0d0a 2320 e69b bfe6 8da2 28e8 a686 e79b  ..# ......(.....
+00000a60: 9629 e4b8 bae7 9c9f e5ae 9ee7 9a84 e985  .)..............
+00000a70: 8de7 bdae 202e 636f 6e66 20e6 9687 e4bb  .... .conf .....
+00000a80: b6ef bc9a 0d0a 2320 e8bf 99e9 878c e698  ......# ........
+00000a90: afe4 b8ba e4ba 86e6 bc94 e7a4 bae6 96b9  ................
+00000aa0: e4be bfef bc8c e6ad a3e5 b8b8 e683 85e5  ................
+00000ab0: 86b5 e698 afe7 9bb4 e68e a5e5 9ca8 2056  .............. V
+00000ac0: 4954 20e8 b7af e5be 84e4 b88b e79a 8420  IT ............ 
+00000ad0: 2e63 6f6e 6620 e985 8de7 bdae e696 87e4  .conf ..........
+00000ae0: bbb6 e5a1 abe4 b88a e4bd a0e9 9c80 e8a6  ................
+00000af0: 81e7 9a84 e985 8de7 bdae e58d b3e5 8faf  ................
+00000b00: 0d0a 2320 e4b8 8de9 9c80 e8a6 81e7 9a84  ..# ............
+00000b10: e985 8de7 bdae e8ae bee7 bdae e4b8 bae7  ................
+00000b20: a9ba efbc 8ce6 8896 e880 85e4 b88d e794  ................
+00000b30: a8e7 9086 e4bc 9ae5 ae83 efbc 8ce6 8896  ................
+00000b40: e880 85e5 88a0 e999 a4e5 ae83 e4b9 9fe5  ................
+00000b50: 8faf e4bb a5ef bc8c e79c 8be4 b8aa e4ba  ................
+00000b60: bae9 8089 e68b a90d 0a63 7020 2f72 6f6f  .........cp /roo
+00000b70: 742f 6d79 7465 6d70 2f2e 636f 6e66 2044  t/mytemp/.conf D
+00000b80: 656d 6f53 7069 6465 722f 5649 542f 2e63  emoSpider/VIT/.c
+00000b90: 6f6e 660d 0a0d 0a23 20e7 949f e688 90e7  onf....# .......
+00000ba0: 88ac e899 abe8 849a e69c ac0d 0a61 7975  .............ayu
+00000bb0: 6765 2067 656e 7370 6964 6572 203c 7370  ge genspider <sp
+00000bc0: 6964 6572 5f6e 616d 653e 203c 6578 616d  ider_name> <exam
+00000bd0: 706c 652e 636f 6d3e 0d0a 0d0a 2320 e8bf  ple.com>....# ..
+00000be0: 90e8 a18c e884 9ae6 9cac 0d0a 7363 7261  ............scra
+00000bf0: 7079 2063 7261 776c 203c 7370 6964 6572  py crawl <spider
+00000c00: 5f6e 616d 653e 0d0a 2320 e6b3 a8ef bc9a  _name>..# ......
+00000c10: e4b9 9fe5 8faf e4bb a5e4 bdbf e794 a820  ............... 
+00000c20: 6179 7567 6520 6372 6177 6c20 3c73 7069  ayuge crawl <spi
+00000c30: 6465 725f 6e61 6d65 3e0d 0a60 6060 0d0a  der_name>..```..
+00000c40: 0d0a e585 b7e4 bd93 e79a 84e5 9cba e699  ................
+00000c50: afe6 a188 e4be 8be8 afb7 e59c a820 5b44  ............. [D
+00000c60: 656d 6f53 7069 6465 725d 2868 7474 7073  emoSpider](https
+00000c70: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+00000c80: 656e 6763 6865 6e79 616e 672f 4465 6d6f  engchenyang/Demo
+00000c90: 5370 6964 6572 290d 0ae9 a1b9 e79b aee4  Spider).........
+00000ca0: b8ad e69f a5e7 9c8b efbc 8ce4 b99f e58f  ................
+00000cb0: afe4 bba5 e59c a820 5b72 6561 6474 6865  ....... [readthe
+00000cc0: 646f 6373 5d28 6874 7470 733a 2f2f 6179  docs](https://ay
+00000cd0: 7567 6573 7069 6465 7274 6f6f 6c73 2e72  ugespidertools.r
+00000ce0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000cf0: 2f6c 6174 6573 742f 2920 e696 87e6 a1a3  /latest/) ......
+00000d00: e4b8 ade6 9fa5 e79c 8be6 9599 e7a8 8be3  ................
+00000d10: 8082 20e7 9bae e589 8de5 b7b2 e980 82e9  .. .............
+00000d20: 858d e4bb a5e4 b88b e59c bae6 99af efbc  ................
+00000d30: 9a0d 0a0d 0a60 6060 6469 6666 0d0a 2320  .....```diff..# 
+00000d40: e695 b0e6 8dae e5ad 98e5 85a5 204d 7973  ............ Mys
+00000d50: 716c 20e7 9a84 e59c bae6 99af efbc 9a0d  ql .............
+00000d60: 0a2b 2031 292e 6465 6d6f 5f6f 6e65 3a20  .+ 1).demo_one: 
+00000d70: e985 8de7 bdae e6a0 b9e6 8dae e69c ace5  ................
+00000d80: 9cb0 2073 6574 7469 6e67 7320 e79a 8420  .. settings ... 
+00000d90: 4c4f 4341 4c5f 4d59 5351 4c5f 434f 4e46  LOCAL_MYSQL_CONF
+00000da0: 4947 20e4 b8ad e58f 96e5 80bc 0d0a 2b20  IG ...........+ 
+00000db0: 3329 2e64 656d 6f5f 7468 7265 653a 20e9  3).demo_three: .
+00000dc0: 858d e7bd aee6 a0b9 e68d ae20 636f 6e73  ........... cons
+00000dd0: 756c 20e7 9a84 e5ba 94e7 94a8 e7ae a1e7  ul .............
+00000de0: 9086 e4b8 ade5 bf83 e4b8 ade5 8f96 e580  ................
+00000df0: bc0d 0a2b 2035 292e 6465 6d6f 5f66 6976  ...+ 5).demo_fiv
+00000e00: 653a 20e5 bc82 e6ad a5e5 ad98 e585 a520  e: ............ 
+00000e10: 4d79 7371 6c20 e79a 84e5 9cba e699 af0d  Mysql ..........
+00000e20: 0a0d 0a23 20e6 95b0 e68d aee5 ad98 e585  ...# ...........
+00000e30: a520 4d6f 6e67 6f44 4220 e79a 84e5 9cba  . MongoDB ......
+00000e40: e699 afef bc9a 0d0a 2b20 3229 2e64 656d  ........+ 2).dem
+00000e50: 6f5f 7477 6f3a 20e9 858d e7bd aee6 a0b9  o_two: .........
+00000e60: e68d aee6 9cac e59c b020 7365 7474 696e  ......... settin
+00000e70: 6773 20e7 9a84 204c 4f43 414c 5f4d 4f4e  gs ... LOCAL_MON
+00000e80: 474f 4442 5f43 4f4e 4649 4720 e4b8 ade5  GODB_CONFIG ....
+00000e90: 8f96 e580 bc0d 0a2b 2034 292e 6465 6d6f  .......+ 4).demo
+00000ea0: 5f66 6f75 723a 20e9 858d e7bd aee6 a0b9  _four: .........
+00000eb0: e68d ae20 636f 6e73 756c 20e7 9a84 e5ba  ... consul .....
+00000ec0: 94e7 94a8 e7ae a1e7 9086 e4b8 ade5 bf83  ................
+00000ed0: e4b8 ade5 8f96 e580 bc0d 0a2b 2036 292e  ...........+ 6).
+00000ee0: 6465 6d6f 5f73 6978 3a20 e5bc 82e6 ada5  demo_six: ......
+00000ef0: e5ad 98e5 85a5 204d 6f6e 676f 4442 20e7  ...... MongoDB .
+00000f00: 9a84 e59c bae6 99af 0d0a 0d0a 2d20 3729  ............- 7)
+00000f10: 2e64 656d 6f5f 7365 7665 6e3a 2073 6372  .demo_seven: scr
+00000f20: 6170 7920 5265 7175 6573 7420 e69b bfe6  apy Request ....
+00000f30: 8da2 e4b8 ba20 7265 7175 6573 7473 20e8  ..... requests .
+00000f40: afb7 e6b1 82e7 9a84 e59c bae6 99af 28e5  ..............(.
+00000f50: b7b2 e588 a0e9 99a4 e6ad a4e5 8a9f e883  ................
+00000f60: bdef bc8c e69b b4e6 8ea8 e88d 90e4 bdbf  ................
+00000f70: e794 a820 6169 6f68 7474 7020 e696 b9e5  ... aiohttp ....
+00000f80: bc8f 290d 0a2b 2038 292e 6465 6d6f 5f65  ..)..+ 8).demo_e
+00000f90: 6967 6874 3a20 e590 8ce6 97b6 e5ad 98e5  ight: ..........
+00000fa0: 85a5 204d 7973 716c 20e5 928c 204d 6f6e  .. Mysql ... Mon
+00000fb0: 676f 4442 20e7 9a84 e59c bae6 99af 0d0a  goDB ...........
+00000fc0: 2b20 3929 2e64 656d 6f5f 6169 6f68 7474  + 9).demo_aiohtt
+00000fd0: 705f 6578 616d 706c 653a 2073 6372 6170  p_example: scrap
+00000fe0: 7920 5265 7175 6573 7420 e69b bfe6 8da2  y Request ......
+00000ff0: e4b8 ba20 6169 6f68 7474 7020 e8af b7e6  ... aiohttp ....
+00001000: b182 e79a 84e5 9cba e699 af0d 0a2b 2031  .............+ 1
+00001010: 3029 2e64 656d 6f5f 6169 6f68 7474 705f  0).demo_aiohttp_
+00001020: 7465 7374 3a20 7363 7261 7079 2061 696f  test: scrapy aio
+00001030: 6874 7470 20e5 9ca8 e585 b7e4 bd93 e9a1  http ...........
+00001040: b9e7 9bae e4b8 ade7 9a84 e4bd bfe7 94a8  ................
+00001050: e696 b9e6 b395 e7a4 bae4 be8b 0d0a 0d0a  ................
+00001060: 2b20 3131 292e 6465 6d6f 5f70 726f 7879  + 11).demo_proxy
+00001070: 5f6f 6e65 3a20 e5bf abe4 bba3 e790 86e5  _one: ..........
+00001080: 8aa8 e680 81e9 9aa7 e981 93e4 bba3 e790  ................
+00001090: 86e7 a4ba e4be 8b0d 0a2b 2031 3229 2e64  .........+ 12).d
+000010a0: 656d 6f5f 7072 6f78 795f 7477 6f3a 20e6  emo_proxy_two: .
+000010b0: b58b e8af 95e5 bfab e4bb a3e7 9086 e78b  ................
+000010c0: ace4 baab e4bb a3e7 9086 0d0a 2b31 3329  ............+13)
+000010d0: 2e64 656d 6f5f 4179 7554 7572 626f 4d79  .demo_AyuTurboMy
+000010e0: 7371 6c50 6970 656c 696e 653a 206d 7973  sqlPipeline: mys
+000010f0: 716c 20e5 908c e6ad a5e8 bf9e e68e a5e6  ql .............
+00001100: b1a0 e79a 84e7 a4ba e4be 8b0d 0a2b 3134  .............+14
+00001110: 292e 6465 6d6f 5f63 7261 776c 3a20 e694  ).demo_crawl: ..
+00001120: afe6 8c81 2073 6372 6170 7920 4372 6177  .... scrapy Craw
+00001130: 6c53 7069 6465 7220 e79a 84e7 a4ba e4be  lSpider ........
+00001140: 8b0d 0a0d 0a23 20e6 9cac e5ba 93e4 b8ad  .....# .........
+00001150: e7bb 99e5 87ba e694 afe6 8c81 2049 7465  ............ Ite
+00001160: 6d20 4c6f 6164 6572 7320 e789 b9e6 80a7  m Loaders ......
+00001170: e79a 84e7 a4ba e4be 8b28 e696 87e6 a1a3  .........(......
+00001180: e59c b0e5 9d80 efbc 9a68 7474 7073 3a2f  .........https:/
+00001190: 2f61 7975 6765 7370 6964 6572 746f 6f6c  /ayugespidertool
+000011a0: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
+000011b0: 2f65 6e2f 6c61 7465 7374 2f74 6f70 6963  /en/latest/topic
+000011c0: 732f 6c6f 6164 6572 732e 6874 6d6c 290d  s/loaders.html).
+000011d0: 0a2b 3135 292e 6465 6d6f 5f69 7465 6d5f  .+15).demo_item_
+000011e0: 6c6f 6164 6572 3a20 e69c ace5 ba93 e4b8  loader: ........
+000011f0: ade4 bdbf e794 a820 4974 656d 204c 6f61  ....... Item Loa
+00001200: 6465 7273 20e7 9a84 e7a4 bae4 be8b 0d0a  ders ...........
+00001210: 2d31 3629 2e64 656d 6f5f 6974 656d 5f6c  -16).demo_item_l
+00001220: 6f61 6465 725f 7477 6f3a 20e6 ada4 e7a4  oader_two: .....
+00001230: bae4 be8b e5b7 b2e5 88a0 e999 a4ef bc8c  ................
+00001240: e58f afe6 9fa5 e79c 8be4 b88a e4b8 aa20  ............... 
+00001250: 6465 6d6f 5f69 7465 6d5f 6c6f 6164 6572  demo_item_loader
+00001260: 20e4 b8ad e79a 84e7 a4ba e4be 8bef bc8c   ...............
+00001270: e79b aee5 898d e5b7 b2e7 bb8f e58f afe4  ................
+00001280: bba5 e5be 88e6 96b9 e4be bfe7 9a84 e4bd  ................
+00001290: bfe7 94a8 2049 7465 6d20 4c6f 6164 6572  .... Item Loader
+000012a0: 7320 e58a 9fe8 83bd e4ba 860d 0a0d 0a2b  s .............+
+000012b0: 3137 292e 6465 6d6f 5f6d 6f6e 676f 5f61  17).demo_mongo_a
+000012c0: 7379 6e63 3a20 6173 796e 6369 6f20 e789  sync: asyncio ..
+000012d0: 88e6 9cac e5ad 98e5 82a8 206d 6f6e 676f  .......... mongo
+000012e0: 4442 20e7 9a84 2070 6970 656c 696e 6573  DB ... pipelines
+000012f0: 20e7 a4ba e4be 8b0d 0a2b 3138 292e 6465   ........+18).de
+00001300: 6d6f 5f6d 713a 20e6 95b0 e68d aee5 ad98  mo_mq: .........
+00001310: e585 a520 7261 6262 6974 6d71 20e7 9a84  ... rabbitmq ...
+00001320: e6a8 a1e6 9dbf e7a4 bae4 be8b 0d0a 2b31  ..............+1
+00001330: 3929 2e64 656d 6f5f 6b61 666b 613a 20e6  9).demo_kafka: .
+00001340: 95b0 e68d aee5 ad98 e585 a520 6b61 666b  ........... kafk
+00001350: 6120 e79a 84e6 a8a1 e69d bfe7 a4ba e4be  a ..............
+00001360: 8b0d 0a2b 3230 292e 6465 6d6f 5f66 696c  ...+20).demo_fil
+00001370: 653a 20e4 b88b e8bd bde5 9bbe e789 87e7  e: .............
+00001380: ad89 e696 87e4 bbb6 e588 b0e6 9cac e59c  ................
+00001390: b0e7 9a84 e6a8 a1e6 9dbf e7a4 bae4 be8b  ................
+000013a0: 0d0a 6060 600d 0a0d 0a23 2320 e8b7 91e9  ..```....## ....
+000013b0: 809a e6b5 8be8 af95 0d0a 0d0a e589 8de6  ................
+000013c0: 8f90 efbc 9ae9 9c80 e8a6 81e5 9ca8 2060  .............. `
+000013d0: 7465 7374 7360 20e7 9a84 2060 5649 5460  tests` ... `VIT`
+000013e0: 20e7 9bae e5bd 95e4 b88b e588 9be5 bbba   ...............
+000013f0: 2060 2e63 6f6e 6660 20e6 9687 e4bb b6ef   `.conf` .......
+00001400: bc8c e5b7 b2e7 bb99 e587 bae7 a4ba e4be  ................
+00001410: 8be6 9687 e4bb b6ef bc8c e8af b7e5 a1ab  ................
+00001420: e586 99e6 b58b e8af 95e6 8980 e99c 80e5  ................
+00001430: 8685 e5ae b9ef bc8c e784 b6e5 908e efbc  ................
+00001440: 9a0d 0a0d 0a2d 20e5 8faf e4bb a5e7 9bb4  .....- .........
+00001450: e68e a5e4 bdbf e794 a820 6074 6f78 6020  ......... `tox` 
+00001460: e69d a5e8 bf90 e8a1 8ce6 b58b e8af 95e3  ................
+00001470: 8082 0d0a 0d0a 2d20 e69c ace5 ba93 e4bb  ......- ........
+00001480: a520 5b70 6f65 7472 795d 2868 7474 7073  . [poetry](https
+00001490: 3a2f 2f70 7974 686f 6e2d 706f 6574 7279  ://python-poetry
+000014a0: 2e6f 7267 2f64 6f63 732f 2920 e5bc 80e5  .org/docs/) ....
+000014b0: 8f91 efbc 8ce9 82a3 e4b9 88e7 9bb4 e68e  ................
+000014c0: a5e6 96b0 e78e afe5 a283 e4b8 8be8 bf90  ................
+000014d0: e8a1 8c20 6070 6f65 7472 7920 696e 7374  ... `poetry inst
+000014e0: 616c 6c60 0d0a 2020 e590 8eef bc8c e689  all`..  ........
+000014f0: 8be5 8aa8 e8bf 90e8 a18c e79b aee6 a087  ................
+00001500: e6b5 8be8 af95 e688 9620 6070 7974 6573  ......... `pytes
+00001510: 7460 20e5 91bd e4bb a4e6 9da5 e6b5 8be8  t` .............
+00001520: af95 e7ad 89e7 9a86 e58f afe3 8082 0d0a  ................
+00001530: 2d20 e4b9 9fe5 8faf e4bb a5e4 bdbf e794  - ..............
+00001540: a820 606d 616b 6560 20e5 b7a5 e585 b7ef  . `make` .......
+00001550: bc8c 606d 616b 6520 7374 6172 7460 20e7  ..`make start` .
+00001560: 84b6 e590 8e20 606d 616b 6520 7465 7374  ..... `make test
+00001570: 6020 e58d b3e5 8faf e380 820d 0a0d 0a23  ` .............#
+00001580: 2320 e4bd a0e5 8faf e883 bde5 9ca8 e684  # ..............
+00001590: 8fe7 9a84 e4ba 8b0d 0a0d 0a31 2e20 e88b  ...........1. ..
+000015a0: a5e4 bda0 e8a7 89e5 be97 e69f 90e4 ba9b  ................
+000015b0: e59c bae6 99af e4b8 8be7 9a84 e58a 9fe8  ................
+000015c0: 83bd e5ae 9ee7 8eb0 e4b8 8de5 a4aa e7ac  ................
+000015d0: a6e5 9088 e4bd a0e7 9a84 e9a2 84e6 9c9f  ................
+000015e0: efbc 8ce6 83b3 e8a6 81e4 bfae e694 b9e6  ................
+000015f0: 8896 e6b7 bbe5 8aa0 e887 aae5 ae9a e4b9  ................
+00001600: 89e5 8a9f e883 bdef bc8c e6af 94e5 a682  ................
+00001610: e7a7 bbe9 99a4 e5af b9e4 bda0 e697 a0e7  ................
+00001620: 94a8 e6a8 a1e5 9d97 e380 81e4 bfae e694  ................
+00001630: b9e5 ba93 e590 8de7 ad89 efbc 8ce4 bda0  ................
+00001640: e58f afe4 bba5 e887 aae8 a18c e4bf aee6  ................
+00001650: 94b9 e590 8e20 6062 7569 6c64 60e3 8082  ..... `build`...
+00001660: 0d0a 322e 20e6 9cac e5ba 93e4 b8bb e68e  ..2. ...........
+00001670: a820 6073 6372 6170 7960 20e6 89a9 e5b1  . `scrapy` .....
+00001680: 95ef bc88 e58d b3e5 a29e e5bc bae7 8988  ................
+00001690: e79a 84e8 87aa e5ae 9ae4 b989 e6a8 a1e6  ................
+000016a0: 9dbf efbc 89e7 9a84 e58a 9fe8 83bd efbc  ................
+000016b0: 8ce5 9ca8 e4bd bfe7 94a8 e69c ace5 ba93  ................
+000016c0: e697 b6ef bc8c e790 86e8 aeba e4b8 8ae5  ................
+000016d0: b9b6 e4b8 8de4 bc9a e5bd b1e5 938d e4bd  ................
+000016e0: a020 6073 6372 6170 7960 0d0a 2020 20e9  . `scrapy`..   .
+000016f0: a1b9 e79b aee5 8f8a e585 b6e5 ae83 e7bb  ................
+00001700: 84e4 bbb6 e380 820d 0a33 2e20 2a2a e5bd  .........3. **..
+00001710: 93e7 84b6 efbc 8ce4 bda0 e4b9 9fe5 8faf  ................
+00001720: e4bb a5e9 8089 e68b a9e7 bb99 e6ad a4e9  ................
+00001730: a1b9 e79b aee5 819a e587 bae8 b4a1 e78c  ................
+00001740: aeef bc8c e6af 94e5 a682 e5a2 9ee5 8aa0  ................
+00001750: e688 96e4 bc98 e58c 96e6 9f90 e4ba 9be5  ................
+00001760: 8a9f e883 bde7 ad89 efbc 8ce4 bd86 e59c  ................
+00001770: a8e6 ada4 e4b9 8be5 898d e8af b7e6 8f90  ................
+00001780: e79b b8e5 85b3 e79a 8420 6049 5353 5545  ......... `ISSUE
+00001790: 5360 0d0a 2020 20e7 bb8f e7a1 aee8 aea4  S`..   .........
+000017a0: e590 8ee5 868d e5bc 80e5 8f91 e592 8ce6  ................
+000017b0: 8f90 e4ba a420 6050 554c 4c20 5245 5155  ..... `PULL REQU
+000017c0: 4553 5453 60ef bc8c e4bb a5e5 858d e4b8  ESTS`...........
+000017d0: 8de5 a4aa e7ac a6e5 9088 e69c ace5 ba93  ................
+000017e0: e59c bae6 99af e688 96e5 b7b2 e5ba 9fe5  ................
+000017f0: bc83 e7ad 89e5 8e9f e59b a0e9 80a0 e688  ................
+00001800: 90e4 bda0 e79a 84e8 b4a1 e78c aee6 b5aa  ................
+00001810: e8b4 b9ef bc8c e982 a3e5 b0b1 e5a4 aae5  ................
+00001820: 8faf e683 9ce4 ba86 efbc 812a 2a0d 0a0d  ...........**...
+00001830: 0a23 2320 e69e 84e5 bbba e4bd a0e7 9a84  .## ............
+00001840: e4b8 93e5 b19e e5ba 930d 0a0d 0a3e 20e5  .............> .
+00001850: 85b7 e4bd 93e5 8685 e5ae b9e8 afb7 e4bb  ................
+00001860: a520 5b70 6f65 7472 7920 e5ae 98e6 96b9  . [poetry ......
+00001870: e696 87e6 a1a3 5d28 6874 7470 733a 2f2f  ......](https://
+00001880: 7079 7468 6f6e 2d70 6f65 7472 792e 6f72  python-poetry.or
+00001890: 672f 646f 6373 2f29 20e4 b8ba e587 86e3  g/docs/) .......
+000018a0: 8082 0d0a 0d0a e68d ae5b e4bd a0e5 8faf  .........[......
+000018b0: e883 bde5 9ca8 e684 8fe7 9a84 e4ba 8b5d  ...............]
+000018c0: 2823 e4bd a0e5 8faf e883 bde5 9ca8 e684  (#..............
+000018d0: 8fe7 9a84 e4ba 8b29 e58f afe7 9fa5 efbc  .......)........
+000018e0: 8ce4 bda0 e58f afe4 bba5 2060 636c 6f6e  .......... `clon
+000018f0: 6560 0d0a e6ba 90e7 a081 e590 8eef bc8c  e`..............
+00001900: e4bf aee6 94b9 e4bb bbe6 848f e696 b9e6  ................
+00001910: b395 efbc 88e6 af94 e5a6 82e4 bda0 e79a  ................
+00001920: 84e9 a1b9 e79b aee5 9cba e699 afe4 b88b  ................
+00001930: e58f afe8 83bd e99c 80e8 a681 e585 b6e5  ................
+00001940: ae83 e79a 84e6 97a5 e5bf 97e9 858d e7bd  ................
+00001950: aee9 bb98 e8ae a4e5 80bc efbc 8ce6 8896  ................
+00001960: e6b7 bbe5 8aa0 e585 b6e5 ae83 e79a 84e9  ................
+00001970: a1b9 e79b aee7 bb93 e69e 84e6 a8a1 e69d  ................
+00001980: bfe7 ad89 efbc 89ef bc8c e4bf aee6 94b9  ................
+00001990: e5ae 8ce6 8890 e590 8e20 6070 6f65 7472  ......... `poetr
+000019a0: 7920 2062 7569 6c64 600d 0ae6 8896 2060  y  build`..... `
+000019b0: 6d61 6b65 2062 7569 6c64 6020 e58d b3e5  make build` ....
+000019c0: 8faf e689 93e5 8c85 e4bd bfe7 94a8 e380  ................
+000019d0: 820d 0a0d 0ae6 af94 e5a6 82e4 bda0 e58f  ................
+000019e0: afe8 83bd e99c 80e8 a681 e69b b4e6 96b0  ................
+000019f0: e4be 9de8 b596 e5ba 93e4 b8ad 2060 7079  ............ `py
+00001a00: 6d6f 6e67 6f60 20e4 b8ba e696 b0e7 8988  mongo` .........
+00001a10: e69c ac20 6078 2e78 2e78 60ef bc8c e982  ... `x.x.x`.....
+00001a20: a3e5 8faa e99c 8020 6070 6f65 7472 7920  ....... `poetry 
+00001a30: 696e 7374 616c 6c60 0d0a e5ae 89e8 a385  install`........
+00001a40: e78e b0e6 9c89 e4be 9de8 b596 e590 8eef  ................
+00001a50: bc8c e586 8d20 6070 6f65 7472 7920 6164  ..... `poetry ad
+00001a60: 6420 7079 6d6f 6e67 6f40 782e 782e 7860  d pymongo@x.x.x`
+00001a70: 20e5 ae89 e8a3 85e7 9bae e6a0 87e7 8988   ...............
+00001a80: e69c acef bc88 e5b0 bde9 878f e4b8 8de8  ................
+00001a90: a681 e4bd bfe7 94a8 2060 706f 6574 7279  ........ `poetry
+00001aa0: 2075 7064 6174 6520 7079 6d6f 6e67 6f60   update pymongo`
+00001ab0: 0d0a efbc 89ef bc8c e7a1 aee5 ae9a e6b5  ................
+00001ac0: 8be8 af95 e6ad a3e5 b8b8 e4ba 86e5 8db3  ................
+00001ad0: e58f af20 6070 6f65 7472 7920 6275 696c  ... `poetry buil
+00001ae0: 6460 20e6 8993 e58c 85e4 bdbf e794 a8e3  d` .............
+00001af0: 8082 0d0a 0d0a 2a2a e5b8 8ce6 9c9b e6ad  ......**........
+00001b00: a4e9 a1b9 e79b aee8 83bd e59c a8e4 bda0  ................
+00001b10: e981 87e5 88b0 e689 a9e5 b195 2073 6372  ............ scr
+00001b20: 6170 7920 e58a 9fe8 83bd e79a 84e5 9cba  apy ............
+00001b30: e699 afe6 97b6 e883 bde5 afb9 e4bd a0e6  ................
+00001b40: 9c89 e689 80e6 8c87 e5bc 95e3 8082 2a2a  ..............**
+00001b50: 0d0a 0d0a 2323 20e5 8a9f e883 bd0d 0a0d  ....## .........
+00001b60: 0a2d 205b 785d 2060 7363 7261 7079 6020  .- [x] `scrapy` 
+00001b70: e79a 84e6 89a9 e5b1 95e5 8a9f e883 bde5  ................
+00001b80: 9cba e699 af0d 0a20 2020 202d 205b 785d  .......    - [x]
+00001b90: 2060 7363 7261 7079 6020 e884 9ae6 9cac   `scrapy` ......
+00001ba0: e8bf 90e8 a18c e4bf a1e6 81af e7bb 9fe8  ................
+00001bb0: aea1 e592 8ce9 a1b9 e79b aee4 be9d e8b5  ................
+00001bc0: 96e8 a1a8 e987 87e9 9b86 e987 8fe7 bb9f  ................
+00001bd0: e8ae a1ef bc8c e58f afe7 94a8 e4ba 8ee6  ................
+00001be0: 97a5 e5bf 97e8 aeb0 e5bd 95e5 928c e9a2  ................
+00001bf0: 84e8 ada6 0d0a 2020 2020 2d20 5b78 5d20  ......    - [x] 
+00001c00: e887 aae5 ae9a e4b9 89e6 a8a1 e69d bfef  ................
+00001c10: bc8c e59c a820 6061 7975 6765 2073 7461  ..... `ayuge sta
+00001c20: 7274 7072 6f6a 6563 7420 3c70 726f 6a6e  rtproject <projn
+00001c30: 616d 653e 6020 e592 8c20 6061 7975 6765  ame>` ... `ayuge
+00001c40: 2067 656e 7370 6964 6572 203c 7370 6964   genspider <spid
+00001c50: 6572 6e61 6d65 3e60 20e6 97b6 e794 9fe6  ername>` .......
+00001c60: 8890 e980 82e5 9088 e69c ace5 ba93 e79a  ................
+00001c70: 84e6 a8a1 e69d bfe6 9687 e4bb b60d 0a20  ............... 
+00001c80: 2020 202d 205b 785d 207e 7ee5 a29e e58a     - [x] ~~.....
+00001c90: a0e6 a0b9 e68d ae20 606e 6163 6f73 6020  ....... `nacos` 
+00001ca0: e69d a5e8 8eb7 e58f 96e9 858d e7bd aee7  ................
+00001cb0: 9a84 e58a 9fe8 83bd 7e7e 202d 3e20 e694  ........~~ -> ..
+00001cc0: b9e4 b8ba e5a2 9ee5 8aa0 e6a0 b9e6 8dae  ................
+00001cd0: 2060 636f 6e73 756c 6020 e69d a5e8 8eb7   `consul` ......
+00001ce0: e58f 96e9 858d e7bd aee7 9a84 e58a 9fe8  ................
+00001cf0: 83bd 0d0a 2020 2020 2d20 5b78 5d20 e4bb  ....    - [x] ..
+00001d00: a3e7 9086 e4b8 ade9 97b4 e4bb b6ef bc88  ................
+00001d10: e78b ace4 baab e4bb a3e7 9086 e380 81e5  ................
+00001d20: 8aa8 e680 81e9 9aa7 e981 93e4 bba3 e790  ................
+00001d30: 86ef bc89 0d0a 2020 2020 2d20 5b78 5d20  ......    - [x] 
+00001d40: e99a 8fe6 9cba e8af b7e6 b182 e5a4 b420  ............... 
+00001d50: 6055 4160 20e4 b8ad e997 b4e4 bbb6 efbc  `UA` ...........
+00001d60: 8ce6 a0b9 e68d ae20 6066 616b 655f 7573  ....... `fake_us
+00001d70: 6572 6167 656e 7460 20e4 b8ad e79a 84e6  eragent` .......
+00001d80: 9d83 e987 8de6 9da5 e99a 8fe6 9cba 0d0a  ................
+00001d90: 2020 2020 2d20 5b78 5d20 e4bd bfe7 94a8      - [x] ......
+00001da0: e4bb a5e4 b88b e5b7 a5e5 85b7 e69d a5e6  ................
+00001db0: 9bbf e68d a220 6073 6372 6170 7960 20e7  ..... `scrapy` .
+00001dc0: 9a84 2060 5265 7175 6573 7460 20e6 9da5  .. `Request` ...
+00001dd0: e58f 91e9 8081 e8af b7e6 b182 0d0a 2020  ..............  
+00001de0: 2020 2020 2020 2d20 5b78 5d20 7e7e 6072        - [x] ~~`r
+00001df0: 6571 7565 7374 7360 3a20 e8bf 99e4 b8aa  equests`: ......
+00001e00: e4b8 8de6 8ea8 e88d 90e4 bdbf e794 a8ef  ................
+00001e10: bc8c 6072 6571 7565 7374 7360 20e5 908c  ..`requests` ...
+00001e20: e6ad a5e5 ba93 e4bc 9ae9 998d e4bd 8e20  ............... 
+00001e30: 6073 6372 6170 7960 20e8 bf90 e8a1 8ce6  `scrapy` .......
+00001e40: 9588 e78e 877e 7eef bc88 e5b7 b2e7 a7bb  .....~~.........
+00001e50: e999 a4e6 ada4 e58a 9fe8 83bd efbc 8ce6  ................
+00001e60: 9bb4 e68e a8e8 8d90 2060 6169 6f68 7474  ........ `aiohtt
+00001e70: 7060 0d0a 2020 2020 2020 2020 2020 e79a  p`..          ..
+00001e80: 84e6 96b9 e5bc 8fef bc89 0d0a 2020 2020  ............    
+00001e90: 2020 2020 2d20 5b78 5d20 6061 696f 6874      - [x] `aioht
+00001ea0: 7470 603a 20e9 9b86 e688 90e5 b086 2060  tp`: ......... `
+00001eb0: 7363 7261 7079 2052 6571 7565 7374 6020  scrapy Request` 
+00001ec0: e69b bfe6 8da2 e4b8 ba20 6061 696f 6874  ......... `aioht
+00001ed0: 7470 6020 e79a 84e5 8d8f e7a8 8be6 96b9  tp` ............
+00001ee0: e5bc 8f0d 0a20 2020 202d 205b 785d 2060  .....    - [x] `
+00001ef0: 4d79 7371 6c60 20e5 ad98 e582 a8e7 9a84  Mysql` .........
+00001f00: e59c bae6 99af e4b8 8be9 8082 e985 8d0d  ................
+00001f10: 0a20 2020 2020 2020 202d 205b 785d 20e8  .        - [x] .
+00001f20: 87aa e58a a8e5 889b e5bb ba20 604d 7973  ........... `Mys
+00001f30: 716c 6020 e794 a8e6 88b7 e59c bae6 99af  ql` ............
+00001f40: e4b8 8be9 9c80 e8a6 81e7 9a84 e695 b0e6  ................
+00001f50: 8dae e5ba 93e5 928c e695 b0e6 8dae e8a1  ................
+00001f60: a8e5 8f8a e5ad 97e6 aeb5 e6a0 bce5 bc8f  ................
+00001f70: efbc 8ce8 bf98 e69c 89e5 ad97 e6ae b5e6  ................
+00001f80: b3a8 e987 8a0d 0a20 2020 202d 205b 785d  .......    - [x]
+00001f90: 2060 4d6f 6e67 6f44 4260 20e5 ad98 e582   `MongoDB` .....
+00001fa0: a8e7 9a84 e59c bae6 99af e4b8 8be9 8082  ................
+00001fb0: e985 8def bc8c e7bc 96e5 8699 e9a3 8ee6  ................
+00001fc0: a0bc e4b8 8e20 604d 7973 716c 6020 e5ad  ..... `Mysql` ..
+00001fd0: 98e5 82a8 e7ad 89e5 9cba e699 afe4 b88b  ................
+00001fe0: e4b8 80e8 87b4 0d0a 2020 2020 2d20 5b78  ........    - [x
+00001ff0: 5d20 6061 7379 6e63 696f 6020 e8af ade6  ] `asyncio` ....
+00002000: b395 e694 afe6 8c81 e4b8 8e20 6061 7379  ........... `asy
+00002010: 6e63 6020 e7ac ace4 b889 e696 b9e5 ba93  nc` ............
+00002020: e694 afe6 8c81 e7a4 bae4 be8b 0d0a 2020  ..............  
+00002030: 2020 2020 2020 2d20 5b78 5d20 6073 7069        - [x] `spi
+00002040: 6465 7260 20e4 b8ad e4bd bfe7 94a8 2060  der` ......... `
+00002050: 6173 796e 6369 6f60 20e7 9a84 2060 6169  asyncio` ... `ai
+00002060: 6f68 7474 7060 20e7 a4ba e4be 8b0d 0a20  ohttp` ........ 
+00002070: 2020 2020 2020 202d 205b 785d 2060 7069         - [x] `pi
+00002080: 7065 6c69 6e65 6020 e4b8 ade4 bdbf e794  peline` ........
+00002090: a820 6061 7379 6e63 696f 6020 e79a 8420  . `asyncio` ... 
+000020a0: 6061 696f 4d79 7371 6c60 20e7 a4ba e4be  `aioMysql` .....
+000020b0: 8b0d 0a20 2020 202d 205b 785d 20e9 9b86  ...    - [x] ...
+000020c0: e688 9020 604b 6166 6b61 60ef bc8c 6052  ... `Kafka`...`R
+000020d0: 6162 6269 744d 5160 20e7 ad89 e695 b0e6  abbitMQ` .......
+000020e0: 8dae e68e a8e9 8081 e58a 9fe8 83bd 0d0a  ................
+000020f0: 2d20 5b78 5d20 e5b8 b8e7 94a8 e5bc 80e5  - [x] ..........
+00002100: 8f91 e59c bae6 99af 0d0a 2020 2020 2d20  ..........    - 
+00002110: 5b78 5d20 6073 716c 6020 e8af ade5 8fa5  [x] `sql` ......
+00002120: e68b bce6 8ea5 efbc 8ce5 8faa e698 afe7  ................
+00002130: ae80 e58d 95e5 9cba e699 afef bc8c e590  ................
+00002140: 8ee7 bbad e4bc 98e5 8c96 e380 82e5 b7b2  ................
+00002150: e7bb 99e5 87ba e4bc 98e5 8c96 e696 b9e5  ................
+00002160: 9091 efbc 8ce5 8f82 e880 83e5 ba93 e7ad  ................
+00002170: 89e4 bfa1 e681 afe3 8082 0d0a 2020 2020  ............    
+00002180: 2d20 5b78 5d20 606d 6f6e 676f 4442 6020  - [x] `mongoDB` 
+00002190: e8af ade5 8fa5 e68b bce6 8ea5 0d0a 2020  ..............  
+000021a0: 2020 2d20 5b78 5d20 e695 b0e6 8dae e6a0    - [x] ........
+000021b0: bce5 bc8f e58c 96e5 a484 e790 86ef bc8c  ................
+000021c0: e6af 94e5 a682 efbc 9ae5 8ebb e999 a4e7  ................
+000021d0: bd91 e9a1 b5e6 a087 e7ad beef bc8c e58e  ................
+000021e0: bbe9 99a4 e697 a0e6 9588 e7a9 bae6 a0bc  ................
+000021f0: e7ad 890d 0a20 2020 202d 205b 785d 20e5  .....    - [x] .
+00002200: ad97 e4bd 93e5 8f8d e788 ace8 bf98 e58e  ................
+00002210: 9fe6 96b9 e6b3 950d 0a20 2020 2020 2020  .........       
+00002220: 202d 205b 785d 20e5 9fba e4ba 8e20 6074   - [x] ...... `t
+00002230: 7466 60ef bc8c 6077 6f66 6660 20e4 b98b  tf`...`woff` ...
+00002240: e7b1 bbe7 9a84 e5ad 97e4 bd93 e696 87e4  ................
+00002250: bbb6 e698 a0e5 b084 efbc 8ce6 8896 e7bb  ................
+00002260: 93e5 9088 2060 6373 7360 20e7 ad89 e5ae  .... `css` .....
+00002270: 9ee7 8eb0 0d0a 2020 2020 2020 2020 2020  ......          
+00002280: 2020 2d20 5b78 5d20 e58f afe4 bba5 e79b    - [x] ........
+00002290: b4e6 8ea5 e59c a8e5 ad97 e4bd 93e6 9687  ................
+000022a0: e4bb b620 6078 6d6c 600d 0a20 2020 2020  ... `xml`..     
+000022b0: 2020 2020 2020 2020 20e4 b8ad e689 bee5           .......
+000022c0: 88b0 e698 a0e5 b084 e585 b3e7 b3bb e79a  ................
+000022d0: 84ef bc9a e4bd bfe7 94a8 205b 666f 6e74  .......... [font
+000022e0: 666f 7267 655d 2868 7474 7073 3a2f 2f67  forge](https://g
+000022f0: 6974 6875 622e 636f 6d2f 666f 6e74 666f  ithub.com/fontfo
+00002300: 7267 652f 666f 6e74 666f 7267 652f 7265  rge/fontforge/re
+00002310: 6c65 6173 6573 2920 e5b7 a5e5 85b7 e5af  leases) ........
+00002320: bce5 87ba e698 a0e5 b084 e58d b3e5 8faf  ................
+00002330: e380 820d 0a20 2020 2020 2020 2020 2020  .....           
+00002340: 202d 205b 785d 20e6 97a0 e6b3 95e6 89be   - [x] .........
+00002350: e588 b0e6 98a0 e5b0 84e5 85b3 e7b3 bbe7  ................
+00002360: 9a84 efbc 8ce5 8899 e4b8 80e8 88ac e4bd  ................
+00002370: bfe7 94a8 2060 6f63 7260 20e8 af86 e588  .... `ocr` .....
+00002380: abef bc88 e587 86e7 a1ae e78e 87e9 9d9e  ................
+00002390: e799 bee5 8886 e799 beef bc89 efbc 8ce9  ................
+000023a0: 809a e8bf 8720 6066 6f6e 7466 6f72 6765  ..... `fontforge
+000023b0: 6020 e5af bce5 87ba e6af 8fe4 b8aa e698  ` ..............
+000023c0: a0e5 b084 e79a 8420 6070 6e67 600d 0a20  ....... `png`.. 
+000023d0: 2020 2020 2020 2020 2020 2020 20ef bc8c               ...
+000023e0: e590 8ee5 868d e980 9ae8 bf87 e590 84e7  ................
+000023f0: a78d e696 b9e5 bc8f e8af 86e5 88ab e380  ................
+00002400: 820d 0a20 2020 202d 205b 785d 2060 6874  ...    - [x] `ht
+00002410: 6d6c 6020 e695 b0e6 8dae e5a4 84e7 9086  ml` ............
+00002420: efbc 8ce5 8ebb e999 a4e6 a087 e7ad beef  ................
+00002430: bc8c e4b8 8de5 8faf e8a7 81e5 ad97 e7ac  ................
+00002440: a6ef bc8c e789 b9e6 ae8a e5ad 97e7 aca6  ................
+00002450: e694 b9e6 8890 e6ad a3e5 b8b8 e698 bee7  ................
+00002460: a4ba e7ad 890d 0a20 2020 202d 205b 785d  .......    - [x]
+00002470: 20e6 b7bb e58a a0e5 b8b8 e794 a8e7 9a84   ...............
+00002480: e59b bee7 8987 e9aa 8ce8 af81 e7a0 81e4  ................
+00002490: b8ad e79a 84e5 a484 e790 86e6 96b9 e6b3  ................
+000024a0: 950d 0a20 2020 2020 2020 202d 205b 785d  ...        - [x]
+000024b0: 20e6 bb91 e59d 97e7 bcba e58f a3e8 b79d   ...............
+000024c0: e7a6 bbe7 9a84 e8af 86e5 88ab e696 b9e6  ................
+000024d0: b395 efbc 88e5 a49a e7a7 8de5 ae9e e78e  ................
+000024e0: b0e6 96b9 e5bc 8fef bc89 0d0a 2020 2020  ............    
+000024f0: 2020 2020 2d20 5b78 5d20 e6a0 b9e6 8dae      - [x] ......
+00002500: e6bb 91e5 9d97 e8b7 9de7 a6bb e794 9fe6  ................
+00002510: 8890 e8bd a8e8 bfb9 e695 b0e7 bb84 e79a  ................
+00002520: 84e6 96b9 e6b3 950d 0a20 2020 2020 2020  .........       
+00002530: 202d 205b 785d 20e8 af86 e588 abe7 82b9   - [x] .........
+00002540: e980 89e9 aa8c e8af 81e7 a081 e4bd 8de7  ................
+00002550: bdae e58f 8ae7 82b9 e587 bbe9 a1ba e5ba  ................
+00002560: 8fef bc8c e8af 86e5 88ab e7bb 93e6 9e9c  ................
+00002570: e4b8 8de5 a4aa e5a5 bdef bc8c e5be 85e4  ................
+00002580: bc98 e58c 960d 0a20 2020 2020 2020 202d  .......        -
+00002590: 205b 785d 20e5 9bbe e789 87e4 b9b1 e5ba   [x] ...........
+000025a0: 8fe6 b7b7 e6b7 86e7 9a84 e8bf 98e5 8e9f  ................
+000025b0: e696 b9e6 b395 e7a4 bae4 be8b 0d0a 0d0a  ................
+000025c0: e6b3 a8e6 848f efbc 9ae5 8a9f e883 bde6  ................
+000025d0: bc94 e7a4 bae6 8891 e5b0 86e6 94be e585  ................
+000025e0: a520 5b72 6561 6474 6865 646f 6373 5d28  . [readthedocs](
+000025f0: 6874 7470 733a 2f2f 6179 7567 6573 7069  https://ayugespi
+00002600: 6465 7274 6f6f 6c73 2e72 6561 6474 6865  dertools.readthe
+00002610: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00002620: 742f 2920 e696 87e6 a1a3 e4b8 adef bc8c  t/) ............
+00002630: e4bb a5e9 98b2 e6ad a4e9 83a8 e588 86e5  ................
+00002640: 8685 e5ae b9e8 bf87 e5a4 9ae3 8082 0d0a  ................
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.3.2/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/encryption.py` & `ayugespidertools-3.3.2/ayugespidertools/common/encryption.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,36 @@
 
 __all__ = [
     "EncryptOperation",
 ]
 
 
 class EncryptOperation:
-    """
-    普通加密方法
-    """
+    """普通加密方法"""
 
     @classmethod
     def md5(cls, encrypt_data: str) -> str:
-        """
-        md5 处理方法
+        """md5 处理方法
+
         Args:
             encrypt_data: 需要 md5 处理的参数
 
         Returns:
             1): md5 处理后的参数
         """
         hl = hashlib.md5()
         hl.update(encrypt_data.encode(encoding="utf-8"))
         return hl.hexdigest()
 
     @classmethod
     def base64_encode(
         cls, encode_data: Union[bytes, str], url_safe: bool = False
     ) -> str:
-        """
-        base64 编码
+        """base64 编码
+
         Args:
             encode_data: 需要 base64 编码的参数
             url_safe: 标准的 Base64 编码后可能出现字符 + 和 /，在 url 中就不能直接作为参数。是否要处理此情况
 
         Returns:
             1). base64 编码后的结果
         """
@@ -48,31 +46,31 @@
             encode_data = bytes(encode_data, encoding="utf-8")
         if url_safe:
             return str(base64.urlsafe_b64encode(encode_data), encoding="utf-8")
         return str(base64.b64encode(encode_data), encoding="utf-8")
 
     @classmethod
     def base64_decode(cls, decode_data: str, url_safe: bool = False) -> str:
-        """
-        base64 解码
+        """base64 解码
+
         Args:
             decode_data: 需要 base64 解码的参数
             url_safe: 标准的 Base64 编码后可能出现字符 + 和 /，在 url 中就不能直接作为参数。是否要处理此情况
 
         Returns:
             1). base64 解码后的结果
         """
         if url_safe:
             return str(base64.urlsafe_b64decode(decode_data), encoding="utf-8")
         return str(base64.b64decode(decode_data), encoding="utf-8")
 
     @staticmethod
     def rsa_encrypt(rsa_public_key: str, encode_data: str) -> str:
-        """
-        rsa encode example
+        """rsa encode example
+
         Args:
             rsa_public_key: rsa publickey
             encode_data: rsa encode data
 
         Returns:
             1). rsa encrypted result
         """
@@ -84,30 +82,30 @@
         a = bytes(encode_data, encoding="utf8")
         rsa_key = RSA.importKey(public_key)
         cipher = Cipher_pkcsl_v1_5.new(rsa_key)
         return str(base64.b64encode(cipher.encrypt(a)), encoding="utf-8")
 
     @staticmethod
     def mm3_hash128_encode(encode_data: str) -> str:
-        """
-        MurmurHash3 非加密哈希之 hash128
+        """MurmurHash3 非加密哈希之 hash128
+
         Args:
             encode_data: 需要 mmh3 hash128 的参数
 
         Returns:
             1). mmh3 hash128 后的结果
         """
         o = mmh3.hash128(encode_data)
         hash128_encoded = hex(((o & 0xFFFFFFFFFFFFFFFF) << 64) + (o >> 64))
         return hash128_encoded[2:]
 
     @staticmethod
     def uni_to_chr(uni: str) -> str:
-        """
-        将 Unicode 码位表示的字符串转换正常的字符，用于获取字体映射时使用
+        """将 Unicode 码位表示的字符串转换正常的字符，用于获取字体映射时使用
+
         Args:
             uni: 需要转换的 unicode 字符串，
                 如：006A，但它可能是非标准的，可能需要去掉前面的 0x 或 uni。
 
         Returns:
             1). 转换后的字符
         """
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/expend.py` & `ayugespidertools-3.3.2/ayugespidertools/common/expend.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 
 __all__ = [
     "MysqlPipeEnhanceMixin",
 ]
 
 
 class MysqlPipeEnhanceMixin:
-    """
-    用于扩展 pipelines 中的功能，作为 Mixin 使用，不要对其实例化和单独使用等
-    """
+    """扩展 pipelines 的功能，作为 Mixin 使用，不要对其实例化或单独使用"""
 
     @retry(
         stop_max_attempt_number=Param.retry_num,
         wait_random_min=Param.retry_time_min,
         wait_random_max=Param.retry_time_max,
     )
     def _connect(
         self,
         mysql_conf: MysqlConf,
     ) -> pymysql.connections.Connection:
-        """
-        链接数据库操作：
+        """链接数据库操作：
             1.如果链接正常，则返回链接句柄；
             2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
+
         Args:
             mysql_conf: pymysql 链接所需的参数
 
         Returns:
             1).pymysql.connections.Connection, 链接句柄
         """
         try:
@@ -61,31 +59,31 @@
             host=mysql_conf.host,
             port=mysql_conf.port,
             database=mysql_conf.database,
             charset=mysql_conf.charset,
         )
 
     def _get_sql_by_item(self, table: str, item: dict) -> str:
-        """
-        根据处理后的 item 生成 sql 插入语句
+        """根据处理后的 item 生成 sql 插入语句
+
         Args:
             table: 数据库表名
             item: 处理后的 item
 
         Returns:
             1). sql 插入语句
         """
         keys = f"""`{"`, `".join(item.keys())}`"""
         values = ", ".join(["%s"] * len(item))
         update = ",".join([f" `{key}` = %s" for key in item])
         return f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
 
     def _get_log_by_spider(self, spider, crawl_time):
-        """
-        获取 spider 的运行日志情况
+        """获取 spider 的运行日志情况
+
         Args:
             spider: scrapy spider
             crawl_time: 爬取时间
 
         Returns:
             log_info: 日志信息
         """
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.3.2/ayugespidertools/common/mongodbpipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,22 @@
     "TwistedAsynchronous",
     "AsyncioAsynchronous",
     "mongodb_pipe",
 ]
 
 
 class AbstractClass(ABC):
-    """
-    用于处理 mongodb pipeline 存储的模板方法类
-    """
+    """用于处理 mongodb pipeline 存储的模板方法类"""
 
     def _get_insert_data(
         self,
         item_dict: Union[ItemAdapter, dict],
     ) -> dict:
-        """
-        获取要插入的数据，将 item 中的存储数据提取出来
+        """获取要插入的数据，将 item 中的存储数据提取出来
+
         Args:
             item_dict: item ItemAdapter 或者 dict 格式数据，可像字典一样操作
 
         Returns:
             None
         """
         insert_data = ReuseOperation.get_items_except_keys(
@@ -43,16 +41,16 @@
         return insert_data
 
     def process_item_template(
         self,
         item_dict: Union[ItemAdapter, dict],
         db: Param.PymongoDataBase,
     ) -> None:
-        """
-        模板方法，用于处理 mongodb pipeline 存储的模板方法类
+        """模板方法，用于处理 mongodb pipeline 存储的模板方法类
+
         Args:
             item_dict: item ItemAdapter 或 dict 格式数据
             db: mongodb 数据库连接
 
         Returns:
             None
         """
@@ -70,16 +68,16 @@
         db: Param.PymongoDataBase,
         item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
         *args,
         **kwargs,
     ) -> None:
-        """
-        数据存储逻辑，需要子类实现
+        """数据存储逻辑，需要子类实现
+
         Args:
             db: mongodb 数据库连接
             item_dict: item ItemAdapter 或 dict 格式数据
             collection_name: 集合名称
             insert_data: 要插入的数据
             *args: 可变参数
             **kwargs:关键字参数
@@ -87,17 +85,15 @@
         Returns:
             None
         """
         pass
 
 
 class Synchronize(AbstractClass):
-    """
-    pipeline 同步执行 mongodb 存储的场景
-    """
+    """pipeline 同步执行 mongodb 存储的场景"""
 
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
         item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
@@ -110,17 +106,15 @@
         else:
             db[collection_name].update(
                 item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
 
 class TwistedAsynchronous(AbstractClass):
-    """
-    pipeline twisted 异步执行 mongodb 存储的场景
-    """
+    """pipeline twisted 异步执行 mongodb 存储的场景"""
 
     def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
         item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
@@ -132,17 +126,15 @@
         else:
             db[collection_name].update(
                 item_dict["_mongo_update_rule"], {"$set": insert_data}, True
             )
 
 
 class AsyncioAsynchronous(AbstractClass):
-    """
-    pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现
-    """
+    """pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现"""
 
     async def _data_storage_logic(
         self,
         db: Param.PymongoDataBase,
         item_dict: Union[ItemAdapter, dict],
         collection_name: str,
         insert_data: dict,
@@ -171,11 +163,9 @@
 
 
 def mongodb_pipe(
     abstract_class: AbstractClass,
     item_dict: Union[ItemAdapter, dict],
     db: Param.PymongoDataBase,
 ) -> None:
-    """
-    mongodb pipeline 存储的通用调用方法
-    """
+    """mongodb pipeline 存储的通用调用方法"""
     abstract_class.process_item_template(item_dict=item_dict, db=db)
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.3.2/ayugespidertools/common/multiplexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,32 @@
 
 __all__ = [
     "ReuseOperation",
 ]
 
 
 class ReuseOperation:
-    """
-    用于存放经常复用的一些操作
-    """
+    """用于存放经常复用的一些操作"""
 
     @staticmethod
     def as_deferred(f):
-        """
-        transform a Twisted Deferred to an Asyncio Future
+        """transform a Twisted Deferred to an Asyncio Future
+
         Args:
             f: async function
 
         Returns:
-            1).Deferred
+            1). Deferred
         """
         return Deferred.fromFuture(asyncio.ensure_future(f))
 
     @staticmethod
     def get_conf_by_settings(vit_dir: str, inner_settings: Settings) -> Settings:
-        """
-        通过 settings 获取所需配置，并将其添加到 inner_settings 中
+        """通过 settings 获取所需配置，并将其添加到 inner_settings 中
+
         Args:
             vit_dir: 配置文件所在的目录
             inner_settings: scrapy 的 inner_settings
 
         Returns:
             inner_settings: 本库所需的配置
         """
@@ -140,70 +138,56 @@
         }
         return inner_settings
 
     @staticmethod
     def item_to_dict(
         item: Union[AyuItem, ScrapyItem, dict]
     ) -> Union[ItemAdapter, dict]:
-        """
-        将 item 转换为 dict 类型
+        """将 item 转换为 dict 类型；
         将 spider 中的 yield 的 item 转换为 dict 类型，方便后续处理
+
         Args:
             item: spider 中的 yield 的 item
 
         Returns:
             1). dict 类型的 item
         """
         return item.asdict() if isinstance(item, AyuItem) else ItemAdapter(item)
 
     @staticmethod
     def is_namedtuple_instance(x: Any) -> bool:
-        """
-        判断 x 是否为 namedtuple 类型
+        """判断 x 是否为 namedtuple 类型
+
         Args:
             x: 需要判断的参数
 
         Returns:
             1). 是否符合 namedtuple 类型
         """
         return isinstance(x, tuple) and hasattr(x, "_fields")
 
     @staticmethod
     def get_files_from_path(path: str) -> list:
-        """
-        获取 path 文件夹下的所有文件，而且输出以 path 为根目录的相对路径
+        """获取 path 文件夹下的所有文件，并输出以 path 为根目录的相对路径
+
         Args:
             path: 需要判断的文件夹路径
 
         Returns:
             1). path 文件夹下的文件列表
         """
         return [f.path for f in os.scandir(path) if f.is_file()]
 
     @staticmethod
-    def get_bytes_by_file(file_path: str) -> bytes:
-        """
-        获取媒体文件的 bytes 内容
-        Args:
-            file_path: 对应文件的路径
-
-        Returns:
-            file_bytes: file_path 对应文件的 bytes 内容
-        """
-        with open(file_path, "rb") as f:
-            file_bytes = f.read()
-        return file_bytes
-
-    @staticmethod
     def read_image_data(
         bg: Union[bytes, str],
         tp: Union[bytes, str],
     ) -> (np.ndarray, np.ndarray):
-        """
-        用 opencv 读取图片数据
+        """用 opencv 读取图片数据
+
         Args:
             bg: 背景图片信息
             tp: 滑块图
 
         Returns:
             bg_cv: opencv 读取背景图片的数据
             tp_cv: opencv 读取滑块图片的数据
@@ -224,16 +208,16 @@
         else:
             # 0 表示采用黑白的方式读取图片
             tp_cv = cv2.imread(tp, 0)
         return bg_cv, tp_cv
 
     @staticmethod
     def random_weight(weight_data: list):
-        """
-        带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
+        """带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
+
         Args:
             weight_data: 带权重的列表信息，示例：
                 [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
 
         Returns:
             ret: 返回当前权重列表 account_arr 中的一个值
         """
@@ -249,16 +233,16 @@
             if ra <= curr_sum:
                 ret = data
                 break
         return ret
 
     @classmethod
     def is_dict_meet_min_limit(cls, dict_conf: dict, key_list: List[str]) -> bool:
-        """
-        判断 dict_conf 是否满足 key_list 中的 key 值限定
+        """判断 dict_conf 是否满足 key_list 中的 key 值限定
+
         Args:
             dict_conf: 需要判断的参数
             key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
 
         Returns:
             1). 是否满足 key 值限制
         """
@@ -269,16 +253,16 @@
 
     @classmethod
     def get_items_by_keys(
         cls,
         dict_conf: dict,
         keys: List[str],
     ) -> dict:
-        """
-        获取 dict_conf 中的含有 keys 的 key 的字段
+        """获取 dict_conf 中的含有 keys 的 key 的字段
+
         Args:
             dict_conf: 需要处理的参数
             keys: 需要取的 key 值列表
 
         Returns:
             1). 取值后的 dict，或不满足请求的 False 值
         """
@@ -287,35 +271,32 @@
             {k: dict_conf[k] for k in keys}
             if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=keys)
             else {}
         )
 
     @classmethod
     def get_items_except_keys(cls, dict_conf, keys: List[str]) -> dict:
-        """
-        获取 dict_conf 中的不含有 keys 的 key 的字段
+        """获取 dict_conf 中的不含有 keys 的 key 的字段
+
         Args:
             dict_conf: 需要处理的参数
             keys: 需要排除的 key 值列表
 
         Returns:
             1). dict_conf 排除 keys 中的键值后的值
         """
         return {k: dict_conf[k] for k in dict_conf if k not in keys}
 
     @classmethod
     def create_database(cls, mysql_conf: MysqlConf) -> None:
-        """
-        创建数据库
-        由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
+        """创建数据库：由于这是在连接数据库，报数据库不存在错误时的场景，则需要
+        新建(不指定数据库)连接创建好所需数据库即可
+
         Args:
             mysql_conf: pymysql 的数据库连接配置
-
-        Returns:
-            None
         """
         conn = pymysql.connect(
             user=mysql_conf.user,
             password=mysql_conf.password,
             host=mysql_conf.host,
             port=mysql_conf.port,
             charset=mysql_conf.charset,
@@ -327,16 +308,16 @@
         conn.close()
         logger.info(
             f"创建数据库 {mysql_conf.database} 成功，其 charset 类型是：{mysql_conf.charset}!"
         )
 
     @classmethod
     def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
-        """
-        将 dict 中 str 类型的 key 值变成小写
+        """将 dict 中 str 类型的 key 值变成小写
+
         Args:
             deal_dict: 需要处理的 dict
 
         Returns:
             1).处理后的 dict 值
         """
         key_to_lower_dict = {}
@@ -350,16 +331,16 @@
                 key_to_lower_dict[key.lower()] = value
             else:
                 key_to_lower_dict[key] = value
         return key_to_lower_dict
 
     @classmethod
     def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
-        """
-        将 dict 中 str 类型的 key 值变成大写
+        """将 dict 中 str 类型的 key 值变成大写
+
         Args:
             deal_dict: 需要处理的 dict
 
         Returns:
             1).处理后的 dict 值
         """
         key_to_upper_dict = {}
@@ -373,51 +354,51 @@
                 key_to_upper_dict[key.upper()] = value
             else:
                 key_to_upper_dict[key] = value
         return key_to_upper_dict
 
     @classmethod
     def get_consul_conf(cls, settings: Settings) -> dict:
-        """
-        获取项目中的 consul 配置，且要根据项目整体情况来取出满足最少要求的 consul 配置
+        """获取项目中的 consul 配置，且要根据项目整体情况来取出满足最少要求的 consul 配置
+
         Args:
             settings: scrapy 的 settings 信息
 
         Returns:
-            consul_conf_dict_min: 满足要求的最少要求的 consul 配置
+            1). 满足最少要求的 consul 配置
         """
         consul_conf_dict = settings.get("CONSUL_CONFIG", {})
         return cls.get_items_by_keys(
             dict_conf=consul_conf_dict, keys=["token", "url", "format"]
         )
 
     @classmethod
     def judge_str_is_json(cls, judge_str: str) -> bool:
-        """
-        判断字符串是否为 json 格式
+        """判断字符串是否为 json 格式
+
         Args:
             judge_str: 需要判断的字符串
 
         Returns:
-            1）.是否为 json 格式
+            1). 是否为 json 格式
         """
         if not isinstance(judge_str, str):
             return False
 
         try:
             json.loads(judge_str)
         except Exception:
             return False
         else:
             return True
 
     @staticmethod
     def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
-        """
-        从 headers 中的 ck str 格式转化为 dict 格式
+        """从 headers 中的 ck str 格式转化为 dict 格式
+
         Args:
             headers_ck_str: request headers ck 的 str 格式
 
         Returns:
             1). 转化 dict 格式后的 ck
         """
         # 也可以这样写，但不推荐
@@ -425,48 +406,48 @@
         return {
             x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
             for x in headers_ck_str.split(";")
         }
 
     @staticmethod
     def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
-        """
-        将 scrapy 请求中的 body 对象转为 dict 格式
+        """将 scrapy 请求中的 body 对象转为 dict 格式
+
         Args:
             req_body_data_str: scrapy 中的 body 参数
 
         Returns:
             1). 转化 dict 格式后的 body
         """
         return {
             x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
         }
 
     @staticmethod
     def get_array_dimension(array: Union[frozenset, list, set, tuple]) -> int:
-        """
-        获取 array 的维度
+        """获取 array 的维度
+
         Args:
             array: 数组
 
         Returns:
-            1).层级数
+            1). 层级数
         """
         # 其实直接返回 len(array) 即可
         return len(np.array(array).shape)
 
     @classmethod
     def get_array_depth(cls, array: list) -> int:
-        """
-        获取 array 的最大层级，深度
+        """获取 array 的最大层级，深度
+
         Args:
             array: 数组
 
         Returns:
-            1).最大层级，深度
+            1). 最大层级，深度
         """
 
         """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
         # 先判断是否为数组类型的元素
         judge_array = isinstance(
             array,
             (
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.3.2/ayugespidertools/common/mysqlerrhandle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,390 +1,371 @@
-import re
-from abc import ABC, abstractmethod
-from typing import Optional, Type, Union
-
-from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import TableEnumTypeVar
-from ayugespidertools.config import logger
-
-__all__ = [
-    "Synchronize",
-    "TwistedAsynchronous",
-    "deal_mysql_err",
-]
-
-
-class AbstractClass(ABC):
-    """
-    用于处理 mysql 异常的模板方法类
-    """
-
-    def _create_table(
-        self,
-        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-        table_name: str,
-        charset: str,
-        collate: str,
-        table_notes: str = "",
-        demand_code: str = "",
-    ) -> None:
-        """
-        创建数据库表
-        Args:
-            cursor: mysql connect cursor，参数选择有：
-                1). 类型为 pymysql.cursors.Cursor，在同步 pipelines 中使用；
-                2). dbpool.runInteraction() 方法会将数据库连接的游标对象作为参数传入
-                回调函数中，而游标对象的类型可能是不同的，比如 DictCursor 或 Cursor 类型，在
-                异步 pipelines 中使用；
-            table_name: 创建表的名称
-            charset: charset
-            collate: collate
-            table_notes: 创建表的注释
-            demand_code: 创建表的需求对应的 code 值，用于和需求中的任务对应
-
-        Returns:
-            None
-        """
-        # 用于表格 comment 的参数生成(即 table_notes 参数)
-        if demand_code != "":
-            table_notes = f"{demand_code}_{table_notes}"
-
-        sql = f"""
-        CREATE TABLE IF NOT EXISTS `{table_name}`
-        (`id` int(32) NOT NULL AUTO_INCREMENT COMMENT 'id', PRIMARY KEY (`id`))
-        ENGINE=InnoDB DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{table_notes}';
-        """
-
-        try:
-            # 执行 sql 查询，获取数据
-            data = cursor.execute(sql)
-            if any([data == 0, not data]):
-                logger.info(f"创建数据表 {table_notes}: {table_name} 成功！")
-
-        except Exception as e:
-            logger.error(
-                f"创建表失败，table_notes：{table_notes}，table_name：{table_name}，error：{e}"
-            )
-
-    def _get_column_type(
-        self,
-        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-        database: str,
-        table: str,
-        column: str,
-    ) -> str:
-        """
-        获取数据字段存储类型
-        Args:
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            column: 字段名称
-
-        Returns:
-            column_type: 字段存储类型
-        """
-        sql = f"""
-        select COLUMN_TYPE from information_schema.columns
-        where table_schema = '{database}' and table_name = '{table}' and COLUMN_NAME= '{column}';
-        """
-        column_type = None
-        try:
-            if _ := cursor.execute(sql):
-                lines = cursor.fetchall()
-                if isinstance(lines, list):
-                    # 注意，此处 AyuMysqlPipeline 返回的结构示例为：[{'COLUMN_TYPE': 'varchar(190)'}]
-                    column_type = lines[0]["COLUMN_TYPE"] if len(lines) == 1 else ""
-                else:
-                    # 注意，此处 AyuTwistedMysqlPipeline 返回的结构示例为：(('varchar(10)',),)
-                    column_type = lines[0][0] if len(lines) == 1 else ""
-
-        except Exception as e:
-            logger.error(f"{e}")
-        return column_type
-
-    def template_method(
-        self,
-        err_msg: str,
-        conn: Param.PymysqlConnect,
-        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-        charset: str,
-        collate: str,
-        database: str,
-        table: str,
-        table_enum: Type[TableEnumTypeVar],
-        note_dic: dict,
-    ) -> None:
-        """
-        模板方法，用于处理 mysql 存储场景的异常
-        Args:
-            err_msg: pipeline 存储时报错内容
-            conn: mysql conn
-            cursor: mysql connect cursor
-            charset: mysql table charset
-            collate: mysql table collate
-            database: 数据库
-            table: 数据表
-            table_enum: 数据表枚举类
-            note_dic: 当前表字段注释
-
-        Returns:
-            None
-        """
-        if "1054" in err_msg:
-            sql, possible_err = self.deal_1054_error(
-                err_msg=err_msg, table=table, note_dic=note_dic
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        elif "1146" in err_msg:
-            table_name, table_notes, demand_code = self.deal_1146_error(
-                err_msg=err_msg,
-                table_enum=table_enum,
-            )
-            self._create_table(
-                cursor=cursor,
-                table_name=table_name,
-                charset=charset,
-                collate=collate,
-                table_notes=table_notes,
-                demand_code=demand_code,
-            )
-
-        elif "1406" in err_msg:
-            sql, possible_err = self.deal_1406_error(
-                err_msg=err_msg,
-                cursor=cursor,
-                database=database,
-                table=table,
-                note_dic=note_dic,
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        elif "1265" in err_msg:
-            sql, possible_err = self.deal_1265_error(
-                err_msg=err_msg,
-                cursor=cursor,
-                database=database,
-                table=table,
-                note_dic=note_dic,
-            )
-            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
-
-        else:
-            # 碰到其他的异常才打印错误日志，已处理的异常不打印
-            logger.error(f"ERROR: {err_msg}")
-
-    def deal_1054_error(self, err_msg: str, table: str, note_dic: dict) -> (str, str):
-        """
-        解决 1054, u"Unknown column 'id' in 'field list'"
-        Args:
-            err_msg: 报错内容
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            1). sql: 用于添加字段的 sql 语句
-            2). 执行此 sql 可能会报错的信息
-        """
-        colum_pattern = re.compile(r"Unknown column '(.*?)' in 'field list'")
-        text = re.findall(colum_pattern, err_msg)
-        colum = text[0]
-        notes = note_dic[colum]
-
-        if colum == "url":
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` TEXT(500) NULL COMMENT '{notes}';"
-        elif colum in {"create_time", "crawl_time", "update_time"}:
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` DATE NULL DEFAULT NULL COMMENT '{notes}';"
-        else:
-            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(190) NULL DEFAULT '' COMMENT '{notes}';"
-        return sql, f"1054: 添加字段 {colum} 已存在"
-
-    def deal_1146_error(
-        self,
-        err_msg: str,
-        table_enum: Type[TableEnumTypeVar],
-    ) -> (str, str, str):
-        """
-        解决 1146, u"Table '(.*?)' doesn't exist"
-        Args:
-            err_msg: 报错内容
-            table_enum: 数据表的枚举信息
-
-        Returns:
-            1). table_name: 数据表名
-            2). table_notes: 数据表注释
-            3). demand_code: 数据表对应的需求 code
-        """
-        table_pattern = re.compile(r"Table '(.*?)' doesn't exist")
-        text = re.findall(table_pattern, err_msg)
-        table = text[0].split(".")[1]
-
-        # 写入表枚举
-        if table_enum:
-            for _, member in table_enum.__members__.items():
-                table_name = member.value.get("value", "")
-                table_notes = member.value.get("notes", "")
-                demand_code = member.value.get("demand_code", "")
-                if table_name == table:
-                    return table_name, table_notes, demand_code
-        else:
-            # 未定义 Tabel_Enum 则建表
-            logger.info("未定义数据库表枚举 Tabel_Enum 参数，进行创表操作")
-        # 1.未定义 Tabel_Enum 和 2.正则未匹配到当前的 table_name 时都以此报错 table 名为准
-        return table, "", ""
-
-    def deal_1406_error(
-        self,
-        err_msg: str,
-        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-        database: str,
-        table: str,
-        note_dic: dict,
-    ) -> (str, str):
-        """
-        解决 1406, u"Data too long for ..."
-        Args:
-            err_msg: 报错内容
-            conn: mysql conn
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            1). sql: 修改字段类型的 sql
-            1). possible_err: 执行此 sql 可能会报错的信息
-        """
-        if "Data too long for" in err_msg:
-            colum_pattern = re.compile(r"Data too long for column '(.*?)' at")
-            text = re.findall(colum_pattern, err_msg)
-            colum = text[0]
-            notes = note_dic[colum]
-            column_type = self._get_column_type(
-                cursor=cursor, database=database, table=table, column=colum
-            )
-            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
-            sql = f"""
-            ALTER TABLE `{table}` CHANGE COLUMN
-            `{colum}` `{colum}` {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";
-            """
-            return sql, f"1406: 更新 {colum} 字段类型为 {change_colum_type} 时失败"
-
-    def deal_1265_error(
-        self,
-        err_msg: str,
-        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-        database: str,
-        table: str,
-        note_dic: dict,
-    ) -> (str, str):
-        """
-        解决 1265, u"Data truncated for column ..."
-        Args:
-            err_msg: 报错内容
-            cursor: mysql connect cursor
-            database: 数据库名
-            table: 数据表名
-            note_dic: 当前表字段的注释
-
-        Returns:
-            None
-        """
-        if "Data truncated for column" in err_msg:
-            colum_pattern = re.compile(r"Data truncated for column '(.*?)' at")
-            text = re.findall(colum_pattern, err_msg)
-            colum = text[0]
-            notes = note_dic[colum]
-            column_type = self._get_column_type(
-                cursor=cursor, database=database, table=table, column=colum
-            )
-            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
-            sql = f"""
-            ALTER TABLE `{table}` CHANGE COLUMN
-            `{colum}` `{colum}` {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";
-            """
-            return sql, f"1265: 更新 {colum} 字段类型为 {change_colum_type} 时失败"
-
-    @abstractmethod
-    def _exec_sql(self, *args, **kwargs) -> None:
-        """
-        子类要实现执行 sql 的不同方法，使得可以正常适配不同的 pipelines 场景
-        Args:
-            *args: None
-            **kwargs: None
-
-        Returns:
-            None
-        """
-        pass
-
-
-class Synchronize(AbstractClass):
-    """
-    pipeline 同步执行 sql 的场景
-    """
-
-    def _exec_sql(
-        self,
-        conn: Param.PymysqlConnect,
-        cursor: Param.PymysqlCursor,
-        sql: str,
-        possible_err: Optional[str] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        try:
-            if cursor.execute(sql):
-                conn.commit()
-        except Exception as e:
-            if possible_err:
-                logger.info(f"{possible_err}")
-            else:
-                logger.info(f"{e}")
-
-
-class TwistedAsynchronous(AbstractClass):
-    """
-    pipeline twisted 异步执行 sql 的场景
-    """
-
-    def _exec_sql(
-        self,
-        cursor: Param.PymysqlDictCursor,
-        sql: str,
-        possible_err: Optional[str] = None,
-        *args,
-        **kwargs,
-    ) -> None:
-        try:
-            cursor.execute(sql)
-        except Exception as e:
-            if possible_err:
-                logger.info(f"{possible_err}")
-            else:
-                logger.info(f"{e}")
-
-
-def deal_mysql_err(
-    abstract_class: AbstractClass,
-    err_msg: str,
-    cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
-    charset: str,
-    collate: str,
-    database: str,
-    table: str,
-    table_enum: Type[TableEnumTypeVar],
-    note_dic: dict,
-    conn: Optional[Param.PymysqlConnect] = None,
-) -> None:
-    abstract_class.template_method(
-        err_msg,
-        conn,
-        cursor,
-        charset,
-        collate,
-        database,
-        table,
-        table_enum,
-        note_dic,
-    )
+import re
+from abc import ABC, abstractmethod
+from typing import Optional, Type, Union
+
+from ayugespidertools.common.params import Param
+from ayugespidertools.common.typevars import TableEnumTypeVar
+from ayugespidertools.config import logger
+
+__all__ = [
+    "Synchronize",
+    "TwistedAsynchronous",
+    "deal_mysql_err",
+]
+
+
+class AbstractClass(ABC):
+    """用于处理 mysql 异常的模板方法类"""
+
+    def _create_table(
+        self,
+        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+        table_name: str,
+        charset: str,
+        collate: str,
+        table_notes: str = "",
+        demand_code: str = "",
+    ) -> None:
+        """创建数据库表
+
+        Args:
+            cursor: mysql connect cursor，参数选择有：
+                1). 类型为 pymysql.cursors.Cursor，在同步 pipelines 中使用；
+                2). dbpool.runInteraction() 方法会将数据库连接的游标对象作为参数传入
+                回调函数中，而游标对象的类型可能是不同的，比如 DictCursor 或 Cursor 类型，在
+                异步 pipelines 中使用；
+            table_name: 创建表的名称
+            charset: charset
+            collate: collate
+            table_notes: 创建表的注释
+            demand_code: 创建表的需求对应的 code 值，用于和需求中的任务对应
+        """
+        # 用于表格 comment 的参数生成(即 table_notes 参数)
+        if demand_code != "":
+            table_notes = f"{demand_code}_{table_notes}"
+
+        sql = f"""
+        CREATE TABLE IF NOT EXISTS `{table_name}`
+        (`id` int(32) NOT NULL AUTO_INCREMENT COMMENT 'id', PRIMARY KEY (`id`))
+        ENGINE=InnoDB DEFAULT CHARSET={charset} COLLATE={collate} COMMENT='{table_notes}';
+        """
+
+        try:
+            # 执行 sql 查询，获取数据
+            data = cursor.execute(sql)
+            if any([data == 0, not data]):
+                logger.info(f"创建数据表 {table_notes}: {table_name} 成功！")
+
+        except Exception as e:
+            logger.error(
+                f"创建表失败，table_notes：{table_notes}，table_name：{table_name}，error：{e}"
+            )
+
+    def _get_column_type(
+        self,
+        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+        database: str,
+        table: str,
+        column: str,
+    ) -> str:
+        """获取数据字段存储类型
+
+        Args:
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            column: 字段名称
+
+        Returns:
+            column_type: 字段存储类型
+        """
+        sql = f"""
+        select COLUMN_TYPE from information_schema.columns
+        where table_schema = '{database}' and table_name = '{table}' and COLUMN_NAME= '{column}';
+        """
+        column_type = None
+        try:
+            if _ := cursor.execute(sql):
+                lines = cursor.fetchall()
+                if isinstance(lines, list):
+                    # 注意，此处 AyuMysqlPipeline 返回的结构示例为：[{'COLUMN_TYPE': 'varchar(190)'}]
+                    column_type = lines[0]["COLUMN_TYPE"] if len(lines) == 1 else ""
+                else:
+                    # 注意，此处 AyuTwistedMysqlPipeline 返回的结构示例为：(('varchar(10)',),)
+                    column_type = lines[0][0] if len(lines) == 1 else ""
+
+        except Exception as e:
+            logger.error(f"{e}")
+        return column_type
+
+    def template_method(
+        self,
+        err_msg: str,
+        conn: Param.PymysqlConnect,
+        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+        charset: str,
+        collate: str,
+        database: str,
+        table: str,
+        table_enum: Type[TableEnumTypeVar],
+        note_dic: dict,
+    ) -> None:
+        """模板方法，用于处理 mysql 存储场景的异常
+
+        Args:
+            err_msg: pipeline 存储时报错内容
+            conn: mysql conn
+            cursor: mysql connect cursor
+            charset: mysql table charset
+            collate: mysql table collate
+            database: 数据库
+            table: 数据表
+            table_enum: 数据表枚举类
+            note_dic: 当前表字段注释
+        """
+        if "1054" in err_msg:
+            sql, possible_err = self.deal_1054_error(
+                err_msg=err_msg, table=table, note_dic=note_dic
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        elif "1146" in err_msg:
+            table_name, table_notes, demand_code = self.deal_1146_error(
+                err_msg=err_msg,
+                table_enum=table_enum,
+            )
+            self._create_table(
+                cursor=cursor,
+                table_name=table_name,
+                charset=charset,
+                collate=collate,
+                table_notes=table_notes,
+                demand_code=demand_code,
+            )
+
+        elif "1406" in err_msg:
+            sql, possible_err = self.deal_1406_error(
+                err_msg=err_msg,
+                cursor=cursor,
+                database=database,
+                table=table,
+                note_dic=note_dic,
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        elif "1265" in err_msg:
+            sql, possible_err = self.deal_1265_error(
+                err_msg=err_msg,
+                cursor=cursor,
+                database=database,
+                table=table,
+                note_dic=note_dic,
+            )
+            self._exec_sql(conn=conn, cursor=cursor, sql=sql, possible_err=possible_err)
+
+        else:
+            # 碰到其他的异常才打印错误日志，已处理的异常不打印
+            logger.error(f"ERROR: {err_msg}")
+
+    def deal_1054_error(self, err_msg: str, table: str, note_dic: dict) -> (str, str):
+        """解决 1054, u"Unknown column 'xx' in 'field list'"
+
+        Args:
+            err_msg: 报错内容
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 用于添加字段的 sql 语句
+            2). 执行此 sql 可能会报错的信息
+        """
+        colum_pattern = re.compile(r"Unknown column '(.*?)' in 'field list'")
+        text = re.findall(colum_pattern, err_msg)
+        colum = text[0]
+        notes = note_dic[colum]
+
+        if colum == "url":
+            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` TEXT(500) NULL COMMENT '{notes}';"
+        elif colum in {"create_time", "crawl_time", "update_time"}:
+            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` DATE NULL DEFAULT NULL COMMENT '{notes}';"
+        else:
+            sql = f"ALTER TABLE `{table}` ADD COLUMN `{colum}` VARCHAR(190) NULL DEFAULT '' COMMENT '{notes}';"
+        return sql, f"1054: 添加字段 {colum} 已存在"
+
+    def deal_1146_error(
+        self,
+        err_msg: str,
+        table_enum: Type[TableEnumTypeVar],
+    ) -> (str, str, str):
+        """解决 1146, u"Table 'xx' doesn't exist"
+
+        Args:
+            err_msg: 报错内容
+            table_enum: 数据表的枚举信息
+
+        Returns:
+            1). table_name: 数据表名
+            2). table_notes: 数据表注释
+            3). demand_code: 数据表对应的需求 code
+        """
+        table_pattern = re.compile(r"Table '(.*?)' doesn't exist")
+        text = re.findall(table_pattern, err_msg)
+        table = text[0].split(".")[1]
+
+        # 写入表枚举
+        if table_enum:
+            for _, member in table_enum.__members__.items():
+                table_name = member.value.get("value", "")
+                table_notes = member.value.get("notes", "")
+                demand_code = member.value.get("demand_code", "")
+                if table_name == table:
+                    return table_name, table_notes, demand_code
+        else:
+            # 未定义 Tabel_Enum 则建表
+            logger.info("未定义数据库表枚举 Tabel_Enum 参数，进行创表操作")
+        # 1.未定义 Tabel_Enum 和 2.正则未匹配到当前的 table_name 时都以此报错 table 名为准
+        return table, "", ""
+
+    def deal_1406_error(
+        self,
+        err_msg: str,
+        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+        database: str,
+        table: str,
+        note_dic: dict,
+    ) -> (str, str):
+        """解决 1406, u"Data too long for 'xx' at ..."
+
+        Args:
+            err_msg: 报错内容
+            conn: mysql conn
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 修改字段类型的 sql
+            2). 执行此 sql 可能会报错的信息
+        """
+        if "Data too long for" in err_msg:
+            colum_pattern = re.compile(r"Data too long for column '(.*?)' at")
+            text = re.findall(colum_pattern, err_msg)
+            colum = text[0]
+            notes = note_dic[colum]
+            column_type = self._get_column_type(
+                cursor=cursor, database=database, table=table, column=colum
+            )
+            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
+            sql = f"""
+            ALTER TABLE `{table}` CHANGE COLUMN
+            `{colum}` `{colum}` {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";
+            """
+            return sql, f"1406: 更新 {colum} 字段类型为 {change_colum_type} 时失败"
+
+    def deal_1265_error(
+        self,
+        err_msg: str,
+        cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+        database: str,
+        table: str,
+        note_dic: dict,
+    ) -> (str, str):
+        """解决 1265, u"Data truncated for column 'xx' at ..."
+
+        Args:
+            err_msg: 报错内容
+            cursor: mysql connect cursor
+            database: 数据库名
+            table: 数据表名
+            note_dic: 当前表字段的注释
+
+        Returns:
+            1). sql: 修改字段类型的 sql
+            2). 执行此 sql 可能会报错的信息
+        """
+        if "Data truncated for column" in err_msg:
+            colum_pattern = re.compile(r"Data truncated for column '(.*?)' at")
+            text = re.findall(colum_pattern, err_msg)
+            colum = text[0]
+            notes = note_dic[colum]
+            column_type = self._get_column_type(
+                cursor=cursor, database=database, table=table, column=colum
+            )
+            change_colum_type = "LONGTEXT" if column_type == "text" else "TEXT"
+            sql = f"""
+            ALTER TABLE `{table}` CHANGE COLUMN
+            `{colum}` `{colum}` {change_colum_type} NULL DEFAULT NULL COMMENT "{notes}";
+            """
+            return sql, f"1265: 更新 {colum} 字段类型为 {change_colum_type} 时失败"
+
+    @abstractmethod
+    def _exec_sql(self, *args, **kwargs) -> None:
+        """子类要实现执行 sql 的不同方法，使得可以正常适配不同的 pipelines 场景"""
+        pass
+
+
+class Synchronize(AbstractClass):
+    """pipeline 同步执行 sql 的场景"""
+
+    def _exec_sql(
+        self,
+        conn: Param.PymysqlConnect,
+        cursor: Param.PymysqlCursor,
+        sql: str,
+        possible_err: Optional[str] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        try:
+            if cursor.execute(sql):
+                conn.commit()
+        except Exception as e:
+            if possible_err:
+                logger.info(f"{possible_err}")
+            else:
+                logger.info(f"{e}")
+
+
+class TwistedAsynchronous(AbstractClass):
+    """pipeline twisted 异步执行 sql 的场景"""
+
+    def _exec_sql(
+        self,
+        cursor: Param.PymysqlDictCursor,
+        sql: str,
+        possible_err: Optional[str] = None,
+        *args,
+        **kwargs,
+    ) -> None:
+        try:
+            cursor.execute(sql)
+        except Exception as e:
+            if possible_err:
+                logger.info(f"{possible_err}")
+            else:
+                logger.info(f"{e}")
+
+
+def deal_mysql_err(
+    abstract_class: AbstractClass,
+    err_msg: str,
+    cursor: Union[Param.PymysqlCursor, Param.PymysqlDictCursor],
+    charset: str,
+    collate: str,
+    database: str,
+    table: str,
+    table_enum: Type[TableEnumTypeVar],
+    note_dic: dict,
+    conn: Optional[Param.PymysqlConnect] = None,
+) -> None:
+    abstract_class.template_method(
+        err_msg,
+        conn,
+        cursor,
+        charset,
+        collate,
+        database,
+        table,
+        table_enum,
+        note_dic,
+    )
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/params.py` & `ayugespidertools-3.3.2/ayugespidertools/common/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 __all__ = [
     "Param",
 ]
 
 
 class Param:
-    """
-    用于存储项目中需要的参数变量设置
-    """
+    """用于存储项目中需要的参数变量设置"""
 
     NoneType = type(None)
     # 用于参数的描述
     I_Str = TypeVar("I_Str", int, str)
     B_Str = TypeVar("B_Str", bytes, str)
     I_Str_N = TypeVar("I_Str_N", int, str, NoneType)
     Str_Lstr = TypeVar("Str_Lstr", str, List[str])
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/spiderconf.py` & `ayugespidertools-3.3.2/ayugespidertools/common/spiderconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,15 @@
     ExclusiveProxyConf,
 )
 
 
 class Product(ABC):
     @abstractmethod
     def get_conn_conf(self) -> Union[SpiderConf, None]:
-        """
-        获取各个工具链接配置信息
-        """
+        """获取各个工具链接配置信息"""
         pass
 
 
 class Creator(ABC):
     @abstractmethod
     def create_product(self, *args, **kwargs) -> Product:
         pass
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.3.2/ayugespidertools/common/sqlformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,30 @@
     "AboutSql",
 ]
 
 SqlModeStr = Literal["and", "or"]
 
 
 class AboutSql:
-    """
-    sql 相关处理: sql 语句的管理方法，
+    """sql 相关处理: sql 语句的管理方法，
     这里的 sql 拼接只能做到最简单的逻辑，如果需要灵活或稍复杂的情况，请参考 directsql, python-sql, pypika
     或 pymilk 等第三方类似功能库的实现方法，以后会再优化此场景
     """
 
     @staticmethod
     def select_generate(
         db_table: str,
         key: list,
         rule: Dict[str, Any],
         base: SqlModeStr = "and",
         order_by: Optional[str] = None,
         limit: Union[bool, int] = False,
     ) -> (str, tuple):
-        """
-        根据一些参数来生成供 pymysql 之类的库中使用的 sql 查询语句（适用于简单情况）
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 查询语句（适用于简单情况）
+
         Args:
             db_table: 需要查询的表名称
             key: 需要查询的关键字段
             rule: 查询需要的规则
             base: 在有多个查询规则时，选择 "and" 或 "or"，默认 "and"
             order_by: 排序的 key 值
             limit: limit 限制，默认无限制（查询所有）；如果需要则指定 int 值即可
@@ -52,16 +51,16 @@
         select_sql = (
             f"""select {select_key} from {db_table} {_where} {_order_by} {_limit}"""
         )
         return select_sql, tuple(rule.values())
 
     @staticmethod
     def insert_generate(db_table: str, data: dict) -> (str, tuple):
-        """
-        根据一些参数来生成供 pymysql 之类的库中使用的 sql 插入语句
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 插入语句
+
         Args:
             db_table: 需要插入的表名称
             data: 需要插入的关键字段，key: 数据表字段；value: 需插入的参数名
 
         Returns:
             select_sql: 生成的 sql 语句
             tuple(rule.values()): 新增字段的参数名称
@@ -71,16 +70,16 @@
         sql = f"""insert into `{db_table}` ({keys}) values ({values})"""
         return sql, tuple(data.values())
 
     @staticmethod
     def update_generate(
         db_table: str, data: dict, rule: Dict[str, Any], base: SqlModeStr = "and"
     ) -> (str, tuple):
-        """
-        根据一些参数来生成供 pymysql 之类的库中使用的 sql 更新语句
+        """根据一些参数来生成供 pymysql 之类的库中使用的 sql 更新语句
+
         Args:
             db_table: 需要插入的表名称
             data: 需要更新的 key 和 value 值
             rule: 更新需要的规则
             base: 在有多个查询规则时，选择 "and" 或 "or"，默认 "and"
 
         Returns:
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/typevars.py` & `ayugespidertools-3.3.2/ayugespidertools/common/typevars.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     notes: str
     # 需求表对应数据，可用于开发任务与需求任务表中任务 code 对应
     demand_code: str
 
 
 @unique
 class TableEnum(Enum):
-    """
-    数据库表枚举信息示例，用于限制存储信息类的字段及值不允许重复和修改
-    """
+    """数据库表枚举信息示例，用于限制存储信息类的字段及值不允许重复和修改"""
 
     demo_table = TableTemplate(
         value="表名(eg: demo)",
         notes="表注释信息(eg: 示例表信息)",
         demand_code="需求表对应数据(eg: Demo_table_demand_code，此示例没有意义，需要自定义)",
     )
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.3.2/ayugespidertools/common/yidungap.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 
 __all__ = [
     "YiDunGetGap",
 ]
 
 
 class YiDunGetGap:
-    """
-    易盾获取滑块缺口距离的相关方法，也可能适配于其它平台
-    """
+    """易盾获取滑块缺口距离的相关方法，也可能适配于其它平台"""
 
     @classmethod
     def clear_white(cls, img):
-        """
-        清除图片的空白区域，这里主要清除滑块的空白
+        """清除图片的空白区域，这里主要清除滑块的空白
+
         Args:
             img: 待处理的图片
 
         Returns:
             1). 清楚图片空白区域的图片
         """
         rows, cols, channel = img.shape
@@ -42,16 +40,16 @@
                 elif y >= max_y:
                     max_y = y
 
         return img[min_x:max_x, min_y:max_y]
 
     @classmethod
     def template_match(cls, tpl, target, out: str = None) -> int:
-        """
-        模板匹配找出滑块缺口的距离
+        """模板匹配找出滑块缺口的距离
+
         Args:
             tpl: 缺口图片
             target: 背景图片
             out: 展示图片的存储全路径，会将绘制的图片保存至此
 
         Returns:
             tl[0]: 滑块缺口的距离
@@ -73,35 +71,35 @@
             # 1：矩形边框大小
             cv2.rectangle(target, tl, br, (0, 0, 255), 2)
             cv2.imwrite(out, target)
         return tl[0]
 
     @classmethod
     def image_edge_detection(cls, img):
-        """
-        图像边缘检测处理，识别图片边缘
+        """图像边缘检测处理，识别图片边缘
+
         Args:
             img: 需要处理的图片，用于边缘检测使用
 
         Returns:
             1). 处理后的图片
         """
         return cv2.Canny(img, 100, 200)
 
     @classmethod
     def discern(cls, slide, bg, out: str = None):
-        """
-        识别滑块缺口方法
+        """识别滑块缺口方法
+
         Args:
             slide: 滑块图，可以是全路径图片，也可以是图片的 bytes 数据
             bg: 带缺口的背景图，可以是全路径图片，也可以是图片的 bytes 数据
             out: 绘制图展示的存储地址，参数格式为图片的全路径
 
         Returns:
-            x: 滑块缺口横坐标
+            1): 滑块缺口横坐标
         """
         # 先用 opencv 读取图片数据
         slide_cv, bg_cv = ReuseOperation.read_image_data(slide, bg)
 
         # 清除图片的空白区域
         img1 = cls.clear_white(slide_cv)
         img1 = cv2.cvtColor(img1, cv2.COLOR_RGB2GRAY)
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/formatdata.py` & `ayugespidertools-3.3.2/ayugespidertools/formatdata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,287 +1,279 @@
-import datetime
-import re
-import time
-from typing import Optional
-from urllib.parse import urljoin
-
-import html2text
-from w3lib.html import remove_tags, replace_entities
-
-__all__ = [
-    "DataHandle",
-]
-
-
-class DataHandle:
-    """数据处理相关方法"""
-
-    @staticmethod
-    def get_full_url(domain_name: str, deal_url: str) -> str:
-        """
-        根据域名 domain_name 拼接 deal_url 来获得完整链接
-        Args:
-            domain_name: 域名链接
-            deal_url: 需要拼接的 url
-
-        Returns:
-            1). 拼接完整的链接
-        """
-        return urljoin(domain_name, deal_url)
-
-    @staticmethod
-    def click_point_deal(decimal: float, decimal_places=2) -> float:
-        """
-        将小数 decimal 保留小数点后 decimal_places 位，结果四舍五入
-        Args:
-            decimal: 需要处理的小数
-            decimal_places: 需要保留的小数点位数
-
-        Returns:
-            decimal(float): 四舍五入后的小数点
-        """
-        # 先拼接需要保留的位数
-        decimal_deal = f"%.{decimal_places}f"
-        return float(decimal_deal % decimal)
-
-    @staticmethod
-    def judge_utc_time(local_time: str) -> bool:
-        """
-        判断 local_time 是否为 utc 格式的时间
-        Args:
-            local_time: 需要判断的时间参数，比如：Thu Jul 21 17:59:44 2022 或 Fri, 22 Jul 2022 01:43:06 +0800 等等
-
-        Returns:
-            1): 是否为 utc 格式的数据
-        """
-        pattern = re.compile(r"""mon|tues|wed|thu|fri|sat|sun""")
-        return bool(pattern.findall(local_time.lower()))
-
-    @staticmethod
-    def judge_include_letter(local_time: str) -> bool:
-        pattern = re.compile(r"""[a-zA-Z]""")
-        return bool(pattern.findall(local_time.lower()))
-
-    @staticmethod
-    def _get_format_t(
-        date_style: str = "",
-        date_is_full: bool = False,
-        specific_date_conn: str = " ",
-        hms_conn: str = ":",
-    ) -> str:
-        """
-        将需要格式化的数据用 date_style 标识来拼接起来，如果 date_is_full 为 True 时，则需要补齐"时分秒"位
-        Args:
-            date_style: 将格式化符拼接时需要的标识，比如：-
-            date_is_full: 是否需要完整的时间格式化（即是否需要补齐"时分秒"单位）
-            specific_date_conn: 年月日与时分秒拼接的方式
-            hms_conn: 时分秒拼接的方式
-
-        Returns:
-            1).最终的格式化拼接结果，比如：%Y-%m-%d %H-%M-%S
-        """
-        # 年月日
-        _y_m_d = ["%Y", "%m", "%d"]
-        _y_m_d_format = date_style.join(_y_m_d)
-
-        if date_is_full:
-            # 时分秒
-            _h_m_s = ["%H", "%M", "%S"]
-            # 时分秒大都为":"连接
-            _h_m_s_format = hms_conn.join(_h_m_s)
-            return specific_date_conn.join([_y_m_d_format, _h_m_s_format])
-        return _y_m_d_format
-
-    @staticmethod
-    def _time_format(date_str) -> str:
-        """
-        判断时间是什么格式的，比如：xxxx-xx-xx 或 xxxx.xx.xx
-        Args:
-            date_str: 需要判断格式的时间
-
-        Returns:
-            1): 时间格式的标识，比如：-，若没有就返回空字符
-        """
-        format_styles = ["-", ".", "/", "年"]
-        return next(
-            (
-                format_style
-                for format_style in format_styles
-                if format_style in date_str
-            ),
-            "",
-        )
-
-    @classmethod
-    def normal_to_stamp(
-        cls,
-        normal_time: str,
-        _format_t: str = None,
-        date_is_full: bool = True,
-        specific_date_conn: str = " ",
-        hms_conn: str = ":",
-    ) -> int:
-        """
-        将网页正常时间转为时间戳
-        Args:
-            normal_time: 需要转换的时间
-            _format_t: 时间格式化符，默认不填。除非在英文时间的参数出错时可指定 _format_t 的值
-            date_is_full: 是否包含"时分秒"单位的完整格式
-            specific_date_conn: 年月日与时分秒拼接的方式
-            hms_conn: 时分秒拼接的方式
-
-        Returns:
-            stamp: 返回的时间戳
-        """
-        # 判断 normal_time 是否是特殊模式
-        is_utc_time = cls.judge_utc_time(normal_time)
-        is_letter_time = cls.judge_include_letter(normal_time)
-        # stamp = None
-        if any([is_utc_time, is_letter_time]):
-            # 如果不传递时间的格式符参数
-            if not _format_t:
-                if "," in normal_time:
-                    _format_t = "%a, %d %b %Y %H:%M:%S +0800"
-                else:
-                    _format_t = "%a %b %d %H:%M:%S %Y"
-            standard_time = datetime.datetime.strptime(normal_time, _format_t)
-            stamp = time.mktime(
-                time.strptime(str(standard_time), cls._get_format_t("-", True))
-            )
-
-        else:
-            # 先判断正常时间的格式
-            date_style = cls._time_format(normal_time)
-            # standard_time_format = _get_format_t(date_style, date_is_full).replace('%m', '%b').replace('-', '/')
-            standard_time_format = cls._get_format_t(
-                date_style, date_is_full, specific_date_conn, hms_conn
-            )
-            stamp = time.mktime(time.strptime(normal_time, standard_time_format))
-        return int(stamp)
-
-    @staticmethod
-    def timestamp_to_normal(timestamp_data: int) -> str:
-        """
-        将时间戳转为正常时间 xxxx-xx-xx xx:xx:xx 的格式
-        Args:
-            timestamp_data: 需要处理的时间格式
-
-        Returns:
-            1). 转换后的时间结果
-        """
-        if len(str(timestamp_data)) > 10:
-            timestamp_data = int(str(timestamp_data[:-3]))
-
-        time_array = time.localtime(timestamp_data)
-        return time.strftime("%Y-%m-%d %H:%M:%S", time_array)
-
-    @staticmethod
-    def remove_all_tags(func):
-        """
-        去除所有标签
-        """
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            func_res = remove_tags(func_res)
-            return func_res
-
-        return inner
-
-    @staticmethod
-    def normal_display(func):
-        """
-        去除掉网页的注释(将网页中的特殊字符的源码改成正常显示)
-        """
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            func_res = replace_entities(func_res)
-            return func_res
-
-        return inner
-
-    @staticmethod
-    def simple_deal_for_extract(func):
-        """
-        将 xpath, css 或 json 提取的数据做简单处理；提取的数据若非数组数据，则统一返回字符类型
-        """
-
-        def inner(*args, **kwargs):
-            func_res = func(*args, **kwargs)
-            if type(func_res) in [str, int, float, bool]:
-                # 这里可添加一些通用的数据处理
-                return str(func_res).strip()
-            else:
-                return func_res
-
-        return inner
-
-    @classmethod
-    def _extract_table_rule(
-        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
-    ):
-        """
-        根据 html2text 来处理 html 中的 table 表格内容
-        Args:
-            html_txt: 网页内容
-            h_obj: html2text 对象句柄
-
-        Returns:
-            1).转换后的结果
-        """
-        if not h_obj:
-            h_obj = html2text.HTML2Text()
-
-        h_obj.protect_links = True
-        h_obj.body_width = 0
-        h_obj.ignore_links = True
-        h_obj.bypass_tables = False
-        return h_obj.handle(html_txt)
-
-    @classmethod
-    def extract_html_to_md(
-        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
-    ) -> str:
-        """
-        将 html 内容转化为 markdown 内容
-
-        更多、更详细的配置参数请查看文档内容: https://github.com/Alir3z4/html2text/blob/master/html2text/cli.py
-        Args:
-            html_txt: 网页内容（一般是带标签的内容）
-            h_obj: html2text 对象句柄
-
-        Returns:
-            1).转换后的结果
-        """
-        if not h_obj:
-            h_obj = html2text.HTML2Text()
-
-        # 以下步骤先处理通用部分，先不处理 table 内容
-        h_obj.body_width = 0
-        # h_obj.protect_links = True
-        h_obj.bypass_tables = True
-        # h_obj.unicode_snob = True
-        h_obj.ignore_links = True
-        content = h_obj.handle(html_txt)
-
-        # 先处理表格 <table> 标签中格式
-        table_pattern = re.compile(r"(<table.*?</table>)", flags=re.S)
-        if table_res_list := table_pattern.findall(content):
-            for table_res in table_res_list:
-                table_deal = cls._extract_table_rule(html_txt=table_res, h_obj=h_obj)
-                # 将 table 转换时去除多余的换行和空白字符等内容
-                table_deal = re.sub(r"\|\s*\n", "| ", table_deal, flags=re.S)
-                table_deal = re.sub(r"\n\s*\|", "| ", table_deal, flags=re.S)
-                table_deal = re.sub(r"\n\s*\n", "\n\n", table_deal, flags=re.S)
-                table_deal = re.sub(r"\r\n", "\n", table_deal, flags=re.S)
-                table_deal = re.sub(r"[\n]{1,}", "\n", table_deal, flags=re.S)
-
-                content = re.sub(
-                    r"(<table.*?</table>)", table_deal + "\n", content, 1, re.S
-                )
-
-        # TODO: 可以添加上通用处理的装饰器
-        # 将三个以上换行改为两个换行
-        content = re.sub(r"[\n]{3,}", "\n\n", content)
-        content = content.strip()
-        return content
+import datetime
+import re
+import time
+from typing import Optional, Union
+from urllib.parse import urljoin
+
+import html2text
+from w3lib.html import remove_tags, replace_entities
+
+__all__ = [
+    "DataHandle",
+]
+
+
+class DataHandle:
+    """数据处理相关方法"""
+
+    @staticmethod
+    def get_full_url(domain_name: str, deal_url: str) -> str:
+        """根据域名 domain_name 拼接 deal_url 来获得完整链接
+
+        Args:
+            domain_name: 域名链接
+            deal_url: 需要拼接的 url
+
+        Returns:
+            1). 拼接完整的链接
+        """
+        return urljoin(domain_name, deal_url)
+
+    @staticmethod
+    def click_point_deal(decimal: float, decimal_places: int = 2) -> float:
+        """将小数 decimal 保留小数点后 decimal_places 位，结果四舍五入
+
+        Args:
+            decimal: 需要处理的小数
+            decimal_places: 需要保留的小数点位数
+
+        Returns:
+            decimal(float): 四舍五入后的小数点
+        """
+        # 先拼接需要保留的位数
+        decimal_deal = f"%.{decimal_places}f"
+        return float(decimal_deal % decimal)
+
+    @staticmethod
+    def judge_utc_time(local_time: str) -> bool:
+        """判断 local_time 是否为 utc 格式的时间
+
+        Args:
+            local_time: 需要判断的时间参数，比如：Thu Jul 21 17:59:44 2022 或 Fri, 22 Jul 2022 01:43:06 +0800 等等
+
+        Returns:
+            1): 是否为 utc 格式的数据
+        """
+        pattern = re.compile(r"""mon|tues|wed|thu|fri|sat|sun""")
+        return bool(pattern.findall(local_time.lower()))
+
+    @staticmethod
+    def judge_include_letter(local_time: str) -> bool:
+        pattern = re.compile(r"""[a-zA-Z]""")
+        return bool(pattern.findall(local_time.lower()))
+
+    @staticmethod
+    def _get_format_t(
+        date_style: str = "",
+        date_is_full: bool = False,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> str:
+        """将需要格式化的数据用 date_style 标识来拼接起来，如果 date_is_full 为 True 时，则需要补齐"时分秒"位
+
+        Args:
+            date_style: 将格式化符拼接时需要的标识，比如：-
+            date_is_full: 是否需要完整的时间格式化（即是否需要补齐"时分秒"单位）
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            1).最终的格式化拼接结果，比如：%Y-%m-%d %H-%M-%S
+        """
+        # 年月日
+        _y_m_d = ["%Y", "%m", "%d"]
+        _y_m_d_format = date_style.join(_y_m_d)
+
+        if date_is_full:
+            # 时分秒
+            _h_m_s = ["%H", "%M", "%S"]
+            # 时分秒大都为":"连接
+            _h_m_s_format = hms_conn.join(_h_m_s)
+            return specific_date_conn.join([_y_m_d_format, _h_m_s_format])
+        return _y_m_d_format
+
+    @staticmethod
+    def _time_format(date_str) -> str:
+        """判断时间是什么格式的，比如：xxxx-xx-xx 或 xxxx.xx.xx
+
+        Args:
+            date_str: 需要判断格式的时间
+
+        Returns:
+            1): 时间格式的标识，比如：-，若没有就返回空字符
+        """
+        format_styles = ["-", ".", "/", "年"]
+        return next(
+            (
+                format_style
+                for format_style in format_styles
+                if format_style in date_str
+            ),
+            "",
+        )
+
+    @classmethod
+    def normal_to_stamp(
+        cls,
+        normal_time: str,
+        _format_t: str = None,
+        date_is_full: bool = True,
+        specific_date_conn: str = " ",
+        hms_conn: str = ":",
+    ) -> int:
+        """将网页正常时间转为时间戳
+
+        Args:
+            normal_time: 需要转换的时间
+            _format_t: 时间格式化符，默认不填。除非在英文时间的参数出错时可指定 _format_t 的值
+            date_is_full: 是否包含"时分秒"单位的完整格式
+            specific_date_conn: 年月日与时分秒拼接的方式
+            hms_conn: 时分秒拼接的方式
+
+        Returns:
+            stamp: 返回的时间戳
+        """
+        # 判断 normal_time 是否是特殊模式
+        is_utc_time = cls.judge_utc_time(normal_time)
+        is_letter_time = cls.judge_include_letter(normal_time)
+        # stamp = None
+        if any([is_utc_time, is_letter_time]):
+            # 如果不传递时间的格式符参数
+            if not _format_t:
+                if "," in normal_time:
+                    _format_t = "%a, %d %b %Y %H:%M:%S +0800"
+                else:
+                    _format_t = "%a %b %d %H:%M:%S %Y"
+            standard_time = datetime.datetime.strptime(normal_time, _format_t)
+            stamp = time.mktime(
+                time.strptime(str(standard_time), cls._get_format_t("-", True))
+            )
+
+        else:
+            # 先判断正常时间的格式
+            date_style = cls._time_format(normal_time)
+            # standard_time_format = _get_format_t(date_style, date_is_full).replace('%m', '%b').replace('-', '/')
+            standard_time_format = cls._get_format_t(
+                date_style, date_is_full, specific_date_conn, hms_conn
+            )
+            stamp = time.mktime(time.strptime(normal_time, standard_time_format))
+        return int(stamp)
+
+    @staticmethod
+    def timestamp_to_normal(timestamp: Union[int, str]) -> str:
+        """将时间戳转为正常时间 xxxx-xx-xx xx:xx:xx 的格式
+
+        Args:
+            timestamp: 需要处理的时间格式
+
+        Returns:
+            1). 转换后的时间结果
+        """
+        _timestamp = str(timestamp) if isinstance(timestamp, int) else timestamp
+        timestamp_normal = int(_timestamp[:10])
+        time_array = time.localtime(timestamp_normal)
+        return time.strftime("%Y-%m-%d %H:%M:%S", time_array)
+
+    @staticmethod
+    def remove_all_tags(func):
+        """去除所有标签"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = remove_tags(func_res)
+            return func_res
+
+        return inner
+
+    @staticmethod
+    def normal_display(func):
+        """去除掉网页的注释(将网页中的特殊字符的源码改成正常显示)"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            func_res = replace_entities(func_res)
+            return func_res
+
+        return inner
+
+    @staticmethod
+    def simple_deal_for_extract(func):
+        """将 xpath, css 或 json 提取的数据做简单处理；提取的数据若非数组数据，则统一返回字符类型"""
+
+        def inner(*args, **kwargs):
+            func_res = func(*args, **kwargs)
+            if type(func_res) in [str, int, float, bool]:
+                # 这里可添加一些通用的数据处理
+                return str(func_res).strip()
+            else:
+                return func_res
+
+        return inner
+
+    @classmethod
+    def _extract_table_rule(
+        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
+    ):
+        """根据 html2text 来处理 html 中的 table 表格内容
+
+        Args:
+            html_txt: 网页内容
+            h_obj: html2text 对象句柄
+
+        Returns:
+            1). 转换后的结果
+        """
+        if not h_obj:
+            h_obj = html2text.HTML2Text()
+
+        h_obj.protect_links = True
+        h_obj.body_width = 0
+        h_obj.ignore_links = True
+        h_obj.bypass_tables = False
+        return h_obj.handle(html_txt)
+
+    @classmethod
+    def extract_html_to_md(
+        cls, html_txt: str, h_obj: Optional[html2text.HTML2Text] = None
+    ) -> str:
+        """将 html 内容转化为 markdown 内容
+        更多、更详细的配置参数请查看文档内容: https://github.com/Alir3z4/html2text/blob/master/html2text/cli.py
+
+        Args:
+            html_txt: 网页内容（一般是带标签的内容）
+            h_obj: html2text 对象句柄
+
+        Returns:
+            1). 转换后的结果
+        """
+        if not h_obj:
+            h_obj = html2text.HTML2Text()
+
+        # 以下步骤先处理通用部分，先不处理 table 内容
+        h_obj.body_width = 0
+        # h_obj.protect_links = True
+        h_obj.bypass_tables = True
+        # h_obj.unicode_snob = True
+        h_obj.ignore_links = True
+        content = h_obj.handle(html_txt)
+
+        # 先处理表格 <table> 标签中格式
+        table_pattern = re.compile(r"(<table.*?</table>)", flags=re.S)
+        if table_res_list := table_pattern.findall(content):
+            for table_res in table_res_list:
+                table_deal = cls._extract_table_rule(html_txt=table_res, h_obj=h_obj)
+                # 将 table 转换时去除多余的换行和空白字符等内容
+                table_deal = re.sub(r"\|\s*\n", "| ", table_deal, flags=re.S)
+                table_deal = re.sub(r"\n\s*\|", "| ", table_deal, flags=re.S)
+                table_deal = re.sub(r"\n\s*\n", "\n\n", table_deal, flags=re.S)
+                table_deal = re.sub(r"\r\n", "\n", table_deal, flags=re.S)
+                table_deal = re.sub(r"[\n]{1,}", "\n", table_deal, flags=re.S)
+
+                content = re.sub(
+                    r"(<table.*?</table>)", table_deal + "\n", content, 1, re.S
+                )
+
+        # TODO: 可以添加上通用处理的装饰器
+        # 将三个以上换行改为两个换行
+        content = re.sub(r"[\n]{3,}", "\n\n", content)
+        content = content.strip()
+        return content
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/imgoperation.py` & `ayugespidertools-3.3.2/ayugespidertools/imgoperation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+from pathlib import Path
 from typing import Optional, Union
 
 import cv2
 from PIL import Image
 
 from ayugespidertools.common.encryption import EncryptOperation
 from ayugespidertools.common.multiplexing import ReuseOperation
 
 __all__ = [
     "Picture",
 ]
 
 
 class Picture:
-    """
-    对验证码图片的一些操作
-    """
+    """对验证码图片的一些操作"""
 
     @classmethod
     def convert_index_to_offset(cls, index):
-        """
-        获取每张小图的偏移量
+        """获取每张小图的偏移量
+
         Args:
             index: 当前小块图片
 
         Returns:
-            当前小图在空白图片的坐标
+            1). 当前小图在空白图片的坐标
         """
 
         # 代码注释
         """
         # 图片大小为：334 159， 22 为 334 / 15 得到，58 是 159 /
         if index < 15:  # 完整的验证码图片是由30个小图片组合而成，共2行15列
             return (index * 22, 0)
@@ -42,37 +41,34 @@
         else:
             i = index - 20
             # 每张小图的大小为 22 * 58
             return i * 13, 58
 
     @classmethod
     def convert_css_to_offset(cls, off):
-        """
-        获取每张小图的坐标，供抠图时使用
+        """获取每张小图的坐标，供抠图时使用
+
         Args:
             off: 根据 css backgound-position 中获取的每张小图的坐标
 
         Returns:
             (int(off[0]), int(off[1]), int(off[0]) + 22, int(off[1]) + 58): 每张小图对应的坐标
         """
         # (left, upper)o ----- o
         #              |       |
         #              o ----- o(right, lower)
         return int(off[0]), int(off[1]), int(off[0]) + 22, int(off[1]) + 58
 
     @classmethod
     def recombine_captcha(cls, offset_list: list, img_path: str):
-        """
-        图片重组: 完美世界网站的图片重组方法
+        """图片重组: 完美世界网站的图片重组方法
+
         Args:
             offset_list: 坐标列表
             img_path: 图片保存路径
-
-        Returns:
-            None
         """
         # 新建空白图片
         captcha = Image.new("RGB", (13 * 20, 60 * 2 - 4))
         # 实例化原始图片Image对象
         img = Image.open(f"{img_path}/captcha.png")
 
         # 切割滑块验证码图片，将背景图和滑块图分开
@@ -90,16 +86,16 @@
             offset = Picture.convert_index_to_offset(i)
             # 根据当前坐标将小图粘贴到空白图片
             captcha.paste(regoin, offset)
         captcha.save(f"{img_path}/regoin.jpg")
 
     @classmethod
     def reset_pic(cls, slide_data):
-        """
-        完美世界滑块验证码重组方法，具体位置根据 background-position 搜索定位
+        """完美世界滑块验证码重组方法，具体位置根据 background-position 搜索定位
+
         Args:
             slide_data: 完美滑块重组所需的数组
 
         Returns:
             true_pic_list: 真实图片的顺序坐标
         """
         c = 260
@@ -115,16 +111,16 @@
             else:
                 curr_position_list.extend((int(c / _l * (curr_data % _l)), 60))
             true_pic_list.append(curr_position_list)
         return true_pic_list
 
     @classmethod
     def find_pic(cls, target, template):
-        """
-        找出图像中最佳匹配位置
+        """找出图像中最佳匹配位置
+
         Args:
             target: 目标（背景图）
             template: 模板（需要找到的图）
 
         Returns:
             value[2:][0][0]: 返回最佳匹配及对应的坐标
             value[2:][1][0]: 返回最差匹配及对应的坐标
@@ -136,16 +132,16 @@
         value = cv2.minMaxLoc(res)
         return value[2:][0][0], value[2:][1][0]
 
     @classmethod
     def identify_gap(
         cls, bg: Union[bytes, str], tp: Union[bytes, str], out: Optional[str] = None
     ) -> int:
-        """
-        通过背景图片和缺口图片识别出滑块距离
+        """通过背景图片和缺口图片识别出滑块距离
+
         Args:
             bg: 背景图片，可以是图片的全路径，也可以是图片的 bytes 内容
             tp: 缺口（滑块）图片，可以是图片的全路径，也可以是图片的 bytes 内容
             out: 输出图片路径，示例：doc/test.jpg；此参数如果为空，则不输出标记后的图片
 
         Returns:
             tl[0]: 滑块缺口距离
@@ -180,20 +176,18 @@
             cv2.imwrite(out, bg_cv)
 
         # 返回缺口的X坐标
         return tl[0]
 
     @classmethod
     def get_data_urls_by_img(cls, mediatype: str, data: Union[bytes, str]) -> str:
-        """
-        根据本地、远程或 bytes 内容的图片生成 Data URLs 格式的数据
+        """根据本地、远程或 bytes 内容的图片生成 Data URLs 格式的数据
         Data URLs 格式示例:
             data:image/png;base64,iVB...
             data:text/html,%3Ch1%3EHello%2C%20World%21%3C%2Fh1%3E
-
         关于 Data URLs 更多的描述，其参考文档: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URLs
 
         Args:
             mediatype: MIME 类型字符串，例如 'image/jpeg' JPEG 图像文件。
                 如果省略，则默认为 text/plain;charset=US-ASCII
             data: 用于获取其 base64 编码的二进制数据
                 参数格式可以为全路径图片，或 bytes 内容
@@ -203,13 +197,13 @@
         """
         assert type(data) in [
             str,
             bytes,
         ], "图片转 Data URLs 的参数 data 需要是全路径 str 或 bytes 数据"
 
         if isinstance(data, str):
-            data_bytes = ReuseOperation.get_bytes_by_file(file_path=data)
+            data_bytes = Path(data).read_bytes()
             data_base64_encoded = EncryptOperation.base64_encode(encode_data=data_bytes)
 
         else:
             data_base64_encoded = EncryptOperation.base64_encode(encode_data=data)
         return f"data:image/{mediatype};base64,{data_base64_encoded}"
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/items.py` & `ayugespidertools-3.3.2/ayugespidertools/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,30 +22,26 @@
 
 
 class ScrapyItem(Item):
     """scrapy item 的标准方式"""
 
 
 class DataItem(NamedTuple):
-    """
-    用于描述 item 中字段
-    """
+    """用于描述 item 中字段"""
 
     key_value: Any
     notes: str = ""
 
 
 # item 中 alldata 的类型
 AllDataType = Dict[str, Union[DataItem, Dict[str, Any], Any]]
 
 
 class ScrapyClassicItem(Item):
-    """
-    scrapy 经典 item 示例
-    """
+    """scrapy 经典 item 示例"""
 
     # 用于存放所有字段信息
     alldata: AllDataType = Field()
     # 用于存放存储的表名
     _table: str = Field()
     # 用于介绍存储场景
     _item_mode: ItemModeStr = Field()
@@ -56,48 +52,41 @@
         new_class = super().__new__(cls, class_name, bases, attrs)
 
         def add_field(
             self: Union[object, AyuItemTypeVar],
             key: Union[str, Any],
             value: Any = None,
         ) -> None:
-            """
-            动态添加字段方法
+            """动态添加字段方法
 
             Args:
                 self: self
                 key: 需要添加的字段名，这里类型为 str，为了消除 ide 的警告才加上了 Any
                 value: 需要添加的字段对应的值
-
-            Returns:
-                None
             """
             if not key:
                 raise EmptyKeyError()
             if key in self._AyuItem__fields:
                 raise FieldAlreadyExistsError(key)
             setattr(self, key, value)
             self._AyuItem__fields.add(key)
 
         def _asdict(
             self,
         ) -> Dict[str, Any]:
-            """
-            将 AyuItem 转换为 dict
-            """
+            """将 AyuItem 转换为 dict"""
             self._AyuItem__fields.discard("_AyuItem__fields")
             _item_dict = {key: getattr(self, key) for key in self._AyuItem__fields}
             return _item_dict
 
         def _asitem(
             self: Any,
             assignment: bool = True,
         ) -> ScrapyItem:
-            """
-            将 AyuItem 转换为 ScrapyItem
+            """将 AyuItem 转换为 ScrapyItem
 
             Args:
                 assignment: 是否将 AyuItem 中的值赋值给 ScrapyItem，默认为 True
 
             Returns:
                 new_class: 转换 ScrapyItem 后的实例
             """
@@ -112,16 +101,15 @@
         new_class._asdict = _asdict
         new_class._asitem = _asitem
         return new_class
 
 
 @dataclass
 class AyuItem(metaclass=ItemMeta):
-    """
-    用于创建和动态添加 item 字段，以及提供转换为 dict 和 ScrapyItem 的方法。
+    """用于创建和动态添加 item 字段，以及提供转换为 dict 和 ScrapyItem 的方法。
 
     Attributes:
         _table: 数据库表名。
         _mongo_update_rule: MongoDB 存储场景下可能需要的查重条件，默认为 None。
         __fields: 为保护字段，用于存放所有字段名，不用理会。
 
     Examples:
@@ -156,16 +144,15 @@
 
     def __init__(
         self,
         _table: str,
         _mongo_update_rule: Dict[str, Any] = None,
         **kwargs,
     ):
-        """
-        初始化 AyuItem 实例
+        """初始化 AyuItem 实例
 
         Args:
             _table: 数据库表名。
             _mongo_update_rule: MongoDB 存储场景下可能需要的查重条件，默认为 None。
         """
         self.__fields = set()
         if _table:
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/middlewares.py` & `ayugespidertools-3.3.2/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/mongoclient.py` & `ayugespidertools-3.3.2/ayugespidertools/mongoclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 
 __all__ = [
     "MongoDbBase",
 ]
 
 
 class MongoDbBase:
-    """
-    mongodb 数据库的相关操作（此功能暂时为残废状态，请参考 pymilk 库中的实现）
-    """
+    """mongodb 数据库的相关操作（此功能暂时为残废状态，请参考 pymilk 库中的实现）"""
 
     def __init__(
         self,
         user: str,
         password: str,
         host: str,
         port: int,
         authsource: str = "admin",
         database: str = None,
         connect_style: str = None,
     ) -> None:
-        """
-        初始化 mongo 连接句柄
+        """初始化 mongo 连接句柄
+
         Args:
             user: 用户名
             password: 用户对应的密码
             host: mongoDB 链接需要的 host
             port: mongoDB 链接需要的端口
             authsource: mongoDB 身份验证需要的数据库名称，默认为 admin
             database: mongoDB 链接需要的数据库
@@ -62,65 +60,65 @@
         else:
             raise ValueError("你指定错误了 connect_style 的 mongo 链接类型，请正确输入！")
 
         if database:
             self.db = self.init_db(database)
 
     def get_state(self):
-        """
-        获取 mongoDB 链接状态
+        """获取 mongoDB 链接状态
+
         Returns:
             1). bool: 链接是否正常
         """
         return all([self.conn is not None, self.db is not None])
 
     def init_db(self, database: str):
-        """
-        指定链接的数据库为 database
+        """指定链接的数据库为 database
+
         Args:
             database: 链接的目标数据库
 
         Returns:
             1). connect: 数据库链接
         """
         return self.conn[database]
 
     def insert_one(self, collection: str, data: dict) -> str:
-        """
-        插入一条数据
+        """插入一条数据
+
         Args:
             collection: 集合名称
             data: 插入的数据
 
         Returns:
             inserted_id: 成功返回的 id
         """
         if self.get_state():
             ret = self.db[collection].insert_one(data)
             return ret.inserted_id
         return ""
 
     def insert_many(self, collection: str, data: List[Dict]):
-        """
-        批量插入
+        """批量插入
+
         Args:
             collection: 集合名称
             data: 插入的数据数组
 
         Returns:
             inserted_ids: list: 成功返回的 ids
         """
         if self.get_state():
             ret = self.db[collection].insert_many(data)
             return ret.inserted_ids
         return ""
 
     def update(self, collection, data):
-        """
-        更新
+        """更新
+
         Args:
             collection: 集合名称
             data: 更新的数据，{key:[old_data,new_data]}
 
         Returns:
             modified_count: 更新影响的个数
         """
@@ -134,16 +132,16 @@
                 self.db[collection]
                 .update_many(data_filter, {"$set": data_revised})
                 .modified_count
             )
         return 0
 
     def find(self, collection, condition, column: Optional[dict] = None):
-        """
-        查询
+        """查询
+
         Args:
             collection: 集合名称
             condition: 查询条件
             column:
 
         Returns:
             1). 查询条件的搜索结果
@@ -171,16 +169,16 @@
         return (
             self.db[collection]
             .update_one({s_key: s_value}, {"$set": {data_style: update_data}})
             .modified_count
         )
 
     def update_super(self, collection: str, select_dict: dict, set_dict: dict):
-        """
-        更新
+        """更新
+
         Args:
             collection: 需要更新的集合
             select_dict: 更新的条件
             set_dict: 更新的内容
 
         Returns:
             1). modified_count: int: 更新影响的数量
@@ -211,16 +209,16 @@
         gridfs_col = GridFS(self.db, collection)
         gf = gridfs_col.get(_id)
         md5 = gf.md5
         _id = gf._id
         return {"_id": _id, "md5": md5}
 
     def upload(self, file_name, _id, content_type, collection, file_data):
-        """
-        上传文件
+        """上传文件
+
         Args:
             file_name: 上传至 mongoDB 的 GridFS 存储桶里的文件名
             _id: 唯一 id，雪花 id，用来标识此上传任务和图片的唯一
             content_type: 上传文件的类型，示例：image/jpeg
             collection: 存储至 GridFS 存储桶名称
             file_data: 文件的 bytes 内容
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.3.2/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/oss.py` & `ayugespidertools-3.3.2/ayugespidertools/oss.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,33 @@
 
 __all__ = [
     "AliOssBase",
 ]
 
 
 class AliOssBase:
-    """
-    阿里云 Oss 对象存储 python sdk 示例
+    """阿里云 Oss 对象存储 python sdk 示例
     其 GitHub 官方文档地址：
         https://github.com/aliyun/aliyun-oss-python-sdk?spm=5176.8465980.tools.dpython-github.572b1450ON6Z9R
     阿里云官方 oss sdk 文档地址：
         https://www.alibabacloud.com/help/zh/object-storage-service/latest/python-quick-start
     """
 
     def __init__(
         self,
         access_key_id: str,
         access_key_secret: str,
         endpoint: str,
         bucket: str,
         doc: str,
     ) -> None:
-        """
-        初始化 auth，bucket 等信息
+        """初始化 auth，bucket 等信息
         注：阿里云账号 AccessKey 拥有所有 API 的访问权限，风险很高；
-            强烈建议您创建并使用 RAM 用户进行 API 访问或日常运维，请登录 RAM 控制台创建 RAM 用户
+        强烈建议您创建并使用 RAM 用户进行 API 访问或日常运维，请登录 RAM 控制台创建 RAM 用户
+
         Args:
             access_key_id: 阿里云账号 AccessKey
             access_key_secret: 阿里云账号 AccessKey 对应的秘钥
             endpoint: 填写 Bucket 所在地域对应的 Endpoint；
                 以华东1（杭州）为例，Endpoint 填写为 https://oss-cn-hangzhou.aliyuncs.com（注意二级域名等问题）
             bucket: 填写 Bucket 名称，此 oss 项目所属 bucket
             doc: 需要操作的 oss 文件夹目录
@@ -48,21 +47,18 @@
         self.doc = doc
         self.bucket = bucket
         self.auth = oss2.Auth(access_key_id, access_key_secret)
         self.bucket = oss2.Bucket(self.auth, f"{self.endpoint}/", self.bucket)
         self.headers = {"Connection": "close"}
 
     def delete_oss(self, del_logo_url: str):
-        """
-        删除单个文件: 以下代码用于删除 bucket 中的 del_logo_url 所对应的文件
+        """删除单个文件: 以下代码用于删除 bucket 中的 del_logo_url 所对应的文件
+
         Args:
             del_logo_url: 需要参数的阿里云链接全路径 url
-
-        Returns:
-            None
         """
         try:
             self.bucket.delete_object(
                 f"{self.doc}/{del_logo_url.replace(f'{self.endpoint}/{self.doc}/', '')}"
             )
         except oss2.exceptions.NoSuchKey as e:
             raise ValueError(
@@ -75,16 +71,16 @@
     def put_oss(
         self,
         put_bytes_or_url: Union[str, bytes],
         file_name: str,
         file_format: str,
         file_name_md5: bool = False,
     ) -> (bool, str):
-        """
-        上传单个文件的 bytes 内容
+        """上传单个文件的 bytes 内容
+
         Args:
             put_bytes_or_url: 需要上传的文件 bytes 内容或链接
             file_name: 需要上传的文件的名称
             file_format: 需要上传的文件格式，比如：jpg, png, wav 等
             file_name_md5: 文件名称是否需要 md5 处理
 
         Returns:
@@ -111,16 +107,16 @@
         return True, input_file_name
 
     def enumer_file_by_pre(
         self,
         prefix: str,
         count_by_type: Union[Param.Str_Lstr, Param.NoneType, list] = None,
     ) -> list:
-        """
-        列举 prefix 文件夹下的所有的 count_by_type 类型的文件元素
+        """列举 prefix 文件夹下的所有的 count_by_type 类型的文件元素
+
         Args:
             prefix: 文件夹目录
             count_by_type: 统计的依据，计数文件夹中的此类型的元素
                 参数示例如下:
                     1. amr
                     2. ["amr", "mp3", "m4a", "wav", "aac", "ogg", "flac", "wma"]
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/pipelines.py` & `ayugespidertools-3.3.2/ayugespidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 __all__ = [
     "AiohttpRequest",
 ]
 
 
 class AiohttpRequest(Request):
-    """
-    为 scrapy 的 Request 对象添加额外的参数
-    """
+    """为 scrapy 的 Request 对象添加额外的参数"""
 
     def __init__(
         self,
         url: str,
         callback: Optional[Callable] = None,
         method: str = "GET",
         headers: Optional[dict] = None,
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/http/request/form.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 __all__ = [
     "AiohttpFormRequest",
 ]
 
 
 class AiohttpFormRequest(AiohttpRequest, FormRequest):
-    """
-    使用 aiohttp 发送 FormRequest 请求
-    """
+    """使用 aiohttp 发送 FormRequest 请求"""
 
     def __init__(
         self,
         url=None,
         callback=None,
         method=None,
         formdata=None,
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 __all__ = [
     "RandomRequestUaMiddleware",
 ]
 
 
 class RandomRequestUaMiddleware:
-    """
-    随机请求头中间件
-    """
+    """随机请求头中间件"""
 
     def __init__(self):
         self.explorer_types = None
         self.explorer_weights = None
 
     def get_random_ua_by_weight(self) -> str:
         # 先按权重取出所需浏览器类型
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,36 +17,34 @@
 __all__ = [
     "AiohttpDownloaderMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
 ]
 
 
 class AiohttpDownloaderMiddleware:
-    """
-    Downloader middleware handling the requests with aiohttp
-    """
+    """Downloader middleware handling the requests with aiohttp"""
 
     def __init__(self):
         self.aiohttp_args = None
 
     def _retry(
         self,
         request: scrapy.Request,
         reason: int,
         spider: scrapy.Spider,
     ) -> Union[scrapy.Request, None]:
-        """
-        重试请求
+        """重试请求
+
         Args:
             request: scrapy request
             reason: reason
             spider: scrapy spider
 
         Returns:
-            retry_req: 重试的 request 对象
+            Union[scrapy.Request, None]: 重试的 request 对象
         """
         retries = request.meta.get("retry_times", 0) + 1
         stats = spider.crawler.stats
         if retries <= self.retry_times:
             return self._retry_with_limit(request, retries, reason, stats)
 
         stats.inc_value("retry/max_reached")
@@ -64,28 +62,24 @@
             reason = global_object_name(reason.__class__)
 
         stats.inc_value("retry/count")
         stats.inc_value(f"retry/reason_count/{reason}")
         return retry_req
 
     def _get_args(self, key: str):
-        """
-        根据优先级依次获取不为 None 的请求参数
-        """
+        """根据优先级依次获取不为 None 的请求参数"""
         data_lst = [
             self.aiohttp_args.get(key),
             getattr(self, key),
         ]
         return ToolsForAyu.first_not_none(data_lst=data_lst)
 
     @classmethod
     def from_crawler(cls, crawler):
-        """
-        初始化 middleware
-        """
+        """初始化 middleware"""
         settings = crawler.settings
         # 自定义 aiohttp 全局配置信息，优先级小于 aiohttp_meta 中的配置
         if local_aiohttp_conf := settings.get("AIOHTTP_CONFIG", {}):
             # 这里的配置信息如果在 aiohttp_meta 中重复设置，则会更新当前请求的参数
             _aiohttp_conf = AiohttpConf(
                 timeout=local_aiohttp_conf.get("timeout"),
                 sleep=local_aiohttp_conf.get("sleep"),
@@ -119,17 +113,16 @@
 
     async def _request_by_aiohttp(
         self,
         aio_request_args: Param.ItemAdapterType,
         timeout: Optional[aiohttp.ClientTimeout] = None,
         connector: Optional[BaseConnector] = None,
     ) -> (int, str):
-        """
-        使用 aiohttp 来请求
-        ps: 后续考虑是否需要使用 aiohttp.ClientSession 来处理 cookies
+        """使用 aiohttp 来请求
+
         Args:
             aio_request_args: 普通的 aiohttp 请求参数
             timeout: aiohttp.ClientSession 的 timeout 参数
             connector: aiohttp connector 参数
 
         Returns:
             1). status_code: 请求状态码
@@ -143,17 +136,15 @@
                     status_code = response.status
                     response_text = await response.text()
                     return status_code, response_text
         except aiohttp.ClientTimeout:
             return 504, ""
 
     async def _process_request(self, request, spider):
-        """
-        使用 aiohttp 来 process spider
-        """
+        """使用 aiohttp 来 process spider"""
         aiohttp_options = request.meta.get("aiohttp")
         self.aiohttp_args = aiohttp_options.setdefault("args", {})
 
         # 根据 LOCAL_AIOHTTP_CONFIG 中设置 aiohttp 请求参数，这里的参数全局生效，不会在 meta 中更新
         _connector = aiohttp.TCPConnector(
             ssl=self.ssl,
             limit=self.limit,
@@ -244,32 +235,30 @@
             headers=aiohttp_req_args.headers,
             body=body,
             encoding="utf-8",
             request=request,
         )
 
     def process_request(self, request, spider):
-        """
-        使用 aiohttp 来 process request
+        """使用 aiohttp 来 process request
+
         Args:
             request: AiohttpRequest 对象
             spider: scrapy spider
 
         Returns:
             1). Deferred
         """
         return ReuseOperation.as_deferred(self._process_request(request, spider))
 
     async def _spider_closed(self):
         pass
 
     def spider_closed(self):
-        """
-        当 spider closed 时调用
-        """
+        """当 spider closed 时调用"""
         return ReuseOperation.as_deferred(self._spider_closed())
 
 
 class AiohttpAsyncDownloaderMiddleware(AiohttpDownloaderMiddleware):
     """aiohttp 协程的另一种实现方法，简化 process_request 方法"""
 
     async def process_request(self, request, spider):
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from scrapy import signals
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
 
 
 class DynamicProxyDownloaderMiddleware:
-    """
-    动态隧道代理中间件
-    """
+    """动态隧道代理中间件"""
 
     def __init__(self):
         self.proxy_url = None
         self.username = None
         self.password = None
 
     @classmethod
@@ -50,21 +48,19 @@
 
         self.proxy_url = spider.dynamicproxy_conf.proxy
         self.username = spider.dynamicproxy_conf.username
         self.password = spider.dynamicproxy_conf.password
 
 
 class AbuDynamicProxyDownloaderMiddleware:
-    """
-    阿布云动态代理 - 隧道验证方式（其实和快代理的写法一致）
-    """
+    """阿布云动态代理 - 隧道验证方式（其实和快代理的写法一致）"""
 
     def __init__(self, settings):
-        """
-        从 scrapy 配置中取出动态隧道代理的信息
+        """从 scrapy 配置中取出动态隧道代理的信息
+
         Args:
             settings: scrapy 配置信息
         """
         dynamic_proxy_conf = settings.get("DYNAMIC_PROXY_CONFIG", None)
         # 查看动态隧道代理配置是否符合要求
         is_match = ReuseOperation.is_dict_meet_min_limit(
             dict_conf=dynamic_proxy_conf,
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 __all__ = [
     "ExclusiveProxyDownloaderMiddleware",
 ]
 
 
 class ExclusiveProxyDownloaderMiddleware:
-    """
-    独享代理中间件
-    """
+    """独享代理中间件"""
 
     def __init__(self):
         self.proxy_url = None
         self.username = None
         self.password = None
         self.proxy_index = None
         # 从 proxy_list 中取出索引为 proxy_index 的值
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 __all__ = [
     "FilesDownloadPipeline",
 ]
 
 
 class FilesDownloadPipeline:
-    """
-    文件下载的 scrapy pipeline 扩展
-    """
+    """文件下载的 scrapy pipeline 扩展"""
 
     _type = "normal"
 
     def __init__(self, file_path=None, doc_path=None):
         self.file_path = file_path or doc_path
 
     @classmethod
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import motor.motor_asyncio
 
 from ayugespidertools.common.mongodbpipe import AsyncioAsynchronous
 from ayugespidertools.common.multiplexing import ReuseOperation
 
 
 class AsyncMongoPipeline:
-    """
-    通过 motor 实现异步写入 MongoDB 的存储管道
-    """
+    """通过 motor 实现异步写入 MongoDB 的存储管道"""
 
     def open_spider(self, spider):
         assert hasattr(
             spider, "mongodb_conf"
         ), "未配置 MongoDB 连接信息，请查看 .conf 或 consul 上对应配置信息！"
 
         _encoded_pwd = urllib.parse.quote_plus(spider.mongodb_conf.password)
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 __all__ = [
     "AyuFtyMongoPipeline",
 ]
 
 
 class AyuFtyMongoPipeline(MongoDbBase):
-    """
-    MongoDB 存储场景的 scrapy pipeline 扩展
-    """
+    """MongoDB 存储场景的 scrapy pipeline 扩展"""
 
     def __init__(self):
         self.conn = None
         self.db = None
 
     def open_spider(self, spider):
         assert hasattr(
@@ -37,18 +35,18 @@
             )
 
     def close_spider(self, spider):
         if self.conn:
             self.conn.close()
 
     def process_item(self, item, spider):
-        """
-        mongoDB 存储的方法，item["mongo_update_rule"] 用于存储查询条件，如果查询数据存在的话就更新，不存在的话就插入；
-        如果没有 mongo_update_rule 则每次都新增
-        此场景不需要像 Mysql 一样依赖备注来生成字段注释
+        """mongoDB 存储的方法，item["mongo_update_rule"] 用于存储查询条件，如果查询数据存在的话就更新，不存在
+        的话就插入；如果没有 mongo_update_rule 字段则每次都新增。
+        另外，此场景不需要像 Mysql 一样依赖备注来生成字段注释
+
         Args:
             item: scrapy item
             spider: scrapy spider
 
         Returns:
             item: scrapy item
         """
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 __all__ = [
     "AyuTwistedMongoPipeline",
 ]
 
 
 class AyuTwistedMongoPipeline(AyuFtyMongoPipeline):
-    """
-    使用 twisted 的 adbapi 实现 mongoDB 存储场景下的异步操作
-    """
+    """使用 twisted 的 adbapi 实现 mongoDB 存储场景下的异步操作"""
 
     def __init__(self, *args, **kwargs):
         super(AyuTwistedMongoPipeline, self).__init__(*args, **kwargs)
 
     def spider_closed(self, spider):
         if self.conn:
             self.conn.close()
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/kafkapub.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 __all__ = [
     "AyuKafkaPipeline",
 ]
 
 
 class KafkaProducerClient:
     def __init__(self, bootstrap_servers: list) -> None:
-        """
-        kafka 生产者
+        """kafka 生产者
+
         Args:
             bootstrap_servers: kafka 服务地址
         """
         self.producer = KafkaProducer(
             bootstrap_servers=bootstrap_servers,
             key_serializer=lambda k: json.dumps(k).encode(),
             value_serializer=lambda v: json.dumps(v).encode(),
@@ -27,25 +27,22 @@
 
     def sendmsg(
         self,
         topic: str,
         value: dict,
         key: Optional[str] = None,
     ) -> None:
-        """
-        发送数据
+        """发送数据
+
         Args:
             topic: kafka topic
             value: message value. Must be type bytes, or be
                 serializable to bytes via configured value_serializer. If value
                 is None, key is required and message acts as a 'delete'.
             key: kafka key
-
-        Returns:
-            None
         """
         # Asynchronous by default
         future = (
             self.producer.send(
                 topic=topic,
                 value=value,
                 key=key,
@@ -63,23 +60,19 @@
             # offset = record_metadata.offset
             # logger.info(f"save success, partition: {partition}, offset: {offset}")
         except KafkaError:
             # Decide what to do if produce request failed...
             logger.error(f"save error, topic: {topic}, value: {value}, key: {key}")
 
     def on_send_success(self, *args, **kwargs):
-        """
-        发送成功回调函数，暂不做任何处理或提示
-        """
+        """发送成功回调函数，暂不做任何处理或提示"""
         return
 
     def on_send_error(self, data, key):
-        """
-        发送失败回调函数，只日志记录
-        """
+        """发送失败回调函数，只日志记录"""
         logger.error(f"send error, data: {data}, key: {key}")
         return
 
     def close_producer(self):
         if self.producer:
             self.producer.close()
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 __all__ = [
     "AyuMQPipeline",
 ]
 
 
 class AyuMQPipeline:
-    """
-    消息队列发布场景的 scrapy pipeline 扩展 - pika mq
-    """
+    """消息队列发布场景的 scrapy pipeline 扩展 - pika mq"""
 
     def __init__(self):
         self.channel = None
 
     def _dict_to_bytes(self, item: dict) -> bytes:
         item_json_str = json.dumps(item)
         return bytes(item_json_str, encoding="utf-8")
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,24 @@
 
 __all__ = [
     "AyuMysqlPipeline",
 ]
 
 
 class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
-    """
-    Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
-    """
+    """Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例"""
 
     def __init__(
         self,
         table_enum: Type[TableEnumTypeVar],
         env: str,
         record_log_to_mysql: Optional[bool] = False,
     ) -> None:
-        """
-        初始化 Mysql 链接所需要的信息
+        """初始化 Mysql 链接所需要的信息
+
         Args:
             table_enum: 数据表的枚举信息
             env: 当前程序部署环境名
             record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
         """
         self.table_enum = table_enum
         self.env = env
@@ -68,16 +66,16 @@
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
         self.conn = self._connect(self.mysql_conf)
         self.cursor = self.conn.cursor()
 
     def get_new_item(self, item_dict: Dict[str, Any]) -> AlterItem:
-        """
-        重新整合 item
+        """重新整合 item
+
         Args:
             item_dict: dict 类型的 item
 
         Returns:
             1). 整合后的 item
         """
         new_item = {}
@@ -105,22 +103,19 @@
         self.insert_item(
             alter_item=self.get_new_item(item_dict),
             table=item_dict["_table"],
         )
         return item
 
     def insert_item(self, alter_item: AlterItem, table: str):
-        """
-        通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
+        """通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
+
         Args:
             alter_item: 经过转变后的 item
             table: 数据库表名
-
-        Returns:
-            None
         """
         if not (new_item := alter_item.new_item):
             return
 
         note_dic = alter_item.notes_dic
         sql = self._get_sql_by_item(table=table, item=new_item)
 
@@ -163,23 +158,20 @@
 
         if self.conn:
             self.conn.close()
 
     def table_collection_statistics(
         self, spider_name: str, database: str, crawl_time: datetime.date
     ):
-        """
-        统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
+        """统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
+
         Args:
             spider_name: 爬虫脚本名称
             database: 数据库，保存程序采集记录保存的数据库
             crawl_time: 采集时间，程序运行时间
-
-        Returns:
-            None
         """
         sql = f"""
         select concat(
         'select "', TABLE_NAME, '", count(id) as num , crawl_time from ', TABLE_SCHEMA, '.', TABLE_NAME,
         ' where crawl_time = "{crawl_time}"') from information_schema.tables
         where TABLE_SCHEMA='{database}' and TABLE_NAME in
         (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
@@ -200,22 +192,19 @@
                     "crawl_time": str((row[2] or crawl_time)),
                 }
                 self.insert_table_statistics(table_statistics)
 
     def insert_table_statistics(
         self, data: dict, table: str = "table_collection_statistics"
     ):
-        """
-        插入统计数据到表中
+        """插入统计数据到表中
+
         Args:
             data: 需要统计的入库信息
             table: 存储表的名称
-
-        Returns:
-            None
         """
         create_table_sql = f"""
         CREATE TABLE IF NOT EXISTS `{table}` (
             `id` int(11) NOT NULL AUTO_INCREMENT,
             `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
             `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
             `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
@@ -233,22 +222,19 @@
         stop_max_attempt_number=Param.retry_num,
         wait_random_min=Param.retry_time_min,
         wait_random_max=Param.retry_time_max,
     )
     def insert_script_statistics(
         self, data: dict, table: str = "script_collection_statistics"
     ):
-        """
-        存储运行脚本的统计信息
+        """存储运行脚本的统计信息
+
         Args:
             data: 需要插入的 log 信息
             table: 存储表的名称
-
-        Returns:
-            None
         """
         self.cursor.execute(
             f"""
             CREATE TABLE IF NOT EXISTS `{table}` (
                 `id` int(11) NOT NULL AUTO_INCREMENT,
                 `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
                 `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
@@ -269,22 +255,19 @@
             """
         )
 
         sql = self._get_sql_by_item(table=table, item=data)
         self._log_record(sql=sql, data=tuple(data.values()) * 2)
 
     def _log_record(self, sql: str, data: Tuple) -> None:
-        """
-        执行日志记录的 sql 语句
+        """执行日志记录的 sql 语句
+
         Args:
             sql: sql 语句
             data: sql 语句中的参数
-
-        Returns:
-            None
         """
         try:
             if self.cursor.execute(sql, data):
                 self.conn.commit()
         except Exception as e:
             self.conn.rollback()
             self.slog.warning(f":{e}")
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 __all__ = [
     "AsyncMysqlPipeline",
     "AsyncNormalMysqlPipeline",
 ]
 
 
 class AsyncNormalMysqlPipeline(AyuMysqlPipeline):
-    """
-    通过 aiomysql 实现异步写入 Mysql 数据库的普通版本
-    """
+    """通过 aiomysql 实现异步写入 Mysql 数据库的普通版本"""
 
     def open_spider(self, spider):
         assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
 
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=spider.mysql_conf)
@@ -57,17 +55,15 @@
 
     def close_spider(self, spider):
         self.db.close()
         return ReuseOperation.as_deferred(self._close_spider())
 
 
 class AsyncMysqlPipeline(AyuMysqlPipeline):
-    """
-    通过 aiomysql 实现异步写入 Mysql 数据库的连接池版本
-    """
+    """通过 aiomysql 实现异步写入 Mysql 数据库的连接池版本"""
 
     def open_spider(self, spider):
         assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
 
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=spider.mysql_conf)
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 __all__ = [
     "AyuStatisticsMysqlPipeline",
 ]
 
 
 class AyuStatisticsMysqlPipeline(AyuMysqlPipeline):
-    """
-    Mysql 存储且记录脚本运行状态的简单示例
-    """
+    """Mysql 存储且记录脚本运行状态的简单示例"""
 
     # Note: 此方法暂用于测试
     def __init__(self, env):
         self.env = env
         self.slog = None
         self.conn = None
         self.cursor = None
@@ -33,22 +31,19 @@
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
 
         self.conn = self._connect(self.mysql_conf)
         self.cursor = self.conn.cursor()
 
     def insert(self, data_item, table):
-        """
-        插入数据
+        """插入数据
+
         Args:
             data_item: scrapy item
             table: 存储至 mysql 的表名
-
-        Returns:
-            None
         """
         data = dataclasses.asdict(data_item)
         sql = self._get_sql_by_item(table=table, item=data)
         self._log_record(sql=sql, data=tuple(data.values()) * 2)
 
     def close_spider(self, spider):
         log_info = self._get_log_by_spider(spider=spider, crawl_time=self.crawl_time)
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 __all__ = [
     "AyuTurboMysqlPipeline",
 ]
 
 
 class AyuTurboMysqlPipeline(AyuMysqlPipeline):
-    """
-    Mysql 存储场景的 scrapy pipeline 扩展，使用 dbutils.pooled_db 实现
-    """
+    """Mysql 存储场景的 scrapy pipeline 扩展，使用 dbutils.pooled_db 实现"""
 
     def __init__(self, pool_db_conf, *args, **kwargs):
         super(AyuTurboMysqlPipeline, self).__init__(*args, **kwargs)
         self.pool_db_conf = pool_db_conf
 
     @classmethod
     def from_crawler(cls, crawler):
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 
 __all__ = [
     "AyuTwistedMysqlPipeline",
 ]
 
 
 class AyuTwistedMysqlPipeline(AyuMysqlPipeline):
-    """
-    使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
-    注意：
-        1. 推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
+    """使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
+    注意：推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
     """
 
     def __init__(self, *args, **kwargs):
         super(AyuTwistedMysqlPipeline, self).__init__(*args, **kwargs)
         self.dbpool = None
 
     def open_spider(self, spider):
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.3.2/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
 __all__ = [
     "AyuSpider",
 ]
 
 
 class MySqlEngineClass:
-    """
-    mysql 链接句柄单例模式
-    """
+    """mysql 链接句柄单例模式"""
 
     _instance_lock = threading.Lock()
 
     def __init__(self, engine_url):
         self.engine = create_engine(
             engine_url, pool_pre_ping=True, pool_recycle=3600 * 7
         )
@@ -39,112 +37,91 @@
                 if not hasattr(MySqlEngineClass, "_instance"):
                     MySqlEngineClass._instance = object.__new__(cls)
 
         return MySqlEngineClass._instance
 
 
 class AyuSpider(Spider):
-    """
-    用于初始配置 scrapy 的各种 setting 的值及 spider 全局变量等
-    """
+    """用于初始配置 scrapy 的各种 setting 的值及 spider 全局变量等"""
 
-    # 自定义 common 设置
     custom_common_settings = {
         "ROBOTSTXT_OBEY": False,
         "TELNETCONSOLE_ENABLED": False,
         "RETRY_TIMES": 3,
         "DEPTH_PRIORITY": -1,
         "ENV": "dev",
     }
 
-    # 自定义 Debug 设置
     custom_debug_settings = {
-        # 日志等级
         "LOG_LEVEL": "DEBUG",
         "ROBOTSTXT_OBEY": False,
-        # 超时
         "DOWNLOAD_TIMEOUT": 20,
-        # 重试次数
         "RETRY_TIMES": 3,
-        # 禁用所有重定向
         "REDIRECT_ENABLED": False,
-        # 后进先出，深度优先
         "DEPTH_PRIORITY": -1,
-        # 环境
         "ENV": "test",
         # 数据库表枚举
         "DATA_ENUM": None,
         # 是否记录程序的采集情况基本信息到 Mysql 数据库
         "RECORD_LOG_TO_MYSQL": False,
     }
 
-    # 自定义 product 设置
     custom_product_settings = {
         "LOG_LEVEL": "ERROR",
         "ROBOTSTXT_OBEY": False,
         "DOWNLOAD_TIMEOUT": 20,
         "RETRY_TIMES": 3,
         "REDIRECT_ENABLED": False,
         "DEPTH_PRIORITY": -1,
         "ENV": "prod",
         "DATA_ENUM": None,
         "RECORD_LOG_TO_MYSQL": False,
     }
 
-    # 开始采集时间
     SPIDER_TIME = time.strftime("%Y-%m-%d", time.localtime())
     # 是否启用 Debug 参数，默认激活 custom_common_settings
     settings_type = "common"
     # 脚本信息
     project_content = ""
-    # 自定义数据库表枚举
     custom_table_enum = None
-    # 数据库引擎开关
     mysql_engine_enabled = False
 
     def parse(self, response, **kwargs):
-        """
-        实现所继承类的 abstract 方法 parse
-        """
+        """实现所继承类的 abstract 方法 parse"""
         super(AyuSpider, self).parse(response, **kwargs)
 
     def __init__(self, *args, **kwargs):
         super(AyuSpider, self).__init__(*args, **kwargs)
         self.mysql_engine = None
 
     @property
     def slog(self):
-        """
-        本库的日志管理模块，使用 loguru 来管理日志
-        注：
+        """本库的日志管理模块，使用 loguru 来管理日志
+        注意：
             1. 本库不是通过适配器模式或 mixin 等方法对 scrapy logger 重写或扩展，而是
         新增一个 slog 的日志管理方法，目前感觉这样最适合；
             2. 本配置可与 Scrapy 的 spider.log 同时管理，根据场景可以自行配置。
         """
-        # 设置 loguru 日志配置
         loguru_conf_tmp = self.crawler.settings.get("LOGURU_CONFIG")
-        # 是否开启 loguru 日志记录
         loguru_enabled = self.crawler.settings.get("LOGURU_ENABLED", True)
         assert isinstance(loguru_enabled, bool), "loguru_enabled 参数格式需要为 bool"
 
-        # 如果开启推荐的 loguru 日志管理功能
         if loguru_enabled:
-            # 则使用 LOGURU_CONFIG 下的配置，或直接使用统一管理的 logger
+            # 使用 LOGURU_CONFIG 下的配置，或直接使用统一管理的 logger
             return loguru_conf_tmp or logger
 
         # 如果关闭推荐的日志管理，则替换为 scrapy 的日志管理
         else:
             return super(AyuSpider, self).logger
 
     @classmethod
     def update_settings(cls, settings):
         custom_table_enum = getattr(cls, "custom_table_enum", None)
         # 设置类型，用于快速设置某些场景下的通用配置。比如测试 test 和生产 prod 下的通用配置；可不设置，默认为 common
         settings_type = getattr(cls, "settings_type", "common")
-        # 根据 settings_type 参数取出对应的 inner_settings 配置
         inner_settings = getattr(cls, f"custom_{settings_type}_settings", {})
 
         if custom_table_enum:
             inner_settings["DATA_ENUM"] = custom_table_enum
 
         if vit_dir := settings.get("VIT_DIR", None):
             # 根据 vit_dir 配置，获取对应的 inner_settings 配置
@@ -159,15 +136,14 @@
         settings.setdict(inner_settings, priority="project")
         settings.setdict(cls.custom_settings or {}, priority="spider")
 
     @classmethod
     def from_crawler(cls, crawler, *args, **kwargs):
         spider = super(AyuSpider, cls).from_crawler(crawler, *args, **kwargs)
         spider.stats = crawler.stats
-        # 先输出下相关日志，用于调试时查看
         spider.slog.debug(f"settings_type 配置: {cls.settings_type}")
 
         _consul_conf = ReuseOperation.get_consul_conf(settings=crawler.settings)
         # 以下将 .conf 中或 consul 中对应的配置信息，赋值给 spider 对象，方便后续使用
         if mysql_conf := get_spider_conf(
             MysqlConfCreator().create_product(crawler.settings, _consul_conf)
         ):
@@ -196,21 +172,19 @@
 
         if kafka_conf := get_spider_conf(
             KafkaConfCreator().create_product(crawler.settings, _consul_conf)
         ):
             spider.slog.debug("项目中配置了 kafka_conf 信息")
             spider.kafka_conf = kafka_conf
 
-        # 动态代理
         if dynamicproxy_conf := get_spider_conf(
             DynamicProxyCreator().create_product(crawler.settings, _consul_conf)
         ):
             spider.slog.debug("项目中配置了 dynamicproxy_conf 信息")
             spider.dynamicproxy_conf = dynamicproxy_conf
 
-        # 独享代理
         if exclusiveproxy_conf := get_spider_conf(
             ExclusiveProxyCreator().create_product(crawler.settings, _consul_conf)
         ):
             spider.slog.debug("项目中配置了 exclusiveproxy_conf 信息")
             spider.exclusiveproxy_conf = exclusiveproxy_conf
         return spider
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         "DOWNLOADER_MIDDLEWARES": {
             "ayugespidertools.middlewares.RandomRequestUaMiddleware": 400,
         },
     }
     mysql_engine_enabled = True
 
     def start_requests(self):
-        """
-        get 请求首页，获取项目列表数据
-        """
+        """get 请求首页，获取项目列表数据"""
         yield Request(
             url="https://blog.csdn.net/phoenix/web/blog/hot-rank?page=0&pageSize=25&type=",
             callback=self.parse_first,
             headers={
                 "referer": "https://blog.csdn.net/rank/list",
             },
             cb_kwargs={
```

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.3.2/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.3.2/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.3.1/ayugespidertools/verificationcode.py` & `ayugespidertools-3.3.2/ayugespidertools/verificationcode.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     "get_yidun_tracks",
     "get_yidun_gap",
     "get_normal_track",
 ]
 
 
 def match_img_get_distance(target, template):
-    """
-    网易易盾（dun163）滑块坐标定位方法，也使用于其它平台滑块验证码的情况
+    """网易易盾（dun163）滑块坐标定位方法，也使用于其它平台滑块验证码的情况
+
     Args:
         target: 1) 带缺口的背景图，全路径; 2) 或者是背景图的 bytes 数据
         template: 1） 滑块图，全路径; 2）或者是滑块图的 bytes 数据
 
     Returns:
         loc[1][0]: 滑块位置坐标
     """
@@ -71,16 +71,16 @@
             R -= (R - L) / 2
 
     # 返回 x 坐标
     return loc[1][0]
 
 
 def get_selenium_tracks(distance):
-    """
-    最简陋的根据缺口距离获取轨迹的方法，以供 selenium 使用
+    """最简陋的根据缺口距离获取轨迹的方法，以供 selenium 使用
+
     Args:
         distance: 滑块缺口的距离
 
     Returns:
         tracks_dict:
             forward_tracks: 往右划的轨迹数组
             back_tracks: 回退（往左划）的轨迹数组
@@ -102,16 +102,17 @@
         forward_tracks.append(round(s))
 
     back_tracks = [-3, -3, -2, -2, -2, -2, -2, -1, -1, -1]
     return {"forward_tracks": forward_tracks, "back_tracks": back_tracks}
 
 
 def get_yidun_tracks(distance):
-    """
-    网易易盾轨迹生成方法（不能直接用极验的轨迹生成和其它如（加减速、匀加速或者先加速后减速，甚至划过再划回）简单生成的方法），生成的轨迹数组中首个位移最好要大于等于 3
+    """网易易盾轨迹生成方法（不能直接用极验的轨迹生成和其它如（加减速、匀加速或者先加速后减速，甚至划过再划回）简单生成
+    的方法），生成的轨迹数组中首个位移最好要大于等于 3
+
     Args:
         distance: 滑块缺口的距离
 
     Returns:
         xyt: 网易易盾轨迹数组
     """
     t_list = [random.randint(50, 160)]
@@ -149,30 +150,30 @@
     xyt = list(zip(x_list, y_list, t_list))
     for j in range(length):
         xyt[j] = list(xyt[j])
     return xyt
 
 
 def get_yidun_gap(slide_img_path, bg_img_path, out_img_path: str = False) -> int:
-    """
-    获取易盾滑块缺口距离
+    """获取易盾滑块缺口距离
+
     Args:
         slide_img_path: 滑块的图片
         bg_img_path: 带缺口的背景图片
         out_img_path: 输出图片
 
     Returns:
         1). 易盾滑块缺口距离
     """
     return YiDunGetGap.discern(slide_img_path, bg_img_path, out_img_path)
 
 
 def get_normal_track(space):
-    """
-    通用的根据滑块距离获取轨迹数组方法
+    """通用的根据滑块距离获取轨迹数组方法
+
     Args:
         space: 滑块缺口距离
 
     Returns:
         tracks_list: 生成的轨迹数组
     """
     x = [0, 0]
```

### Comparing `ayugespidertools-3.3.1/pyproject.toml` & `ayugespidertools-3.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.3.1"
-description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
+version = "3.3.2"
+description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
 keywords = ["crawler", "scraping", "twisted", "aiohttp", "asyncio", "scrapy", "aiomysql", "mmh3"]
@@ -18,27 +18,25 @@
 PyMySQL = "^1.0.2"
 loguru = "~0.7.0"
 numpy = "~1.24.3"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
 Scrapy = "2.9.0"
 pandas = "^1.5.0"
-WorkWeixinRobot = "^1.0.1"
 retrying = "^1.3.3"
 SQLAlchemy = "^1.4.41"
 DBUtils = "^3.0.2"
 itemadapter = "^0.7.0"
 aiohttp = "^3.8.3"
 html2text = "^2020.1.16"
 pymongo = "^3.12.3"
 mmh3 = "^3.0.0"
 pycryptodome = "^3.15.0"
 oss2 = "^2.16.0"
 aiomysql = "^0.1.1"
-attrs = "^22.2.0"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
 urllib3 = "~1.26.15"
 pika = "~1.3.2"
 kafka-python = "2.0.2"
```

