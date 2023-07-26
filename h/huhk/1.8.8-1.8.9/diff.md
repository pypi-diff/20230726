# Comparing `tmp/huhk-1.8.8.tar.gz` & `tmp/huhk-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.8.8.tar", last modified: Wed Jul 26 08:43:19 2023, max compression
+gzip compressed data, was "huhk-1.8.9.tar", last modified: Wed Jul 26 08:46:36 2023, max compression
```

## Comparing `huhk-1.8.8.tar` & `huhk-1.8.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.258850 huhk-1.8.8/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:43:19.255858 huhk-1.8.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.188490 huhk-1.8.8/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.8.8/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.407540 huhk-1.8.8/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.8.8/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21410 2023-07-26 08:38:20.000000 huhk-1.8.8/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.8.8/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    17860 2023-07-26 08:42:52.000000 huhk-1.8.8/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.8.8/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-26 08:43:13.000000 huhk-1.8.8/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    12802 2023-07-26 08:10:46.000000 huhk-1.8.8/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.8.8/huhk/main.py
--rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.8.8/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.415518 huhk-1.8.8/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.657355 huhk-1.8.8/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.8.8/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.8.8/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.8.8/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.8.8/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28433 2023-07-26 06:32:08.000000 huhk-1.8.8/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.8.8/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.8.8/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.8.8/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.282522 huhk-1.8.8/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:43:14.000000 huhk-1.8.8/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2839 2023-07-26 08:43:15.000000 huhk-1.8.8/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:43:14.000000 huhk-1.8.8/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-26 08:43:14.000000 huhk-1.8.8/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-26 08:43:14.000000 huhk-1.8.8/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 08:43:14.000000 huhk-1.8.8/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:16.778059 huhk-1.8.8/service/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.749200 huhk-1.8.8/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.8.8/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.765157 huhk-1.8.8/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.8/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.778123 huhk-1.8.8/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.814026 huhk-1.8.8/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    35088 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    36705 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.871510 huhk-1.8.8/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    48149 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    39604 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.8.8/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.877497 huhk-1.8.8/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.8/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.891457 huhk-1.8.8/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.929356 huhk-1.8.8/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:18.989195 huhk-1.8.8/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.8.8/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.022108 huhk-1.8.8/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.8.8/service/app_t/funs/__init__.py
--rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.8.8/service/app_t/funs/funs_app_t.py
--rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.8.8/service/app_t/funs/funs_open.py
--rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.8.8/service/app_t/funs/funs_points.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.042062 huhk-1.8.8/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.8/service/app_t/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.8.8/service/app_t/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.062375 huhk-1.8.8/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.8/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.123212 huhk-1.8.8/service/app_t/funs/points/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.8.8/service/app_t/funs/points/__init__.py
--rw-rw-rw-   0        0        0     3201 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/funs/points/funs_points_points.py
--rw-rw-rw-   0        0        0     2040 2023-07-26 08:10:30.000000 huhk-1.8.8/service/app_t/funs/points/funs_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.130193 huhk-1.8.8/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.8/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.147148 huhk-1.8.8/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.191036 huhk-1.8.8/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:43:19.245887 huhk-1.8.8/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.8.8/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-26 08:43:19.259847 huhk-1.8.8/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.824959 huhk-1.8.9/
+-rw-rw-rw-   0        0        0      223 2023-07-26 08:46:36.823970 huhk-1.8.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.597446 huhk-1.8.9/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.8.9/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.641948 huhk-1.8.9/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.8.9/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21410 2023-07-26 08:38:20.000000 huhk-1.8.9/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.8.9/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    17878 2023-07-26 08:45:18.000000 huhk-1.8.9/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.8.9/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    12802 2023-07-26 08:10:46.000000 huhk-1.8.9/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.8.9/huhk/main.py
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.8.9/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.643947 huhk-1.8.9/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.693814 huhk-1.8.9/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.8.9/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.8.9/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.8.9/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.8.9/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28433 2023-07-26 06:32:08.000000 huhk-1.8.9/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.8.9/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.8.9/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.8.9/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.615395 huhk-1.8.9/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 08:46:36.000000 huhk-1.8.9/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.541837 huhk-1.8.9/service/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.702787 huhk-1.8.9/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.8.9/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.704782 huhk-1.8.9/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.708771 huhk-1.8.9/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.718752 huhk-1.8.9/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    35088 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    36705 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.727721 huhk-1.8.9/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    48149 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    39604 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.8.9/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.730713 huhk-1.8.9/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.733705 huhk-1.8.9/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.743759 huhk-1.8.9/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.753534 huhk-1.8.9/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.8.9/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.766505 huhk-1.8.9/service/app_t/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.8.9/service/app_t/funs/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.8.9/service/app_t/funs/funs_app_t.py
+-rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.8.9/service/app_t/funs/funs_open.py
+-rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.8.9/service/app_t/funs/funs_points.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.771492 huhk-1.8.9/service/app_t/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.9/service/app_t/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.8.9/service/app_t/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.780068 huhk-1.8.9/service/app_t/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.9/service/app_t/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      959 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.790042 huhk-1.8.9/service/app_t/funs/points/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.8.9/service/app_t/funs/points/__init__.py
+-rw-rw-rw-   0        0        0     3201 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/points/funs_points_points.py
+-rw-rw-rw-   0        0        0     2040 2023-07-26 08:10:30.000000 huhk-1.8.9/service/app_t/funs/points/funs_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.792036 huhk-1.8.9/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.9/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.796026 huhk-1.8.9/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.806996 huhk-1.8.9/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:46:36.818982 huhk-1.8.9/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.8.9/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:46:36.824959 huhk-1.8.9/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.8.9/setup.py
```

### Comparing `huhk-1.8.8/huhk/__init__.py` & `huhk-1.8.9/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/case_project/json_coder.py` & `huhk-1.8.9/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/case_project/main_fun.py` & `huhk-1.8.9/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/case_project/project_base.py` & `huhk-1.8.9/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/case_project/project_init.py` & `huhk-1.8.9/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/case_project/project_string.py` & `huhk-1.8.9/huhk/case_project/project_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         api_fun_fun_str += '\n' if data_list else ''
         api_fun_fun_str += "        _kwargs = self.get_kwargs(locals())\n"
         api_fun_fun_str += f"        self.res = {api_path.import_path.rsplit('.', 1)[1]}.{fun_name}(**_kwargs)\n\n"
         api_fun_fun_str += "        self.assert_%s(_assert, **_kwargs)\n" % fun_name
         if set(api.input) & set(self.page_and_size) or str(api.method).lower() == "get":
             api_fun_fun_str += "        self.set_output_value(_kwargs)\n"
         api_fun_fun_str += "        self.set_value(_kwargs)\n\n\n"
-        api_fun_fun_str.replace(", , ", ", ")
+        api_fun_fun_str = api_fun_fun_str.replace(", , ", ", ")
         return api_fun_fun_str
 
     def get_api_testcase_header_str(self, fun_name):
         api = self.this_fun_list.api[fun_name]
         header_str = "import allure\n\n"
         header_str += f"from service.{self.name}.funs.funs_{self.name} " \
                       f"import Funs{self.name.title().replace('_', '')}\n\n\n"
```

### Comparing `huhk-1.8.8/huhk/case_project/setup_set.py` & `huhk-1.8.9/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/init_project.py` & `huhk-1.8.9/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/main.py` & `huhk-1.8.9/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/beam_class.py` & `huhk-1.8.9/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/data.py` & `huhk-1.8.9/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/par_do.py` & `huhk-1.8.9/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.8.9/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_fiter.py` & `huhk-1.8.9/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_flatmap.py` & `huhk-1.8.9/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_map.py` & `huhk-1.8.9/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_par_do.py` & `huhk-1.8.9/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_regex.py` & `huhk-1.8.9/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/testcase/apache/test_time.py` & `huhk-1.8.9/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_apache_beam.py` & `huhk-1.8.9/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_dict.py` & `huhk-1.8.9/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_encryption.py` & `huhk-1.8.9/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_fun.py` & `huhk-1.8.9/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_logger.py` & `huhk-1.8.9/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_request.py` & `huhk-1.8.9/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/unit_tasks.py` & `huhk-1.8.9/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk/常用命令.py` & `huhk-1.8.9/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/huhk.egg-info/SOURCES.txt` & `huhk-1.8.9/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.8.9/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/apis/points/apis_points_points.py` & `huhk-1.8.9/service/app_t/apis/points/apis_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.8.9/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/app_t_fun.py` & `huhk-1.8.9/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.8.9/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.8.9/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.8.9/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.8.9/service/app_t/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/funs/points/funs_points_points.py` & `huhk-1.8.9/service/app_t/funs/points/funs_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/funs/points/funs_points_pointsApp.py` & `huhk-1.8.9/service/app_t/funs/points/funs_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.8.9/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.8.9/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.8/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.8.9/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

