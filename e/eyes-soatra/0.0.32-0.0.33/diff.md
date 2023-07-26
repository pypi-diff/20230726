# Comparing `tmp/eyes_soatra-0.0.32.tar.gz` & `tmp/eyes_soatra-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.32.tar", last modified: Wed Jul 19 04:03:07 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.33.tar", last modified: Wed Jul 26 02:39:48 2023, max compression
```

## Comparing `eyes_soatra-0.0.32.tar` & `eyes_soatra-0.0.33.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.079004 eyes_soatra-0.0.32/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.32/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-19 04:03:07.078759 eyes_soatra-0.0.32/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.32/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.067803 eyes_soatra-0.0.32/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.32/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.070017 eyes_soatra-0.0.32/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.32/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.070284 eyes_soatra-0.0.32/eyes_soatra/constant/area/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:26.000000 eyes_soatra-0.0.32/eyes_soatra/constant/area/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    19032 2023-06-14 01:12:10.000000 eyes_soatra-0.0.32/eyes_soatra/constant/area/id.py
--rw-r--r--   0 soatra     (501) staff       (20)      233 2023-06-14 03:16:23.000000 eyes_soatra-0.0.32/eyes_soatra/constant/classes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.070695 eyes_soatra-0.0.32/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.071555 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.072657 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.073189 eyes_soatra-0.0.32/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.32/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.32/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.073446 eyes_soatra-0.0.32/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.32/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.32/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.073663 eyes_soatra-0.0.32/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.32/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.32/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.32/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      174 2023-06-14 04:10:56.000000 eyes_soatra-0.0.32/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.075184 eyes_soatra-0.0.32/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.075412 eyes_soatra-0.0.32/eyes_soatra/funcs/listener/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:35.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/listener/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     9251 2023-06-14 07:16:46.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/listener/watch_changes.py
--rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-09 08:49:06.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.077311 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      602 2023-06-14 06:18:06.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/console.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)       82 2023-06-14 03:20:51.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/number.py
--rw-r--r--   0 soatra     (501) staff       (20)     2624 2023-06-14 04:22:54.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)       99 2023-06-14 06:54:22.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/utils/time.py
--rw-r--r--   0 soatra     (501) staff       (20)    14387 2023-07-19 03:59:47.000000 eyes_soatra-0.0.32/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.068672 eyes_soatra-0.0.32/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-19 04:03:07.000000 eyes_soatra-0.0.32/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1644 2023-07-19 04:03:07.000000 eyes_soatra-0.0.32/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-07-19 04:03:07.000000 eyes_soatra-0.0.32/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       34 2023-07-19 04:03:07.000000 eyes_soatra-0.0.32/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-07-19 04:03:07.000000 eyes_soatra-0.0.32/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-07-19 04:03:07.079058 eyes_soatra-0.0.32/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-07-19 04:02:29.000000 eyes_soatra-0.0.32/setup.py
--rw-r--r--   0 soatra     (501) staff       (20)     1123 2023-06-02 02:26:19.000000 eyes_soatra-0.0.32/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 04:03:07.078491 eyes_soatra-0.0.32/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.32/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.32/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      208 2023-07-19 03:59:18.000000 eyes_soatra-0.0.32/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.681699 eyes_soatra-0.0.33/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.33/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-26 02:39:48.681557 eyes_soatra-0.0.33/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.33/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.668738 eyes_soatra-0.0.33/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.33/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.670665 eyes_soatra-0.0.33/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.33/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.671181 eyes_soatra-0.0.33/eyes_soatra/constant/area/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:26.000000 eyes_soatra-0.0.33/eyes_soatra/constant/area/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    19032 2023-06-14 01:12:10.000000 eyes_soatra-0.0.33/eyes_soatra/constant/area/id.py
+-rw-r--r--   0 soatra     (501) staff       (20)      233 2023-06-14 03:16:23.000000 eyes_soatra-0.0.33/eyes_soatra/constant/classes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.671628 eyes_soatra-0.0.33/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.672499 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.673370 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.674077 eyes_soatra-0.0.33/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7309 2023-07-26 02:38:45.000000 eyes_soatra-0.0.33/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.33/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.674450 eyes_soatra-0.0.33/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.33/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.33/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.674842 eyes_soatra-0.0.33/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.33/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.33/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)    23799 2023-07-19 09:58:30.000000 eyes_soatra-0.0.33/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      234 2023-07-19 09:40:36.000000 eyes_soatra-0.0.33/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.678145 eyes_soatra-0.0.33/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.678534 eyes_soatra-0.0.33/eyes_soatra/funcs/listener/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:35.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/listener/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9251 2023-06-14 07:16:46.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/listener/watch_changes.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-09 08:49:06.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.680416 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      602 2023-06-14 06:18:06.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/console.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)       82 2023-06-14 03:20:51.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/number.py
+-rw-r--r--   0 soatra     (501) staff       (20)     3013 2023-07-19 09:42:29.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)       99 2023-06-14 06:54:22.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/utils/time.py
+-rw-r--r--   0 soatra     (501) staff       (20)    14387 2023-07-19 03:59:47.000000 eyes_soatra-0.0.33/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.669748 eyes_soatra-0.0.33/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-26 02:39:48.000000 eyes_soatra-0.0.33/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1644 2023-07-26 02:39:48.000000 eyes_soatra-0.0.33/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-07-26 02:39:48.000000 eyes_soatra-0.0.33/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       34 2023-07-26 02:39:48.000000 eyes_soatra-0.0.33/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-07-26 02:39:48.000000 eyes_soatra-0.0.33/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-07-26 02:39:48.681748 eyes_soatra-0.0.33/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-07-26 02:39:31.000000 eyes_soatra-0.0.33/setup.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1123 2023-06-02 02:26:19.000000 eyes_soatra-0.0.33/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-26 02:39:48.681214 eyes_soatra-0.0.33/test/
+-rw-r--r--   0 soatra     (501) staff       (20)      577 2023-07-20 07:12:14.000000 eyes_soatra-0.0.33/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)      223 2023-07-26 02:34:26.000000 eyes_soatra-0.0.33/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)      150 2023-07-19 10:04:31.000000 eyes_soatra-0.0.33/test/test3.py
```

### Comparing `eyes_soatra-0.0.32/PKG-INFO` & `eyes_soatra-0.0.33/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.32
+Version: 0.0.33
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/area/id.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/area/id.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/depends/view/not_found.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     "エラー404 お探しのページは存在しません。",
     "エラーが発生しました",
     "エラーが発生しました。",
     "エラーページ",
     "コンテンツを表示することができません",
     "コンテンツを表示することができません。",
     "サーバー エラーが発生しました。（タイムアウトの可能性もあります）",
-    "システムエラー",
     "ファイルが見つかりません",
     "ページがみつかりません",
     "ページがみつかりません - 404 Not Found -",
     "ページがみつかりませんでした",
     "ページが見つかりません",
     "ページが見つかりません Not Found",
     "ページが見つかりません （404 Not Found)",
```

### Comparing `eyes_soatra-0.0.32/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.33/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/funcs/listener/watch_changes.py` & `eyes_soatra-0.0.33/eyes_soatra/funcs/listener/watch_changes.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.33/eyes_soatra/funcs/time_app.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/funcs/utils/console.py` & `eyes_soatra-0.0.33/eyes_soatra/funcs/utils/console.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.33/eyes_soatra/funcs/utils/string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+#!python3
 from eyes_soatra.constant.vars import xpath_prefix as __xpath_prefix
 from eyes_soatra.constant.vars import tag_stop as __tag_stop
 from eyes_soatra.constant.vars import protocols as __protocols
+from eyes_soatra.constant.vars import invisibles as __invisibles
+from eyes_soatra.funcs.utils.list import map_list as __map_list
 import re as __re
 
 def strip_space(text):
     return __re.sub(r'\s+', ' ', text).strip()
 
 def symbol(string):
     temp_symbol = True
@@ -111,7 +114,14 @@
         return True
 
     return False
 
 def clean_url(url):
     if url:
         return __re.sub(r'\s+', '', remove_slash(url))
+    
+    
+def remove_invisible(string: str):
+    unicodes = '|'.join(__map_list(lambda each: f'\\\\{each}', __invisibles))
+    __string = __re.sub (unicodes.encode(), b'', string.encode('unicode_escape'))
+
+    return __string.decode('unicode_escape')
```

### Comparing `eyes_soatra-0.0.32/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.33/eyes_soatra/funcs/view_page.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.32/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.33/eyes_soatra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.32
+Version: 0.0.33
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.32/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.33/eyes_soatra.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,9 +40,9 @@
 eyes_soatra/funcs/utils/console.py
 eyes_soatra/funcs/utils/dict.py
 eyes_soatra/funcs/utils/list.py
 eyes_soatra/funcs/utils/number.py
 eyes_soatra/funcs/utils/string.py
 eyes_soatra/funcs/utils/time.py
 test/test.py
-test/test1.py
-test/test2.py
+test/test2.py
+test/test3.py
```

### Comparing `eyes_soatra-0.0.32/setup.py` & `eyes_soatra-0.0.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.32'
+VERSION = '0.0.33'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.32/start.py` & `eyes_soatra-0.0.33/start.py`

 * *Files identical despite different names*

