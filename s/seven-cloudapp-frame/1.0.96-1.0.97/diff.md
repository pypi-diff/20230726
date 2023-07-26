# Comparing `tmp/seven_cloudapp_frame-1.0.96.tar.gz` & `tmp/seven_cloudapp_frame-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\Project\Gao7Git\seven_cloudapp_frame\dist\.tmp-3offk0lk\seven_cloudapp_frame-1.0.96.tar", last modified: Mon Jul 24 09:22:03 2023, max compression
+gzip compressed data, was "E:\Project\Gao7Git\seven_cloudapp_frame\dist\.tmp-6gx93nla\seven_cloudapp_frame-1.0.97.tar", last modified: Wed Jul 26 06:14:43 2023, max compression
```

## Comparing `seven_cloudapp_frame-1.0.96.tar` & `seven_cloudapp_frame-1.0.97.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.169438 seven_cloudapp_frame-1.0.96/
--rw-rw-rw-   0        0        0     1081 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.0.96/LICENSE
--rw-rw-rw-   0        0        0     8582 2023-07-24 09:22:03.168438 seven_cloudapp_frame-1.0.96/PKG-INFO
--rw-rw-rw-   0        0        0     7779 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 09:22:03.170438 seven_cloudapp_frame-1.0.96/setup.cfg
--rw-rw-rw-   0        0        0     1516 2023-07-24 09:21:24.000000 seven_cloudapp_frame-1.0.96/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:01.915155 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/
--rw-rw-rw-   0        0        0      164 2021-08-26 01:25:55.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:01.967125 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/
--rw-rw-rw-   0        0        0      182 2021-07-15 04:00:34.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.039084 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/
--rw-rw-rw-   0        0        0      263 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/__init__.py
--rw-rw-rw-   0        0        0    14013 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/act.py
--rw-rw-rw-   0        0        0   411248 2022-06-14 06:44:47.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/address.py
--rw-rw-rw-   0        0        0     7208 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/app.py
--rw-rw-rw-   0        0        0     3849 2022-07-27 10:21:00.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/goods.py
--rw-rw-rw-   0        0        0     1825 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/ip_c.py
--rw-rw-rw-   0        0        0    17290 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/order.py
--rw-rw-rw-   0        0        0    34999 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/pay.py
--rw-rw-rw-   0        0        0     5038 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/stat.py
--rw-rw-rw-   0        0        0    61113 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/task.py
--rw-rw-rw-   0        0        0     5070 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/theme.py
--rw-rw-rw-   0        0        0    20371 2023-06-19 07:18:00.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/user.py
--rw-rw-rw-   0        0        0      986 2023-02-10 01:47:47.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/core.py
--rw-rw-rw-   0        0        0     3005 2023-04-12 10:06:46.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/filter_base.py
--rw-rw-rw-   0        0        0    41284 2023-06-13 10:47:25.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/frame_base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.140026 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/
--rw-rw-rw-   0        0        0      331 2023-04-19 08:30:34.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/__init__.py
--rw-rw-rw-   0        0        0    22416 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/act_s.py
--rw-rw-rw-   0        0        0    20114 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/app_s.py
--rw-rw-rw-   0        0        0     7213 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/base_s.py
--rw-rw-rw-   0        0        0    11160 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/cms_s.py
--rw-rw-rw-   0        0        0     9607 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/goods_s.py
--rw-rw-rw-   0        0        0    14810 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/ip_s.py
--rw-rw-rw-   0        0        0    14383 2023-04-10 10:46:37.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/launch_s.py
--rw-rw-rw-   0        0        0    16183 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/module_s.py
--rw-rw-rw-   0        0        0    34887 2023-06-09 02:30:25.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/order_s.py
--rw-rw-rw-   0        0        0     8509 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/price_s.py
--rw-rw-rw-   0        0        0    19482 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/prize_s.py
--rw-rw-rw-   0        0        0     5568 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/report_s.py
--rw-rw-rw-   0        0        0     7123 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/task_s.py
--rw-rw-rw-   0        0        0     2622 2023-04-04 01:58:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/theme_s.py
--rw-rw-rw-   0        0        0    23860 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/user_s.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.147022 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/
--rw-rw-rw-   0        0        0      139 2021-07-15 07:37:39.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.168010 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/
--rw-rw-rw-   0        0        0      190 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/__init__.py
--rw-rw-rw-   0        0        0      437 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/frame_console.py
--rw-rw-rw-   0        0        0      443 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/frame_tornado.py
--rw-rw-rw-   0        0        0     1864 2023-04-18 01:25:51.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/share_config.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.274950 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/
--rw-rw-rw-   0        0        0      162 2021-08-23 06:06:41.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/__init__.py
--rw-rw-rw-   0        0        0     5792 2022-05-31 10:11:02.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/action_helper.py
--rw-rw-rw-   0        0        0    10880 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/alipay_helper.py
--rw-rw-rw-   0        0        0     8816 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/baidubce_helper.py
--rw-rw-rw-   0        0        0     3195 2022-05-31 10:11:02.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py
--rw-rw-rw-   0        0        0     7562 2022-12-14 10:22:52.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/counter_helper.py
--rw-rw-rw-   0        0        0     6437 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/cryptography_helper.py
--rw-rw-rw-   0        0        0     2430 2022-04-24 01:23:12.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/email_helper.py
--rw-rw-rw-   0        0        0     8982 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/logistics_helper.py
--rw-rw-rw-   0        0        0     4116 2023-04-06 03:12:26.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/oss2_helper.py
--rw-rw-rw-   0        0        0    36523 2023-07-19 11:04:49.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/queue_up_helper.py
--rw-rw-rw-   0        0        0     4638 2023-04-04 01:58:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/redis_helper.py
--rw-rw-rw-   0        0        0     9745 2023-07-03 09:38:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/riskmanage_helper.py
--rw-rw-rw-   0        0        0    22874 2023-04-19 01:04:19.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/seven_helper.py
--rw-rw-rw-   0        0        0    32214 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/tiktok_helper.py
--rw-rw-rw-   0        0        0     3623 2022-12-07 08:50:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/time_helper.py
--rw-rw-rw-   0        0        0    91008 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/wechat_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.430860 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/
--rw-rw-rw-   0        0        0      139 2021-08-26 01:24:55.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/__init__.py
--rw-rw-rw-   0        0        0    22422 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/act_base_model.py
--rw-rw-rw-   0        0        0    19019 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/app_base_model.py
--rw-rw-rw-   0        0        0    49176 2023-07-24 09:19:44.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/asset_base_model.py
--rw-rw-rw-   0        0        0    32216 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/cache_model.py
--rw-rw-rw-   0        0        0    13597 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/cms_base_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.476833 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/
--rw-rw-rw-   0        0        0        0 2022-02-28 03:11:16.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/__init__.py
--rw-rw-rw-   0        0        0    16684 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/asset_console_model.py
--rw-rw-rw-   0        0        0    19804 2023-07-19 04:02:32.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/erp_console_model.py
--rw-rw-rw-   0        0        0    10806 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/launch_console_model.py
--rw-rw-rw-   0        0        0    25513 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/stat_console_model.py
--rw-rw-rw-   0        0        0     3195 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/task_console_model.py
--rw-rw-rw-   0        0        0     5432 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/timing_work_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.482831 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/
--rw-rw-rw-   0        0        0        0 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.515811 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/
--rw-rw-rw-   0        0        0       81 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/__init__.py
--rw-rw-rw-   0        0        0     3768 2023-02-03 11:07:31.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_info_model.py
--rw-rw-rw-   0        0        0     3050 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_module_model.py
--rw-rw-rw-   0        0        0     3834 2023-05-05 07:16:16.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_prize_model.py
--rw-rw-rw-   0        0        0     2611 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_type_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.527805 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/app/
--rw-rw-rw-   0        0        0       27 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/app/__init__.py
--rw-rw-rw-   0        0        0     3207 2022-09-27 12:57:23.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/app/app_info_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.556789 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/
--rw-rw-rw-   0        0        0       97 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py
--rw-rw-rw-   0        0        0     3243 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py
--rw-rw-rw-   0        0        0     1723 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py
--rw-rw-rw-   0        0        0     2154 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.567782 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/base/
--rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/base/__init__.py
--rw-rw-rw-   0        0        0     3034 2021-07-29 10:30:05.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/base/base_info_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.578776 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/browse/
--rw-rw-rw-   0        0        0       29 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/browse/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.606759 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/
--rw-rw-rw-   0        0        0       45 2022-09-27 01:02:35.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py
--rw-rw-rw-   0        0        0     1901 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.618752 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/collect/
--rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/collect/__init__.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.629747 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/counter/
--rw-rw-rw-   0        0        0       32 2022-12-07 08:50:15.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/counter/__init__.py
--rw-rw-rw-   0        0        0     1679 2022-12-07 08:50:15.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.648735 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/dict/
--rw-rw-rw-   0        0        0      191 2023-04-19 08:29:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/dict/__init__.py
--rw-rw-rw-   0        0        0     1811 2022-09-28 03:13:57.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.659730 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/erp/
--rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/erp/__init__.py
--rw-rw-rw-   0        0        0     1613 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.670723 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/friend/
--rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/friend/__init__.py
--rw-rw-rw-   0        0        0     1855 2021-07-29 10:31:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.717697 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/
--rw-rw-rw-   0        0        0      132 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_info_model.py
--rw-rw-rw-   0        0        0     1980 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_module_model.py
--rw-rw-rw-   0        0        0     1584 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_product_model.py
--rw-rw-rw-   0        0        0     2752 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_shop_model.py
--rw-rw-rw-   0        0        0     1716 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_skin_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.735686 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/
--rw-rw-rw-   0        0        0       48 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py
--rw-rw-rw-   0        0        0     2090 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.751677 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/
--rw-rw-rw-   0        0        0       42 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/__init__.py
--rw-rw-rw-   0        0        0     2016 2022-09-28 09:53:25.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py
--rw-rw-rw-   0        0        0     1602 2023-05-05 03:59:47.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.769668 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/
--rw-rw-rw-   0        0        0       51 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/__init__.py
--rw-rw-rw-   0        0        0     1755 2021-08-10 10:06:24.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py
--rw-rw-rw-   0        0        0     1734 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.783658 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/marketing/
--rw-rw-rw-   0        0        0       36 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/marketing/__init__.py
--rw-rw-rw-   0        0        0     1687 2021-08-03 07:45:59.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.795652 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/middler/
--rw-rw-rw-   0        0        0       34 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/middler/__init__.py
--rw-rw-rw-   0        0        0     1847 2021-07-29 10:33:15.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.837627 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/
--rw-rw-rw-   0        0        0       61 2022-10-10 07:00:27.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/__init__.py
--rw-rw-rw-   0        0        0     1357 2022-10-10 07:00:27.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py
--rw-rw-rw-   0        0        0     2588 2022-10-19 07:14:37.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.850620 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/pay/
--rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/pay/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.868611 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/price/
--rw-rw-rw-   0        0        0       29 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/price/__init__.py
--rw-rw-rw-   0        0        0     1835 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/price/price_gear_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.899593 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/
--rw-rw-rw-   0        0        0       51 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/__init__.py
--rw-rw-rw-   0        0        0     4075 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py
--rw-rw-rw-   0        0        0     4149 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.911585 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/product/
--rw-rw-rw-   0        0        0       32 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/product/__init__.py
--rw-rw-rw-   0        0        0     2012 2023-07-14 01:35:07.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/product/product_price_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.922579 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/refund/
--rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/refund/__init__.py
--rw-rw-rw-   0        0        0     2346 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.933573 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/saas/
--rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/saas/__init__.py
--rw-rw-rw-   0        0        0     1891 2021-07-29 10:35:09.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.944567 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/skin/
--rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/skin/__init__.py
--rw-rw-rw-   0        0        0     1737 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.954560 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/special/
--rw-rw-rw-   0        0        0       32 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/special/__init__.py
--rw-rw-rw-   0        0        0     1458 2021-08-10 10:07:00.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/special/special_goods_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:02.996537 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/
--rw-rw-rw-   0        0        0      130 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py
--rw-rw-rw-   0        0        0     2271 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py
--rw-rw-rw-   0        0        0     1882 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py
--rw-rw-rw-   0        0        0     1845 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py
--rw-rw-rw-   0        0        0     1902 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py
--rw-rw-rw-   0        0        0     2834 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.012528 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/
--rw-rw-rw-   0        0        0       54 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/__init__.py
--rw-rw-rw-   0        0        0     3042 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py
--rw-rw-rw-   0        0        0     2078 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/store_asset_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.035514 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/
--rw-rw-rw-   0        0        0       73 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/__init__.py
--rw-rw-rw-   0        0        0     2152 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py
--rw-rw-rw-   0        0        0     1610 2021-07-29 10:37:32.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py
--rw-rw-rw-   0        0        0     3082 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.081488 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/
--rw-rw-rw-   0        0        0       94 2023-05-30 10:15:46.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/__init__.py
--rw-rw-rw-   0        0        0     2204 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_count_model.py
--rw-rw-rw-   0        0        0     2066 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py
--rw-rw-rw-   0        0        0     2319 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_info_model.py
--rw-rw-rw-   0        0        0     2451 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_log_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.097479 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/
--rw-rw-rw-   0        0        0       47 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/__init__.py
--rw-rw-rw-   0        0        0     1775 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py
--rw-rw-rw-   0        0        0     1490 2021-07-29 10:38:24.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.109473 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/third/
--rw-rw-rw-   0        0        0       34 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/third/__init__.py
--rw-rw-rw-   0        0        0     2785 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.148450 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/
--rw-rw-rw-   0        0        0      108 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/__init__.py
--rw-rw-rw-   0        0        0     2504 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_account_model.py
--rw-rw-rw-   0        0        0     1984 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_address_model.py
--rw-rw-rw-   0        0        0     2190 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_asset_model.py
--rw-rw-rw-   0        0        0     2134 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_black_model.py
--rw-rw-rw-   0        0        0     3144 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_info_model.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:03.162442 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/version/
--rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/version/__init__.py
--rw-rw-rw-   0        0        0     1849 2021-07-29 10:40:28.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/version/version_info_model.py
--rw-rw-rw-   0        0        0     9631 2023-07-14 01:35:07.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/enum.py
--rw-rw-rw-   0        0        0    26015 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/frame_base_model.py
--rw-rw-rw-   0        0        0    11676 2023-07-21 02:15:33.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/goods_base_model.py
--rw-rw-rw-   0        0        0    14366 2023-05-09 01:25:26.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/ip_base_model.py
--rw-rw-rw-   0        0        0    28969 2023-04-10 10:46:37.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/launch_base_model.py
--rw-rw-rw-   0        0        0    12189 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/module_base_model.py
--rw-rw-rw-   0        0        0    20856 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/mp_base_model.py
--rw-rw-rw-   0        0        0    14717 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/operate_base_model.py
--rw-rw-rw-   0        0        0    65363 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/order_base_model.py
--rw-rw-rw-   0        0        0    10690 2023-02-03 11:07:31.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/price_base_model.py
--rw-rw-rw-   0        0        0    15569 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/prize_base_model.py
--rw-rw-rw-   0        0        0     4592 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/push_base_model.py
--rw-rw-rw-   0        0        0    14491 2023-05-09 01:25:26.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/seven_model.py
--rw-rw-rw-   0        0        0    13015 2023-04-13 02:27:45.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/shakeshop_base_model.py
--rw-rw-rw-   0        0        0    23707 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/stat_base_model.py
--rw-rw-rw-   0        0        0   267629 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/task_base_model.py
--rw-rw-rw-   0        0        0    13440 2023-04-04 01:58:15.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/theme_base_model.py
--rw-rw-rw-   0        0        0    92615 2023-04-07 08:19:28.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/top_base_model.py
--rw-rw-rw-   0        0        0    46775 2023-07-24 06:39:30.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/user_base_model.py
--rw-rw-rw-   0        0        0    14845 2023-07-18 05:35:20.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/route.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:22:01.944139 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/
--rw-rw-rw-   0        0        0     8582 2023-07-24 09:22:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10800 2023-07-24 09:22:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:22:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-07-24 09:22:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-24 09:22:01.000000 seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.616853 seven_cloudapp_frame-1.0.97/
+-rw-rw-rw-   0        0        0     1081 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.0.97/LICENSE
+-rw-rw-rw-   0        0        0     8582 2023-07-26 06:14:43.615853 seven_cloudapp_frame-1.0.97/PKG-INFO
+-rw-rw-rw-   0        0        0     7779 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 06:14:43.616853 seven_cloudapp_frame-1.0.97/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-07-26 06:14:00.000000 seven_cloudapp_frame-1.0.97/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.201661 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/
+-rw-rw-rw-   0        0        0      164 2021-08-26 01:25:55.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.252632 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/
+-rw-rw-rw-   0        0        0      182 2021-07-15 04:00:34.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.400548 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/
+-rw-rw-rw-   0        0        0      263 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/__init__.py
+-rw-rw-rw-   0        0        0    14013 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/act.py
+-rw-rw-rw-   0        0        0   411248 2022-06-14 06:44:47.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/address.py
+-rw-rw-rw-   0        0        0     7208 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/app.py
+-rw-rw-rw-   0        0        0     3849 2022-07-27 10:21:00.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/goods.py
+-rw-rw-rw-   0        0        0     1825 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/ip_c.py
+-rw-rw-rw-   0        0        0    17290 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/order.py
+-rw-rw-rw-   0        0        0    34999 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/pay.py
+-rw-rw-rw-   0        0        0     5038 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/stat.py
+-rw-rw-rw-   0        0        0    61113 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/task.py
+-rw-rw-rw-   0        0        0     5070 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/theme.py
+-rw-rw-rw-   0        0        0    20371 2023-06-19 07:18:00.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/user.py
+-rw-rw-rw-   0        0        0      986 2023-02-10 01:47:47.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/core.py
+-rw-rw-rw-   0        0        0     3005 2023-04-12 10:06:46.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/filter_base.py
+-rw-rw-rw-   0        0        0    41284 2023-06-13 10:47:25.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/frame_base.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.494494 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/
+-rw-rw-rw-   0        0        0      331 2023-04-19 08:30:34.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/__init__.py
+-rw-rw-rw-   0        0        0    22416 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/act_s.py
+-rw-rw-rw-   0        0        0    20114 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/app_s.py
+-rw-rw-rw-   0        0        0     7213 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/base_s.py
+-rw-rw-rw-   0        0        0    11160 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/cms_s.py
+-rw-rw-rw-   0        0        0     9607 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/goods_s.py
+-rw-rw-rw-   0        0        0    14810 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/ip_s.py
+-rw-rw-rw-   0        0        0    14383 2023-04-10 10:46:37.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/launch_s.py
+-rw-rw-rw-   0        0        0    16183 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/module_s.py
+-rw-rw-rw-   0        0        0    34887 2023-06-09 02:30:25.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/order_s.py
+-rw-rw-rw-   0        0        0     8509 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/price_s.py
+-rw-rw-rw-   0        0        0    19482 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/prize_s.py
+-rw-rw-rw-   0        0        0     5568 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/report_s.py
+-rw-rw-rw-   0        0        0     7123 2023-02-03 11:07:30.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/task_s.py
+-rw-rw-rw-   0        0        0     2622 2023-04-04 01:58:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/theme_s.py
+-rw-rw-rw-   0        0        0    23860 2023-05-12 02:13:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/user_s.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.500491 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/
+-rw-rw-rw-   0        0        0      139 2021-07-15 07:37:39.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.519479 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/
+-rw-rw-rw-   0        0        0      190 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/frame_console.py
+-rw-rw-rw-   0        0        0      443 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/frame_tornado.py
+-rw-rw-rw-   0        0        0     1864 2023-04-18 01:25:51.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/share_config.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.618423 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/
+-rw-rw-rw-   0        0        0      162 2021-08-23 06:06:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/__init__.py
+-rw-rw-rw-   0        0        0     5792 2022-05-31 10:11:02.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/action_helper.py
+-rw-rw-rw-   0        0        0    10880 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/alipay_helper.py
+-rw-rw-rw-   0        0        0     8816 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/baidubce_helper.py
+-rw-rw-rw-   0        0        0     3195 2022-05-31 10:11:02.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py
+-rw-rw-rw-   0        0        0     7562 2022-12-14 10:22:52.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/counter_helper.py
+-rw-rw-rw-   0        0        0     6437 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/cryptography_helper.py
+-rw-rw-rw-   0        0        0     2430 2022-04-24 01:23:12.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/email_helper.py
+-rw-rw-rw-   0        0        0     8982 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/logistics_helper.py
+-rw-rw-rw-   0        0        0     4116 2023-04-06 03:12:26.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/oss2_helper.py
+-rw-rw-rw-   0        0        0    36523 2023-07-19 11:04:49.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/queue_up_helper.py
+-rw-rw-rw-   0        0        0     4638 2023-04-04 01:58:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/redis_helper.py
+-rw-rw-rw-   0        0        0     9745 2023-07-03 09:38:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/riskmanage_helper.py
+-rw-rw-rw-   0        0        0    22874 2023-04-19 01:04:19.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/seven_helper.py
+-rw-rw-rw-   0        0        0    32214 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/tiktok_helper.py
+-rw-rw-rw-   0        0        0     3623 2022-12-07 08:50:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/time_helper.py
+-rw-rw-rw-   0        0        0    91008 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/wechat_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.816310 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/
+-rw-rw-rw-   0        0        0      139 2021-08-26 01:24:55.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/__init__.py
+-rw-rw-rw-   0        0        0    22422 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/act_base_model.py
+-rw-rw-rw-   0        0        0    19019 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/app_base_model.py
+-rw-rw-rw-   0        0        0    48537 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/asset_base_model.py
+-rw-rw-rw-   0        0        0    31515 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/cache_model.py
+-rw-rw-rw-   0        0        0    12778 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/cms_base_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.863283 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/
+-rw-rw-rw-   0        0        0        0 2022-02-28 03:11:16.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/__init__.py
+-rw-rw-rw-   0        0        0    15849 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/asset_console_model.py
+-rw-rw-rw-   0        0        0    19804 2023-07-19 04:02:32.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/erp_console_model.py
+-rw-rw-rw-   0        0        0    10806 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/launch_console_model.py
+-rw-rw-rw-   0        0        0    24234 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/stat_console_model.py
+-rw-rw-rw-   0        0        0     2545 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/task_console_model.py
+-rw-rw-rw-   0        0        0     5379 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/timing_work_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.868281 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/
+-rw-rw-rw-   0        0        0        0 2021-04-09 01:22:35.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.895265 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/
+-rw-rw-rw-   0        0        0       81 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/__init__.py
+-rw-rw-rw-   0        0        0     3768 2023-02-03 11:07:31.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_info_model.py
+-rw-rw-rw-   0        0        0     3050 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_module_model.py
+-rw-rw-rw-   0        0        0     3834 2023-05-05 07:16:16.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_prize_model.py
+-rw-rw-rw-   0        0        0     2611 2023-07-14 01:35:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_type_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.907257 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/app/
+-rw-rw-rw-   0        0        0       27 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/app/__init__.py
+-rw-rw-rw-   0        0        0     3207 2022-09-27 12:57:23.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/app/app_info_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.939239 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/
+-rw-rw-rw-   0        0        0       97 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/__init__.py
+-rw-rw-rw-   0        0        0     2208 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py
+-rw-rw-rw-   0        0        0     3088 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py
+-rw-rw-rw-   0        0        0     1568 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py
+-rw-rw-rw-   0        0        0     1999 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.951233 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/base/
+-rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/base/__init__.py
+-rw-rw-rw-   0        0        0     3034 2021-07-29 10:30:05.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/base/base_info_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.964226 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/browse/
+-rw-rw-rw-   0        0        0       29 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/browse/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.021192 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/cms/
+-rw-rw-rw-   0        0        0       45 2022-09-27 01:02:35.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/cms/__init__.py
+-rw-rw-rw-   0        0        0     2743 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py
+-rw-rw-rw-   0        0        0     1752 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.037184 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/collect/
+-rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/collect/__init__.py
+-rw-rw-rw-   0        0        0     1581 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.051175 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/counter/
+-rw-rw-rw-   0        0        0       32 2022-12-07 08:50:15.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/counter/__init__.py
+-rw-rw-rw-   0        0        0     1679 2022-12-07 08:50:15.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.099148 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/dict/
+-rw-rw-rw-   0        0        0      191 2023-04-19 08:29:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/dict/__init__.py
+-rw-rw-rw-   0        0        0     1811 2022-09-28 03:13:57.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.111142 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/erp/
+-rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/erp/__init__.py
+-rw-rw-rw-   0        0        0     1613 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.120136 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/friend/
+-rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/friend/__init__.py
+-rw-rw-rw-   0        0        0     1855 2021-07-29 10:31:01.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.158114 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/
+-rw-rw-rw-   0        0        0      132 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_info_model.py
+-rw-rw-rw-   0        0        0     1980 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_module_model.py
+-rw-rw-rw-   0        0        0     1584 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_product_model.py
+-rw-rw-rw-   0        0        0     2752 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_shop_model.py
+-rw-rw-rw-   0        0        0     1716 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_skin_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.175105 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/
+-rw-rw-rw-   0        0        0       48 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/__init__.py
+-rw-rw-rw-   0        0        0     2359 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py
+-rw-rw-rw-   0        0        0     1938 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.192095 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/
+-rw-rw-rw-   0        0        0       42 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/__init__.py
+-rw-rw-rw-   0        0        0     2016 2022-09-28 09:53:25.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py
+-rw-rw-rw-   0        0        0     1602 2023-05-05 03:59:47.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.211085 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/
+-rw-rw-rw-   0        0        0       51 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/__init__.py
+-rw-rw-rw-   0        0        0     1755 2021-08-10 10:06:24.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py
+-rw-rw-rw-   0        0        0     1734 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.221078 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/marketing/
+-rw-rw-rw-   0        0        0       36 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/marketing/__init__.py
+-rw-rw-rw-   0        0        0     1687 2021-08-03 07:45:59.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.237069 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/middler/
+-rw-rw-rw-   0        0        0       34 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/middler/__init__.py
+-rw-rw-rw-   0        0        0     1847 2021-07-29 10:33:15.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.252061 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/
+-rw-rw-rw-   0        0        0       61 2022-10-10 07:00:27.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/__init__.py
+-rw-rw-rw-   0        0        0     1357 2022-10-10 07:00:27.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py
+-rw-rw-rw-   0        0        0     2588 2022-10-19 07:14:37.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.263054 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/pay/
+-rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/pay/__init__.py
+-rw-rw-rw-   0        0        0     2629 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.281043 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/price/
+-rw-rw-rw-   0        0        0       29 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/price/__init__.py
+-rw-rw-rw-   0        0        0     1835 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/price/price_gear_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.301033 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/
+-rw-rw-rw-   0        0        0       51 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/__init__.py
+-rw-rw-rw-   0        0        0     3920 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py
+-rw-rw-rw-   0        0        0     3994 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.312027 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/product/
+-rw-rw-rw-   0        0        0       32 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/product/__init__.py
+-rw-rw-rw-   0        0        0     2012 2023-07-14 01:35:07.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/product/product_price_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.321021 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/refund/
+-rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/refund/__init__.py
+-rw-rw-rw-   0        0        0     2191 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.333015 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/saas/
+-rw-rw-rw-   0        0        0       30 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/saas/__init__.py
+-rw-rw-rw-   0        0        0     1891 2021-07-29 10:35:09.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.346007 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/skin/
+-rw-rw-rw-   0        0        0       28 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/skin/__init__.py
+-rw-rw-rw-   0        0        0     1737 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.356001 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/special/
+-rw-rw-rw-   0        0        0       32 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/special/__init__.py
+-rw-rw-rw-   0        0        0     1458 2021-08-10 10:07:00.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/special/special_goods_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.441952 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/
+-rw-rw-rw-   0        0        0      130 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py
+-rw-rw-rw-   0        0        0     2119 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py
+-rw-rw-rw-   0        0        0     1730 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py
+-rw-rw-rw-   0        0        0     1693 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py
+-rw-rw-rw-   0        0        0     1750 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py
+-rw-rw-rw-   0        0        0     2682 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.462940 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/
+-rw-rw-rw-   0        0        0       54 2022-09-27 07:45:06.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/__init__.py
+-rw-rw-rw-   0        0        0     2887 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py
+-rw-rw-rw-   0        0        0     1923 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/store_asset_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.512911 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/
+-rw-rw-rw-   0        0        0       73 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/__init__.py
+-rw-rw-rw-   0        0        0     2152 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py
+-rw-rw-rw-   0        0        0     1610 2021-07-29 10:37:32.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py
+-rw-rw-rw-   0        0        0     3082 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.537897 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/
+-rw-rw-rw-   0        0        0       94 2023-05-30 10:15:46.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/__init__.py
+-rw-rw-rw-   0        0        0     2052 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_count_model.py
+-rw-rw-rw-   0        0        0     1914 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py
+-rw-rw-rw-   0        0        0     2167 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_info_model.py
+-rw-rw-rw-   0        0        0     2299 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_log_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.555887 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/
+-rw-rw-rw-   0        0        0       47 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/__init__.py
+-rw-rw-rw-   0        0        0     1775 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py
+-rw-rw-rw-   0        0        0     1490 2021-07-29 10:38:24.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.568879 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/third/
+-rw-rw-rw-   0        0        0       34 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/third/__init__.py
+-rw-rw-rw-   0        0        0     2785 2022-01-24 10:37:43.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.600862 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/
+-rw-rw-rw-   0        0        0      108 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/__init__.py
+-rw-rw-rw-   0        0        0     2352 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_account_model.py
+-rw-rw-rw-   0        0        0     1832 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_address_model.py
+-rw-rw-rw-   0        0        0     2035 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_asset_model.py
+-rw-rw-rw-   0        0        0     1982 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_black_model.py
+-rw-rw-rw-   0        0        0     2992 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_info_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:43.609856 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/version/
+-rw-rw-rw-   0        0        0       31 2022-09-26 07:19:56.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/version/__init__.py
+-rw-rw-rw-   0        0        0     1849 2021-07-29 10:40:28.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/version/version_info_model.py
+-rw-rw-rw-   0        0        0     9631 2023-07-14 01:35:07.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/enum.py
+-rw-rw-rw-   0        0        0    26015 2023-05-17 09:07:23.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/frame_base_model.py
+-rw-rw-rw-   0        0        0    11676 2023-07-21 02:15:33.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/goods_base_model.py
+-rw-rw-rw-   0        0        0    14366 2023-05-09 01:25:26.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/ip_base_model.py
+-rw-rw-rw-   0        0        0    28969 2023-04-10 10:46:37.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/launch_base_model.py
+-rw-rw-rw-   0        0        0    12189 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/module_base_model.py
+-rw-rw-rw-   0        0        0    20856 2023-04-21 03:12:11.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/mp_base_model.py
+-rw-rw-rw-   0        0        0    14717 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/operate_base_model.py
+-rw-rw-rw-   0        0        0    65106 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/order_base_model.py
+-rw-rw-rw-   0        0        0    10690 2023-02-03 11:07:31.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/price_base_model.py
+-rw-rw-rw-   0        0        0    15569 2023-03-22 04:00:14.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/prize_base_model.py
+-rw-rw-rw-   0        0        0     4592 2022-07-27 10:58:17.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/push_base_model.py
+-rw-rw-rw-   0        0        0    14491 2023-05-09 01:25:26.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/seven_model.py
+-rw-rw-rw-   0        0        0    13015 2023-04-13 02:27:45.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/shakeshop_base_model.py
+-rw-rw-rw-   0        0        0    23371 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/stat_base_model.py
+-rw-rw-rw-   0        0        0   262022 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/task_base_model.py
+-rw-rw-rw-   0        0        0    13440 2023-04-04 01:58:15.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/theme_base_model.py
+-rw-rw-rw-   0        0        0    92615 2023-04-07 08:19:28.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/top_base_model.py
+-rw-rw-rw-   0        0        0    46669 2023-07-26 06:13:38.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/user_base_model.py
+-rw-rw-rw-   0        0        0    14845 2023-07-18 05:35:20.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/route.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:14:42.230645 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/
+-rw-rw-rw-   0        0        0     8582 2023-07-26 06:14:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10800 2023-07-26 06:14:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 06:14:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-07-26 06:14:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-26 06:14:41.000000 seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/top_level.txt
```

### Comparing `seven_cloudapp_frame-1.0.96/LICENSE` & `seven_cloudapp_frame-1.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/PKG-INFO` & `seven_cloudapp_frame-1.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_cloudapp_frame
-Version: 1.0.96
+Version: 1.0.97
 Summary: seven cloudapp frame
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

### Comparing `seven_cloudapp_frame-1.0.96/README.md` & `seven_cloudapp_frame-1.0.97/README.md`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/setup.py` & `seven_cloudapp_frame-1.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_cloudapp_frame",
-    version="1.0.96",
+    version="1.0.97",
     author="seven",
     author_email="tech@gao7.com",
     description="seven cloudapp frame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git",
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/act.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/act.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/address.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/address.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/app.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/app.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/goods.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/goods.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/ip_c.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/ip_c.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/order.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/order.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/pay.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/pay.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/stat.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/stat.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/task.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/task.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/theme.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/theme.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/client/user.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/client/user.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/core.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/core.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/filter_base.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/filter_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/frame_base.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/frame_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/act_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/act_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/app_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/app_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/base_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/base_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/cms_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/cms_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/goods_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/goods_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/ip_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/ip_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/launch_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/launch_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/module_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/module_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/order_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/order_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/price_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/price_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/prize_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/prize_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/report_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/report_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/task_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/task_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/theme_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/theme_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/handlers/server/user_s.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/handlers/server/user_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/common/share_config.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/common/share_config.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/action_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/action_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/alipay_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/alipay_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/baidubce_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/baidubce_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/bloomfilter_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/counter_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/counter_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/cryptography_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/cryptography_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/email_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/email_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/logistics_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/logistics_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/oss2_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/oss2_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/queue_up_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/queue_up_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/redis_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/redis_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/riskmanage_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/riskmanage_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/seven_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/seven_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/tiktok_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/tiktok_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/time_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/time_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/libs/customize/wechat_helper.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/libs/customize/wechat_helper.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/act_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/act_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/app_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/app_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/asset_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/asset_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJianYi
 :Date: 2020-05-12 20:11:48
-@LastEditTime: 2023-07-24 17:19:12
+@LastEditTime: 2023-05-05 19:30:39
 @LastEditors: HuangJianYi
 :description: 
 """
 from seven_cloudapp_frame.libs.common import *
 from seven_cloudapp_frame.libs.customize.seven_helper import *
 from seven_cloudapp_frame.models.db_models.asset.asset_log_model import *
 from seven_cloudapp_frame.models.db_models.asset.asset_only_model import *
@@ -25,46 +25,36 @@
     def __init__(self,context=None,logging_error=None,logging_info=None, db_connect_key='db_cloudapp', redis_config_dict=None):
         self.context = context
         self.logging_link_error = logging_error
         self.logging_link_info = logging_info
         self.db_connect_key = db_connect_key
         self.redis_config_dict = redis_config_dict
 
-    def __get_redis_dict(self):
-        """
-        :description: 获取资产redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_asset"):
-            config_dict = config.get_value("redis_asset")
-        return config_dict
 
     def _delete_asset_dependency_key(self, act_id, user_id, delay_delete_time=0.01):
         """
         :description: 删除资产依赖建
         :param act_id: 活动标识
         :param user_id: 用户标识
         :param delay_delete_time: 延迟删除时间，传0则不进行延迟
         :return: 
         :last_editors: HuangJianYi
         """
-        AssetLogModel(db_connect_key=self.db_connect_key).delete_dependency_key(DependencyKey.asset_log_list(act_id,user_id), delay_delete_time, redis_config_dict=self.__get_redis_dict())
+        AssetLogModel().delete_dependency_key(DependencyKey.asset_log_list(act_id,user_id), delay_delete_time,redis_config_dict=self.redis_config_dict)
 
     def _add_onlyid_warn_stat(self,handler_name):
         """
         :description: 添加唯一标识预警拦截计数
         :param handler_name：接口名称
         :return: 
         :last_editors: HuangJianYi
         """
         if handler_name:
             handler_name = str(handler_name).lower()
-            redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+            redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
 
             hash_name_1 = f"warn_handler_list_{str(SevenHelper.get_now_int(fmt='%Y%m%d'))}"
             hash_key_1 = f"handlername_{handler_name}"
             if not redis_init.hexists(hash_name_1, hash_key_1):
                 redis_init.hset(hash_name_1,hash_key_1,SevenHelper.json_dumps({"app_id":'',"handler_name":handler_name}))
                 redis_init.expire(hash_name_1, 24 * 3600)
 
@@ -78,15 +68,15 @@
         :param act_id：活动标识
         :param only_id：资产唯一标识
         :param create_day：整形的创建天20200506
         :param app_id：应用标识
         :return: 
         :last_editors: HuangJianYi
         """
-        redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+        redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
         hash_name = f"asset_only_list:{act_id}" if act_id > 0 else f"asset_only_list:{app_id}_0"
         if create_day <= 0:
             hash_name += f"_{SevenHelper.get_now_day_int()}"
         else:
             hash_name += f"_{create_day}"
         if redis_init.hexists(hash_name, only_id):
             redis_init.hdel(hash_name, only_id)
@@ -106,15 +96,15 @@
         """
         if not user_id or not asset_type:
             return 0
         if act_id > 0:
             return CryptoHelper.md5_encrypt_int(f"{act_id}_{user_id}_{asset_type}_{asset_object_id}")
         else:
             return CryptoHelper.md5_encrypt_int(f"{app_id}_0_{user_id}_{asset_type}_{asset_object_id}")
-
+            
     def get_asset_check_code(self, id_md5, asset_value, sign_key):
         """
         :description: 生成资产校验码
         :param id_md5：id_md5
         :param asset_value：当前资产值
         :param sign_key：签名key,目前使用app_id作为签名key
         :return: 用户资产校验码
@@ -164,24 +154,24 @@
         user_asset_id_md5 = self.get_user_asset_id_md5(app_id, act_id, user_id, asset_type, asset_object_id)
         if user_asset_id_md5 == 0:
             invoke_result_data.success = False
             invoke_result_data.error_code = "error"
             invoke_result_data.error_message = "修改失败"
             return invoke_result_data
         #如果only_id已经存在，直接在redis进行拦截,减少数据库的请求，时限1天
-        redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+        redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
         is_asset_warn = share_config.get_value("is_asset_warn",False) #是否开启资产预警，跟控制台配套使用
         only_cache_key = ""
         if only_id:
             only_cache_key = f"asset_only_list:{act_id}_{SevenHelper.get_now_day_int()}"  if act_id > 0 else f"asset_only_list:{app_id}_0_{SevenHelper.get_now_day_int()}"
             if redis_init.hexists(only_cache_key, only_id):
                 invoke_result_data.success = False
                 invoke_result_data.error_code = "error"
                 invoke_result_data.error_message = "only_id已经存在"
-
+                
                 if is_asset_warn == True:
                     asset_warn_notice = AssetWarnNotice()
                     asset_warn_notice.app_id = app_id
                     asset_warn_notice.act_id = act_id
                     asset_warn_notice.ascription_type = 2
                     asset_warn_notice.handler_name = handler_name
                     asset_warn_notice.request_code = request_code
@@ -198,18 +188,17 @@
                     asset_warn_notice.info_json = {"asset_value":asset_value}
                     asset_warn_notice.create_date = SevenHelper.get_now_datetime()
                     asset_warn_notice.create_day = SevenHelper.get_now_day_int()
                     redis_init.rpush("asset_intercept_queue_list",SevenHelper.json_dumps(asset_warn_notice))
                     redis_init.expire("asset_intercept_queue_list", 7 * 24 * 3600)
                     #添加唯一标识预警拦截计数,用于控制台跑数据进行并发预警
                     self._add_onlyid_warn_stat(handler_name)
-
+                
                 return invoke_result_data
-        db_config_dict = config.get_value("db_asset") if config.get_value("db_asset") else config.get_value(self.db_connect_key)
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+        db_transaction = DbTransaction(db_config_dict=config.get_value(self.db_connect_key),context=self.context)
         frame_base_model = FrameBaseModel(context=self.context)
         user_asset_model = UserAssetModel(db_connect_key=self.db_connect_key,sub_table=frame_base_model.get_business_sub_table("user_asset_tb",{"app_id":app_id}),db_transaction=db_transaction, context=self.context)
         asset_log_model = AssetLogModel(db_connect_key=self.db_connect_key,sub_table=frame_base_model.get_business_sub_table("asset_log_tb",{"app_id":app_id}),db_transaction=db_transaction, context=self.context)
         asset_only_model = AssetOnlyModel(db_connect_key=self.db_connect_key,db_transaction=db_transaction, context=self.context)
 
         acquire_lock_name = f"userasset:{user_asset_id_md5}"
         acquire_lock_status, identifier = SevenHelper.redis_acquire_lock(acquire_lock_name)
@@ -327,15 +316,15 @@
                 invoke_result_data.error_message = "系统繁忙,请稍后再试"
                 return invoke_result_data
             try:
                 if only_id:
                     redis_init.hset(only_cache_key, only_id, 1)
                     redis_init.expire(only_cache_key, 24 * 3600)
                 self._delete_asset_dependency_key(act_id,user_id)
-
+                
                 if is_asset_warn == True:
                     asset_queue = {}
                     asset_queue["app_id"] = app_id
                     asset_queue["act_id"] = act_id
                     asset_queue["open_id"] = open_id
                     asset_queue["user_nick"] = user_nick
                     asset_queue["user_id"] = user_id
@@ -349,15 +338,15 @@
                     redis_init.rpush(f"asset_queue_list",SevenHelper.json_dumps(asset_queue))
                     redis_init.expire(f"asset_queue_list", 7 * 24 * 3600)
             except Exception as ex:
                 if self.context:
                     self.context.logging_link_error("【资产队列】" + traceback.format_exc())
                 elif self.logging_link_error:
                     self.logging_link_error("【资产队列】" + traceback.format_exc())
-
+            
             invoke_result_data.data = {"user_asset":user_asset.__dict__}
 
         except Exception as ex:
             if self.context:
                 self.context.logging_link_error("【变更资产】" + traceback.format_exc())
             elif self.logging_link_error:
                 self.logging_link_error("【变更资产】" + traceback.format_exc())
@@ -498,15 +487,15 @@
             elif type(source_object_id) == list:
                 condition += " AND " + SevenHelper.get_condition_by_str_list("source_object_id",source_object_id)
             else:
                 condition += " AND source_object_id=%s"
                 params.append(source_object_id)
         asset_log_model = AssetLogModel(db_connect_key=self.db_connect_key,sub_table=FrameBaseModel(context=self.context).get_business_sub_table("asset_log_tb",{"app_id":app_id}),context=self.context)
         if is_cache:
-            page_list = asset_log_model.get_cache_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params, dependency_key=DependencyKey.asset_log_list(act_id, user_id), page_count_mode=page_count_mode, redis_config_dict=self.__get_redis_dict())
+            page_list = asset_log_model.get_cache_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params, dependency_key=DependencyKey.asset_log_list(act_id,user_id), page_count_mode=page_count_mode)
         else:
             page_list = asset_log_model.get_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params, page_count_mode=page_count_mode)
         result = None
         if page_count_mode in ['total','next']:
             result = page_list[1]
             page_list = page_list[0]
         if len(page_list) > 0:
@@ -671,16 +660,15 @@
         if store_asset_id_md5 == 0:
             invoke_result_data.success = False
             invoke_result_data.error_code = "error"
             invoke_result_data.error_message = "修改失败"
             return invoke_result_data
         if not db_connect_key:
             db_connect_key=self.db_connect_key
-        db_config_dict = config.get_value("db_asset") if config.get_value("db_asset") else config.get_value(db_connect_key)
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+        db_transaction = DbTransaction(db_config_dict=config.get_value(db_connect_key),context=self.context)
         store_asset_model = StoreAssetModel(db_connect_key=db_connect_key, db_transaction=db_transaction, context=self.context)
         store_asset_log_model = StoreAssetLogModel(db_connect_key=db_connect_key, db_transaction=db_transaction, context=self.context)
 
         acquire_lock_name = f"storeasset:{store_asset_id_md5}"
         acquire_lock_status, identifier = SevenHelper.redis_acquire_lock(acquire_lock_name)
         if acquire_lock_status == False:
             invoke_result_data.success = False
@@ -765,15 +753,15 @@
                 elif self.logging_link_error:
                     self.logging_link_error("【变更商家资产】" + message)
                 SevenHelper.redis_release_lock(acquire_lock_name, identifier)
                 invoke_result_data.success = False
                 invoke_result_data.error_code = "fail"
                 invoke_result_data.error_message = "系统繁忙,请稍后再试"
                 return invoke_result_data
-            store_asset_log_model.delete_dependency_key(DependencyKey.store_asset_log_list(app_id), redis_config_dict=self.__get_redis_dict())
+            store_asset_log_model.delete_dependency_key(DependencyKey.store_asset_log_list(app_id))
             invoke_result_data.data = {"store_asset":store_asset.__dict__}
 
         except Exception as ex:
             if self.context:
                 self.context.logging_link_error("【变更商家资产】" + traceback.format_exc())
             elif self.logging_link_error:
                 self.logging_link_error("【变更商家资产】" + traceback.format_exc())
@@ -805,15 +793,15 @@
         if store_asset_dict:
             if share_config.get_value("is_check_asset",True) == True: #是否开启资产校验
                 if store_asset_dict["app_id"] != str(app_id):
                     store_asset_dict["asset_value"] = 0
                 if self.get_asset_check_code(store_asset_dict["id_md5"], store_asset_dict["asset_value"], app_id) != store_asset_dict["asset_check_code"]:
                     store_asset_dict["asset_value"] = 0
         return store_asset_dict
-
+    
     def get_store_asset_list(self, app_ids, asset_type=0, db_connect_key='db_cloudapp'):
         """
         :description: 获取商家资产列表
         :param app_ids：应用标识 多个逗号,分隔
         :param asset_type：资产类型(1-次数2-积分3-价格档位)
         :param db_connect_key：db_connect_key
         :return: 返回list
@@ -823,15 +811,15 @@
             return []
         condition_where = ConditionWhere()
         params_list = []
         if asset_type > 0:
             condition_where.add_condition("asset_type=%s")
             params_list.append(asset_type)
         if ',' in str(app_ids):
-            app_ids = app_ids.split(',')
+                app_ids = app_ids.split(',')
         if isinstance(app_ids,list):
             condition_where.add_condition(SevenHelper.get_condition_by_str_list("app_id",app_ids))
         else:
             condition_where.add_condition("app_id=%s")
             params_list.append(app_ids)
         if not db_connect_key:
             db_connect_key=self.db_connect_key
@@ -902,15 +890,15 @@
             else:
                 condition += " AND source_object_id=%s"
                 params.append(source_object_id)
         if not db_connect_key:
             db_connect_key=self.db_connect_key
         store_asset_log_model = StoreAssetLogModel(db_connect_key=db_connect_key,context=self.context)
         if is_cache:
-            page_list, total = store_asset_log_model.get_cache_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params, dependency_key=DependencyKey.store_asset_log_list(app_id), redis_config_dict=self.__get_redis_dict())
+            page_list, total = store_asset_log_model.get_cache_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params,dependency_key=DependencyKey.store_asset_log_list(app_id))
         else:
             page_list, total = store_asset_log_model.get_dict_page_list(field, page_index, page_size, condition, order_by="id desc", params=params)
         if len(page_list) > 0:
             for item in page_list:
                 if item["app_id"] != app_id:
                     return [],0
                 item["create_day"] = TimeHelper.format_time_to_datetime(str(item["create_date"])).strftime('%Y-%m-%d')
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/cache_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/cache_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJianYi
 :Date: 2020-03-06 23:17:54
-@LastEditTime: 2023-07-20 18:26:59
+@LastEditTime: 2023-07-13 16:11:57
 @LastEditors: HuangJianYi
 :Description: 数据缓存业务模型
 """
 import json
 from copy import deepcopy
 from seven_framework.base_model import *
 from seven_framework import *
@@ -157,16 +157,14 @@
         """
         :description: redis初始化
         :param config_dict: config_dict
         :param decode_responses: decode_responses
         :return: redis_cli
         :last_editors: HuangJianYi
         """
-        if hasattr(self, "redis_config_dict"):
-            config_dict = self.redis_config_dict
         if not config_dict:
             config_dict = config.get_value("redis_cache")
             if not config_dict:
                 config_dict = config.get_value("redis")
         redis_cli = RedisHelper.redis_init(config_dict=config_dict, decode_responses=decode_responses)
         return redis_cli
 
@@ -199,25 +197,14 @@
                         success_count = redis_init.delete(self.get_dependency_key(dependency_key))
                         if success_count == 1:
                             break
                 except:
                     print(traceback.print_exc())
                     pass
 
-    def delete_dependency_keys(self, dependency_keys=[], delay_delete_time=0.01, redis_config_dict=None):
-        """
-        :Description: 删除依赖键,支持延迟删除和重试机制，同时删除多个依赖建
-        :param dependency_keys: 依赖键数组,为空则删除默认依赖建
-        :param delay_delete_time: 延迟删除时间，传0则不进行延迟
-        :param redis_config_dict: redis_config_dict
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        return self.delete_dependency_key(dependency_keys, delay_delete_time, redis_config_dict)
-
     def get_cache_list(self, where='', group_by='', order_by='', limit='', field="*", params=None,dependency_key='', cache_expire=1800, redis_config_dict=None):
         """
         :Description: 根据条件获取列表
         :param where: 数据库查询条件语句
         :param group_by: GROUP BY 语句
         :param order_by:  ORDER BY 语句
         :param limit:  LIMIT 语句
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/cms_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/cms_base_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-11-26 10:22:44
-@LastEditTime: 2023-07-19 16:14:15
+@LastEditTime: 2023-02-16 17:31:18
 @LastEditors: HuangJianYi
 @Description: 
 """
 from seven_cloudapp_frame.models.seven_model import *
 from seven_cloudapp_frame.libs.customize.seven_helper import *
 from seven_cloudapp_frame.models.seven_model import PageInfo
 from seven_cloudapp_frame.models.db_models.cms.cms_info_model import *
 
 class CmsBaseModel():
     """
     :description: 资讯相关业务模型 用于后台或者中台案例和教程等配置信息、字典表用于管理标签、分类等信息
     """
-
-    def __init__(self, context=None, logging_error=None, logging_info=None, db_connect_key='db_cloudapp', redis_config_dict=None):
+    def __init__(self,context=None,logging_error=None,logging_info=None):
         self.context = context
         self.logging_link_error = logging_error
         self.logging_link_info = logging_info
-        self.db_connect_key = db_connect_key
-        self.redis_config_dict = redis_config_dict
-
-    def __get_redis_dict(self):
-        """
-        :description: 获取资讯redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_cms"):
-            config_dict = config.get_value("redis_cms")
-        return config_dict
 
     def _delete_cms_info_dependency_key(self, place_id, delay_delete_time=0.01):
         """
         :description: 删除资讯信息依赖建
         :param place_id: 位置标识
         :param act_id: 活动标识
         :param delay_delete_time: 延迟删除时间，传0则不进行延迟
         :return: 
         :last_editors: HuangJianYi
         """
-        CmsInfoModel(db_connect_key=self.db_connect_key).delete_dependency_key(DependencyKey.cms_info_list(place_id), delay_delete_time, redis_config_dict=self.__get_redis_dict())
+        CmsInfoModel().delete_dependency_key(DependencyKey.cms_info_list(place_id), delay_delete_time)
 
     def save_cms_info(self, place_id, cms_id, app_id, act_id, info_title=None, simple_title=None, simple_title_url=None, info_type=-1, info_summary=None, info_tag=None, info_mark=None, target_url=None, min_pic=None, mid_pic=None, max_pic=None, info_data=None, pic_collect_json=None, sort_index=-1, is_release=-1, i1=-1, i2=-1, i3=-1, i4=-1, s1=None, s2=None, s3=None, s4=None):
         """
         :description: 保存资讯信息
         :param place_id：位置标识
         :param cms_id：信息标识
         :param app_id：应用标识
@@ -78,15 +64,15 @@
         :return
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
         old_cms_info = None
         cms_info = None
         is_add = False
-        cms_info_model = CmsInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        cms_info_model = CmsInfoModel(context=self.context)
         if cms_id > 0:
             cms_info = cms_info_model.get_entity_by_id(cms_id)
             if not cms_info or (app_id and cms_info.app_id != app_id):
                 invoke_result_data.success = False
                 invoke_result_data.error_code = "error"
                 invoke_result_data.error_message = "信息不存在"
                 return invoke_result_data
@@ -167,15 +153,15 @@
         :description: 删除资讯信息
         :param app_id：应用标识
         :param cms_id：资讯标识
         :return: 
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
-        cms_info_model = CmsInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        cms_info_model = CmsInfoModel(context=self.context)
         cms_info_dict = cms_info_model.get_dict_by_id(cms_id)
         if not cms_info_dict or cms_info_dict["app_id"] != app_id:
             invoke_result_data.success = False
             invoke_result_data.error_code = "error"
             invoke_result_data.error_message = "资讯信息不存在"
             return invoke_result_data
         invoke_result_data.success = cms_info_model.del_entity("id=%s",params=[cms_info_dict["id"]])
@@ -189,15 +175,15 @@
         :param app_id：应用标识
         :param cms_id：资讯标识
         :param is_release: 是否发布 1-是 0-否
         :return: 
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
-        cms_info_model = CmsInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        cms_info_model = CmsInfoModel(context=self.context)
         cms_info_dict = cms_info_model.get_dict_by_id(cms_id)
         if not cms_info_dict or cms_info_dict["app_id"] != app_id:
             invoke_result_data.success = False
             invoke_result_data.error_code = "error"
             invoke_result_data.error_message = "资讯信息不存在"
             return invoke_result_data
         modify_date = SevenHelper.get_now_datetime()
@@ -227,22 +213,22 @@
         if app_id:
             condition+=" and app_id=%s"
             params.append(app_id)
         if act_id:
             condition+=" and act_id=%s"
             params.append(act_id)
 
-        cms_info_model = CmsInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        cms_info_model = CmsInfoModel(context=self.context)
         if is_cache == True:
-            page_list = cms_info_model.get_cache_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition, group_by="", order_by=order_by, params=params, dependency_key=DependencyKey.cms_info_list(place_id), cache_expire=600, page_count_mode=page_count_mode, redis_config_dict=self.__get_redis_dict())
+            page_list = cms_info_model.get_cache_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition, group_by="", order_by=order_by,params=params,dependency_key=DependencyKey.cms_info_list(place_id),cache_expire=600,page_count_mode=page_count_mode)
         else:
             page_list = cms_info_model.get_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition, group_by="", order_by=order_by,params=params,page_count_mode=page_count_mode)
-
+        
         return page_list
-
+    
     def get_cms_info_list_v2(self, place_id, page_size, page_index, order_by="id desc", field="*", condition=None, params=None, is_cache=True, page_count_mode="total"):
         """
         :description: 位置信息列表
         :param place_id：位置标识
         :param page_size：页大小
         :param page_index：页索引
         :param order_by：排序
@@ -258,14 +244,14 @@
         condition_where = ConditionWhere()
         condition_where.add_condition("place_id=%s")
         params_list = [place_id]
         if condition:
             condition_where.add_condition(condition)
             params_list.extend(params)
 
-        cms_info_model = CmsInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        cms_info_model = CmsInfoModel(context=self.context)
         if is_cache == True:
-            page_list = cms_info_model.get_cache_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition_where.to_string(), group_by="", order_by=order_by, params=params_list, dependency_key=DependencyKey.cms_info_list(place_id), cache_expire=600, page_count_mode=page_count_mode, redis_config_dict=self.__get_redis_dict())
+            page_list = cms_info_model.get_cache_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition_where.to_string(), group_by="", order_by=order_by,params=params_list,dependency_key=DependencyKey.cms_info_list(place_id),cache_expire=600,page_count_mode=page_count_mode)
         else:
             page_list = cms_info_model.get_dict_page_list(field=field, page_index=page_index, page_size=page_size, where=condition_where.to_string(), group_by="", order_by=order_by,params=params_list,page_count_mode=page_count_mode)
-
+        
         return page_list
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/asset_console_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/asset_console_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-19 13:37:16
-@LastEditTime: 2023-07-19 11:02:08
+@LastEditTime: 2023-04-20 19:18:05
 @LastEditors: HuangJianYi
 @Description: 
 """
 import threading, multiprocessing
 from seven_framework.console.base_console import *
 from seven_cloudapp_frame.libs.customize.seven_helper import *
 from seven_cloudapp_frame.models.db_models.asset.asset_inventory_model import *
@@ -14,18 +14,14 @@
 
 
 
 class AssetConsoleModel():
     """
     :description: 资产控制台业务模型
     """
-    def __init__(self, db_connect_key="db_cloudapp", redis_config_dict=None):
-        self.db_connect_key = db_connect_key
-        self.redis_config_dict = redis_config_dict
-
     def console_asset(self, mod_count=1):
         """
         :description: 控制台资产预警
         :param mod_count: 单表队列数
         :return: 
         :last_editors: HuangJianYi
         """
@@ -35,38 +31,25 @@
 
         n = threading.Thread(target=self._process_asset_inventory_queue, args=[])
         n.start()
 
         t = threading.Thread(target=self._process_asset_intercept_queue, args=[])
         t.start()
 
-
-    def __get_redis_dict(self):
-        """
-        :description: 获取资产redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_asset"):
-            config_dict = config.get_value("redis_asset")
-        return config_dict
-
-
     def _process_onlyid_warn(self):
         """
         :description: 处理唯一值并发预警
         :return: 
         :last_editors: HuangJianYi
         """
         while True:
             try:
                 time.sleep(0.1)
-                asset_warn_notice_model = AssetWarnNoticeModel(db_connect_key=self.db_connect_key)
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+                asset_warn_notice_model = AssetWarnNoticeModel()
+                redis_init = SevenHelper.redis_init()
                 hash_name_1 = f"warn_handler_list_{str(SevenHelper.get_now_int(fmt='%Y%m%d'))}"
                 hkeys = redis_init.hkeys(hash_name_1)
                 if len(hkeys)<=0:
                     time.sleep(1)
                     continue
                 for key in hkeys:
                     date_start = TimeHelper.format_time_to_datetime(format='%Y-%m-%d %H:%M')
@@ -103,25 +86,24 @@
                     asset_warn_notice.create_date = SevenHelper.get_now_datetime()
                     asset_warn_notice.create_day = SevenHelper.get_now_day_int()
                     asset_warn_notice_model.add_entity(asset_warn_notice)
                 time.sleep(5*60)
             except Exception as ex:
                 time.sleep(5)
 
-
     def _push_warn_notice(self):
         """
         :description: 推送预警通知到消息系统
         :return: 
         :last_editors: HuangJianYi
         """
         while True:
             try:
                 time.sleep(0.1)
-                asset_warn_notice_model = AssetWarnNoticeModel(db_connect_key=self.db_connect_key)
+                asset_warn_notice_model = AssetWarnNoticeModel()
                 redis_init = SevenHelper.redis_init(config_dict=config.get_value("warn_redis"))
                 warn_notice_list = asset_warn_notice_model.get_list("is_notice=0 and ascription_type=1",order_by="create_date asc",limit="200")
                 if len(warn_notice_list) > 0:
                     for warn_notice in warn_notice_list:
                         try:
                             push_message = {}
                             push_message["project_id"] = int(config.get_value("project_name",0))
@@ -138,29 +120,28 @@
                         except Exception as ex:
                             logger_error.error(f"推送预警通知异常,json串:{SevenHelper.json_dumps(warn_notice)},ex:{traceback.format_exc()}")
                             continue
                 time.sleep(1)
             except Exception as ex:
                 time.sleep(5)
 
-
     def _process_asset_inventory_warn(self, mod_value, mod_count):
         """
         :description: 处理资产每日进销存是否对等预警
         :param mod_value: 当前队列值
         :param mod_count: 队列数
         :return: 
         :last_editors: HuangJianYi
         """
         print(f"{TimeHelper.get_now_format_time()} 资产每日进销存预警队列{mod_value}启动")
         while True:
             try:
                 time.sleep(0.1)
-                asset_inventory_model = AssetInventoryModel(db_connect_key=self.db_connect_key)
-                asset_warn_notice_model = AssetWarnNoticeModel(db_connect_key=self.db_connect_key)
+                asset_inventory_model = AssetInventoryModel()
+                asset_warn_notice_model = AssetWarnNoticeModel()
                 now_date = TimeHelper.get_now_format_time()
                 now_day_int = SevenHelper.get_now_day_int()
                 if mod_count == 1:
                     asset_inventory_list = asset_inventory_model.get_list(f"create_day={now_day_int} and process_count=0", order_by="create_date asc", limit="200")
                 else:
                     asset_inventory_list = asset_inventory_model.get_list(f"create_day={now_day_int} and process_count=0 and MOD(user_id,{mod_count})={mod_value}", order_by="create_date asc", limit="200")
                 if len(asset_inventory_list) > 0:
@@ -201,26 +182,25 @@
                             logger_error.error(f"资产每日进销存预警队列{mod_value}异常,json串:{SevenHelper.json_dumps(asset_inventory)},ex:{traceback.format_exc()}")
                             continue
                 else:
                     time.sleep(60 * 60)
             except Exception as ex:
                 time.sleep(5)
 
-
     def _process_asset_inventory_queue(self):
         """
         :description: 处理资产队列入进销存
         :return: 
         :last_editors: HuangJianYi
         """
         while True:
             try:
                 time.sleep(0.1)
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
-                asset_inventory_model = AssetInventoryModel(db_connect_key=self.db_connect_key)
+                redis_init = SevenHelper.redis_init()
+                asset_inventory_model = AssetInventoryModel()
                 asset_queue_json = redis_init.lpop(f"asset_queue_list")
                 if not asset_queue_json:
                     time.sleep(1)
                     continue
                 asset_queue_dict = SevenHelper.json_loads(asset_queue_json)
                 try:
                     old_asset_inventory_id = 0
@@ -277,26 +257,25 @@
                     else:
                         logger_error.error(f"资产队列异常,json串:{SevenHelper.json_dumps(asset_queue_dict)},ex:{traceback.format_exc()}")
                     continue
             except Exception as ex:
                 logger_error.error(f"资产队列异常,ex:{traceback.format_exc()}")
                 time.sleep(5)
 
-
     def _process_asset_intercept_queue(self):
         """
         :description: 处理资产拦截队列入库
         :return: 
         :last_editors: HuangJianYi
         """
         while True:
             try:
                 time.sleep(0.1)
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
-                asset_warn_notice_model = AssetWarnNoticeModel(db_connect_key=self.db_connect_key)
+                redis_init = SevenHelper.redis_init()
+                asset_warn_notice_model = AssetWarnNoticeModel()
                 queue_json = redis_init.lpop(f"asset_intercept_queue_list")
                 if not queue_json:
                     time.sleep(1)
                     continue
                 try:
                     queue_dict = SevenHelper.json_loads(queue_json)
                     asset_warn_notice = SevenHelper.auto_mapper(AssetWarnNotice,queue_dict)
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/erp_console_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/erp_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/launch_console_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/launch_console_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/stat_console_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/stat_base_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,432 +1,469 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-19 13:37:16
-@LastEditTime: 2023-07-19 11:24:57
+@Date: 2021-07-26 09:39:08
+@LastEditTime: 2023-06-12 18:48:29
 @LastEditors: HuangJianYi
 @Description: 
 """
-import threading, multiprocessing
-from seven_framework.console.base_console import *
-from seven_cloudapp_frame.models.seven_model import InvokeResultData
-from seven_cloudapp_frame.models.frame_base_model import *
+from seven_cloudapp_frame.models.seven_model import *
 from seven_cloudapp_frame.libs.customize.seven_helper import *
 from seven_cloudapp_frame.libs.common import *
-from seven_cloudapp_frame.models.console_models.timing_work_model import *
+from seven_cloudapp_frame.models.frame_base_model import FrameBaseModel
 from seven_cloudapp_frame.models.db_models.stat.stat_queue_model import *
-from seven_cloudapp_frame.models.db_models.stat.stat_orm_model import *
 from seven_cloudapp_frame.models.db_models.stat.stat_report_model import *
-from seven_cloudapp_frame.models.db_models.stat.stat_log_model import *
-from seven_cloudapp_frame.models.db_models.stat.stat_user_report_model import *
-from seven_cloudapp_frame.models.db_models.stat.stat_user_log_model import *
+from seven_cloudapp_frame.models.db_models.stat.stat_orm_model import *
 
-class StatConsoleModel():
+class StatBaseModel(FrameBaseModel):
     """
-    :description: 统计控制台业务模型
+    :description: 统计上报业务模型
     """
-    def __init__(self, db_connect_key="db_cloudapp", redis_config_dict=None):
+    def __init__(self, context=None,logging_error=None, logging_info=None, db_connect_key='db_cloudapp', redis_config_dict=None):
+        self.context = context
+        self.logging_link_error = logging_error
+        self.logging_link_info = logging_info
         self.db_connect_key = db_connect_key
         self.redis_config_dict = redis_config_dict
+        super(StatBaseModel,self).__init__(context)
 
-    def __get_redis_dict(self):
+    def add_stat(self, app_id, act_id, module_id, user_id, open_id, key_name, key_value, object_id=''):
         """
-        :description: 获取统计redis
-        :return: 
+        :description: 添加活动（模块）上报
+        :param app_id：应用标识
+        :param act_id：活动标识
+        :param module_id：活动模块标识
+        :param user_id：用户标识(比传)
+        :param open_id：open_id(可不传)
+        :param key_name：统计key
+        :param key_value：统计value
+        :param object_id：对象标识
+        :return:
         :last_editors: HuangJianYi
         """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_stat"):
-            config_dict = config.get_value("redis_stat")
-        return config_dict
-
-    def console_stat_queue(self, mod_count=1):
-        """
-        :description: 控制台统计上报
-        :param mod_count: 单表队列数
-        :return: 
+        stat_queue = StatQueue()
+        stat_queue.app_id = app_id
+        stat_queue.act_id = act_id
+        stat_queue.module_id = module_id
+        stat_queue.object_id = object_id
+        stat_queue.user_id = user_id
+        stat_queue.open_id = open_id
+        stat_queue.key_name = key_name
+        stat_queue.key_value = key_value
+        stat_queue.create_date = SevenHelper.get_now_datetime()
+        stat_queue.process_date = SevenHelper.get_now_datetime()
+
+        redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
+        stat_process_ways = share_config.get_value("stat_process_ways","redis")
+        if stat_process_ways == "mysql":
+            stat_queue_model = StatQueueModel(db_connect_key=self.db_connect_key,context=self.context)
+            stat_queue_model.add_entity(stat_queue)
+        else:
+            redis_init.rpush(f"stat_queue_list:{str(user_id % 10)}", SevenHelper.json_dumps(stat_queue))
+
+    def add_stat_list(self, app_id, act_id, module_id, user_id, open_id, stat_data, object_id=''):
+        """
+        :description: 添加活动（模块）上报
+        :param app_id：应用标识
+        :param act_id：活动标识
+        :param module_id：活动模块标识
+        :param user_id：用户标识(比传)
+        :param open_id：open_id(可不传)
+        :param stat_data:统计数据
+        :param object_id：对象标识
+        :return:
         :last_editors: HuangJianYi
         """
-        stat_config = share_config.get_value("stat_config", {})
-        is_process_stat = stat_config.get("is_process_stat", True)
-        if is_process_stat:
-            stat_process_ways = share_config.get_value("stat_process_ways", "redis")
-            if stat_process_ways == "mysql":
-                for i in range(mod_count):
-                    t = threading.Thread(target=self._process_stat_queue, args=[i, mod_count])
-                    t.start()
-            else:
-                for i in range(10):
-                    j = threading.Thread(target=self._process_redis_stat_queue, args=[i])
-                    j.start()
-
-            clea_data_work = ClearDataWork()
-            clea_data_work.start_hours = 2
-            clea_data_work.end_hours = 4
-            clea_data_work.sleep_time = 3600
-            clea_data_work.db_connect_key = self.db_connect_key
-            clea_data_work.start_work("清理统计流水数据作业")
-
-        is_process_stat_user = stat_config.get("is_process_stat_user",False)
-        if is_process_stat_user:
-            for i in range(10):
-                k = threading.Thread(target=self._process_redis_stat_user_queue, args=[i])
-                k.start()
-
-            stat_user_data_work = StatUserDataWork()
-            stat_user_data_work.start_hours = 2
-            stat_user_data_work.end_hours = 4
-            stat_user_data_work.sleep_time = 3600
-            stat_user_data_work.db_connect_key = self.db_connect_key
-            stat_user_data_work.start_work("处理统计用户数据作业")
-
-
-    def _process_stat_queue(self, mod_value, mod_count):
-        """
-        :description: 处理mysql统计队列
-        :param mod_value: 当前队列值
-        :param mod_count: 队列数
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        print(f"{TimeHelper.get_now_format_time()} 统计队列{mod_value}启动")
-        while True:
-            try:
-                time.sleep(0.1)
-                db_transaction = DbTransaction(db_config_dict=config.get_value(self.db_connect_key))
-                stat_queue_model = StatQueueModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction)
-                stat_orm_model = StatOrmModel(db_connect_key=self.db_connect_key)
-                now_date = TimeHelper.get_now_format_time()
-                if mod_count == 1:
-                    stat_queue_list = stat_queue_model.get_list(f"process_count<10 and '{now_date}'>process_date", order_by="process_date asc", limit="200")
+        stat_process_ways = share_config.get_value("stat_process_ways","redis")
+        stat_queue_list = []
+        if isinstance(stat_data,list):
+            for item in stat_data:
+                stat_queue = StatQueue()
+                stat_queue.app_id = app_id
+                stat_queue.act_id = act_id
+                stat_queue.module_id = module_id
+                stat_queue.object_id = object_id
+                stat_queue.user_id = user_id
+                stat_queue.open_id = open_id
+                stat_queue.key_name = item["key"]
+                stat_queue.key_value = item["value"]
+                stat_queue.create_date = SevenHelper.get_now_datetime()
+                stat_queue.process_date = SevenHelper.get_now_datetime()
+                if stat_process_ways == "mysql":
+                    stat_queue_list.append(stat_queue)
                 else:
-                    stat_queue_list = stat_queue_model.get_list(f"MOD(user_id,{mod_count})={mod_value} and process_count<10 and '{now_date}'>process_date", order_by="process_date asc", limit="200")
-                if len(stat_queue_list) > 0:
-                    for stat_queue in stat_queue_list:
-                        try:
-                            stat_report_model = StatReportModel(db_connect_key=self.db_connect_key,db_transaction=db_transaction)
-                            stat_orm = stat_orm_model.get_cache_entity("((act_id=%s and module_id=%s and object_id=%s) or (act_id=0 and module_id=0 and object_id='')) and key_name=%s", params=[stat_queue.act_id, stat_queue.module_id, stat_queue.object_id, stat_queue.key_name], redis_config_dict=self.__get_redis_dict())
-                            if not stat_orm:
-                                stat_queue_model.del_entity("id=%s", params=[stat_queue.id])
-                                continue
-                            create_date = TimeHelper.format_time_to_datetime(stat_queue.create_date)
-                            create_day_int = int(create_date.strftime('%Y%m%d'))
-                            create_month_int = int(create_date.strftime('%Y%m'))
-                            create_year_int = int(create_date.strftime('%Y'))
-                            stat_log_model = StatLogModel(db_connect_key=self.db_connect_key, sub_table=FrameBaseModel().get_business_sub_table("stat_log_tb", {"app_id": stat_queue.app_id}), db_transaction=db_transaction)
-                            is_add = True
-                            if stat_orm.repeat_type > 0:
-                                if stat_orm.repeat_type == 2:
-                                    stat_log_dict = stat_log_model.get_dict("act_id=%s and module_id=%s and orm_id=%s and user_id=%s and object_id=%s", field="id", params=[stat_queue.act_id, stat_queue.module_id, stat_orm.id, stat_queue.user_id, stat_queue.object_id])
-                                else:
-                                    stat_log_dict = stat_log_model.get_dict("act_id=%s and module_id=%s and orm_id=%s and user_id=%s and create_day=%s and object_id=%s", field="id", params=[stat_queue.act_id, stat_queue.module_id, stat_orm.id, stat_queue.user_id, create_day_int, stat_queue.object_id])
-                                if stat_log_dict:
-                                    is_add = False
-
-                            stat_log = StatLog()
-                            stat_log.app_id = stat_queue.app_id
-                            stat_log.act_id = stat_queue.act_id
-                            stat_log.module_id = stat_queue.module_id
-                            stat_log.orm_id = stat_orm.id
-                            stat_log.user_id = stat_queue.user_id
-                            stat_log.open_id = stat_queue.open_id
-                            stat_log.key_value = stat_queue.key_value
-                            stat_log.create_day = create_day_int
-                            stat_log.create_month = create_month_int
-                            stat_log.create_date = create_date
-
-                            stat_report_condition = "act_id=%s and module_id=%s and object_id=%s and key_name=%s and create_day=%s"
-                            stat_report_param = [stat_queue.act_id, stat_queue.module_id, stat_queue.object_id, stat_queue.key_name, create_day_int]
-                            stat_report_dict = stat_report_model.get_dict(stat_report_condition, params=stat_report_param)
-
-                            db_transaction.begin_transaction()
-                            if is_add:
-                                if not stat_report_dict:
-                                    stat_report = StatReport()
-                                    stat_report.app_id = stat_queue.app_id
-                                    stat_report.act_id = stat_queue.act_id
-                                    stat_report.module_id = stat_queue.module_id
-                                    stat_report.object_id = stat_queue.object_id
-                                    stat_report.key_name = stat_queue.key_name
-                                    stat_report.key_value = stat_queue.key_value
-                                    stat_report.create_date = create_date
-                                    stat_report.create_year = create_year_int
-                                    stat_report.create_month = create_month_int
-                                    stat_report.create_day = create_day_int
-                                    stat_report_model.add_entity(stat_report)
-                                else:
-                                    stat_report_model.update_table(f"key_value=key_value+{stat_queue.key_value}", stat_report_condition, params=stat_report_param)
-                                stat_log_model.add_entity(stat_log)
-                            stat_queue_model.del_entity("id=%s", params=[stat_queue.id])
-                            result,message = db_transaction.commit_transaction(True)
-                            if result == False:
-                                raise Exception("执行事务失败", message)
-                        except Exception as ex:
-                            stat_queue.process_count += 1
-                            if stat_queue.process_count <= 10:
-                                stat_queue.process_result = f"出现异常,json串:{SevenHelper.json_dumps(stat_queue)},ex:{traceback.format_exc()}"
-                                minute = 1 if stat_queue.process_count <= 5 else 5
-                                stat_queue.process_date = TimeHelper.add_minutes_by_format_time(minute=minute)
-                                stat_queue_model.update_entity(stat_queue, "process_count,process_result,process_date")
-                            else:
-                                logger_error.error(f"统计队列{mod_value}异常,json串:{SevenHelper.json_dumps(stat_queue)},ex:{traceback.format_exc()}")
-                            continue
+                    stat_queue_list.append(SevenHelper.json_dumps(stat_queue))
+        else:
+            for key,value in stat_data.items():
+                stat_queue = StatQueue()
+                stat_queue.app_id = app_id
+                stat_queue.act_id = act_id
+                stat_queue.module_id = module_id
+                stat_queue.object_id = object_id
+                stat_queue.user_id = user_id
+                stat_queue.open_id = open_id
+                stat_queue.key_name = key
+                stat_queue.key_value = value
+                stat_queue.create_date = SevenHelper.get_now_datetime()
+                stat_queue.process_date = SevenHelper.get_now_datetime()
+                if stat_process_ways == "mysql":
+                    stat_queue_list.append(stat_queue)
                 else:
-                    time.sleep(1)
-            except Exception as ex:
-                logger_error.error(f"统计队列{mod_value}异常,ex:{traceback.format_exc()}")
-                time.sleep(5)
-
+                    stat_queue_list.append(SevenHelper.json_dumps(stat_queue))
 
-    def _process_redis_stat_queue(self, mod_value):
-        """
-        :description: 处理redis统计队列
-        :param mod_value: 当前队列值
-        :return: 
+        if stat_process_ways == "mysql":
+            stat_queue_model = StatQueueModel(db_connect_key=self.db_connect_key,context=self.context)
+            return stat_queue_model.add_list(stat_queue_list)
+        else:
+            if len(stat_queue_list) > 0:
+                redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
+                redis_init.rpush(f"stat_queue_list:{str(user_id % 10)}", *stat_queue_list)
+
+    def get_stat_report_list(self, app_id, act_id, module_id, start_date, end_date, order_by="sort_index asc", is_only_module=False, orm_condition=None, orm_params=None, report_condition=None, report_params=None, object_id=''):
+        """
+        :description: 报表数据列表(表格)
+        :param app_id：应用标识
+        :param act_id：活动标识
+        :param module_id：活动模块标识
+        :param start_date：开始时间
+        :param end_date：结束时间
+        :param order_by：orm排序
+        :param is_only_module：是否只取module的数据
+        :param orm_condition：orm查询条件
+        :param orm_params：orm参数数组
+        :param report_condition：report查询条件
+        :param report_params：report参数数组
+        :param object_id：对象标识
+        :return list
         :last_editors: HuangJianYi
         """
-        print(f"{TimeHelper.get_now_format_time()} 统计队列{mod_value}启动")
-
-        while True:
-            try:
-                time.sleep(0.1)
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
-                redis_stat_key = f"stat_queue_list:{mod_value}"
-                stat_queue_json = redis_init.lindex(redis_stat_key, index=0)
-                if not stat_queue_json:
-                    time.sleep(1)
-                    continue
-                try:
-                    stat_queue_dict = SevenHelper.json_loads(stat_queue_json)
-                    db_transaction = DbTransaction(db_config_dict=config.get_value(self.db_connect_key))
-                    stat_orm_model = StatOrmModel(db_connect_key=self.db_connect_key)
-                    stat_report_model = StatReportModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction)
-                    stat_orm = stat_orm_model.get_cache_entity("((act_id=%s and module_id=%s and object_id=%s) or (act_id=0 and module_id=0 and object_id='')) and key_name=%s", params=[stat_queue_dict["act_id"], stat_queue_dict["module_id"], stat_queue_dict.get("object_id", ''), stat_queue_dict["key_name"]], redis_config_dict=self.__get_redis_dict())
-                    if not stat_orm:
-                        redis_init.lpop(redis_stat_key)
-                        continue
-                    create_date = TimeHelper.format_time_to_datetime(stat_queue_dict["create_date"])
-                    create_day_int = int(create_date.strftime('%Y%m%d'))
-                    create_month_int = int(create_date.strftime('%Y%m'))
-                    create_year_int = int(create_date.strftime('%Y'))
-                    stat_log_model = StatLogModel(sub_table=FrameBaseModel().get_business_sub_table("stat_log_tb", {"app_id": stat_queue_dict["app_id"]}), db_transaction=db_transaction)
-                    is_add = True
-                    if stat_orm.repeat_type > 0:
-                        if stat_orm.repeat_type == 2:
-                            stat_log_dict = stat_log_model.get_dict("act_id=%s and module_id=%s and orm_id=%s and user_id=%s and object_id=%s", field="id", params=[stat_queue_dict["act_id"], stat_queue_dict["module_id"], stat_orm.id, stat_queue_dict["user_id"], stat_queue_dict.get("object_id",'')])
+        if not report_condition:
+            report_condition = "app_id=%s and act_id=%s and module_id=%s and object_id=%s"
+        if not report_params:
+            report_params = [app_id, act_id, module_id, object_id]
+        if start_date != "":
+            report_condition += " and create_date>=%s"
+            report_params.append(start_date)
+        if end_date != "":
+            report_condition += " and create_date<%s"
+            report_params.append(end_date)
+        if is_only_module == True:
+            if not orm_condition:
+                orm_condition = "act_id=%s and module_id=%s and object_id=%s and is_show=1"
+            if not orm_params:
+                orm_params = [act_id, module_id, object_id]
+        else:
+            if not orm_condition:
+                orm_condition = "((act_id=%s and module_id=%s and object_id=%s) or (act_id=0 and module_id=0 and object_id='')) and is_show=1"
+            if not orm_params:
+                orm_params = [act_id, module_id, object_id]
+        stat_orm_list = StatOrmModel(db_connect_key=self.db_connect_key,context=self.context).get_list(where=orm_condition, group_by="key_name", order_by=order_by, params=orm_params)
+        if len(stat_orm_list)<=0:
+            return []
+        key_name_s = ','.join(["'%s'" % str(stat_orm.key_name) for stat_orm in stat_orm_list])
+        report_condition += f" and key_name in({key_name_s})"
+        stat_report_model = StatReportModel(db_connect_key=self.db_connect_key,context=self.context)
+        behavior_report_list = stat_report_model.get_dict_list(report_condition, group_by="key_name", field="key_name,SUM(key_value) AS key_value",params=report_params)
+        #公共映射组（未去重）
+        common_groups_1 = [orm.group_name for orm in stat_orm_list]
+        #公共映射组(去重)
+        common_groups = list(set(common_groups_1))
+        common_groups.sort(key=common_groups_1.index)
+
+        common_group_data_list = []
+
+        for common_group in common_groups:
+            group_data = {}
+            group_data["group_name"] = common_group
+            data_list = []
+
+            # 无子节点
+            orm_list = [orm for orm in stat_orm_list if orm.group_name == common_group and orm.group_sub_name == '']
+            for orm in orm_list:
+                data = {}
+                data["title"] = orm.key_value
+                data["tip_title"] = orm.tip_title
+                data["name"] = orm.key_name
+                data["value"] = 0
+                for behavior_report in behavior_report_list:
+                    if behavior_report["key_name"] == orm.key_name:
+                        if orm.value_type == 2:
+                            data["value"] = behavior_report["key_value"]
                         else:
-                            stat_log_dict = stat_log_model.get_dict("act_id=%s and module_id=%s and orm_id=%s and user_id=%s and create_day=%s and object_id=%s", field="id", params=[stat_queue_dict["act_id"], stat_queue_dict["module_id"], stat_orm.id, stat_queue_dict["user_id"], create_day_int, stat_queue_dict.get("object_id",'')])
-                        if stat_log_dict:
-                            is_add = False
-
-                    stat_log = StatLog()
-                    stat_log.app_id = stat_queue_dict["app_id"]
-                    stat_log.act_id = stat_queue_dict["act_id"]
-                    stat_log.module_id = stat_queue_dict["module_id"]
-                    stat_log.object_id = stat_queue_dict.get("object_id",'')
-                    stat_log.orm_id = stat_orm.id
-                    stat_log.user_id = stat_queue_dict["user_id"]
-                    stat_log.open_id = stat_queue_dict["open_id"]
-                    stat_log.key_value = stat_queue_dict["key_value"]
-                    stat_log.create_day = create_day_int
-                    stat_log.create_month = create_month_int
-                    stat_log.create_date = create_date
-
-                    stat_report_condition = "act_id=%s and module_id=%s and object_id=%s and key_name=%s and create_day=%s"
-                    stat_report_param = [stat_queue_dict["act_id"], stat_queue_dict["module_id"], stat_queue_dict.get("object_id",''), stat_queue_dict["key_name"], create_day_int]
-                    stat_report_dict = stat_report_model.get_dict(stat_report_condition, params=stat_report_param)
-
-                    if is_add:
-                        db_transaction.begin_transaction()
-                        if not stat_report_dict:
-                            stat_report = StatReport()
-                            stat_report.app_id = stat_queue_dict["app_id"]
-                            stat_report.act_id = stat_queue_dict["act_id"]
-                            stat_report.module_id = stat_queue_dict["module_id"]
-                            stat_report.object_id = stat_queue_dict.get("object_id",'')
-                            stat_report.key_name = stat_queue_dict["key_name"]
-                            stat_report.key_value = stat_queue_dict["key_value"]
-                            stat_report.create_date = create_date
-                            stat_report.create_year = create_year_int
-                            stat_report.create_month = create_month_int
-                            stat_report.create_day = create_day_int
-                            stat_report_model.add_entity(stat_report)
-                        else:
-                            key_value = stat_queue_dict["key_value"]
-                            stat_report_model.update_table(f"key_value=key_value+{key_value}", stat_report_condition, params=stat_report_param)
-                        stat_log_model.add_entity(stat_log)
-                        result,message = db_transaction.commit_transaction(True)
-                        if result == False:
-                            raise Exception("执行事务失败", message)
-
-                    redis_init.lpop(redis_stat_key)
-
-                except Exception as ex:
-                    logger_error.error(f"统计队列{mod_value}异常,json串:{SevenHelper.json_dumps(stat_queue_dict)},ex:{traceback.format_exc()}")
-                    continue
-
-            except Exception as ex:
-                logger_error.error(f"统计队列{mod_value}异常,ex:{traceback.format_exc()}")
-                time.sleep(5)
-
-
-    def _process_redis_stat_user_queue(self, mod_value):
+                            data["value"] = int(behavior_report["key_value"])
+                data_list.append(data)
+            if len(data_list) > 0:
+                group_data["data_list"] = data_list
+
+            # 有子节点
+            orm_list_sub = [orm for orm in stat_orm_list if orm.group_name == common_group and orm.group_sub_name != '']
+            if orm_list_sub:
+                groups_sub_name = [orm.group_sub_name for orm in orm_list_sub]
+                #公共映射组(去重)
+                sub_names = list(set(groups_sub_name))
+                sub_names.sort(key=groups_sub_name.index)
+                sub_group_data_list = []
+                for sub_name in sub_names:
+                    sub_group_data = {}
+                    sub_group_data["group_name"] = sub_name
+                    sub_data_list = []
+
+                    # 无子节点
+                    orm_list_1 = [orm for orm in stat_orm_list if orm.group_sub_name == sub_name]
+                    for orm in orm_list_1:
+                        data = {}
+                        data["title"] = orm.key_value
+                        data["tip_title"] = orm.tip_title
+                        data["name"] = orm.key_name
+                        data["value"] = 0
+                        for behavior_report in behavior_report_list:
+                            if behavior_report["key_name"] == orm.key_name:
+                                if orm.value_type == 2:
+                                    data["value"] = behavior_report["key_value"]
+                                else:
+                                    data["value"] = int(behavior_report["key_value"])
+                        sub_data_list.append(data)
+                    sub_group_data["data_list"] = sub_data_list
+                    sub_group_data_list.append(sub_group_data)
+                group_data["sub_data_list"] = sub_group_data_list
+
+            common_group_data_list.append(group_data)
+
+        return common_group_data_list
+
+    def get_trend_report_list(self, app_id, act_id, module_id, start_date, end_date, order_by="sort_index asc", is_only_module=False, orm_condition=None, orm_params=None, report_condition=None, report_params=None, object_id=''):
+        """
+        :description: 报表数据列表(趋势图)
+        :param app_id：应用标识
+        :param act_id：活动标识
+        :param module_id：活动模块标识
+        :param start_date：开始时间
+        :param end_date：结束时间
+        :param order_by：orm排序
+        :param is_only_module：是否只取module的数据
+        :param orm_condition：orm查询条件
+        :param orm_params：orm参数数组
+        :param report_condition：report查询条件
+        :param report_params：report参数数组
+        :param object_id：对象标识
+        :return list
+        :last_editors: HuangJianYi
         """
-        :description: 处理redis统计用户队列
-        :param mod_value: 当前队列值
-        :return: 
+        if not report_condition:
+            report_condition = "app_id=%s and act_id=%s and module_id=%s and object_id=%s"
+        if not report_params:
+            report_params = [app_id, act_id, module_id, object_id]
+        if start_date != "":
+            report_condition += " and create_date>=%s"
+            report_params.append(start_date)
+        if end_date != "":
+            report_condition += " and create_date<%s"
+            report_params.append(end_date)
+        if is_only_module == True:
+            if not orm_condition:
+                orm_condition = "act_id=%s and module_id=%s and object_id=%s and is_show=1"
+            if not orm_params:
+                orm_params = [act_id, module_id, object_id]
+        else:
+            if not orm_condition:
+                orm_condition = "((act_id=%s and module_id=%s and object_id=%s) or (act_id=0 and module_id=0 and object_id='')) and is_show=1"
+            if not orm_params:
+                orm_params = [act_id, module_id, object_id]
+        stat_orm_list = StatOrmModel(db_connect_key=self.db_connect_key,context=self.context).get_list(where=orm_condition, group_by="key_name", order_by=order_by, params=orm_params)
+        if len(stat_orm_list)<=0:
+            return []
+        key_name_s = ','.join(["'%s'" % str(stat_orm.key_name) for stat_orm in stat_orm_list])
+        report_condition += f" and key_name in({key_name_s})"
+        stat_report_model = StatReportModel(db_connect_key=self.db_connect_key,context=self.context)
+        stat_report_list = stat_report_model.get_dict_list(report_condition, field="key_name,key_value,DATE_FORMAT(create_date,'%%Y-%%m-%%d') AS create_date",params=report_params)
+        date_list = SevenHelper.get_date_list(start_date, end_date)
+        #公共映射组（未去重）
+        common_groups_1 = [orm.group_name for orm in stat_orm_list]
+        #公共映射组(去重)
+        common_groups = list(set(common_groups_1))
+        common_groups.sort(key=common_groups_1.index)
+
+        common_group_data_list = []
+
+        for common_group in common_groups:
+            group_data = {}
+            group_data["group_name"] = common_group
+            data_list = []
+
+            # 无子节点
+            orm_list = [orm for orm in stat_orm_list if orm.group_name == common_group and orm.group_sub_name == '']
+            for orm in orm_list:
+                data = {}
+                data["title"] = orm.key_value
+                data["name"] = orm.key_name
+                data["value"] = []
+                for date_day in date_list:
+                    behavior_date_report = {}
+                    for behavior_report in stat_report_list:
+                        if behavior_report["key_name"] == orm.key_name and behavior_report["create_date"] == date_day:
+                            if orm.value_type != 2:
+                                behavior_report["key_value"] = int(behavior_report["key_value"])
+                            behavior_date_report = {"title": orm.key_value, "date": date_day, "value": behavior_report["key_value"]}
+                            break
+                    if not behavior_date_report:
+                        behavior_date_report = {"title": orm.key_value, "date": date_day, "value": 0}
+                    data["value"].append(behavior_date_report)
+                data_list.append(data)
+            if len(data_list) > 0:
+                group_data["data_list"] = data_list
+
+            # 有子节点
+            orm_list_sub = [orm for orm in stat_orm_list if orm.group_name == common_group and orm.group_sub_name != '']
+            if orm_list_sub:
+                groups_sub_name = [orm.group_sub_name for orm in orm_list_sub]
+                #公共映射组(去重)
+                sub_names = list(set(groups_sub_name))
+                sub_names.sort(key=groups_sub_name.index)
+                sub_group_data_list = []
+                for sub_name in sub_names:
+                    sub_group_data = {}
+                    sub_group_data["group_name"] = sub_name
+                    sub_data_list = []
+
+                    # 无子节点
+                    orm_list_1 = [orm for orm in stat_orm_list if orm.group_sub_name == sub_name]
+                    for orm in orm_list_1:
+                        data = {}
+                        data["title"] = orm.key_value
+                        data["name"] = orm.key_name
+                        data["value"] = []
+                        for date_day in date_list:
+                            behavior_date_report = {}
+                            for behavior_report in stat_report_list:
+                                if behavior_report["key_name"] == orm.key_name and behavior_report["create_date"] == date_day:
+                                    if orm.value_type != 2:
+                                        behavior_report["key_value"] = int(behavior_report["key_value"])
+                                    behavior_date_report = {"title": orm.key_value, "date": date_day, "value": behavior_report["key_value"]}
+                                    break
+                            if not behavior_date_report:
+                                behavior_date_report = {"title": orm.key_value, "date": date_day, "value": 0}
+                            data["value"].append(behavior_date_report)
+                        sub_data_list.append(data)
+                    sub_group_data["data_list"] = sub_data_list
+                    sub_group_data_list.append(sub_group_data)
+                group_data["sub_data_list"] = sub_group_data_list
+
+            common_group_data_list.append(group_data)
+
+        return common_group_data_list
+
+    def process_invite_report(self, app_id, act_id, module_id, user_id, open_id, invite_user_id):
+        """
+        :description: 处理邀请进入上报
+        :param app_id:应用标识
+        :param act_id:活动标识
+        :param module_id:活动模块标识
+        :param user_id:用户标识
+        :param open_id:open_id
+        :param invite_user_id:邀请人用户标识
+        :param handler_name:接口名称
+        :return 
         :last_editors: HuangJianYi
         """
-        print(f"{TimeHelper.get_now_format_time()} 统计用户队列{mod_value}启动")
-
-        while True:
-            try:
-                time.sleep(0.1)
-                db_transaction = DbTransaction(db_config_dict=config.get_value(self.db_connect_key))
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
-                redis_stat_key = f"stat_user_queue_list:{mod_value}"
-                stat_queue_json = redis_init.lindex(redis_stat_key, index=0)
-                if not stat_queue_json:
-                    time.sleep(1)
-                    continue
-                try:
-                    stat_queue_dict = SevenHelper.json_loads(stat_queue_json)
-                    stat_user_log_model = StatUserLogModel(db_connect_key=self.db_connect_key, sub_table=FrameBaseModel().get_business_sub_table("stat_user_log_tb", {"app_id": stat_queue_dict["app_id"]}), db_transaction=db_transaction)
-                    stat_user_report_model = StatUserReportModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction)
-                    create_date = TimeHelper.format_time_to_datetime(stat_queue_dict["create_date"])
-                    create_day_int = int(create_date.strftime('%Y%m%d'))
-                    create_month_int = int(create_date.strftime('%Y%m'))
-                    create_year_int = int(create_date.strftime('%Y'))
-                    field_name = stat_queue_dict["key_name"]
-
-                    stat_user_log = StatUserLog()
-                    stat_user_log.app_id = stat_queue_dict["app_id"]
-                    stat_user_log.act_id = stat_queue_dict["act_id"]
-                    stat_user_log.module_id = stat_queue_dict["module_id"]
-                    stat_user_log.user_id = stat_queue_dict["user_id"]
-                    stat_user_log.open_id = stat_queue_dict["open_id"]
-                    stat_user_log.key_name = field_name
-                    stat_user_log.key_value = stat_queue_dict["key_value"]
-                    stat_user_log.request_code = stat_queue_dict.get("request_code","")
-                    stat_user_log.create_day = create_day_int
-                    stat_user_log.create_month = create_month_int
-                    stat_user_log.create_date = create_date
-
-                    stat_report_condition = "act_id=%s and module_id=%s and create_day=%s and user_id=%s"
-                    stat_report_param = [stat_queue_dict["act_id"], stat_queue_dict["module_id"], create_day_int, stat_queue_dict["user_id"]]
-                    stat_report_dict = stat_user_report_model.get_dict(stat_report_condition, params=stat_report_param)
-                    if not stat_report_dict:
-                        stat_user_report = StatUserReport()
-                        stat_user_report.app_id = stat_queue_dict["app_id"]
-                        stat_user_report.act_id = stat_queue_dict["act_id"]
-                        stat_user_report.module_id = stat_queue_dict["module_id"]
-                        stat_user_report.user_id = stat_queue_dict["user_id"]
-                        stat_user_report.open_id = stat_queue_dict["open_id"]
-                        stat_user_report.key_name = field_name
-                        stat_user_report.key_value = stat_queue_dict["key_value"]
-                        stat_user_report.create_date = create_date
-                        stat_user_report.create_year = create_year_int
-                        stat_user_report.create_month = create_month_int
-                        stat_user_report.create_day = create_day_int
-                        stat_user_report_model.add_entity(stat_user_report)
-
-                    db_transaction.begin_transaction()
-                    key_value = stat_queue_dict["key_value"]
-                    stat_user_report_model.update_table(f"{field_name}={field_name}+{key_value}", stat_report_condition, params=stat_report_param)
-                    stat_user_log_model.add_entity(stat_user_log)
-                    result,message = db_transaction.commit_transaction(True)
-                    if result == False:
-                        raise Exception("执行事务失败", message)
-
-                    redis_init.lpop(redis_stat_key)
-
-                except Exception as ex:
-                    logger_error.error(f"统计用户队列{mod_value}异常,json串:{SevenHelper.json_dumps(stat_queue_dict)},ex:{traceback.format_exc()}")
-                    continue
-
-            except Exception as ex:
-                logger_error.error(f"统计用户队列{mod_value}异常,ex:{traceback.format_exc()}")
-                time.sleep(5)
-
-
-class ClearDataWork(TimingWork):
-    """
-    :description: 清理数据
-    :return: 
-    :last_editors: HuangJianYi
-    """
-    def execute(self):
         invoke_result_data = InvokeResultData()
-        self.process_only_table()
+        try:
+            if user_id == invite_user_id:
+                invoke_result_data.success = False
+                invoke_result_data.error_code = "error"
+                invoke_result_data.error_message = "无效邀请"
+                return invoke_result_data
+            key_list_dict = {}
+            key_list_dict["AddBeInvitedUserCount"] = 1 #从分享进入新增用户数
+            key_list_dict["BeInvitedUserCount"] = 1  #从分享进入用户数
+            key_list_dict["BeInvitedCount"] = 1  #从分享进入次数
+            self.add_stat_list(app_id, act_id, module_id, user_id, open_id, key_list_dict)
+        except Exception as ex:
+            if self.context:
+                self.context.logging_link_error("【处理邀请上报】" + traceback.format_exc())
+            elif self.logging_link_error:
+                self.logging_link_error("【处理邀请上报】" + traceback.format_exc())
+            invoke_result_data.success = False
+            invoke_result_data.error_code = "exception"
+            invoke_result_data.error_message = "系统繁忙,请稍后再试"
+            return invoke_result_data
 
         return invoke_result_data
 
-    def process_only_table(self):
+    def process_share_report(self, app_id, act_id, module_id, user_id, open_id):
         """
-        :description: 处理单表
-        :return: 
+        :description: 处理分享上报
+        :param app_id:应用标识
+        :param act_id:活动标识
+        :param module_id:活动模块标识
+        :param user_id:用户标识
+        :param open_id:open_id
+        :return 
         :last_editors: HuangJianYi
         """
-        self.db_connect_key = self.db_connect_key if self.db_connect_key else "db_cloudapp"
-        stat_log_model = StatLogModel(db_connect_key=self.db_connect_key)
-        stat_orm_model = StatOrmModel(db_connect_key=self.db_connect_key)
-        page_index = 0
-        while True:
-            stat_orm_dict_list, is_next = stat_orm_model.get_dict_page_list(field="id,repeat_type", page_index=page_index, page_size=200, order_by="id asc", page_count_mode="next")
-            if len(stat_orm_dict_list) <= 0:
-                break
-            for stat_orm_dict in stat_orm_dict_list:
-                if stat_orm_dict["repeat_type"] != 2:
-                    while True:
-                        is_del = stat_log_model.del_entity("orm_id=%s and create_day<%s", params=[stat_orm_dict["id"], SevenHelper.get_now_day_int(-24 * 15)], limit="100")
-                        if is_del == False:
-                            break
-            page_index += 1
-
-
-class StatUserDataWork(TimingWork):
-    """
-    :description: 处理统计用户数据（用户汇总报表只保留1年的记录，流水只保留1个月）
-    :return: 
-    :last_editors: HuangJianYi
-    """
-
-    def execute(self):
         invoke_result_data = InvokeResultData()
-        self.clear_log()
-        self.clear_report()
-        return invoke_result_data
+        try:
+            key_list_dict = {}
+            key_list_dict["ShareUserCount"] = 1 #分享用户数
+            key_list_dict["ShareCount"] = 1 #分享次数
+            self.add_stat_list(app_id, act_id, module_id, user_id, open_id, key_list_dict)
+        except Exception as ex:
+            if self.context:
+                self.context.logging_link_error("【处理分享上报】" + traceback.format_exc())
+            elif self.logging_link_error:
+                self.logging_link_error("【处理分享上报】" + traceback.format_exc())
+            invoke_result_data.success = False
+            invoke_result_data.error_code = "exception"
+            invoke_result_data.error_message = "系统繁忙,请稍后再试"
+            return invoke_result_data
 
-    def clear_log(self):
-        """
-        :description: 清理流水
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        self.db_connect_key = self.db_connect_key if self.db_connect_key else "db_cloudapp"
-        stat_log_model = StatUserLogModel(db_connect_key=self.db_connect_key)
-        stat_config = share_config.get_value("stat_config", {})
-        space_day = int(stat_config.get("user_log_space_day", 30))
-        while True:
-            is_del = stat_log_model.del_entity("create_day<%s", params=[SevenHelper.get_now_day_int(-24 * space_day)], limit="100")
-            if is_del == False:
-                break
+        return invoke_result_data
 
-    def clear_report(self):
+    def add_stat_user_list(self, app_id, act_id, module_id, user_id, open_id, stat_data, object_id=''):
         """
-        :description: 清理报表(用户统计表需要按年创建分表，然后把数据加入到对应的年分表中，没建表则无法清理报表)
-        :return: 
+        :description: 添加用户行为上报
+        :param app_id：应用标识
+        :param act_id：活动标识
+        :param module_id：活动模块标识
+        :param user_id：用户标识
+        :param open_id：open_id
+        :param stat_data:统计数据
+        :param object_id：对象标识
+        :return:
         :last_editors: HuangJianYi
         """
-        self.db_connect_key = self.db_connect_key if self.db_connect_key else "db_cloudapp"
-        stat_user_report_model = StatUserReportModel(db_connect_key=self.db_connect_key)
-        stat_config = share_config.get_value("stat_config", {})
-        space_day = int(stat_config.get("user_report_space_day", 365))
-        while True:
-            stat_user_report_list = stat_user_report_model.get_list(where="create_day<%s", order_by="id asc", limit="200", params=[SevenHelper.get_now_day_int(-24 * space_day)])
-            if len(stat_user_report_list) <= 0:
-                break
-            for item in stat_user_report_list:
-                create_year = item.create_year
-                stat_user_report_year_model = StatUserReportModel(db_connect_key=self.db_connect_key, sub_table=f"{create_year}")
-                stat_user_report_year_model.add_entity(item)
-                stat_user_report_model.del_entity("id=%s", params=[item.id])
+        stat_queue_list = []
+        if isinstance(stat_data,list):
+            for item in stat_data:
+                stat_queue = StatQueue()
+                stat_queue.app_id = app_id
+                stat_queue.act_id = act_id
+                stat_queue.module_id = module_id
+                stat_queue.object_id = object_id
+                stat_queue.user_id = user_id
+                stat_queue.open_id = open_id
+                stat_queue.key_name = item["key"]
+                stat_queue.key_value = item["value"]
+                if hasattr(self.context, "request_code"):
+                    stat_queue.request_code = self.context.request_code
+                stat_queue.create_date = SevenHelper.get_now_datetime()
+                stat_queue.process_date = SevenHelper.get_now_datetime()
+                stat_queue_list.append(SevenHelper.json_dumps(stat_queue))
+        else:
+            for key,value in stat_data.items():
+                stat_queue = StatQueue()
+                stat_queue.app_id = app_id
+                stat_queue.act_id = act_id
+                stat_queue.module_id = module_id
+                stat_queue.object_id = object_id
+                stat_queue.user_id = user_id
+                stat_queue.open_id = open_id
+                stat_queue.key_name = key
+                stat_queue.key_value = value
+                if hasattr(self.context, "request_code"):
+                    stat_queue.request_code = self.context.request_code
+                stat_queue.create_date = SevenHelper.get_now_datetime()
+                stat_queue.process_date = SevenHelper.get_now_datetime()
+                stat_queue_list.append(SevenHelper.json_dumps(stat_queue))
+
+        redis_init = SevenHelper.redis_init(config_dict=self.redis_config_dict)
+        for stat_queue in stat_queue_list:
+            redis_init.rpush(f"stat_user_queue_list:{str(user_id % 10)}", *stat_queue_list)
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/task_console_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/task_console_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-19 13:37:16
-@LastEditTime: 2023-07-19 10:43:02
+@LastEditTime: 2023-06-08 17:49:57
 @LastEditors: HuangJianYi
 @Description: 
 """
 import threading
 from seven_framework.console.base_console import *
 from seven_cloudapp_frame.models.enum import *
 from seven_cloudapp_frame.models.frame_base_model import *
@@ -19,59 +19,45 @@
 
 
 class TaskConsoleModel():
     """
     :description: 任务控制台业务模型
     """
 
-    def __init__(self, db_connect_key="db_cloudapp", redis_config_dict=None):
-        self.db_connect_key = db_connect_key
-        self.redis_config_dict = redis_config_dict
-
     def console_task_queue(self):
         """
         :description: 控制台统计上报
         :return: 
         :last_editors: HuangJianYi
         """
         for i in range(10):
             j = threading.Thread(target=self.process_task_queue, args=[i])
             j.start()
 
-    def __get_redis_dict(self):
-        """
-        :description: 获取任务redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_task"):
-            config_dict = config.get_value("redis_task")
-        return config_dict
-
     def process_task_queue(self, mod_value):
         """
         :description: 处理档位任务队列
         :param mod_value: 当前队列值
         :return: 
         :last_editors: HuangJianYi
         """
         print(f"{TimeHelper.get_now_format_time()} 档位任务队列{mod_value}启动")
 
         while True:
             try:
                 time.sleep(0.1)
-                redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+
+                redis_init = SevenHelper.redis_init()
                 redis_key = f"task_gear_list:{mod_value}"
                 task_queue_json = redis_init.lindex(redis_key, index=0)
                 if not task_queue_json:
                     time.sleep(1)
                     continue
                 task_queue_dict = SevenHelper.json_loads(task_queue_json)
-                task_base_model = TaskBaseModel(logging_error=logger_error, logging_info=logger_info, db_connect_key=self.db_connect_key, redis_config_dict=self.__get_redis_dict())
+                task_base_model = TaskBaseModel(logging_error=logger_error)
                 invoke_result_data = task_base_model.add_gear_task_count_to_db(task_queue_dict["app_id"], task_queue_dict["act_id"], task_queue_dict["module_id"], task_queue_dict["user_id"], task_queue_dict["open_id"], task_queue_dict["task_type"], task_queue_dict["now_count"], task_queue_dict["remark"])
                 if invoke_result_data.success == True:
                     redis_init.lpop(redis_key)
 
             except Exception as ex:
                 logger_error.error(f"档位任务队列{mod_value}异常,ex:{traceback.format_exc()}")
                 time.sleep(5)
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/console_models/timing_work_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/console_models/timing_work_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self.work_name = "" #作业名称
         self.start_hours = 0 #开始小时
         self.end_hours = 24 #结束小时
         self.fail_count = 0 #失败重试次数
         self.fail_sleep_time = 1 #失败休眠时间，单位秒
         self.sleep_time = 1 #休眠时间，单位秒
         self.is_execute_one = False #是否执行一次
-        self.db_connect_key = None  #db_connect_key
 
     do_work_thread = None
 
     def execute(self):
         """
         :description: 执行内容，用于重写
         :return: InvokeResultData
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_module_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_module_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_prize_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_prize_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/act/act_type_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/act/act_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/app/app_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/app/app_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_inventory_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-19 22:41:48
-@LastEditTime: 2023-07-19 09:42:59
+@LastEditTime: 2021-09-02 18:30:45
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class AssetInventoryModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(AssetInventoryModel, self).__init__(AssetInventory, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
 class AssetInventory:
 
     def __init__(self):
         super(AssetInventory, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_log_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class AssetLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(AssetLogModel, self).__init__(AssetLog, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
 class AssetLog:
 
     def __init__(self):
         super(AssetLog, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_only_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 class AssetOnlyModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(AssetOnlyModel, self).__init__(AssetOnly, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
 class AssetOnly:
 
     def __init__(self):
         super(AssetOnly, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,49 @@
+# -*- coding: utf-8 -*-
+"""
+@Author: HuangJianYi
+@Date: 2021-07-26 09:40:36
+@LastEditTime: 2022-12-07 14:18:05
+@LastEditors: HuangJianYi
+@Description: 
+"""
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
+from seven_cloudapp_frame.models.cache_model import *
 
 
-class AssetWarnNoticeModel(BaseModel):
+class CounterConfigModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(AssetWarnNoticeModel, self).__init__(AssetWarnNotice, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
+        super(CounterConfigModel, self).__init__(CounterConfig, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
-class AssetWarnNotice:
+
+class CounterConfig:
 
     def __init__(self):
-        super(AssetWarnNotice, self).__init__()
+        super(CounterConfig, self).__init__()
         self.id = 0  # id
-        self.app_id = ""  # 应用标识
-        self.act_id = 0  # 活动标识
-        self.ascription_type = 1 # 归属类型(1-预警2-拦截)
-        self.user_id = 0  # 用户标识
-        self.open_id = ""  # open_id
-        self.user_nick = ""  # 用户昵称
-        self.asset_type = 0  # 资产类型(1-次数2-积分3-价格档位)
-        self.asset_object_id = ""  # 对象标识
-        self.handler_name = ""  # 接口名称
-        self.request_code = ""  # 请求代码
-        self.log_title = ""  # 标题
-        self.info_desc = ""  # 详情
-        self.info_json = ""  # 详情json
-        self.is_notice = 0  # 是否通知
-        self.notice_date = "1900-01-01 00:00:00"  # 通知时间
-        self.create_day = 0  # 创建时间天
+        self.key_name = ""  # 计数key
+        self.key_expire = 0  # 计数key过期时间
+        self.db_connect_key = ""  # 数据库连接串Key
+        self.table_name = ""  # 表名
+        self.id_field_name = ""  # 主键字段名称
+        self.value_field_name = ""  # 值字段名称
+        self.is_release = 0  # 是否发布(1是0否)
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id','ascription_type', 'user_id', 'open_id', 'user_nick', 'asset_type', 'asset_object_id', 'handler_name', 'request_code', 'log_title', 'info_desc', 'info_json', 'is_notice', 'notice_date', 'create_day', 'create_date']
+        return ['id', 'key_name', 'key_expire', 'db_connect_key', 'table_name', 'id_field_name', 'value_field_name', 'is_release', 'create_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "asset_warn_notice_tb"
+        return "counter_config_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/base/base_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/base/base_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/browse/browse_log_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class BrowseLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(BrowseLogModel, self).__init__(BrowseLog, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 class BrowseLog:
 
     def __init__(self):
         super(BrowseLog, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/cms_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_log_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,61 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-11-25 18:38:13
-@LastEditTime: 2021-11-26 10:59:17
+@Date: 2021-07-15 17:17:08
+@LastEditTime: 2023-05-18 14:32:11
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class CmsInfoModel(CacheModel):
+class TaskLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(CmsInfoModel, self).__init__(CmsInfo, sub_table)
-        db_connect_key = "db_cms" if config.get_value("db_cms") else db_connect_key
+        super(TaskLogModel, self).__init__(TaskLog, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_cms")
 
     #方法扩展请继承此类
 
-class CmsInfo:
+class TaskLog:
 
     def __init__(self):
-        super(CmsInfo, self).__init__()
+        super(TaskLog, self).__init__()
         self.id = 0  # id
         self.app_id = ""  # 应用标识
         self.act_id = 0  # 活动标识
-        self.place_id = 0  # 信息位标识
-        self.info_title = ""  # 信息标题
-        self.simple_title = ""  # 信息短标题
-        self.simple_title_url = ""  # 短标题链接
-        self.info_type = 0  # 信息类型
-        self.info_summary = ""  # 信息摘要
-        self.info_tag = ""  # 信息标签[文章内容特性][砍人事件]
-        self.info_mark = ""  # 信息标记[首发,推荐,独家，热门]
-        self.target_url = ""  # 跳转地址
-        self.min_pic = ""  # 信息小图
-        self.mid_pic = ""  # 信息中图
-        self.max_pic = ""  # 信息大图
-        self.info_data = ""  # 信息内容
-        self.pic_collect_json = ""  # 图集json
-        self.sort_index = 0  # 排序
-        self.is_release = 0  # 是否发布（1是0否）
-        self.release_date = "1900-01-01 00:00:00"  # 发布时间
+        self.module_id = 0  # 活动模块标识
+        self.user_id = 0  # 用户标识
+        self.open_id = ""  # open_id
+        self.user_nick = ""  # 昵称
+        self.log_title = ""  # 标题
+        self.info_json = ""  # 详情信息
+        self.task_type = 0  # 任务类型
+        self.task_sub_type = ""  # 任务子类型
+        self.task_name = ""  # 任务名称
+        self.reward_type = ""  # 奖励类型
+        self.reward_object_id = ""  # 奖励对象标识
+        self.reward_name = ""  # 奖励名称
+        self.reward_num = 0  # 奖励数量
+        self.handler_name = ""  # 接口名称
+        self.request_code = ""  # 请求代码
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.modify_date = "1900-01-01 00:00:00"  # 更新时间
+        self.create_day = 0  # 创建天
         self.i1 = 0  # i1
-        self.i2 = 0  # i2
-        self.i3 = 0  # i3
-        self.i4 = 0  # i4
         self.s1 = ""  # s1
-        self.s2 = ""  # s2
-        self.s3 = ""  # s3
-        self.s4 = ""  # s4
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'place_id', 'info_title', 'simple_title', 'simple_title_url', 'info_type', 'info_summary', 'info_tag', 'info_mark', 'target_url', 'min_pic', 'mid_pic', 'max_pic', 'info_data', 'pic_collect_json', 'sort_index', 'is_release', 'release_date', 'create_date', 'modify_date', 'i1', 'i2', 'i3', 'i4', 's1', 's2', 's3','s4']
+        return ['id', 'app_id', 'act_id', 'module_id', 'user_id', 'open_id', 'user_nick', 'log_title', 'info_json', 'task_type', 'task_sub_type', 'task_name', 'reward_type', 'reward_object_id', 'reward_name', 'reward_num', 'handler_name', 'request_code', 'create_date', 'create_day', 'i1', 's1']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "cms_info_tb"
+        return "task_log_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/cms/cms_place_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class CmsPlaceModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(CmsPlaceModel, self).__init__(CmsPlace, sub_table)
-        db_connect_key = "db_cms" if config.get_value("db_cms") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_cms")
 
     #方法扩展请继承此类
 
 class CmsPlace:
 
     def __init__(self):
         super(CmsPlace, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/collect/collect_log_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 class CollectLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         super(CollectLogModel, self).__init__(CollectLog, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 class CollectLog:
 
     def __init__(self):
         super(CollectLog, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/counter/counter_config_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-26 09:40:36
-@LastEditTime: 2022-12-07 14:18:05
+@LastEditTime: 2023-05-24 18:33:19
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class CounterConfigModel(CacheModel):
+class StatOrmModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(CounterConfigModel, self).__init__(CounterConfig, sub_table)
+        super(StatOrmModel, self).__init__(StatOrm, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
 
     #方法扩展请继承此类
 
-
-class CounterConfig:
+class StatOrm:
 
     def __init__(self):
-        super(CounterConfig, self).__init__()
+        super(StatOrm, self).__init__()
         self.id = 0  # id
-        self.key_name = ""  # 计数key
-        self.key_expire = 0  # 计数key过期时间
-        self.db_connect_key = ""  # 数据库连接串Key
-        self.table_name = ""  # 表名
-        self.id_field_name = ""  # 主键字段名称
-        self.value_field_name = ""  # 值字段名称
-        self.is_release = 0  # 是否发布(1是0否)
+        self.app_id = ""  # 应用标识
+        self.act_id = 0  # 活动标识
+        self.module_id = 0  # 活动模块标识
+        self.object_id = ""  # 对象标识
+        self.group_name = ""  # 分组名称
+        self.group_sub_name = ""  # 分组子名称
+        self.key_name = ""  # key名称
+        self.key_value = ""  # key值
+        self.tip_title = "" # 提示标题
+        self.value_type = 0 # 输出类型(1-int，2-decimal)
+        self.repeat_type = 0  # 去重方式(0不去重1当日去重2全部去重)
+        self.sort_index = 0  # 排序号
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
+        self.is_show = 0  # 是否显示(1是0否)
+        self.i1 = 0  # i1
+        self.i2 = 0  # i2
+        self.s1 = ""  # s1
+        self.s2 = ""  # s2
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'key_name', 'key_expire', 'db_connect_key', 'table_name', 'id_field_name', 'value_field_name', 'is_release', 'create_date']
+        return ['id', 'app_id', 'act_id', 'module_id', 'object_id', 'group_name', 'group_sub_name', 'key_name', 'key_value', 'tip_title', 'value_type', 'repeat_type', 'sort_index', 'create_date', 'is_show', 'i1', 'i2', 's1', 's2']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "counter_config_tb"
+        return "stat_orm_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/dict/dict_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/erp/erp_relation_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/friend/friend_link_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_module_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_module_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_product_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_product_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_shop_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_shop_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/function/function_skin_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/function/function_skin_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/invite_help_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class InviteHelpModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(InviteHelpModel, self).__init__(InviteHelp, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 class InviteHelp:
 
     def __init__(self):
         super(InviteHelp, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/invite/invite_log_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class InviteLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(InviteLogModel, self).__init__(InviteLog, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 class InviteLog:
 
     def __init__(self):
         super(InviteLog, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/ip_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/ip/ip_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/launch_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/launch/launch_plan_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/marketing/marketing_program_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/middler/middler_product_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/operation_config_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/operation/operation_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/pay/pay_order_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class PayOrderModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(PayOrderModel, self).__init__(PayOrder, sub_table)
-        db_connect_key = "db_order" if config.get_value("db_order") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_order")
 
     #方法扩展请继承此类
 
 class PayOrder:
 
     def __init__(self):
         super(PayOrder, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/price/price_gear_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/price/price_gear_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/prize_order_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class PrizeOrderModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(PrizeOrderModel, self).__init__(PrizeOrder, sub_table)
-        db_connect_key = "db_order" if config.get_value("db_order") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_order")
 
     #方法扩展请继承此类
 
 class PrizeOrder:
 
     def __init__(self):
         super(PrizeOrder, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/prize/prize_roster_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class PrizeRosterModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(PrizeRosterModel, self).__init__(PrizeRoster, sub_table)
-        db_connect_key = "db_order" if config.get_value("db_order") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_order")
 
     #方法扩展请继承此类
 
 class PrizeRoster:
 
     def __init__(self):
         super(PrizeRoster, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/product/product_price_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/product/product_price_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/refund/refund_order_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-09-13 16:26:10
-@LastEditTime: 2023-07-19 13:40:52
+@LastEditTime: 2021-09-30 10:19:50
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class RefundOrderModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(RefundOrderModel, self).__init__(RefundOrder, sub_table)
-        db_connect_key = "db_order" if config.get_value("db_order") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_order")
 
     #方法扩展请继承此类
 
 class RefundOrder:
 
     def __init__(self):
         super(RefundOrder, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/saas/saas_custom_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/skin/skin_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/special/special_goods_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/special/special_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-26 09:40:36
-@LastEditTime: 2023-07-19 11:13:04
+@LastEditTime: 2021-07-29 18:36:50
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class StatLogModel(CacheModel):
+class StatReportModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(StatLogModel, self).__init__(StatLog, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
+        super(StatReportModel, self).__init__(StatReport, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
-class StatLog:
+class StatReport:
 
     def __init__(self):
-        super(StatLog, self).__init__()
+        super(StatReport, self).__init__()
         self.id = 0  # id
         self.app_id = ""  # 应用标识
         self.act_id = 0  # 活动标识
         self.module_id = 0  # 活动模块标识
         self.object_id = ""  # 对象标识
-        self.orm_id = 0  # 映射标识
-        self.user_id = 0  # 用户标识
-        self.open_id = ""  # open_id
+        self.key_name = ""  # key名称
         self.key_value = 0  # key值
-        self.create_day = 0  # 创建日
+        self.create_day = 0  # 创建天
         self.create_month = 0  # 创建月
+        self.create_year = 0  # 创建年
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'module_id', 'object_id', 'orm_id', 'user_id', 'open_id', 'key_value', 'create_day', 'create_month', 'create_date']
+        return ['id', 'app_id', 'act_id', 'module_id', 'object_id', 'key_name', 'key_value', 'create_day', 'create_month', 'create_year', 'create_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "stat_log_tb"
+        return "stat_report_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_orm_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_info_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-26 09:40:36
-@LastEditTime: 2023-05-24 18:33:19
+@Date: 2021-08-10 10:09:06
+@LastEditTime: 2021-08-12 10:11:20
 @LastEditors: HuangJianYi
 @Description: 
 """
+
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class StatOrmModel(CacheModel):
+class TaskInfoModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(StatOrmModel, self).__init__(StatOrm, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
+        super(TaskInfoModel, self).__init__(TaskInfo, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
-class StatOrm:
+class TaskInfo:
 
     def __init__(self):
-        super(StatOrm, self).__init__()
-        self.id = 0  # id
+        super(TaskInfo, self).__init__()
+        self.id = 0  # 标识
         self.app_id = ""  # 应用标识
         self.act_id = 0  # 活动标识
         self.module_id = 0  # 活动模块标识
-        self.object_id = ""  # 对象标识
-        self.group_name = ""  # 分组名称
-        self.group_sub_name = ""  # 分组子名称
-        self.key_name = ""  # key名称
-        self.key_value = ""  # key值
-        self.tip_title = "" # 提示标题
-        self.value_type = 0 # 输出类型(1-int，2-decimal)
-        self.repeat_type = 0  # 去重方式(0不去重1当日去重2全部去重)
-        self.sort_index = 0  # 排序号
+        self.complete_type = 0  # 完成类型(1-每日任务 2-每周任务 3-持久任务 4-每月任务)
+        self.task_name = ""  # 任务名称
+        self.task_type = 0  # 任务类型（公共枚举TaskType，业务继承公共枚举进行拓展）
+        self.config_json = ""  # 任务配置（json字符串，TaskType里面的注释都有详细例子）
+        self.sort_index = 0  # 排序
+        self.is_release = 0  # 是否发布
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.is_show = 0  # 是否显示(1是0否)
+        self.modify_date = "1900-01-01 00:00:00"  # 更新时间
+        self.route_url = ""  # 路由地址
         self.i1 = 0  # i1
         self.i2 = 0  # i2
         self.s1 = ""  # s1
         self.s2 = ""  # s2
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'module_id', 'object_id', 'group_name', 'group_sub_name', 'key_name', 'key_value', 'tip_title', 'value_type', 'repeat_type', 'sort_index', 'create_date', 'is_show', 'i1', 'i2', 's1', 's2']
+        return ['id', 'app_id', 'act_id', 'module_id', 'complete_type', 'task_name', 'task_type', 'config_json', 'sort_index', 'is_release', 'create_date', 'modify_date', 'route_url', 'i1', 'i2', 's1', 's2']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "stat_orm_tb"
+        return "task_info_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_queue_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class StatQueueModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(StatQueueModel, self).__init__(StatQueue, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
 class StatQueue:
 
     def __init__(self):
         super(StatQueue, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_report_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-26 09:40:36
-@LastEditTime: 2023-07-19 11:14:53
+@Date: 2021-07-26 15:41:57
+@LastEditTime: 2021-07-29 18:38:20
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class StatReportModel(CacheModel):
+class ThemeVerModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(StatReportModel, self).__init__(StatReport, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
+        super(ThemeVerModel, self).__init__(ThemeVer, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
-class StatReport:
+class ThemeVer:
 
     def __init__(self):
-        super(StatReport, self).__init__()
+        super(ThemeVer, self).__init__()
         self.id = 0  # id
-        self.app_id = ""  # 应用标识
-        self.act_id = 0  # 活动标识
-        self.module_id = 0  # 活动模块标识
-        self.object_id = ""  # 对象标识
-        self.key_name = ""  # key名称
-        self.key_value = 0  # key值
-        self.create_day = 0  # 创建天
-        self.create_month = 0  # 创建月
-        self.create_year = 0  # 创建年
+        self.theme_id = 0  # 主题标识
+        self.out_id = ""  # 外部id
+        self.client_json = ""  # 客户端内容json
+        self.ver_no = ""  # 客户端版本号
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
+        self.modify_date = "1900-01-01 00:00:00"  # 修改时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'module_id', 'object_id', 'key_name', 'key_value', 'create_day', 'create_month', 'create_year', 'create_date']
+        return ['id', 'theme_id', 'out_id', 'client_json', 'ver_no', 'create_date', 'modify_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "stat_report_tb"
+        return "theme_ver_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_user_log_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class StatUserLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(StatUserLogModel, self).__init__(StatUserLog, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
 class StatUserLog:
 
     def __init__(self):
         super(StatUserLog, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/stat/stat_user_report_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 class StatUserReportModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(StatUserReportModel, self).__init__(StatUserReport, sub_table)
-        db_connect_key = "db_stat" if config.get_value("db_stat") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_stat")
 
     #方法扩展请继承此类
 
 class StatUserReport:
 
     def __init__(self):
         super(StatUserReport, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/store_asset_log_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-15 17:17:08
-@LastEditTime: 2023-07-19 09:47:20
+@LastEditTime: 2022-10-27 17:08:51
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class StoreAssetLogModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(StoreAssetLogModel, self).__init__(StoreAssetLog, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
 
 class StoreAssetLog:
 
     def __init__(self):
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/store/store_asset_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/store/store_asset_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class StoreAssetModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(StoreAssetModel, self).__init__(StoreAsset, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
 
 class StoreAsset:
 
     def __init__(self):
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_coupon_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_login_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/tao/tao_pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_count_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_count_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-10 10:09:06
-@LastEditTime: 2023-07-18 15:40:15
+@LastEditTime: 2021-09-02 17:41:04
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 
 
 class TaskCountModel(BaseModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(TaskCountModel, self).__init__(TaskCount, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 class TaskCount:
 
     def __init__(self):
         super(TaskCount, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/task/task_gear_count_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 
 
 class TaskGearCountModel(BaseModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(TaskGearCountModel, self).__init__(TaskGearCount, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
 
 class TaskGearCount:
 
     def __init__(self):
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,50 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-08-10 10:09:06
-@LastEditTime: 2021-08-12 10:11:20
+@Date: 2021-07-26 15:41:57
+@LastEditTime: 2021-11-25 10:31:12
 @LastEditors: HuangJianYi
 @Description: 
 """
-
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class TaskInfoModel(CacheModel):
+class ThemeInfoModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(TaskInfoModel, self).__init__(TaskInfo, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
+        super(ThemeInfoModel, self).__init__(ThemeInfo, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
-class TaskInfo:
+class ThemeInfo:
 
     def __init__(self):
-        super(TaskInfo, self).__init__()
-        self.id = 0  # 标识
-        self.app_id = ""  # 应用标识
-        self.act_id = 0  # 活动标识
-        self.module_id = 0  # 活动模块标识
-        self.complete_type = 0  # 完成类型(1-每日任务 2-每周任务 3-持久任务 4-每月任务)
-        self.task_name = ""  # 任务名称
-        self.task_type = 0  # 任务类型（公共枚举TaskType，业务继承公共枚举进行拓展）
-        self.config_json = ""  # 任务配置（json字符串，TaskType里面的注释都有详细例子）
-        self.sort_index = 0  # 排序
-        self.is_release = 0  # 是否发布
+        super(ThemeInfo, self).__init__()
+        self.id = 0  # id
+        self.app_id = ""  # 应用唯一标识
+        self.ascription_type = 1  #归属类型(1公共)
+        self.theme_name = ""  # 主题名称
+        self.server_json = ""  # 服务端内容json
+        self.out_id = ""  # 外部id
+        self.style_type = 0  # 样式类型
+        self.sort_index = 0  # 排序号
+        self.is_release = 0  # 是否发布（1发布0未发布）
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.modify_date = "1900-01-01 00:00:00"  # 更新时间
-        self.route_url = ""  # 路由地址
-        self.i1 = 0  # i1
-        self.i2 = 0  # i2
-        self.s1 = ""  # s1
-        self.s2 = ""  # s2
+        self.modify_date = "1900-01-01 00:00:00"  # 修改时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'module_id', 'complete_type', 'task_name', 'task_type', 'config_json', 'sort_index', 'is_release', 'create_date', 'modify_date', 'route_url', 'i1', 'i2', 's1', 's2']
+        return ['id', 'app_id', 'ascription_type', 'theme_name', 'server_json', 'out_id', 'style_type', 'sort_index', 'is_release', 'create_date', 'modify_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "task_info_tb"
+        return "theme_info_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/task/task_log_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_black_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-15 17:17:08
-@LastEditTime: 2023-05-18 14:32:11
+@Date: 2021-07-22 16:03:01
+@LastEditTime: 2021-07-29 18:39:05
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class TaskLogModel(CacheModel):
+class UserBlackModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(TaskLogModel, self).__init__(TaskLog, sub_table)
-        db_connect_key = "db_task" if config.get_value("db_task") else db_connect_key
+        super(UserBlackModel, self).__init__(UserBlack, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_task")
 
     #方法扩展请继承此类
 
-class TaskLog:
+class UserBlack:
 
     def __init__(self):
-        super(TaskLog, self).__init__()
-        self.id = 0  # id
+        super(UserBlack, self).__init__()
+        self.id = 0  # 标识
         self.app_id = ""  # 应用标识
         self.act_id = 0  # 活动标识
-        self.module_id = 0  # 活动模块标识
         self.user_id = 0  # 用户标识
         self.open_id = ""  # open_id
-        self.user_nick = ""  # 昵称
-        self.log_title = ""  # 标题
-        self.info_json = ""  # 详情信息
-        self.task_type = 0  # 任务类型
-        self.task_sub_type = ""  # 任务子类型
-        self.task_name = ""  # 任务名称
-        self.reward_type = ""  # 奖励类型
-        self.reward_object_id = ""  # 奖励对象标识
-        self.reward_name = ""  # 奖励名称
-        self.reward_num = 0  # 奖励数量
-        self.handler_name = ""  # 接口名称
-        self.request_code = ""  # 请求代码
-        self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.create_day = 0  # 创建天
-        self.i1 = 0  # i1
-        self.s1 = ""  # s1
+        self.user_nick = ""  # 用户昵称
+        self.black_type = 0  # 拉黑类型（1自动2手动）
+        self.reason = ""  # 申请原因
+        self.audit_status = 0  # 审核状态(0黑名单1申请中2同意3拒绝)
+        self.audit_remark = ""  # 审核备注
+        self.refund_count = 0  # 退款次数
+        self.refund_order_data = ""  # 退款主订单号(逗号分隔)
+        self.create_date = "1900-01-01 00:00:00"  # 申请时间
+        self.audit_date = "1900-01-01 00:00:00"  # 审核时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'module_id', 'user_id', 'open_id', 'user_nick', 'log_title', 'info_json', 'task_type', 'task_sub_type', 'task_name', 'reward_type', 'reward_object_id', 'reward_name', 'reward_num', 'handler_name', 'request_code', 'create_date', 'create_day', 'i1', 's1']
+        return ['id', 'app_id', 'act_id', 'user_id', 'open_id', 'user_nick', 'black_type', 'reason', 'audit_status', 'audit_remark', 'refund_count', 'refund_order_data', 'create_date', 'audit_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "task_log_tb"
+        return "user_black_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/theme_info_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_asset_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-26 15:41:57
-@LastEditTime: 2021-11-25 10:31:12
+@Date: 2021-07-15 17:17:08
+@LastEditTime: 2021-09-02 18:27:58
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class ThemeInfoModel(CacheModel):
+class UserAssetModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(ThemeInfoModel, self).__init__(ThemeInfo, sub_table)
+        super(UserAssetModel, self).__init__(UserAsset, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
 
     #方法扩展请继承此类
 
-class ThemeInfo:
+class UserAsset:
 
     def __init__(self):
-        super(ThemeInfo, self).__init__()
+        super(UserAsset, self).__init__()
         self.id = 0  # id
-        self.app_id = ""  # 应用唯一标识
-        self.ascription_type = 1  #归属类型(1公共)
-        self.theme_name = ""  # 主题名称
-        self.server_json = ""  # 服务端内容json
-        self.out_id = ""  # 外部id
-        self.style_type = 0  # 样式类型
-        self.sort_index = 0  # 排序号
-        self.is_release = 0  # 是否发布（1发布0未发布）
+        self.id_md5 = 0  # id_md5(act_id+user_id+asset_type+asset_object_id)md5int生成
+        self.app_id = ""  # 应用标识
+        self.act_id = 0  # 活动标识
+        self.user_id = 0  # 用户标识
+        self.open_id = ""  # open_id
+        self.user_nick = ""  # 用户昵称
+        self.asset_type = 0  # 资产类型(1-次数2-积分3-价格档位4-运费券，业务自定义类型从101起，避免跟公共冲突)
+        self.asset_object_id = ""  # 资产对象标识
+        self.asset_value = 0  # 资产值
+        self.asset_check_code = ""  # 资产检验码(id+asset_value+加密签名)md5生成
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.modify_date = "1900-01-01 00:00:00"  # 修改时间
+        self.modify_date = "1900-01-01 00:00:00"  # 更新时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'ascription_type', 'theme_name', 'server_json', 'out_id', 'style_type', 'sort_index', 'is_release', 'create_date', 'modify_date']
+        return ['id', 'id_md5', 'app_id', 'act_id', 'user_id', 'open_id', 'user_nick', 'asset_type', 'asset_object_id', 'asset_value', 'asset_check_code', 'create_date', 'modify_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "theme_info_tb"
+        return "user_asset_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/theme/theme_ver_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_account_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
-@Date: 2021-07-26 15:41:57
-@LastEditTime: 2021-07-29 18:38:20
+@Date: 2021-07-22 10:59:39
+@LastEditTime: 2022-07-20 14:11:07
 @LastEditors: HuangJianYi
 @Description: 
 """
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class ThemeVerModel(CacheModel):
+class UserAccountModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(ThemeVerModel, self).__init__(ThemeVer, sub_table)
+        super(UserAccountModel, self).__init__(UserAccount, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
 
     #方法扩展请继承此类
 
-class ThemeVer:
+
+class UserAccount:
 
     def __init__(self):
-        super(ThemeVer, self).__init__()
+        super(UserAccount, self).__init__()
         self.id = 0  # id
-        self.theme_id = 0  # 主题标识
-        self.out_id = ""  # 外部id
-        self.client_json = ""  # 客户端内容json
-        self.ver_no = ""  # 客户端版本号
+        self.union_id = ""  # union_id
+        self.open_id = ""  # open_id
+        self.user_nick = ""  # 用户昵称
+        self.user_nick_encrypt = ""  # 昵称加密值
+        self.mix_nick = ""  # 混淆昵称
+        self.avatar = ""  # 头像
+        self.user_state = 0  # 用户状态（0-正常，1-黑名单）
+        self.full_name = ""  # 姓名
+        self.telephone = ""  #电话号码
+        self.sex = 0  #性别（1-男，2-女）
+        self.birthday = "1900-01-01"  #生日
+        self.certificate_type = 1  #证件类型(1身份证2军官证)
+        self.certificate_no = "" #证件号码
+        self.relieve_date = "1900-01-01 00:00:00"  # 解禁时间
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
+        self.create_ip = "" #创建IP
         self.modify_date = "1900-01-01 00:00:00"  # 修改时间
+        self.login_date = "1900-01-01 00:00:00"  # 登录时间
+        self.login_ip = "" #登录IP
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'theme_id', 'out_id', 'client_json', 'ver_no', 'create_date', 'modify_date']
+        return ['id', 'union_id', 'open_id', 'user_nick', 'user_nick_encrypt', 'mix_nick', 'avatar', 'user_state', 'full_name', 'telephone', 'sex', 'birthday', 'certificate_type', 'certificate_no', 'relieve_date', 'create_date', 'create_ip', 'modify_date', 'login_date', 'login_ip']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "theme_ver_tb"
+        return "user_account_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/third/third_pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_account_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_info_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-07-22 10:59:39
-@LastEditTime: 2022-07-20 14:11:07
+@LastEditTime: 2022-01-24 10:11:52
 @LastEditors: HuangJianYi
 @Description: 
 """
+
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class UserAccountModel(CacheModel):
+class UserInfoModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(UserAccountModel, self).__init__(UserAccount, sub_table)
-        db_connect_key = "db_user" if config.get_value("db_user") else db_connect_key
+        super(UserInfoModel, self).__init__(UserInfo, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_user")
 
     #方法扩展请继承此类
 
-
-class UserAccount:
+class UserInfo:
 
     def __init__(self):
-        super(UserAccount, self).__init__()
+        super(UserInfo, self).__init__()
         self.id = 0  # id
+        self.id_md5 = ""  # id_md5(act_id+user_id)md5int生成
+        self.app_id = ""  # 应用标识
+        self.act_id = 0  # 活动标识
+        self.user_id = 0  # 用户标识
         self.union_id = ""  # union_id
         self.open_id = ""  # open_id
-        self.user_nick = ""  # 用户昵称
+        self.user_nick = ""  # 昵称
         self.user_nick_encrypt = ""  # 昵称加密值
-        self.mix_nick = ""  # 混淆昵称
         self.avatar = ""  # 头像
+        self.is_auth = 0  # 是否授权（1是0否）
+        self.is_new = 0  # 是否新用户
+        self.pay_price = 0  # 累计支付金额
+        self.pay_num = 0  # 累计支付笔数
+        self.login_token = ""  # 登录令牌
         self.user_state = 0  # 用户状态（0-正常，1-黑名单）
-        self.full_name = ""  # 姓名
-        self.telephone = ""  #电话号码
-        self.sex = 0  #性别（1-男，2-女）
-        self.birthday = "1900-01-01"  #生日
-        self.certificate_type = 1  #证件类型(1身份证2军官证)
-        self.certificate_no = "" #证件号码
+        self.is_member = 0  # 是否会员
+        self.is_member_before = 0  # 用户最初会员状态
+        self.is_favor = 0  # 是否关注店铺
+        self.is_favor_before = 0  # 用户最初关注状态（0未关注1已关注）
         self.relieve_date = "1900-01-01 00:00:00"  # 解禁时间
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
-        self.create_ip = "" #创建IP
-        self.modify_date = "1900-01-01 00:00:00"  # 修改时间
-        self.login_date = "1900-01-01 00:00:00"  # 登录时间
-        self.login_ip = "" #登录IP
+        self.modify_date = "1900-01-01 00:00:00"  # 更新时间
+        self.i1 = 0  # i1
+        self.i2 = 0  # i2
+        self.i3 = 0  # i3
+        self.i4 = 0  # i4
+        self.i5 = 0  # i5
+        self.s1 = ""  # s1
+        self.s2 = ""  # s2
+        self.s3 = ""  # s3
+        self.s4 = ""  # s4
+        self.s5 = ""  # s5
+        self.d1 = "1900-01-01 00:00:00"  # d1
+        self.d2 = "1900-01-01 00:00:00"  # d2
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'union_id', 'open_id', 'user_nick', 'user_nick_encrypt', 'mix_nick', 'avatar', 'user_state', 'full_name', 'telephone', 'sex', 'birthday', 'certificate_type', 'certificate_no', 'relieve_date', 'create_date', 'create_ip', 'modify_date', 'login_date', 'login_ip']
+        return ['id', 'id_md5', 'app_id', 'act_id', 'user_id', 'union_id', 'open_id', 'user_nick', 'user_nick_encrypt', 'avatar', 'is_auth', 'is_new', 'pay_price', 'pay_num', 'login_token', 'user_state', 'is_member', 'is_member_before', 'is_favor', 'is_favor_before', 'relieve_date', 'create_date', 'modify_date', 'i1', 'i2', 'i3', 'i4', 'i5', 's1', 's2', 's3', 's4', 's5', 'd1', 'd2']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "user_account_tb"
+        return "user_info_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_address_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/user/user_address_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
 class UserAddressModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
         super(UserAddressModel, self).__init__(UserAddress, sub_table)
-        db_connect_key = "db_user" if config.get_value("db_user") else db_connect_key
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_user")
 
     #方法扩展请继承此类
 
 class UserAddress:
 
     def __init__(self):
         super(UserAddress, self).__init__()
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_asset_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/version/version_info_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,42 @@
-# -*- coding: utf-8 -*-
-"""
-@Author: HuangJianYi
-@Date: 2021-07-15 17:17:08
-@LastEditTime: 2021-09-02 18:27:58
-@LastEditors: HuangJianYi
-@Description: 
-"""
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
 from seven_cloudapp_frame.models.cache_model import *
 
 
-class UserAssetModel(CacheModel):
+class VersionInfoModel(CacheModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(UserAssetModel, self).__init__(UserAsset, sub_table)
-        db_connect_key = "db_asset" if config.get_value("db_asset") else db_connect_key
+        super(VersionInfoModel, self).__init__(VersionInfo, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_asset")
 
     #方法扩展请继承此类
 
-class UserAsset:
+class VersionInfo:
 
     def __init__(self):
-        super(UserAsset, self).__init__()
+        super(VersionInfo, self).__init__()
         self.id = 0  # id
-        self.id_md5 = 0  # id_md5(act_id+user_id+asset_type+asset_object_id)md5int生成
-        self.app_id = ""  # 应用标识
-        self.act_id = 0  # 活动标识
-        self.user_id = 0  # 用户标识
-        self.open_id = ""  # open_id
-        self.user_nick = ""  # 用户昵称
-        self.asset_type = 0  # 资产类型(1-次数2-积分3-价格档位4-运费券，业务自定义类型从101起，避免跟公共冲突)
-        self.asset_object_id = ""  # 资产对象标识
-        self.asset_value = 0  # 资产值
-        self.asset_check_code = ""  # 资产检验码(id+asset_value+加密签名)md5生成
+        self.type_id = 0  # 类型（1消费者端2千牛端）
+        self.version_number = ""  # 更新版本号
+        self.is_force_update = 0  # 是否强制更新（1是0否）
+        self.content = ""  # 更新内容
+        self.update_scope = 0  # 更新范围(1-全部,会同步更新到baseinfo表2-指定用户) 取最新记录，如果指定用户取最新记录的值，否则取baseinfo表的值
+        self.white_lists = ""  # 更新白名单(多个逗号分隔)
+        self.is_release = 0  # 是否发布（1是0否）
+        self.release_date = "1900-01-01 00:00:00"  # 发布时间
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
         self.modify_date = "1900-01-01 00:00:00"  # 更新时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'id_md5', 'app_id', 'act_id', 'user_id', 'open_id', 'user_nick', 'asset_type', 'asset_object_id', 'asset_value', 'asset_check_code', 'create_date', 'modify_date']
+        return ['id', 'type_id', 'version_number', 'is_force_update', 'content', 'update_scope', 'white_lists', 'is_release', 'release_date', 'create_date', 'modify_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "user_asset_tb"
+        return "version_info_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/db_models/user/user_black_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/db_models/asset/asset_warn_notice_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,48 @@
-# -*- coding: utf-8 -*-
-"""
-@Author: HuangJianYi
-@Date: 2021-07-22 16:03:01
-@LastEditTime: 2021-07-29 18:39:05
-@LastEditors: HuangJianYi
-@Description: 
-"""
 #此文件由rigger自动生成
 from seven_framework.mysql import MySQLHelper
 from seven_framework.base_model import *
-from seven_cloudapp_frame.models.cache_model import *
 
 
-class UserBlackModel(CacheModel):
+class AssetWarnNoticeModel(BaseModel):
     def __init__(self, db_connect_key='db_cloudapp', sub_table=None, db_transaction=None, context=None):
-        super(UserBlackModel, self).__init__(UserBlack, sub_table)
-        db_connect_key = "db_user" if config.get_value("db_user") else db_connect_key
+        super(AssetWarnNoticeModel, self).__init__(AssetWarnNotice, sub_table)
         self.db = MySQLHelper(config.get_value(db_connect_key))
         self.db_connect_key = db_connect_key
         self.db_transaction = db_transaction
         self.db.context = context
-        self.redis_config_dict = config.get_value("redis_user")
 
     #方法扩展请继承此类
 
-class UserBlack:
+class AssetWarnNotice:
 
     def __init__(self):
-        super(UserBlack, self).__init__()
-        self.id = 0  # 标识
+        super(AssetWarnNotice, self).__init__()
+        self.id = 0  # id
         self.app_id = ""  # 应用标识
         self.act_id = 0  # 活动标识
+        self.ascription_type = 1 # 归属类型(1-预警2-拦截)
         self.user_id = 0  # 用户标识
         self.open_id = ""  # open_id
         self.user_nick = ""  # 用户昵称
-        self.black_type = 0  # 拉黑类型（1自动2手动）
-        self.reason = ""  # 申请原因
-        self.audit_status = 0  # 审核状态(0黑名单1申请中2同意3拒绝)
-        self.audit_remark = ""  # 审核备注
-        self.refund_count = 0  # 退款次数
-        self.refund_order_data = ""  # 退款主订单号(逗号分隔)
-        self.create_date = "1900-01-01 00:00:00"  # 申请时间
-        self.audit_date = "1900-01-01 00:00:00"  # 审核时间
+        self.asset_type = 0  # 资产类型(1-次数2-积分3-价格档位)
+        self.asset_object_id = ""  # 对象标识
+        self.handler_name = ""  # 接口名称
+        self.request_code = ""  # 请求代码
+        self.log_title = ""  # 标题
+        self.info_desc = ""  # 详情
+        self.info_json = ""  # 详情json
+        self.is_notice = 0  # 是否通知
+        self.notice_date = "1900-01-01 00:00:00"  # 通知时间
+        self.create_day = 0  # 创建时间天
+        self.create_date = "1900-01-01 00:00:00"  # 创建时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'user_id', 'open_id', 'user_nick', 'black_type', 'reason', 'audit_status', 'audit_remark', 'refund_count', 'refund_order_data', 'create_date', 'audit_date']
+        return ['id', 'app_id', 'act_id','ascription_type', 'user_id', 'open_id', 'user_nick', 'asset_type', 'asset_object_id', 'handler_name', 'request_code', 'log_title', 'info_desc', 'info_json', 'is_notice', 'notice_date', 'create_day', 'create_date']
 
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
-        return "user_black_tb"
+        return "asset_warn_notice_tb"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/enum.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/frame_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/frame_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/goods_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/goods_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/ip_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/ip_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/launch_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/launch_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/module_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/module_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/mp_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/mp_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/operate_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/operate_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/order_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/order_base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-09 09:24:43
-@LastEditTime: 2023-07-19 11:58:30
+@LastEditTime: 2023-06-25 17:20:45
 @LastEditors: HuangJianYi
 @Description: 
 """
 from seven_cloudapp_frame.libs.customize.wechat_helper import WeChatPayRequest
 from seven_cloudapp_frame.models.user_base_model import UserBaseModel
 from seven_cloudapp_frame.models.frame_base_model import FrameBaseModel
 from seven_cloudapp_frame.models.seven_model import *
@@ -159,16 +159,15 @@
         :param express_company：快递公司
         :param express_no：快递单号
         :param prize_roster_sub_table：奖品记录分表名称
         :return: 实体模型InvokeResultData
         :last_editors: HuangJianYi
         """
         now_datetime = SevenHelper.get_now_datetime()
-        db_config_dict = config.get_value("db_order") if config.get_value("db_order") else config.get_value("db_cloudapp")
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+        db_transaction = DbTransaction(db_config_dict=config.get_value("db_cloudapp"),context=self.context)
         prize_order_model = PrizeOrderModel(sub_table=self.get_business_sub_table("prize_order_tb",{"app_id":app_id}), db_transaction=db_transaction, context=self.context)
         if not prize_roster_sub_table:
             prize_roster_sub_table = self.get_business_sub_table("prize_roster_tb",{"app_id":app_id})
         prize_roster_model = PrizeRosterModel(sub_table=prize_roster_sub_table, db_transaction=db_transaction, context=self.context)
         invoke_result_data = InvokeResultData()
 
         prize_order = prize_order_model.get_entity_by_id(prize_order_id)
@@ -412,16 +411,16 @@
         :param county:区县
         :param street:街道
         :param address:地址
         :return 
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
-        db_config_dict = config.get_value("db_order") if config.get_value("db_order") else config.get_value("db_cloudapp")
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+
+        db_transaction = DbTransaction(db_config_dict=config.get_value("db_cloudapp"),context=self.context)
         prize_roster_model = PrizeRosterModel(sub_table=self.get_business_sub_table("prize_roster_tb",{"app_id":app_id}), db_transaction=db_transaction, context=self.context)
         prize_order_model = PrizeOrderModel(sub_table=self.get_business_sub_table("prize_order_tb",{"app_id":app_id}),db_transaction=db_transaction, context=self.context)
         prize_ids_list = []
         if prize_ids:
             prize_ids_list = prize_ids.split(',')
             for prize_id in prize_ids_list:
                 try:
@@ -570,15 +569,15 @@
         """
         :description: 获取已获取奖励的订单子编号列表
         :param app_id:应用标识
         :param user_id:用户标识
         :return: 
         :last_editors: HuangJianYi
         """
-        redis_init = SevenHelper.redis_init(config_dict=config.get_value("redis_order"))
+        redis_init = SevenHelper.redis_init()
         pay_order_cache_key = f"sub_pay_order_no_list:appid_{app_id}_userid_{user_id}"
         pay_order_no_list = redis_init.lrange(pay_order_cache_key,0,-1)
         pay_order_list = []
         is_add = False
         if not pay_order_no_list or len(pay_order_no_list)<=0:
             tao_pay_order_model = TaoPayOrderModel(sub_table=FrameBaseModel(context=self.context).get_business_sub_table("tao_pay_order_tb",{"app_id":app_id}),context=self.context)
             pay_order_list = tao_pay_order_model.get_dict_list("app_id=%s and user_id=%s",field="sub_pay_order_no", params=[app_id,user_id])
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/price_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/price_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/prize_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/prize_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/push_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/push_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/seven_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/shakeshop_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/shakeshop_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/task_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/task_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJianYi
 @Date: 2021-08-10 10:41:13
-@LastEditTime: 2023-07-21 16:12:07
+@LastEditTime: 2023-07-21 16:10:01
 @LastEditors: HuangJianYi
 @Description: 
 """
 from asq.initiators import query
 from seven_cloudapp_frame.models.enum import *
 from seven_cloudapp_frame.models.top_base_model import *
 from seven_cloudapp_frame.models.frame_base_model import FrameBaseModel
@@ -27,74 +27,35 @@
 
 
 
 class TaskBaseModel(FrameBaseModel):
     """
     :description: 任务业务模型
     """
-    def __init__(self, context=None, logging_error=None, logging_info=None, db_connect_key="db_cloudapp", redis_config_dict=None, db_asset_connect_key="db_cloudapp", redis_asset_config_dict=None):
-        """
-        :description: 初始化
-        :param context: 请求上下文
-        :param logging_error: 错误日志对象
-        :param logging_info: 信息日志对象
-        :param db_connect_key: 任务数据库db_key
-        :param redis_config_dict: 任务缓存reids配置
-        :param db_asset_connect_key: 资产数据库db_key
-        :param redis_asset_config_dict: 资产缓存reids配置
-        :return: 
-        :last_editors: HuangJianYi
-        """
+    def __init__(self, context=None,logging_error=None, logging_info=None):
         self.context = context
         self.logging_link_error = logging_error
         self.logging_link_info = logging_info
-        self.db_connect_key = db_connect_key
-        self.redis_config_dict = redis_config_dict
-        self.db_asset_connect_key = db_asset_connect_key
-        self.redis_asset_config_dict = redis_asset_config_dict
-
         super(TaskBaseModel,self).__init__(context)
 
-    def __get_redis_dict(self):
-        """
-        :description: 获取任务redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_config_dict
-        if config.get_value("redis_task"):
-            config_dict = config.get_value("redis_task")
-        return config_dict
-
-    def __get_redis_asset_dict(self):
-        """
-        :description: 获取资产redis
-        :return: 
-        :last_editors: HuangJianYi
-        """
-        config_dict = self.redis_asset_config_dict
-        if config.get_value("redis_asset"):
-            config_dict = config.get_value("redis_asset")
-        return config_dict
-
     def _delete_task_info_dependency_key(self, act_id, task_id=0, delay_delete_time=0.01):
         """
         :description: 删除任务依赖建
         :param act_id: 活动标识
         :param task_id: 任务标识
         :param delay_delete_time: 延迟删除时间，传0则不进行延迟
         :return: 
         :last_editors: HuangJianYi
         """
         dependency_key_list = []
         if task_id:
             dependency_key_list.append(DependencyKey.task_info(task_id))
         if act_id:
             dependency_key_list.append(DependencyKey.task_info_list(act_id))
-        TaskInfoModel(db_connect_key=self.db_connect_key).delete_dependency_key(dependency_key_list, delay_delete_time, self.__get_redis_dict())
+        TaskInfoModel().delete_dependency_key(dependency_key_list,delay_delete_time)
 
     def get_task_info_dict_list(self,app_id,act_id,module_id,is_release,is_cache=True):
         """
         :description: 获取任务列表
         :param app_id: 应用标识
         :param act_id: 活动标识
         :param module_id: 活动模块标识
@@ -112,17 +73,17 @@
         if module_id !=-1:
             condition += " and module_id=%s"
             params.append(module_id)
         if app_id:
             condition += " and app_id=%s"
             params.append(app_id)
 
-        task_info_model = TaskInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        task_info_model = TaskInfoModel(context=self.context)
         if is_cache:
-            dict_list = task_info_model.get_cache_dict_list(condition, group_by="", order_by=order_by, params=params, dependency_key=DependencyKey.task_info_list(act_id), redis_config_dict=self.__get_redis_dict())
+            dict_list = task_info_model.get_cache_dict_list(condition, group_by="", order_by=order_by, params=params,dependency_key=DependencyKey.task_info_list(act_id))
         else:
             dict_list = task_info_model.get_dict_list(condition, group_by="", order_by=order_by, params=params)
         for task_info in dict_list:
             task_info["config_json"] = SevenHelper.json_loads(task_info["config_json"]) if task_info["config_json"] else {}
         return dict_list
 
     def get_task_info_dict(self,task_id,is_cache=True,is_filter=True):
@@ -130,18 +91,18 @@
         :description: 获取任务信息
         :param task_id: 任务标识
         :param is_cache: 是否缓存
         :param is_filter: 是否过滤未发布的数据
         :return: 
         :last_editors: HuangJianYi
         """
-        task_info_model = TaskInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+        task_info_model = TaskInfoModel(context=self.context)
         task_info_dict = None
         if is_cache:
-            task_info_dict = task_info_model.get_cache_dict_by_id(task_id, dependency_key=DependencyKey.task_info(task_id), redis_config_dict=self.__get_redis_dict())
+            task_info_dict = task_info_model.get_cache_dict_by_id(task_id,dependency_key=DependencyKey.task_info(task_id))
         else:
             task_info_dict = task_info_model.get_dict_by_id(task_id)
         if is_filter == True:
             if not task_info_dict or task_info_dict["is_release"] == 0:
                 return None
         return task_info_dict
 
@@ -209,19 +170,19 @@
         :param task_type:任务类型
         :param task_id:任务标识
         :return 
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
         try:
-            task_info_model = TaskInfoModel(db_connect_key=self.db_connect_key, context=self.context)
+            task_info_model = TaskInfoModel(context=self.context)
             if task_id>0:
                 task_info_dict = self.get_task_info_dict(task_id)
             else:
-                task_info_dict = task_info_model.get_cache_dict("act_id=%s and is_release=1 and task_type=%s and module_id=%s",limit="1",params=[act_id,task_type,module_id],dependency_key=f"task_info_list:actid_{act_id}", redis_config_dict=self.__get_redis_dict())
+                task_info_dict = task_info_model.get_cache_dict("act_id=%s and is_release=1 and task_type=%s and module_id=%s",limit="1",params=[act_id,task_type,module_id],dependency_key=f"task_info_list:actid_{act_id}")
             if not task_info_dict or task_info_dict["is_release"] == 0:
                 invoke_result_data.success = False
                 invoke_result_data.error_code = "error"
                 invoke_result_data.error_message = "任务信息不存在"
                 return invoke_result_data
             config_json = SevenHelper.json_loads(task_info_dict["config_json"])
             if not config_json:
@@ -482,15 +443,15 @@
                 task_log.reward_name = reward_name if reward_name else ""
                 task_log.reward_num = reward_num if reward_num else 0
                 task_log.handler_name = handler_name
                 task_log.request_code = request_code
                 task_log.info_json = SevenHelper.json_dumps(info_json) if info_json else {}
                 task_log.create_date = SevenHelper.get_now_datetime()
                 task_log.create_day = SevenHelper.get_now_day_int()
-                task_log_model = TaskLogModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_log_tb",{"app_id":app_id}), context=self.context)
+                task_log_model = TaskLogModel(sub_table=self.get_business_sub_table("task_log_tb",{"app_id":app_id}), context=self.context)
                 task_log_model.add_entity(task_log)
             except Exception as ex:
                 self.context.logging_link_error("【添加任务日志】" + traceback.format_exc())
 
     def add_gear_task_count(self, app_id, act_id, module_id, user_id, open_id, task_type, value, remark='', is_async=True):
         """
         :description: 添加档位任务累计值，目前支持消费类任务、累计抽盒/抽奖次数档位任务
@@ -515,15 +476,15 @@
             task_gear_count.open_id = open_id
             task_gear_count.task_type = task_type
             task_gear_count.now_count = value
             task_gear_count.create_day = SevenHelper.get_now_day_int()
             task_gear_count.create_month = SevenHelper.get_now_month_int()
             task_gear_count.create_date = SevenHelper.get_now_datetime()
             task_gear_count.remark = remark
-            redis_init = SevenHelper.redis_init(config_dict=self.__get_redis_dict())
+            redis_init = SevenHelper.redis_init()
             redis_init.rpush(f"task_gear_list:{str(user_id % 10)}", SevenHelper.json_dumps(task_gear_count))
         else:
             self.add_gear_task_count_to_db(app_id, act_id, module_id, user_id, open_id, task_type, value, remark)
 
     def add_gear_task_count_to_db(self, app_id, act_id, module_id, user_id, open_id, task_type, value, remark=''):
         """
         :description: 添加档位任务累计值，目前支持消费类任务、累计抽盒/抽奖次数档位任务
@@ -538,20 +499,19 @@
         :return:
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
         try:
             create_day = SevenHelper.get_now_day_int()
             create_month = SevenHelper.get_now_month_int()
-            task_info_model = TaskInfoModel(db_connect_key=self.db_connect_key, context=self.context)
-            db_config_dict = config.get_value("db_task") if config.get_value("db_task") else config.get_value(self.db_connect_key)
-            db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+            task_info_model = TaskInfoModel(context=self.context)
+            db_transaction = DbTransaction(db_config_dict=config.get_value("db_cloudapp"))
             frame_base_model = FrameBaseModel()
-            task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=frame_base_model.get_business_sub_table("task_count_tb", {"app_id": app_id}), db_transaction=db_transaction)
-            task_gear_count_model = TaskGearCountModel(db_connect_key=self.db_connect_key, sub_table=frame_base_model.get_business_sub_table("task_gear_count_tb", {"app_id": app_id}), db_transaction=db_transaction)
+            task_count_model = TaskCountModel(sub_table=frame_base_model.get_business_sub_table("task_count_tb", {"app_id": app_id}), db_transaction=db_transaction)
+            task_gear_count_model = TaskGearCountModel(sub_table=frame_base_model.get_business_sub_table("task_gear_count_tb", {"app_id": app_id}), db_transaction=db_transaction)
             task_info_dict = task_info_model.get_dict("act_id=%s and module_id=%s and task_type=%s", params=[act_id, module_id, task_type])
             task_gear_count_id_md5 = CryptoHelper.md5_encrypt_int(f"{act_id}_{module_id}_{task_type}_{user_id}")
             task_gear_count = task_gear_count_model.get_entity("id_md5=%s and create_day=%s", params=[task_gear_count_id_md5, create_day])
             db_transaction.begin_transaction()
             if not task_gear_count:
                 task_gear_count = TaskGearCount()
                 task_gear_count.id_md5 = task_gear_count_id_md5
@@ -643,15 +603,15 @@
                     return invoke_result_data
                 limit_num = int(sub_config_json["limit_num"]) if sub_config_json.__contains__("limit_num") else 1
                 satisfy_num = int(sub_config_json["satisfy_num"]) if sub_config_json.__contains__("satisfy_num") else 1
             else:
                 config_json = task_info_dict["config_json"]
                 limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-            task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+            task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
             task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],task_sub_type,user_id)
             task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
             task_count_list = [task_count] if task_count else []
             task_count = self.init_task_count(task_info_dict, task_count_list, task_sub_type)
             count = int(task_count.complete_count * satisfy_num) + task_count.now_count
             is_limit = True if count >= (limit_num * satisfy_num) else False
             if is_limit == True:
@@ -689,15 +649,15 @@
         :param module_id：活动模块标识
         :param user_id：用户标识(比传)
         :param task_type：任务类型
         :param complete_type：完成类型
         :return:
         :last_editors: HuangJianYi
         """
-        task_gear_count_model = TaskGearCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_gear_count_tb", {"app_id": app_id}), context=self.context)
+        task_gear_count_model = TaskGearCountModel(sub_table=self.get_business_sub_table("task_gear_count_tb", {"app_id": app_id}), context=self.context)
         condition_where = ConditionWhere()
         task_gear_count_id_md5 = CryptoHelper.md5_encrypt_int(f"{act_id}_{module_id}_{task_type}_{user_id}")
         condition_where.add_condition("id_md5=%s")
         params = [task_gear_count_id_md5]
         if complete_type == TaskCompleteType.day.value:
             condition_where.add_condition("create_day=%s")
             params.append(SevenHelper.get_now_day_int())
@@ -804,15 +764,15 @@
         :param is_log:是否记录top请求日志
         :param daily_repeat_browse:单个商品可每日重复浏览 True是False否
         :param mix_nick:混淆昵称
         :return 
         :last_editors: HuangJianYi
         """
         task_info_list = self.get_task_info_dict_list(app_id,act_id,module_id,1)
-        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
         task_count_list = task_count_model.get_list("act_id=%s and module_id=%s and user_id=%s", params=[act_id, module_id, user_id])
         now_day = TimeExHelper.get_now_day_int()
         app_info_dict = None
         result_list = []
         for task_info_dict in task_info_list:
             if task_types:
                 if str(task_info_dict["task_type"]) not in task_types.split(','):
@@ -991,18 +951,18 @@
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                 if task_count.complete_count >= limit_num:
                     result["status"] = 2
                 elif task_count.now_count >= satisfy_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                collect_log_model = CollectLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                collect_log_model = CollectLogModel(context=self.context)
                 condition = "act_id=%s and user_id=%s"
                 params = [act_id, user_id]
-                user_goods_list = collect_log_model.get_cache_list(condition, params=params, dependency_key=f"collect_log:actid_{act_id}_userid_{user_id}", redis_config_dict=self.__get_redis_dict())
+                user_goods_list = collect_log_model.get_cache_list(condition, params=params,dependency_key=f"collect_log:actid_{act_id}_userid_{user_id}")
                 result["goods_list"] = config_json["goods_list"] if config_json.__contains__("goods_list") else []
                 result["user_goods_list"] = [str(i.goods_id) for i in user_goods_list] if len(user_goods_list) > 0 else []
                 result["complete_count"] = task_count.complete_count
                 result["now_count"] = task_count.now_count
                 result["limit_num"] = limit_num
                 result["satisfy_num"] = satisfy_num
                 result["content"] = f"完成次数上限{limit_num}次，当前剩余{limit_num-task_count.complete_count}次"
@@ -1014,21 +974,21 @@
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                 if task_count.complete_count >= limit_num:
                     result["status"] = 2
                 elif task_count.now_count >= satisfy_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                browse_log_model = BrowseLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                browse_log_model = BrowseLogModel(context=self.context)
                 condition = "act_id=%s and user_id=%s"
                 params = [act_id,user_id]
                 if daily_repeat_browse == True:
                     condition += " and create_day=%s"
                     params.append(now_day)
-                user_goods_list = browse_log_model.get_cache_list(condition, params=params,dependency_key=f"browse_log:actid_{act_id}_userid_{user_id}", redis_config_dict=self.__get_redis_dict())
+                user_goods_list = browse_log_model.get_cache_list(condition, params=params,dependency_key=f"browse_log:actid_{act_id}_userid_{user_id}")
                 result["goods_list"] = config_json["goods_list"] if config_json.__contains__("goods_list") else []
                 result["user_goods_list"] = [str(i.goods_id) for i in user_goods_list] if len(user_goods_list) > 0 else []
                 result["complete_count"] = task_count.complete_count
                 result["now_count"] = task_count.now_count
                 result["limit_num"] = limit_num
                 result["satisfy_num"] = satisfy_num
                 result["content"] = f"完成次数上限{limit_num}次，当前剩余{limit_num-task_count.complete_count}次"
@@ -1121,19 +1081,19 @@
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                 if task_count.complete_count >= limit_num:
                     result["status"] = 2
                 elif task_count.now_count >= satisfy_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                invite_help_model = InviteHelpModel(db_connect_key=self.db_connect_key, context=self.context)
+                invite_help_model = InviteHelpModel(context=self.context)
                 help_type = 1
                 help_object_id = ''
                 help_id_md5 = CryptoHelper.md5_encrypt_int(f"{app_id}_{act_id}_{module_id}_{help_type}_{help_object_id}")
-                invite_help_list = invite_help_model.get_cache_dict_list("id_md5=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invited_avatar", params=[help_id_md5, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_user_help_list(help_id_md5,user_id), redis_config_dict=self.__get_redis_dict())
+                invite_help_list = invite_help_model.get_cache_dict_list("id_md5=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invited_avatar", params=[help_id_md5, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_user_help_list(help_id_md5,user_id))
                 result["data"] = invite_help_list if len(invite_help_list) > 0 else []
                 result["complete_count"] = task_count.complete_count
                 result["now_count"] = task_count.now_count
                 result["limit_num"] = limit_num
                 result["satisfy_num"] = satisfy_num
                 result["content"] = f"完成次数上限{limit_num}次，当前剩余{limit_num-task_count.complete_count}次"
                 result["text"] = ["去邀请", "领取", "已完成"]
@@ -1174,15 +1134,15 @@
         :param user_id:用户标识
         :param task_types:任务类型 多个逗号,分隔
         :param daily_repeat_browse:单个商品可每日重复浏览 True是False否
         :return 
         :last_editors: HuangJianYi
         """
         task_info_list = self.get_task_info_dict_list(app_id,act_id,module_id,1)
-        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
         task_count_list = task_count_model.get_list("act_id=%s and module_id=%s and user_id=%s", params=[act_id, module_id, user_id])
         now_day = TimeExHelper.get_now_day_int()
         result_list = []
         for task_info_dict in task_info_list:
             if task_types:
                 if str(task_info_dict["task_type"]) not in task_types.split(','):
                     continue
@@ -1304,16 +1264,16 @@
                 limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 0
                 get_ways = config_json["get_ways"] if config_json.__contains__("get_ways") else 1
                 if task_count.complete_count >= limit_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, context=self.context)
-                invite_log_list = invite_log_model.get_cache_dict_list("act_id=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invite_avatar", params=[act_id, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_log_list(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                invite_log_model = InviteLogModel(context=self.context)
+                invite_log_list = invite_log_model.get_cache_dict_list("act_id=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invite_avatar", params=[act_id, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_log_list(act_id,user_id))
                 result["data"] = invite_log_list if len(invite_log_list) > 0 else []
                 result["title"] = f"每日邀请{satisfy_num}名新用户"
                 result["total"] = satisfy_num
                 result["current"] = task_count.now_count
                 result["complete_count"] = limit_num #可以完成的次数
                 result["current_complete_count"] = task_count.complete_count #当前完成的次数
                 result["desc"] = f"{complete_type_name}完成上限{limit_num}次，当前剩余" + "{remain_complete_count}次"
@@ -1326,16 +1286,16 @@
                 limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 0
                 get_ways = config_json["get_ways"] if config_json.__contains__("get_ways") else 1
                 if task_count.complete_count >= limit_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, sub_table="member", context=self.context)
-                invite_log_list = invite_log_model.get_cache_dict_list("act_id=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invite_avatar", params=[act_id, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_log_member_list(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                invite_log_model = InviteLogModel(context=self.context, sub_table="member")
+                invite_log_list = invite_log_model.get_cache_dict_list("act_id=%s and user_id=%s and create_day=%s", "", order_by="id desc", field="invite_avatar", params=[act_id, user_id, SevenHelper.get_now_day_int()], dependency_key=DependencyKey.invite_log_member_list(act_id,user_id))
                 result["data"] = invite_log_list if len(invite_log_list) > 0 else []
                 result["title"] = f"每日邀请{satisfy_num}名入会"
                 result["total"] = satisfy_num
                 result["current"] = task_count.now_count
                 result["complete_count"] = limit_num #可以完成的次数
                 result["current_complete_count"] = task_count.complete_count #当前完成的次数
                 result["desc"] = f"{complete_type_name}完成上限{limit_num}次，当前剩余" + "{remain_complete_count}次"
@@ -1392,38 +1352,38 @@
                 result["current_complete_count"] = task_count.complete_count #当前完成的次数
                 result["btn_text"] = ["立即入会", "已领取"]
                 result["route_url"] = "task_member"
                 result_list.append(result)
             #收藏商品
             elif task_info_dict["task_type"] == TaskType.collect_goods.value:
                 get_ways = config_json["get_ways"] if config_json.__contains__("get_ways") else 1
-                collect_log_model = CollectLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                collect_log_model = CollectLogModel(context=self.context)
                 condition = "act_id=%s and user_id=%s"
                 params = [act_id, user_id]
-                user_goods_list = collect_log_model.get_cache_list(condition, params=params,dependency_key=DependencyKey.collect_log(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                user_goods_list = collect_log_model.get_cache_list(condition, params=params,dependency_key=DependencyKey.collect_log(act_id,user_id))
                 result["data"] = config_json["goods_list"] if config_json.__contains__("goods_list") else []
                 result["completed_ids"] = [str(i.goods_id) for i in user_goods_list] if len(user_goods_list) > 0 else []
                 result["current"] = task_count.now_count
                 result["total"] = len(result["data"])
                 result["status"] = 1 if len(result["data"]) == len(result["completed_ids"]) else 0
                 result["get_ways"] = get_ways
                 result["current_complete_count"] = 1 if result["status"] == 1 else 0 #当前完成的次数
                 result["btn_text"] = ["去收藏", "已完成"]
                 result["route_url"] = "task_collect"
                 result_list.append(result)
             #浏览商品
             elif task_info_dict["task_type"] == TaskType.browse_goods.value:
                 get_ways = config_json["get_ways"] if config_json.__contains__("get_ways") else 1
-                browse_log_model = BrowseLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                browse_log_model = BrowseLogModel(context=self.context)
                 condition = "act_id=%s and user_id=%s"
                 params = [act_id,user_id]
                 if daily_repeat_browse == True:
                     condition += " and create_day=%s"
                     params.append(now_day)
-                user_goods_list = browse_log_model.get_cache_list(condition, params=params,dependency_key=DependencyKey.browse_log(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                user_goods_list = browse_log_model.get_cache_list(condition, params=params,dependency_key=DependencyKey.browse_log(act_id,user_id))
                 result["data"] = config_json["goods_list"] if config_json.__contains__("goods_list") else []
                 result["completed_ids"] = [str(i.goods_id) for i in user_goods_list] if len(user_goods_list) > 0 else []
                 result["current"] = task_count.now_count
                 result["total"] = len(result["data"])
                 result["status"] = 1 if len(result["data"]) == len(result["completed_ids"]) else 0
                 result["get_ways"] = get_ways
                 result["current_complete_count"] = 1 if result["status"] == 1 else 0 #当前完成的次数
@@ -1477,19 +1437,19 @@
                 get_ways = config_json["get_ways"] if config_json.__contains__("get_ways") else 1
                 limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                 satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 0
                 if task_count.complete_count >= limit_num:
                     result["status"] = 1
                 else:
                     result["status"] = 0
-                invite_help_model = InviteHelpModel(db_connect_key=self.db_connect_key, context=self.context)
+                invite_help_model = InviteHelpModel(context=self.context)
                 help_type = 1
                 help_object_id = ''
                 help_id_md5 = CryptoHelper.md5_encrypt_int(f"{app_id}_{act_id}_{module_id}_{help_type}_{help_object_id}")
-                invite_help_list = invite_help_model.get_cache_dict_list("id_md5=%s and user_id=%s", "", order_by="id desc", field="invited_avatar", params=[help_id_md5, user_id], dependency_key=DependencyKey.invite_user_help_list(help_id_md5, user_id), redis_config_dict=self.__get_redis_dict())
+                invite_help_list = invite_help_model.get_cache_dict_list("id_md5=%s and user_id=%s", "", order_by="id desc", field="invited_avatar", params=[help_id_md5, user_id], dependency_key=DependencyKey.invite_user_help_list(help_id_md5, user_id))
                 result["data"] = invite_help_list if len(invite_help_list) > 0 else []
                 result["title"] = f"每日邀请{satisfy_num}名用户"
                 result["total"] = satisfy_num
                 result["current"] = task_count.now_count
                 result["get_ways"] = get_ways
                 result["complete_count"] = limit_num #可以完成的次数
                 result["current_complete_count"] = task_count.complete_count #当前完成的次数
@@ -1647,16 +1607,15 @@
             acquire_lock_name = f"process_receive_reward_taskid:{act_id}_{module_id}_{task_id}_{user_id}"
         else:
             source_object_id = f"tasktype_{task_type}"
             acquire_lock_name = f"process_receive_reward_tasktype:{act_id}_{module_id}_{task_type}_{user_id}"
 
         log_title = ""
         now_day = TimeExHelper.get_now_day_int()
-        db_config_dict = config.get_value("db_task") if config.get_value("db_task") else config.get_value(self.db_connect_key)
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+        db_transaction = DbTransaction(db_config_dict=config.get_value("db_cloudapp"),context=self.context)
         try:
             invoke_result_data = self.business_process_executing(app_id, act_id, module_id, user_id, login_token, handler_name, check_new_user, check_user_nick, continue_request_expire, acquire_lock_name, source_object_id=source_object_id,check_act_info_release=check_act_info_release,check_act_module_release=check_act_module_release)
             if invoke_result_data.success == True:
                 task_invoke_result_data = self.check_task_info(act_id,module_id,task_type=task_type,task_id=task_id)
                 if task_invoke_result_data.success == True:
                     task_info_dict = task_invoke_result_data.data
                     config_json = task_info_dict["config_json"]
@@ -1671,15 +1630,15 @@
                     reward_value = int(config_json["reward_value"]) if config_json.__contains__("reward_value") else 0
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     satisfy_num = decimal.Decimal(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
                     invoke_result_data.data["task_info_dict"] = task_info_dict
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), db_transaction=db_transaction, context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),db_transaction=db_transaction, context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_type,task_sub_type,user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     if task_info_dict["complete_type"] == TaskCompleteType.day.value and task_count.modify_day != now_day:
                         task_count.complete_count = 0
                         task_count.now_count = 0
                         task_count.remark = ""
@@ -1718,15 +1677,15 @@
                                 cur_complete_count = int(task_count.now_count / satisfy_num)
                             reward_value = cur_complete_count * reward_value
                             cur_now_count = task_count.now_count - (cur_complete_count * satisfy_num)
                             if task_type == TaskType.invite_new_user.value:
                                 invite_sub_table = ""
                             else:
                                 invite_sub_table = "member"
-                            invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, sub_table=invite_sub_table, db_transaction=db_transaction, context=self.context)
+                            invite_log_model = InviteLogModel(sub_table=invite_sub_table,db_transaction=db_transaction,context=self.context)
                             #获取邀请用户数
                             if task_info_dict["complete_type"] == 1:
                                 invite_list = invite_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, now_day])
                             elif task_info_dict["complete_type"] == 2:
                                 start_day = int(TimeHelper.get_first_day_of_the_week().strftime('%Y%m%d'))
                                 end_day = int(TimeHelper.get_last_day_of_the_week().strftime('%Y%m%d'))
                                 invite_list = invite_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day>=%s and create_day<=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, start_day,end_day])
@@ -1746,15 +1705,15 @@
                         elif task_type == TaskType.invite_user_help.value:
                             if task_count.complete_count + int(task_count.now_count/satisfy_num) > limit_num:
                                 cur_complete_count = limit_num - task_count.complete_count
                             else:
                                 cur_complete_count = int(task_count.now_count / satisfy_num)
                             reward_value = cur_complete_count * reward_value
                             cur_now_count = task_count.now_count - (cur_complete_count * satisfy_num)
-                            invite_help_model = InviteHelpModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction, context=self.context)
+                            invite_help_model = InviteHelpModel(db_transaction=db_transaction,context=self.context)
                             #获取邀请用户数
                             help_type = 1
                             help_object_id = ''
                             help_id_md5 = CryptoHelper.md5_encrypt_int(f"{app_id}_{act_id}_{module_id}_{help_type}_{help_object_id}")
                             invite_help_list = invite_help_model.get_list("id_md5=%s and user_id=%s and is_handle=0",limit=str(cur_complete_count * satisfy_num), params=[help_id_md5,user_id])
                             if not info_json:
                                 info_json = {}
@@ -1771,15 +1730,15 @@
                             if task_count.complete_count + int(task_count.now_count/satisfy_num) > limit_num:
                                 cur_complete_count = limit_num - task_count.complete_count
                             else:
                                 cur_complete_count = int(task_count.now_count / satisfy_num)
                             reward_value = cur_complete_count * reward_value
                             cur_now_count = task_count.now_count - (cur_complete_count * satisfy_num)
                             if task_type == TaskType.collect_goods.value:
-                                collect_log_model = CollectLogModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction,context=self.context)
+                                collect_log_model = CollectLogModel(db_transaction=db_transaction,context=self.context)
                                 if task_info_dict["complete_type"] == 1:
                                     collect_list = collect_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, now_day])
                                 elif task_info_dict["complete_type"] == 2:
                                     start_day = int(TimeHelper.get_first_day_of_the_week().strftime('%Y%m%d'))
                                     end_day = int(TimeHelper.get_last_day_of_the_week().strftime('%Y%m%d'))
                                     collect_list = collect_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day>=%s and create_day<=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, start_day,end_day])
                                 else:
@@ -1787,15 +1746,15 @@
                                 if not info_json:
                                     info_json = {}
                                     info_json["title"] = f"收藏{len(collect_list)}个"
                                     info_json["list"] = collect_list
                                 collect_goods_id_list = [str(i.goods_id) for i in collect_list]
                                 log_title = "被收藏商品ID：" + ",".join(collect_goods_id_list)
                             else:
-                                browse_log_model = BrowseLogModel(db_connect_key=self.db_connect_key, db_transaction=db_transaction, context=self.context)
+                                browse_log_model = BrowseLogModel(db_transaction=db_transaction,context=self.context)
                                 if task_info_dict["complete_type"] == 1:
                                     browse_list = browse_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, now_day])
                                 elif task_info_dict["complete_type"] == 2:
                                     start_day = int(TimeHelper.get_first_day_of_the_week().strftime('%Y%m%d'))
                                     end_day = int(TimeHelper.get_last_day_of_the_week().strftime('%Y%m%d'))
                                     browse_list = browse_log_model.get_list("act_id=%s and user_id=%s and is_handle=0 and create_day>=%s and create_day<=%s",limit=str(cur_complete_count * satisfy_num), params=[act_id,user_id, start_day,end_day])
                                 else:
@@ -1884,15 +1843,15 @@
                             #奖励类型为资产走资产系统
                             if task_reward_type == TaskRewardType.asset.value:
                                 only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_info_dict["task_type"],task_sub_type,task_count.complete_count)
                                 if module_id > 0:
                                     only_id = f"{module_id}_{only_id}"
                                 asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_info_dict["task_type"])
                                 reward_object_id = asset_type
-                                asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                                asset_base_model = AssetBaseModel(context=self.context)
                                 log_title = log_title if log_title else task_info_dict["task_name"]
                                 asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_info_dict["task_type"],task_info_dict["task_name"],log_title,only_id,handler_name,request_code,info_json=info_json)
                                 if asset_invoke_result_data.success == False:
                                     reward_value = 0
                             invoke_result_data.data["config_json"] = config_json
                             invoke_result_data.data["reward_value"] = reward_value
 
@@ -1949,15 +1908,15 @@
                     config_json = task_info_dict["config_json"]
                     reward_value = int(config_json["reward_value"]) if config_json.__contains__("reward_value") else 0
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     act_module_dict = invoke_result_data.data["act_module_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     limit_meaasge = ""
                     if task_info_dict["complete_type"] == 1:
                         limit_meaasge = "今日领取上限"
                         if task_count.modify_day != now_day:
@@ -1994,15 +1953,15 @@
                         reward_object_id = ""
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type,complete_count=task_count.complete_count)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],task_info_dict["task_name"],only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                         invoke_result_data.data["reward_value"] = reward_value
                         self.add_task_stat(task_type, app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                         self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=task_info_dict["task_name"],reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
                 else:
@@ -2052,15 +2011,15 @@
                     task_info_dict = task_invoke_result_data.data
                     config_json = task_info_dict["config_json"]
                     reward_value = int(config_json["reward_value"]) if config_json.__contains__("reward_value") else 0
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     act_module_dict = invoke_result_data.data["act_module_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     if task_info_dict["complete_type"] == 1 and task_count.modify_day == now_day:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = "error"
                         invoke_result_data.error_message = "今日已签到"
@@ -2090,15 +2049,15 @@
                         reward_object_id = ""
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type,complete_count=task_count.complete_count)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],"签到1天",only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                         invoke_result_data.data["reward_value"] = reward_value
                         self.add_task_stat(task_type,app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                         self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=log_title,reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
                 else:
@@ -2150,15 +2109,15 @@
                     task_info_dict = task_invoke_result_data.data
                     config_json = task_info_dict["config_json"]
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     day_list = config_json["day_list"] if config_json.__contains__("day_list") else {}
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     act_module_dict = invoke_result_data.data["act_module_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     if task_count.modify_day == now_day:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = "error"
                         invoke_result_data.error_message = "今日已签到"
@@ -2188,15 +2147,15 @@
                         reward_object_id = ""
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,2,task_type,complete_count=task_count.complete_count)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],f"签到{task_count.complete_count}天",only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                         invoke_result_data.data["reward_value"] = reward_value
                         self.add_task_stat(task_type,app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                         self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=f"签到{task_count.complete_count}天",reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
                 else:
@@ -2247,15 +2206,15 @@
                     task_info_dict = task_invoke_result_data.data
                     config_json = task_info_dict["config_json"]
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     day_list = config_json["day_list"] if config_json.__contains__("day_list") else {}
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     act_module_dict = invoke_result_data.data["act_module_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     if task_count.modify_day == now_day:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = "error"
                         invoke_result_data.error_message = "今日已签到"
@@ -2295,15 +2254,15 @@
                             reward_object_id = ""
                             if reward_value > 0:
                                 only_id = self.get_only_id(user_id,3,task_type,complete_count=task_count.complete_count)
                                 if module_id > 0:
                                     only_id = f"{module_id}_{only_id}"
                                 asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                                 reward_object_id = asset_type
-                                asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                                asset_base_model = AssetBaseModel(context=self.context)
                                 asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],f"签到{task_count.complete_count}天",only_id,handler_name,request_code,info_json=info_json)
                                 if asset_invoke_result_data.success == False:
                                     reward_value = 0
                             invoke_result_data.data["reward_value"] = reward_value
                             self.add_task_stat(task_type,app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                             self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=f"签到{task_count.complete_count}天",reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
                 else:
@@ -2356,15 +2315,15 @@
             if invoke_result_data.success == True:
                 act_info_dict = invoke_result_data.data["act_info_dict"]
                 act_module_dict = invoke_result_data.data["act_module_dict"]
                 user_info_dict = invoke_result_data.data["user_info_dict"]
 
                 user_base_model = UserBaseModel(context=self.context)
                 from_user_info_dict = user_base_model.get_user_info_dict(app_id,act_id,from_user_id)
-                invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                invite_log_model = InviteLogModel(context=self.context)
                 invite_log_dict = invite_log_model.get_dict("act_id=%s and invite_user_id=%s", params=[act_id, user_id])
                 if invite_log_dict:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
                     invoke_result_data.error_message = "此用户已经被邀请过"
                 elif not from_user_info_dict:
                     invoke_result_data.success = False
@@ -2373,15 +2332,15 @@
                 else:
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",from_user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if task_info_dict["complete_type"] == 1:
                             limit_meaasge = "今日邀请上限"
                             if task_count.modify_day != now_day:
@@ -2424,15 +2383,15 @@
                             task_count.task_type = task_type
                             task_count.task_sub_type = ""
                             task_count.now_count = task_count.now_count + 1
                             task_count.create_date = now_datetime
                             task_count.modify_date = now_datetime
                             task_count.modify_day = now_day
                             task_count_model.add_update_entity(task_count,"complete_count=%s,now_count=%s,modify_date=%s,modify_day=%s",params=[task_count.complete_count,task_count.now_count,task_count.modify_date,now_day])
-                            invite_log_model.delete_dependency_key(DependencyKey.invite_log_list(act_id,from_user_id), redis_config_dict=self.__get_redis_dict())
+                            invite_log_model.delete_dependency_key(DependencyKey.invite_log_list(act_id,from_user_id))
                     else:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = task_invoke_result_data.error_code
                         invoke_result_data.error_message = task_invoke_result_data.error_message
 
         except Exception as ex:
             if self.context:
@@ -2475,18 +2434,21 @@
                 invoke_result_data.error_code = "error"
                 invoke_result_data.error_message = "无效邀请"
                 return invoke_result_data
 
             invoke_result_data = self.business_process_executing(app_id,act_id,module_id,user_id,login_token,handler_name,False,check_user_nick,continue_request_expire,acquire_lock_name)
 
             if invoke_result_data.success == True:
+                act_info_dict = invoke_result_data.data["act_info_dict"]
+                act_module_dict = invoke_result_data.data["act_module_dict"]
                 user_info_dict = invoke_result_data.data["user_info_dict"]
+
                 user_base_model = UserBaseModel(context=self.context)
                 from_user_info_dict = user_base_model.get_user_info_dict(app_id, act_id, from_user_id)
-                invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, context=self.context, sub_table="member")
+                invite_log_model = InviteLogModel(context=self.context,sub_table="member")
                 invite_log_dict = invite_log_model.get_dict("act_id=%s and invite_user_id=%s", params=[act_id, user_id])
                 if invite_log_dict:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
                     invoke_result_data.error_message = "此用户已经被邀请过"
                 elif not from_user_info_dict:
                     invoke_result_data.success = False
@@ -2495,15 +2457,15 @@
                 else:
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",from_user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if task_info_dict["complete_type"] == 1:
                             limit_meaasge = "今日邀请上限"
                             if task_count.modify_day != now_day:
@@ -2547,15 +2509,15 @@
                             task_count.task_type = task_type
                             task_count.task_sub_type = ""
                             task_count.now_count = task_count.now_count + 1
                             task_count.create_date = now_datetime
                             task_count.modify_date = now_datetime
                             task_count.modify_day = now_day
                             task_count_model.add_update_entity(task_count,"complete_count=%s,now_count=%s,modify_date=%s,modify_day=%s",params=[task_count.complete_count,task_count.now_count,task_count.modify_date,now_day])
-                            invite_log_model.delete_dependency_key(DependencyKey.invite_log_member_list(act_id,from_user_id), redis_config_dict=self.__get_redis_dict())
+                            invite_log_model.delete_dependency_key(DependencyKey.invite_log_member_list(act_id,from_user_id))
                     else:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = task_invoke_result_data.error_code
                         invoke_result_data.error_message = task_invoke_result_data.error_message
 
         except Exception as ex:
             if self.context:
@@ -2590,15 +2552,15 @@
         task_type = TaskType.collect_goods.value
         now_day = TimeExHelper.get_now_day_int()
         now_datetime = TimeHelper.get_now_format_time()
         try:
             invoke_result_data = self.business_process_executing(app_id,act_id,module_id,user_id,login_token,handler_name,False,check_user_nick,continue_request_expire,acquire_lock_name)
             if invoke_result_data.success == True:
                 user_info_dict = invoke_result_data.data["user_info_dict"]
-                collect_log_model = CollectLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                collect_log_model = CollectLogModel(context=self.context)
                 where = "act_id=%s and user_id=%s and goods_id=%s"
                 params = [act_id, user_id, goods_id]
                 collect_log_dict = collect_log_model.get_dict(where, params=params)
                 if collect_log_dict:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
                     invoke_result_data.error_message = "此商品已经收藏过"
@@ -2606,15 +2568,15 @@
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                         goods_ids_list = list(set(str(config_json["goods_ids"]).split(','))) if config_json.__contains__("goods_ids") else []
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if str(goods_id) not in goods_ids_list:
                             invoke_result_data.success = False
                             invoke_result_data.error_code = "error"
@@ -2635,26 +2597,26 @@
                         collect_count = int(task_count.complete_count * satisfy_num) + task_count.now_count
                         is_collect_limit = True if collect_count >= (limit_num * satisfy_num) else False
                         if is_collect_limit == True:
                             invoke_result_data.success = False
                             invoke_result_data.error_code = "error"
                             invoke_result_data.error_message = limit_meaasge
                         else:
-                            collect_log_model = CollectLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                            collect_log_model = CollectLogModel(context=self.context)
                             collect_log = CollectLog()
                             collect_log.app_id = app_id
                             collect_log.act_id = act_id
                             collect_log.user_id = user_id
                             collect_log.open_id = user_info_dict["open_id"]
                             collect_log.goods_id = goods_id
                             collect_log.is_handle = 0
                             collect_log.create_date = now_datetime
                             collect_log.create_day = now_day
                             collect_log_model.add_entity(collect_log)
-                            collect_log_model.delete_dependency_key(DependencyKey.collect_log(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                            collect_log_model.delete_dependency_key(DependencyKey.collect_log(act_id,user_id))
 
                             task_count.id_md5 = task_count_id_md5
                             task_count.app_id = app_id
                             task_count.act_id = act_id
                             task_count.module_id = module_id
                             task_count.user_id = user_id
                             task_count.open_id = user_info_dict["open_id"]
@@ -2706,15 +2668,15 @@
         task_type = TaskType.browse_goods.value
         now_day = TimeExHelper.get_now_day_int()
         now_datetime = TimeHelper.get_now_format_time()
         try:
             invoke_result_data = self.business_process_executing(app_id,act_id,module_id,user_id,login_token,handler_name,False,check_user_nick,continue_request_expire,acquire_lock_name)
             if invoke_result_data.success == True:
                 user_info_dict = invoke_result_data.data["user_info_dict"]
-                browse_log_model = BrowseLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                browse_log_model = BrowseLogModel(context=self.context)
                 where = "act_id=%s and user_id=%s and goods_id=%s"
                 params = [act_id, user_id, goods_id]
                 if daily_repeat_browse == True:
                     where+=" and create_day=%s"
                     params.append(TimeExHelper.get_now_day_int())
                 browse_log_dict = browse_log_model.get_dict(where, params=params)
                 if browse_log_dict:
@@ -2725,15 +2687,15 @@
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
                         goods_ids_list = list(set(str(config_json["goods_ids"]).split(','))) if config_json.__contains__("goods_ids") else []
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if str(goods_id) not in goods_ids_list:
                             invoke_result_data.success = False
                             invoke_result_data.error_code = "error"
@@ -2754,26 +2716,26 @@
                         browse_count = int(task_count.complete_count * satisfy_num) + task_count.now_count
                         is_browse_limit = True if browse_count >= (limit_num * satisfy_num) else False
                         if is_browse_limit == True:
                             invoke_result_data.success = False
                             invoke_result_data.error_code = "error"
                             invoke_result_data.error_message = limit_meaasge
                         else:
-                            browse_log_model = BrowseLogModel(db_connect_key=self.db_connect_key, context=self.context)
+                            browse_log_model = BrowseLogModel(context=self.context)
                             browse_log = BrowseLog()
                             browse_log.app_id = app_id
                             browse_log.act_id = act_id
                             browse_log.user_id = user_id
                             browse_log.open_id = user_info_dict["open_id"]
                             browse_log.goods_id = goods_id
                             browse_log.is_handle = 0
                             browse_log.create_date = now_datetime
                             browse_log.create_day = now_day
                             browse_log_model.add_entity(browse_log)
-                            browse_log_model.delete_dependency_key(DependencyKey.browse_log(act_id,user_id), redis_config_dict=self.__get_redis_dict())
+                            browse_log_model.delete_dependency_key(DependencyKey.browse_log(act_id,user_id))
 
                             task_count.id_md5 = task_count_id_md5
                             task_count.app_id = app_id
                             task_count.act_id = act_id
                             task_count.module_id = module_id
                             task_count.user_id = user_id
                             task_count.open_id = user_info_dict["open_id"]
@@ -2837,15 +2799,15 @@
                 user_info_dict = invoke_result_data.data["user_info_dict"]
 
                 if user_info_dict["is_favor_before"] == 0:
                     if is_stat == True:
                         #新增关注用户数
                         stat_base_model.add_stat(app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], "AddFollowUserCount",1)
                 is_limit = False
-                task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                 task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_type,"",user_id)
                 task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                 task_count = task_count if task_count else TaskCount()
                 if module_id:
                     is_limit = True if task_count.complete_count >= 1 else False
                 else:
                     is_limit = True if task_count.complete_count >= 1 or user_info_dict["is_favor"] == 1 else False
@@ -2886,15 +2848,15 @@
                             reward_value = 0
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],task_info_dict["task_name"],only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                     invoke_result_data.data["reward_value"] = reward_value
                     self.add_task_stat(task_type, app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                     self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=task_info_dict["task_name"],reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
 
@@ -2943,15 +2905,15 @@
                 user_info_dict = invoke_result_data.data["user_info_dict"]
 
                 if user_info_dict["is_member_before"] == 0:
                     #新增入会用户数
                     if is_stat == True:
                         stat_base_model.add_stat(app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], "AddMemberUserCount",1)
                 is_limit = False
-                task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                 task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_type,"",user_id)
                 task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                 task_count = task_count if task_count else TaskCount()
                 if module_id:
                     is_limit = True if task_count.complete_count >= 1 else False
                 else:
                     is_limit = True if task_count.complete_count >= 1 or user_info_dict["is_member"] == 1 else False
@@ -2992,15 +2954,15 @@
                             reward_value = 0
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],task_info_dict["task_name"],only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                     invoke_result_data.data["reward_value"] = reward_value
                     self.add_task_stat(task_type, app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                     self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=task_info_dict["task_name"],reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
         except Exception as ex:
@@ -3046,15 +3008,15 @@
                 task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                 if task_invoke_result_data.success == True:
                     task_info_dict = task_invoke_result_data.data
                     sub_config_json = [sub_config_json for sub_config_json in task_info_dict["config_json"] if task_sub_type == sub_config_json["id"]]
                     if sub_config_json:
                         limit_num = int(sub_config_json["limit_num"]) if sub_config_json.__contains__("limit_num") else 1
                         satisfy_num = int(sub_config_json["satisfy_num"]) if sub_config_json.__contains__("satisfy_num") else 1
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],task_sub_type,user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if task_info_dict["complete_type"] == 1:
                             limit_meaasge = "今日浏览上限"
                             if task_count.modify_day != now_day:
@@ -3135,15 +3097,15 @@
             if invoke_result_data.success == True:
                 task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                 if task_invoke_result_data.success == True:
                     task_info_dict = task_invoke_result_data.data
                     config_json = task_info_dict["config_json"]
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     limit_meaasge = ""
                     if task_info_dict["complete_type"] == 1:
                         limit_meaasge = "今日领取上限"
                         if task_count.modify_day != now_day:
@@ -3225,15 +3187,15 @@
 
             invoke_result_data = self.business_process_executing(app_id,act_id,module_id,user_id,login_token,handler_name,check_new_user,check_user_nick,continue_request_expire,acquire_lock_name,check_act_info_release=check_act_info_release,check_act_module_release=check_act_module_release)
             if invoke_result_data.success == True:
                 user_info_dict = invoke_result_data.data["user_info_dict"]
 
                 user_base_model = UserBaseModel(context=self.context)
                 from_user_info_dict = user_base_model.get_user_info_dict(app_id,act_id,from_user_id)
-                invite_help_model = InviteHelpModel(db_connect_key=self.db_connect_key, context=self.context)
+                invite_help_model = InviteHelpModel(context=self.context)
                 help_type = 1
                 help_object_id = ''
                 help_id_md5 = CryptoHelper.md5_encrypt_int(f"{app_id}_{act_id}_{module_id}_{help_type}_{help_object_id}")
                 invite_help_dict = invite_help_model.get_dict("id_md5=%s and user_id=%s and invited_user_id=%s", params=[help_id_md5, from_user_id, user_id])
                 if invite_help_dict:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
@@ -3245,15 +3207,15 @@
                 else:
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",from_user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if task_info_dict["complete_type"] == 1:
                             limit_meaasge = "今日邀请上限"
                             if task_count.modify_day != now_day:
@@ -3300,15 +3262,15 @@
                             task_count.task_type = task_type
                             task_count.task_sub_type = ""
                             task_count.now_count = task_count.now_count + 1
                             task_count.create_date = now_datetime
                             task_count.modify_date = now_datetime
                             task_count.modify_day = now_day
                             task_count_model.add_update_entity(task_count,"complete_count=%s,now_count=%s,modify_date=%s,modify_day=%s",params=[task_count.complete_count,task_count.now_count,task_count.modify_date,now_day])
-                            invite_help_model.delete_dependency_key(DependencyKey.invite_user_help_list(help_id_md5,from_user_id), redis_config_dict=self.__get_redis_dict())
+                            invite_help_model.delete_dependency_key(DependencyKey.invite_user_help_list(help_id_md5,from_user_id))
                     else:
                         invoke_result_data.success = False
                         invoke_result_data.error_code = task_invoke_result_data.error_code
                         invoke_result_data.error_message = task_invoke_result_data.error_message
 
         except Exception as ex:
             if self.context:
@@ -3358,15 +3320,15 @@
                     config_json = task_info_dict["config_json"]
                     reward_value = int(config_json["reward_value"]) if config_json.__contains__("reward_value") else 0
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     cur_secret_code = config_json["secret_code"] if config_json.__contains__("secret_code") else ''
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     limit_meaasge = ""
 
                     if task_info_dict["complete_type"] == 1:
                         limit_meaasge = "今日领取上限"
@@ -3407,15 +3369,15 @@
                         reward_object_id = ""
                         if reward_value > 0:
                             only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type,complete_count=task_count.complete_count)
                             if module_id > 0:
                                 only_id = f"{module_id}_{only_id}"
                             asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                             reward_object_id = asset_type
-                            asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                            asset_base_model = AssetBaseModel(context=self.context)
                             asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],task_info_dict["task_name"],only_id,handler_name,request_code,info_json=info_json)
                             if asset_invoke_result_data.success == False:
                                 reward_value = 0
                         invoke_result_data.data["reward_value"] = reward_value
                         self.add_task_stat(task_type, app_id, act_id, module_id, user_info_dict["user_id"], user_info_dict["open_id"], reward_value, is_stat)
                         self.add_task_log(task_type=task_type, task_sub_type='', app_id=app_id, act_id=act_id, module_id=module_id, user_id=user_info_dict["user_id"], open_id=user_info_dict["open_id"], user_nick=user_info_dict["user_nick"],task_name=task_info_dict["task_name"],log_title=task_info_dict["task_name"],reward_type=1, reward_object_id=reward_object_id, reward_name="", reward_num=reward_value, handler_name=handler_name, request_code=request_code, info_json=info_json)
 
@@ -3475,15 +3437,15 @@
                     config_json = task_info_dict["config_json"]
                     reward_value = int(config_json["reward_value"]) if config_json.__contains__("reward_value") else 0
                     asset_object_id = config_json["asset_object_id"] if config_json.__contains__("asset_object_id") else ""
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     need_crm_point = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 0
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     limit_meaasge = ""
                     top_base_model = TopBaseModel(context=self.context)
 
                     if task_info_dict["complete_type"] == 1:
@@ -3539,15 +3501,15 @@
                                 crm_point_invoke_result_data = top_base_model.change_crm_point(user_info_dict["open_id"], mix_nick, 1, 1, need_crm_point, access_token, app_key, app_secret, 0, "", True)
                                 if crm_point_invoke_result_data.success == True:
                                     only_id = self.get_only_id(user_id,task_info_dict["complete_type"],task_type,complete_count=task_count.complete_count)
                                     if module_id > 0:
                                         only_id = f"{module_id}_{only_id}"
                                     asset_type = self.get_task_asset_type(act_info_dict["task_asset_type_json"],task_type)
                                     reward_object_id = asset_type
-                                    asset_base_model = AssetBaseModel(context=self.context, logging_error=self.logging_error, logging_info=self.logging_info, db_connect_key=self.db_asset_connect_key, redis_config_dict=self.__get_redis_asset_dict())
+                                    asset_base_model = AssetBaseModel(context=self.context)
                                     asset_invoke_result_data = asset_base_model.update_user_asset(app_id,act_id,module_id,user_id,user_info_dict["open_id"],user_info_dict["user_nick"],asset_type,reward_value,asset_object_id,2,task_type,task_info_dict["task_name"],task_info_dict["task_name"],only_id,handler_name,request_code,info_json=info_json)
                                     if asset_invoke_result_data.success == False:
                                         reward_value = 0
                                 else:
                                     reward_value = 0
 
                             invoke_result_data.data["reward_value"] = reward_value
@@ -3650,32 +3612,32 @@
                 return invoke_result_data
 
             invoke_result_data = self.business_process_executing(app_id,act_id,module_id,user_id,login_token,handler_name,check_new_user,check_user_nick,continue_request_expire,acquire_lock_name)
             if invoke_result_data.success == True:
                 user_info_dict = invoke_result_data.data["user_info_dict"]
                 user_base_model = UserBaseModel(context=self.context)
                 from_user_info_dict = user_base_model.get_user_info_dict(app_id,act_id,from_user_id)
-                invite_log_model = InviteLogModel(db_connect_key=self.db_connect_key, sub_table=invite_sub_table, context=self.context)
-                invite_log_dict = invite_log_model.get_dict("act_id=%s and invite_user_id=%s", params=[act_id, user_id])
-                if invite_log_dict:
+                invite_log_model = InviteLogModel(context=self.context,sub_table=invite_sub_table)
+                is_invite = invite_log_model.get_total("act_id=%s and invite_user_id=%s", params=[act_id, user_id])
+                if is_invite > 0:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
                     invoke_result_data.error_message = "此用户已经被邀请过"
                 elif not from_user_info_dict:
                     invoke_result_data.success = False
                     invoke_result_data.error_code = "error"
                     invoke_result_data.error_message = "邀请人不存在"
                 else:
                     task_invoke_result_data = self.check_task_info(act_id,module_id,task_type)
                     if task_invoke_result_data.success == True:
                         task_info_dict = task_invoke_result_data.data
                         config_json = task_info_dict["config_json"]
                         limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                         satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-                        task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                        task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                         task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",from_user_id)
                         task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                         task_count = TaskCount() if not task_count else task_count
                         limit_meaasge = ""
                         if task_info_dict["complete_type"] == TaskCompleteType.day.value:
                             limit_meaasge = "今日邀请上限"
                             if task_count.modify_day != now_day:
@@ -3779,15 +3741,15 @@
                     config_json = task_info_dict["config_json"]
                     act_info_dict = invoke_result_data.data["act_info_dict"]
                     act_module_dict = invoke_result_data.data["act_module_dict"]
                     user_info_dict = invoke_result_data.data["user_info_dict"]
                     goods_ids_list = list(set(str(config_json["goods_ids"]).split(','))) if config_json.__contains__("goods_ids") else []
                     limit_num = int(config_json["limit_num"]) if config_json.__contains__("limit_num") else 1
                     satisfy_num = int(config_json["satisfy_num"]) if config_json.__contains__("satisfy_num") else 1
-                    task_count_model = TaskCountModel(db_connect_key=self.db_connect_key, sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}), context=self.context)
+                    task_count_model = TaskCountModel(sub_table=self.get_business_sub_table("task_count_tb",{"app_id":app_id}),context=self.context)
                     task_count_id_md5 = self._get_task_count_id_md5(act_id,module_id,task_info_dict["task_type"],"",user_id)
                     task_count = task_count_model.get_entity("id_md5=%s",params=[task_count_id_md5])
                     task_count = TaskCount() if not task_count else task_count
                     limit_meaasge = ""
                     if task_info_dict["complete_type"] == 1:
                         limit_meaasge = "今日购买上限"
                         if task_count.modify_day != now_day:
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/theme_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/theme_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/top_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/top_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/models/user_base_model.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/models/user_base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,16 +418,15 @@
         :param act_id：活动标识
         :param user_id：用户标识
         :param reason：拉黑理由
         :return:
         :last_editors: HuangJianYi
         """
         invoke_result_data = InvokeResultData()
-        db_config_dict = config.get_value("db_user") if config.get_value("db_user") else config.get_value("db_cloudapp")
-        db_transaction = DbTransaction(db_config_dict=db_config_dict, context=self.context)
+        db_transaction = DbTransaction(db_config_dict=config.get_value("db_cloudapp"),context=self.context)
         user_info_model = UserInfoModel(sub_table=self.get_business_sub_table("user_info_tb",{"app_id":app_id}), db_transaction=db_transaction, context=self.context)
         user_black_model = UserBlackModel(db_transaction=db_transaction, context=self.context)
 
         user_info_dict = self.get_user_info_dict(app_id, act_id, user_id)
         if not user_info_dict:
             invoke_result_data.success = False
             invoke_result_data.error_code = "error"
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame/route.py` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame/route.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/PKG-INFO` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-cloudapp-frame
-Version: 1.0.96
+Version: 1.0.97
 Summary: seven cloudapp frame
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_frame.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
```

### Comparing `seven_cloudapp_frame-1.0.96/seven_cloudapp_frame.egg-info/SOURCES.txt` & `seven_cloudapp_frame-1.0.97/seven_cloudapp_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

