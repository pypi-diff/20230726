# Comparing `tmp/huhk-1.8.6.tar.gz` & `tmp/huhk-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.8.6.tar", last modified: Wed Jul 26 08:26:02 2023, max compression
+gzip compressed data, was "huhk-1.8.7.tar", last modified: Wed Jul 26 08:38:53 2023, max compression
```

## Comparing `huhk-1.8.6.tar` & `huhk-1.8.7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.958062 huhk-1.8.6/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:26:02.958062 huhk-1.8.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.772813 huhk-1.8.6/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.8.6/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.807257 huhk-1.8.6/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.8.6/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21333 2023-07-26 08:11:21.000000 huhk-1.8.6/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.8.6/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    17089 2023-07-26 06:37:18.000000 huhk-1.8.6/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.8.6/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    12802 2023-07-26 08:10:46.000000 huhk-1.8.6/huhk/init_project.py
--rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.8.6/huhk/main.py
--rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.8.6/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.809249 huhk-1.8.6/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.852806 huhk-1.8.6/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.8.6/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.8.6/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.8.6/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.8.6/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28433 2023-07-26 06:32:08.000000 huhk-1.8.6/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.8.6/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.8.6/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.8.6/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.785780 huhk-1.8.6/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2839 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 08:26:02.000000 huhk-1.8.6/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.734484 huhk-1.8.6/service/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.859758 huhk-1.8.6/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.8.6/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.862750 huhk-1.8.6/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.6/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.865742 huhk-1.8.6/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.874719 huhk-1.8.6/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    35088 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    36705 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.881699 huhk-1.8.6/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    48149 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    39604 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.8.6/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.883694 huhk-1.8.6/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.6/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.886721 huhk-1.8.6/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.895697 huhk-1.8.6/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.904674 huhk-1.8.6/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.8.6/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.914513 huhk-1.8.6/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.8.6/service/app_t/funs/__init__.py
--rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.8.6/service/app_t/funs/funs_app_t.py
--rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.8.6/service/app_t/funs/funs_open.py
--rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.8.6/service/app_t/funs/funs_points.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.918539 huhk-1.8.6/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.6/service/app_t/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.8.6/service/app_t/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.925490 huhk-1.8.6/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.6/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      871 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      959 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.932482 huhk-1.8.6/service/app_t/funs/points/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.8.6/service/app_t/funs/points/__init__.py
--rw-rw-rw-   0        0        0     3201 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/funs/points/funs_points_points.py
--rw-rw-rw-   0        0        0     2040 2023-07-26 08:10:30.000000 huhk-1.8.6/service/app_t/funs/points/funs_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.934492 huhk-1.8.6/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.6/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.937455 huhk-1.8.6/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.946002 huhk-1.8.6/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:26:02.955067 huhk-1.8.6/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.8.6/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-26 08:26:02.958062 huhk-1.8.6/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.396052 huhk-1.8.7/
+-rw-rw-rw-   0        0        0      223 2023-07-26 08:38:53.396052 huhk-1.8.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.206266 huhk-1.8.7/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.8.7/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.241689 huhk-1.8.7/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3258 2023-07-26 08:25:43.000000 huhk-1.8.7/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21410 2023-07-26 08:38:20.000000 huhk-1.8.7/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.8.7/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    17815 2023-07-26 08:38:20.000000 huhk-1.8.7/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      895 2023-07-26 08:22:28.000000 huhk-1.8.7/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-26 08:38:52.000000 huhk-1.8.7/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    12802 2023-07-26 08:10:46.000000 huhk-1.8.7/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1267 2023-07-25 09:00:59.000000 huhk-1.8.7/huhk/main.py
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.8.7/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.243683 huhk-1.8.7/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.285571 huhk-1.8.7/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.8.7/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.8.7/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.8.7/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.8.7/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28433 2023-07-26 06:32:08.000000 huhk-1.8.7/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.8.7/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.8.7/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.8.7/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.220201 huhk-1.8.7/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2839 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 08:38:53.000000 huhk-1.8.7/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.166482 huhk-1.8.7/service/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.292553 huhk-1.8.7/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.8.7/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.294554 huhk-1.8.7/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.7/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.297544 huhk-1.8.7/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.306520 huhk-1.8.7/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    35088 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    36705 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.314499 huhk-1.8.7/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    48149 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    39604 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.8.7/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.316493 huhk-1.8.7/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.7/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.319520 huhk-1.8.7/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.328231 huhk-1.8.7/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.337207 huhk-1.8.7/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.8.7/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.347760 huhk-1.8.7/service/app_t/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.8.7/service/app_t/funs/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.8.7/service/app_t/funs/funs_app_t.py
+-rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.8.7/service/app_t/funs/funs_open.py
+-rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.8.7/service/app_t/funs/funs_points.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.353199 huhk-1.8.7/service/app_t/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.7/service/app_t/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.8.7/service/app_t/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.361146 huhk-1.8.7/service/app_t/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.8.7/service/app_t/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      959 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.368159 huhk-1.8.7/service/app_t/funs/points/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.8.7/service/app_t/funs/points/__init__.py
+-rw-rw-rw-   0        0        0     3201 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/funs/points/funs_points_points.py
+-rw-rw-rw-   0        0        0     2040 2023-07-26 08:10:30.000000 huhk-1.8.7/service/app_t/funs/points/funs_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.370155 huhk-1.8.7/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.8.7/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.373112 huhk-1.8.7/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.382123 huhk-1.8.7/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:53.392096 huhk-1.8.7/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.8.7/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:38:53.397050 huhk-1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.8.7/setup.py
```

### Comparing `huhk-1.8.6/huhk/__init__.py` & `huhk-1.8.7/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/case_project/json_coder.py` & `huhk-1.8.7/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/case_project/main_fun.py` & `huhk-1.8.7/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/case_project/project_base.py` & `huhk-1.8.7/huhk/case_project/project_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,15 @@
                 fun_name, file_str)
             if ord_str:
                 if _update:
                     new_str = self.get_api_fun_fun_str(fun_name)
                     file_str = file_str.replace(ord_str[0][0], new_str)
                     FunBase.write_file(fun_path.path, file_str)
             else:
+                file_str = self.get_api_fun_header_str2(fun_name, file_str)
                 tmp_list = file_str.split("if __name__ == '__main__':")
                 tmp_list[0] += self.get_api_fun_fun_str(fun_name)
                 file_str = "if __name__ == '__main__':".join(tmp_list)
                 FunBase.write_file(fun_path.path, file_str)
         else:
             file_str = self.get_api_fun_header_str(fun_name) + self.get_api_fun_fun_str(fun_name)
             FunBase.mkdir_file(fun_path.path)
```

### Comparing `huhk-1.8.6/huhk/case_project/project_init.py` & `huhk-1.8.7/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/case_project/project_string.py` & `huhk-1.8.7/huhk/case_project/project_string.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,14 +227,28 @@
         api_path = self.get_path(fun_name, fun_type='apis')
         header_str = "import allure\n\n"
         header_str += f"from {assert_path.import_path} import {assert_path.class_name}\n"
         header_str += f"from {api_path.import_path.rsplit('.', 1)[0]} import {api_path.import_path.rsplit('.', 1)[1]}\n\n\n"
         header_str += f"class {fun_path.class_name}({assert_path.class_name}):\n"
         return header_str
 
+    def get_api_fun_header_str2(self, fun_name, file_str):
+        assert_path = self.get_path(fun_name, fun_type='asserts')
+        api_path = self.get_path(fun_name, fun_type='apis')
+        header_str = "import allure\n"
+        if header_str not in file_str:
+            file_str = header_str + file_str
+        header_str = f"from {assert_path.import_path} import {assert_path.class_name}\n"
+        if header_str not in file_str:
+            file_str = header_str + file_str
+        header_str = f"from {api_path.import_path.rsplit('.', 1)[0]} import {api_path.import_path.rsplit('.', 1)[1]}\n"
+        if header_str not in file_str:
+            file_str = header_str + file_str
+        return file_str
+
     def get_api_fun_fun_str(self, fun_name):
         api_path = self.get_path(fun_name, fun_type='apis')
         api = self.this_fun_list.api[fun_name]
         data_list_tmp = []
         for n in api.input:
             if n in self.size_names:
                 data_list_tmp.append(n.strip() + '=10')
@@ -254,15 +268,15 @@
         api_fun_fun_str += "        \"\"\"\n"
         if set(api.input) & set(self.page_and_size) or str(api.method).lower() == "get":
             for n in data_list:
                 api_fun_fun_str += "        %s = self.get_list_choice(%s, list_or_dict=None, key=\"%s\")\n" % (n, n, n)
         else:
             for n in data_list:
                 api_fun_fun_str += "        %s = self.get_value_choice(%s, list_or_dict=None, key=None" % (n, n)
-                api_fun_fun_str += ", _all_is_None=_all_is_None)"
+                api_fun_fun_str += ", _all_is_None=_all_is_None)\n"
         api_fun_fun_str += '\n' if data_list else ''
         api_fun_fun_str += "        _kwargs = self.get_kwargs(locals())\n"
         api_fun_fun_str += f"        self.res = {api_path.import_path.rsplit('.', 1)[1]}.{fun_name}(**_kwargs)\n\n"
         api_fun_fun_str += "        self.assert_%s(_assert, **_kwargs)\n" % fun_name
         if set(api.input) & set(self.page_and_size) or str(api.method).lower() == "get":
             api_fun_fun_str += "        self.set_output_value(_kwargs)\n"
         api_fun_fun_str += "        self.set_value(_kwargs)\n\n\n"
```

### Comparing `huhk-1.8.6/huhk/case_project/setup_set.py` & `huhk-1.8.7/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/init_project.py` & `huhk-1.8.7/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/main.py` & `huhk-1.8.7/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/beam_class.py` & `huhk-1.8.7/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/data.py` & `huhk-1.8.7/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/par_do.py` & `huhk-1.8.7/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.8.7/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_fiter.py` & `huhk-1.8.7/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_flatmap.py` & `huhk-1.8.7/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_map.py` & `huhk-1.8.7/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_par_do.py` & `huhk-1.8.7/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_regex.py` & `huhk-1.8.7/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/testcase/apache/test_time.py` & `huhk-1.8.7/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_apache_beam.py` & `huhk-1.8.7/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_dict.py` & `huhk-1.8.7/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_encryption.py` & `huhk-1.8.7/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_fun.py` & `huhk-1.8.7/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_logger.py` & `huhk-1.8.7/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_request.py` & `huhk-1.8.7/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/unit_tasks.py` & `huhk-1.8.7/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk/常用命令.py` & `huhk-1.8.7/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/huhk.egg-info/SOURCES.txt` & `huhk-1.8.7/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.8.7/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.8.7/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/apis/points/apis_points_points.py` & `huhk-1.8.7/service/app_t/apis/points/apis_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.8.7/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/app_t_fun.py` & `huhk-1.8.7/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.8.7/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.8.7/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.8.7/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.8.7/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.8.7/service/app_t/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.8.7/service/app_t/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/funs/points/funs_points_points.py` & `huhk-1.8.7/service/app_t/funs/points/funs_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/funs/points/funs_points_pointsApp.py` & `huhk-1.8.7/service/app_t/funs/points/funs_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.8.7/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.8.7/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.8.7/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.8.6/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.8.7/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

