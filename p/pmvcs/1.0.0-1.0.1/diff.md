# Comparing `tmp/pmvcs-1.0.0.tar.gz` & `tmp/pmvcs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmvcs-1.0.0.tar", last modified: Wed Jul 26 01:12:48 2023, max compression
+gzip compressed data, was "pmvcs-1.0.1.tar", last modified: Wed Jul 26 15:09:07 2023, max compression
```

## Comparing `pmvcs-1.0.0.tar` & `pmvcs-1.0.1.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.824262 pmvcs-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-07-10 09:52:19.000000 pmvcs-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      881 2023-07-26 00:17:43.000000 pmvcs-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4356 2023-07-26 01:12:48.820258 pmvcs-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4032 2023-07-26 01:11:33.000000 pmvcs-1.0.0/README.ES.md
--rw-rw-rw-   0        0        0     3636 2023-07-26 01:06:10.000000 pmvcs-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.744463 pmvcs-1.0.0/pmvcs/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/__init__.py
--rw-rw-rw-   0        0        0      134 2023-07-10 10:34:58.000000 pmvcs-1.0.0/pmvcs/__main__.py
--rw-rw-rw-   0        0        0      129 2023-07-26 01:12:15.000000 pmvcs-1.0.0/pmvcs/__version__.py
--rw-rw-rw-   0        0        0     1595 2023-07-26 00:50:16.000000 pmvcs-1.0.0/pmvcs/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.752245 pmvcs-1.0.0/pmvcs/core/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.752245 pmvcs-1.0.0/pmvcs/core/controllers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/controllers/__init__.py
--rw-rw-rw-   0        0        0     3292 2023-07-24 03:47:22.000000 pmvcs-1.0.0/pmvcs/core/controllers/base_controller.py
--rw-rw-rw-   0        0        0     3271 2023-07-24 03:36:42.000000 pmvcs-1.0.0/pmvcs/core/controllers/menus.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.756248 pmvcs-1.0.0/pmvcs/core/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/decorators/__init__.py
--rw-rw-rw-   0        0        0      886 2023-07-23 22:57:39.000000 pmvcs-1.0.0/pmvcs/core/decorators/decorators_views.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.760307 pmvcs-1.0.0/pmvcs/core/helpers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/helpers/__init__.py
--rw-rw-rw-   0        0        0     1107 2023-07-24 03:29:48.000000 pmvcs-1.0.0/pmvcs/core/helpers/base_helper.py
--rw-rw-rw-   0        0        0     1440 2023-07-24 03:16:46.000000 pmvcs-1.0.0/pmvcs/core/helpers/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.764310 pmvcs-1.0.0/pmvcs/core/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/interfaces/__init__.py
--rw-rw-rw-   0        0        0      730 2023-07-24 02:56:34.000000 pmvcs-1.0.0/pmvcs/core/interfaces/base_controller.py
--rw-rw-rw-   0        0        0      197 2023-07-13 14:26:55.000000 pmvcs-1.0.0/pmvcs/core/interfaces/base_helper.py
--rw-rw-rw-   0        0        0     1746 2023-07-24 03:21:41.000000 pmvcs-1.0.0/pmvcs/core/interfaces/base_model.py
--rw-rw-rw-   0        0        0     1764 2023-07-24 03:04:12.000000 pmvcs-1.0.0/pmvcs/core/interfaces/base_view.py
--rw-rw-rw-   0        0        0      941 2023-07-24 02:59:42.000000 pmvcs-1.0.0/pmvcs/core/interfaces/menus.py
--rw-rw-rw-   0        0        0     2025 2023-07-24 03:05:25.000000 pmvcs-1.0.0/pmvcs/core/interfaces/router.py
--rw-rw-rw-   0        0        0      933 2023-07-24 00:28:53.000000 pmvcs-1.0.0/pmvcs/core/interfaces/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.772388 pmvcs-1.0.0/pmvcs/core/models/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/models/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:04.000000 pmvcs-1.0.0/pmvcs/core/models/about.py
--rw-rw-rw-   0        0        0     1977 2023-07-24 03:18:08.000000 pmvcs-1.0.0/pmvcs/core/models/base_model.py
--rw-rw-rw-   0        0        0      688 2023-07-12 06:21:03.000000 pmvcs-1.0.0/pmvcs/core/models/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.772388 pmvcs-1.0.0/pmvcs/core/models/entities/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/models/entities/__init__.py
--rw-rw-rw-   0        0        0     2312 2023-07-24 03:44:22.000000 pmvcs-1.0.0/pmvcs/core/models/language.py
--rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:41.000000 pmvcs-1.0.0/pmvcs/core/models/menus.py
--rw-rw-rw-   0        0        0     3239 2023-07-24 02:38:28.000000 pmvcs-1.0.0/pmvcs/core/models/parser.py
--rw-rw-rw-   0        0        0     5082 2023-07-24 05:01:16.000000 pmvcs-1.0.0/pmvcs/core/router.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.784437 pmvcs-1.0.0/pmvcs/core/setup/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.784437 pmvcs-1.0.0/pmvcs/core/setup/languages/
--rw-rw-rw-   0        0        0     2113 2023-07-23 19:31:08.000000 pmvcs-1.0.0/pmvcs/core/setup/languages/en.setup.ini
--rw-rw-rw-   0        0        0     2409 2023-07-23 21:29:37.000000 pmvcs-1.0.0/pmvcs/core/setup/languages/es.setup.ini
--rw-rw-rw-   0        0        0     3251 2023-07-24 03:46:11.000000 pmvcs-1.0.0/pmvcs/core/setup/setup.py
--rw-rw-rw-   0        0        0     3419 2023-07-24 02:35:12.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_config_file.py
--rw-rw-rw-   0        0        0      718 2023-07-23 23:48:39.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_defaults.py
--rw-rw-rw-   0        0        0     1035 2023-07-23 23:59:48.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_example.py
--rw-rw-rw-   0        0        0     1541 2023-07-23 22:57:42.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_extras.py
--rw-rw-rw-   0        0        0     4361 2023-07-24 04:48:12.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_files.py
--rw-rw-rw-   0        0        0     4878 2023-07-24 03:46:58.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_install.py
--rw-rw-rw-   0        0        0     3128 2023-07-24 04:06:23.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_menus.py
--rw-rw-rw-   0        0        0     3734 2023-07-24 05:13:48.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_multiple.py
--rw-rw-rw-   0        0        0      957 2023-07-23 22:57:43.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_parser.py
--rw-rw-rw-   0        0        0     1952 2023-07-23 23:56:31.000000 pmvcs-1.0.0/pmvcs/core/setup/setup_unique.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.787944 pmvcs-1.0.0/pmvcs/core/views/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/core/views/__init__.py
--rw-rw-rw-   0        0        0     2813 2023-07-24 03:04:20.000000 pmvcs-1.0.0/pmvcs/core/views/base_view.py
--rw-rw-rw-   0        0        0     5226 2023-07-24 04:56:15.000000 pmvcs-1.0.0/pmvcs/core/views/sample.py
--rw-rw-rw-   0        0        0      803 2023-07-24 05:10:48.000000 pmvcs-1.0.0/pmvcs/pmvcs.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.787944 pmvcs-1.0.0/pmvcs/setup/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/__init__.py
--rw-rw-rw-   0        0        0      169 2023-07-12 07:38:03.000000 pmvcs-1.0.0/pmvcs/setup/app.py
--rw-rw-rw-   0        0        0      683 2023-07-13 21:01:35.000000 pmvcs-1.0.0/pmvcs/setup/config.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.792437 pmvcs-1.0.0/pmvcs/setup/defaults/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.792437 pmvcs-1.0.0/pmvcs/setup/defaults/controllers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/controllers/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-23 22:57:44.000000 pmvcs-1.0.0/pmvcs/setup/defaults/controllers/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.792437 pmvcs-1.0.0/pmvcs/setup/defaults/decorators/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.796440 pmvcs-1.0.0/pmvcs/setup/defaults/helpers/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.797947 pmvcs-1.0.0/pmvcs/setup/defaults/interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/interfaces/__init__.py
--rw-rw-rw-   0        0        0      266 2023-07-23 23:45:10.000000 pmvcs-1.0.0/pmvcs/setup/defaults/interfaces/base_controller.py
--rw-rw-rw-   0        0        0      161 2023-07-12 21:12:21.000000 pmvcs-1.0.0/pmvcs/setup/defaults/interfaces/base_model.py
--rw-rw-rw-   0        0        0      142 2023-07-12 21:10:40.000000 pmvcs-1.0.0/pmvcs/setup/defaults/interfaces/base_view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.804461 pmvcs-1.0.0/pmvcs/setup/defaults/languages/
--rw-rw-rw-   0        0        0      547 2023-07-13 20:50:52.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/en.about.ini
--rw-rw-rw-   0        0        0      427 2023-07-13 20:59:38.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/en.ini
--rw-rw-rw-   0        0        0        7 2023-07-23 17:22:52.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/en.menus.ini
--rw-rw-rw-   0        0        0      590 2023-07-13 20:50:43.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/es.about.ini
--rw-rw-rw-   0        0        0      462 2023-07-13 20:59:47.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/es.ini
--rw-rw-rw-   0        0        0        7 2023-07-23 17:22:57.000000 pmvcs-1.0.0/pmvcs/setup/defaults/languages/es.menus.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.804461 pmvcs-1.0.0/pmvcs/setup/defaults/models/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/models/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-12 21:12:40.000000 pmvcs-1.0.0/pmvcs/setup/defaults/models/base_model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.807969 pmvcs-1.0.0/pmvcs/setup/defaults/models/entities/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.807969 pmvcs-1.0.0/pmvcs/setup/defaults/views/
--rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.0/pmvcs/setup/defaults/views/__init__.py
--rw-rw-rw-   0        0        0      499 2023-07-12 21:13:12.000000 pmvcs-1.0.0/pmvcs/setup/defaults/views/base_view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.732284 pmvcs-1.0.0/pmvcs/setup/example/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.807969 pmvcs-1.0.0/pmvcs/setup/example/controllers/
--rw-rw-rw-   0        0        0     1462 2023-07-23 22:57:46.000000 pmvcs-1.0.0/pmvcs/setup/example/controllers/base_controller.py
--rw-rw-rw-   0        0        0     1212 2023-07-23 22:57:46.000000 pmvcs-1.0.0/pmvcs/setup/example/controllers/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.816195 pmvcs-1.0.0/pmvcs/setup/example/languages/
--rw-rw-rw-   0        0        0      622 2023-07-13 20:19:29.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/en.ini
--rw-rw-rw-   0        0        0      142 2023-07-10 11:18:47.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/en.menus.ini
--rw-rw-rw-   0        0        0     1280 2023-07-13 19:46:27.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/en.sample.ini
--rw-rw-rw-   0        0        0      664 2023-07-13 20:19:41.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/es.ini
--rw-rw-rw-   0        0        0      142 2023-07-10 11:18:26.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/es.menus.ini
--rw-rw-rw-   0        0        0     1408 2023-07-13 19:46:48.000000 pmvcs-1.0.0/pmvcs/setup/example/languages/es.sample.ini
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.816195 pmvcs-1.0.0/pmvcs/setup/example/models/
--rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.0/pmvcs/setup/example/models/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.816195 pmvcs-1.0.0/pmvcs/setup/example/views/
--rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.0/pmvcs/setup/example/views/example_one.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.732284 pmvcs-1.0.0/pmvcs/setup/module_unique/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.818203 pmvcs-1.0.0/pmvcs/setup/module_unique/controllers/
--rw-rw-rw-   0        0        0      852 2023-07-23 22:57:46.000000 pmvcs-1.0.0/pmvcs/setup/module_unique/controllers/unique.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.732284 pmvcs-1.0.0/pmvcs/setup/modules_base/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.820258 pmvcs-1.0.0/pmvcs/setup/modules_base/controllers/
--rw-rw-rw-   0        0        0      958 2023-07-23 22:57:46.000000 pmvcs-1.0.0/pmvcs/setup/modules_base/controllers/controller.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.820258 pmvcs-1.0.0/pmvcs/setup/modules_base/models/
--rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.0/pmvcs/setup/modules_base/models/model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.820258 pmvcs-1.0.0/pmvcs/setup/modules_base/views/
--rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.0/pmvcs/setup/modules_base/views/view.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.820258 pmvcs-1.0.0/pmvcs/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 22:50:30.000000 pmvcs-1.0.0/pmvcs/tests/__init__.py
--rw-rw-rw-   0        0        0      736 2023-07-24 00:03:55.000000 pmvcs-1.0.0/pmvcs/tests/test_default.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:12:48.747970 pmvcs-1.0.0/pmvcs.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-07-26 01:12:48.000000 pmvcs-1.0.0/pmvcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3306 2023-07-26 01:12:48.000000 pmvcs-1.0.0/pmvcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:12:48.000000 pmvcs-1.0.0/pmvcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-26 01:12:48.000000 pmvcs-1.0.0/pmvcs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 01:12:48.000000 pmvcs-1.0.0/pmvcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1525 2023-07-26 01:12:19.000000 pmvcs-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-25 21:31:09.000000 pmvcs-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 01:12:48.824262 pmvcs-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/
+-rw-rw-rw-   0        0        0      589 2023-07-26 15:00:48.000000 pmvcs-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35823 2023-07-10 09:52:19.000000 pmvcs-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      894 2023-07-26 15:02:59.000000 pmvcs-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7460 2023-07-26 15:09:07.860775 pmvcs-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7424 2023-07-26 14:57:22.000000 pmvcs-1.0.1/README.ES.md
+-rw-rw-rw-   0        0        0     6740 2023-07-26 14:57:46.000000 pmvcs-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/__init__.py
+-rw-rw-rw-   0        0        0      134 2023-07-10 10:34:58.000000 pmvcs-1.0.1/pmvcs/__main__.py
+-rw-rw-rw-   0        0        0      129 2023-07-26 15:01:51.000000 pmvcs-1.0.1/pmvcs/__version__.py
+-rw-rw-rw-   0        0        0     1595 2023-07-26 00:50:16.000000 pmvcs-1.0.1/pmvcs/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/core/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs/core/controllers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/controllers/__init__.py
+-rw-rw-rw-   0        0        0     3292 2023-07-24 03:47:22.000000 pmvcs-1.0.1/pmvcs/core/controllers/base_controller.py
+-rw-rw-rw-   0        0        0     3271 2023-07-24 03:36:42.000000 pmvcs-1.0.1/pmvcs/core/controllers/menus.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.800813 pmvcs-1.0.1/pmvcs/core/decorators/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/decorators/__init__.py
+-rw-rw-rw-   0        0        0      920 2023-07-26 14:00:32.000000 pmvcs-1.0.1/pmvcs/core/decorators/decorators_views.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.800813 pmvcs-1.0.1/pmvcs/core/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1107 2023-07-24 03:29:48.000000 pmvcs-1.0.1/pmvcs/core/helpers/base_helper.py
+-rw-rw-rw-   0        0        0     1440 2023-07-24 03:16:46.000000 pmvcs-1.0.1/pmvcs/core/helpers/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      730 2023-07-24 02:56:34.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_controller.py
+-rw-rw-rw-   0        0        0      197 2023-07-13 14:26:55.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_helper.py
+-rw-rw-rw-   0        0        0     1746 2023-07-24 03:21:41.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_model.py
+-rw-rw-rw-   0        0        0     1764 2023-07-24 03:04:12.000000 pmvcs-1.0.1/pmvcs/core/interfaces/base_view.py
+-rw-rw-rw-   0        0        0      941 2023-07-24 02:59:42.000000 pmvcs-1.0.1/pmvcs/core/interfaces/menus.py
+-rw-rw-rw-   0        0        0     2025 2023-07-24 03:05:25.000000 pmvcs-1.0.1/pmvcs/core/interfaces/router.py
+-rw-rw-rw-   0        0        0      933 2023-07-24 00:28:53.000000 pmvcs-1.0.1/pmvcs/core/interfaces/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/models/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/models/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:04.000000 pmvcs-1.0.1/pmvcs/core/models/about.py
+-rw-rw-rw-   0        0        0     1977 2023-07-24 03:18:08.000000 pmvcs-1.0.1/pmvcs/core/models/base_model.py
+-rw-rw-rw-   0        0        0      688 2023-07-12 06:21:03.000000 pmvcs-1.0.1/pmvcs/core/models/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.810935 pmvcs-1.0.1/pmvcs/core/models/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/models/entities/__init__.py
+-rw-rw-rw-   0        0        0     2312 2023-07-24 03:44:22.000000 pmvcs-1.0.1/pmvcs/core/models/language.py
+-rw-rw-rw-   0        0        0     1291 2023-07-23 23:08:41.000000 pmvcs-1.0.1/pmvcs/core/models/menus.py
+-rw-rw-rw-   0        0        0     3239 2023-07-24 02:38:28.000000 pmvcs-1.0.1/pmvcs/core/models/parser.py
+-rw-rw-rw-   0        0        0     5082 2023-07-24 05:01:16.000000 pmvcs-1.0.1/pmvcs/core/router.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.820867 pmvcs-1.0.1/pmvcs/core/setup/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.820867 pmvcs-1.0.1/pmvcs/core/setup/languages/
+-rw-rw-rw-   0        0        0     2113 2023-07-23 19:31:08.000000 pmvcs-1.0.1/pmvcs/core/setup/languages/en.setup.ini
+-rw-rw-rw-   0        0        0     2409 2023-07-23 21:29:37.000000 pmvcs-1.0.1/pmvcs/core/setup/languages/es.setup.ini
+-rw-rw-rw-   0        0        0     3251 2023-07-24 03:46:11.000000 pmvcs-1.0.1/pmvcs/core/setup/setup.py
+-rw-rw-rw-   0        0        0     3419 2023-07-24 02:35:12.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_config_file.py
+-rw-rw-rw-   0        0        0      718 2023-07-23 23:48:39.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_defaults.py
+-rw-rw-rw-   0        0        0     1035 2023-07-23 23:59:48.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_example.py
+-rw-rw-rw-   0        0        0     1541 2023-07-23 22:57:42.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_extras.py
+-rw-rw-rw-   0        0        0     4361 2023-07-24 04:48:12.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_files.py
+-rw-rw-rw-   0        0        0     4878 2023-07-24 03:46:58.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_install.py
+-rw-rw-rw-   0        0        0     3128 2023-07-24 04:06:23.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_menus.py
+-rw-rw-rw-   0        0        0     3734 2023-07-24 05:13:48.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_multiple.py
+-rw-rw-rw-   0        0        0      957 2023-07-23 22:57:43.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_parser.py
+-rw-rw-rw-   0        0        0     1952 2023-07-23 23:56:31.000000 pmvcs-1.0.1/pmvcs/core/setup/setup_unique.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/core/views/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/core/views/__init__.py
+-rw-rw-rw-   0        0        0     2813 2023-07-24 03:04:20.000000 pmvcs-1.0.1/pmvcs/core/views/base_view.py
+-rw-rw-rw-   0        0        0     5226 2023-07-24 04:56:15.000000 pmvcs-1.0.1/pmvcs/core/views/sample.py
+-rw-rw-rw-   0        0        0      803 2023-07-24 05:10:48.000000 pmvcs-1.0.1/pmvcs/pmvcs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-07-12 07:38:03.000000 pmvcs-1.0.1/pmvcs/setup/app.py
+-rw-rw-rw-   0        0        0      683 2023-07-13 21:01:35.000000 pmvcs-1.0.1/pmvcs/setup/config.ini
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-23 22:57:44.000000 pmvcs-1.0.1/pmvcs/setup/defaults/controllers/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/decorators/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.830580 pmvcs-1.0.1/pmvcs/setup/defaults/helpers/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-07-23 23:45:10.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_controller.py
+-rw-rw-rw-   0        0        0      161 2023-07-12 21:12:21.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_model.py
+-rw-rw-rw-   0        0        0      142 2023-07-12 21:10:40.000000 pmvcs-1.0.1/pmvcs/setup/defaults/interfaces/base_view.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/languages/
+-rw-rw-rw-   0        0        0      547 2023-07-13 20:50:52.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.about.ini
+-rw-rw-rw-   0        0        0      427 2023-07-13 20:59:38.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.ini
+-rw-rw-rw-   0        0        0        7 2023-07-23 17:22:52.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.menus.ini
+-rw-rw-rw-   0        0        0      590 2023-07-13 20:50:43.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.about.ini
+-rw-rw-rw-   0        0        0      467 2023-07-26 14:23:27.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.ini
+-rw-rw-rw-   0        0        0        7 2023-07-23 17:22:57.000000 pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.menus.ini
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/models/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-12 21:12:40.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/base_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.840946 pmvcs-1.0.1/pmvcs/setup/defaults/models/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/defaults/views/
+-rw-rw-rw-   0        0        0        0 2023-06-12 08:58:48.000000 pmvcs-1.0.1/pmvcs/setup/defaults/views/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-07-12 21:13:12.000000 pmvcs-1.0.1/pmvcs/setup/defaults/views/base_view.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/example/
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/controllers/
+-rw-rw-rw-   0        0        0     1462 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/example/controllers/base_controller.py
+-rw-rw-rw-   0        0        0     1212 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/example/controllers/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/languages/
+-rw-rw-rw-   0        0        0      622 2023-07-13 20:19:29.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.ini
+-rw-rw-rw-   0        0        0      142 2023-07-10 11:18:47.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.menus.ini
+-rw-rw-rw-   0        0        0     1280 2023-07-13 19:46:27.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/en.sample.ini
+-rw-rw-rw-   0        0        0      669 2023-07-26 14:21:30.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.ini
+-rw-rw-rw-   0        0        0      142 2023-07-10 11:18:26.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.menus.ini
+-rw-rw-rw-   0        0        0     1408 2023-07-13 19:46:48.000000 pmvcs-1.0.1/pmvcs/setup/example/languages/es.sample.ini
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.851024 pmvcs-1.0.1/pmvcs/setup/example/models/
+-rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.1/pmvcs/setup/example/models/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/example/views/
+-rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.1/pmvcs/setup/example/views/example_one.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/module_unique/
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/
+-rw-rw-rw-   0        0        0      852 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/unique.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.770691 pmvcs-1.0.1/pmvcs/setup/modules_base/
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/
+-rw-rw-rw-   0        0        0      958 2023-07-23 22:57:46.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/controller.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/models/
+-rw-rw-rw-   0        0        0      176 2023-07-12 07:57:48.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/models/model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/setup/modules_base/views/
+-rw-rw-rw-   0        0        0      165 2023-07-12 07:57:34.000000 pmvcs-1.0.1/pmvcs/setup/modules_base/views/view.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.860775 pmvcs-1.0.1/pmvcs/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 22:50:30.000000 pmvcs-1.0.1/pmvcs/tests/__init__.py
+-rw-rw-rw-   0        0        0      736 2023-07-24 00:03:55.000000 pmvcs-1.0.1/pmvcs/tests/test_default.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:07.790839 pmvcs-1.0.1/pmvcs.egg-info/
+-rw-rw-rw-   0        0        0     7460 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3319 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 15:09:07.000000 pmvcs-1.0.1/pmvcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1525 2023-07-26 15:01:55.000000 pmvcs-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-25 21:31:09.000000 pmvcs-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:09:07.860775 pmvcs-1.0.1/setup.cfg
```

### Comparing `pmvcs-1.0.0/LICENSE` & `pmvcs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/MANIFEST.in` & `pmvcs-1.0.1/MANIFEST.in`

 * *Files 11% similar despite different names*

```diff
@@ -1 +1 @@
-include requirements.txt README.md README.ES.md LICENSE pmvcs/core/setup/languages/en.setup.ini pmvcs/core/setup/languages/es.setup.ini pmvcs/setup/config.ini  pmvcs/setup/defaults/languages/en.ini pmvcs/setup/defaults/languages/en.about.ini pmvcs/setup/defaults/languages/en.menus.ini pmvcs/setup/defaults/languages/es.ini pmvcs/setup/defaults/languages/es.about.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.menus.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.sample.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.menus.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.sample.ini
+include requirements.txt README.md README.ES.md CHANGELOG.md LICENSE pmvcs/core/setup/languages/en.setup.ini pmvcs/core/setup/languages/es.setup.ini pmvcs/setup/config.ini  pmvcs/setup/defaults/languages/en.ini pmvcs/setup/defaults/languages/en.about.ini pmvcs/setup/defaults/languages/en.menus.ini pmvcs/setup/defaults/languages/es.ini pmvcs/setup/defaults/languages/es.about.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.menus.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/en.sample.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.menus.ini pmvcs/setup/defaults/languages/es.menus.ini pmvcs/setup/example/languages/es.sample.ini
```

### Comparing `pmvcs-1.0.0/pmvcs/cli.py` & `pmvcs-1.0.1/pmvcs/cli.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/controllers/base_controller.py` & `pmvcs-1.0.1/pmvcs/core/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/controllers/menus.py` & `pmvcs-1.0.1/pmvcs/core/controllers/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/decorators/decorators_views.py` & `pmvcs-1.0.1/pmvcs/core/decorators/decorators_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     """
     Decorator for intro banner and exit banner
     Repeats lines before and after of each intro or exit message
     """
     def decorator_decorate_intro(func: str):
 
         @functools.wraps(func)
-        def wrapped_decorate_intro(self) -> list:
+        def wrapped_decorate_intro(self, *args, **kwargs) -> list:
             line = '-' * 49 + ' \n'
             message = ''
             counter_start = counter_end = 1
             while counter_start <= num_lines:
                 message += line
                 counter_start += 1
 
-            message += func(self)
+            message += func(self, *args, **kwargs)
 
             while counter_end <= num_lines:
                 message += line
                 counter_end += 1
 
             return message
         return wrapped_decorate_intro
```

### Comparing `pmvcs-1.0.0/pmvcs/core/helpers/base_helper.py` & `pmvcs-1.0.1/pmvcs/core/helpers/base_helper.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/helpers/filters.py` & `pmvcs-1.0.1/pmvcs/core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/base_controller.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/base_model.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/base_view.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/base_view.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/menus.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/router.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/router.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/interfaces/sample.py` & `pmvcs-1.0.1/pmvcs/core/interfaces/sample.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/about.py` & `pmvcs-1.0.1/pmvcs/core/models/about.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/base_model.py` & `pmvcs-1.0.1/pmvcs/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/configuration.py` & `pmvcs-1.0.1/pmvcs/core/models/configuration.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/language.py` & `pmvcs-1.0.1/pmvcs/core/models/language.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/menus.py` & `pmvcs-1.0.1/pmvcs/core/models/menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/models/parser.py` & `pmvcs-1.0.1/pmvcs/core/models/parser.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/router.py` & `pmvcs-1.0.1/pmvcs/core/router.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/languages/en.setup.ini` & `pmvcs-1.0.1/pmvcs/core/setup/languages/en.setup.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/languages/es.setup.ini` & `pmvcs-1.0.1/pmvcs/core/setup/languages/es.setup.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_config_file.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_config_file.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_defaults.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_defaults.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_example.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_example.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_extras.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_extras.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_files.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_files.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_install.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_install.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_menus.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_menus.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_multiple.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_multiple.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_parser.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_parser.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/setup/setup_unique.py` & `pmvcs-1.0.1/pmvcs/core/setup/setup_unique.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/views/base_view.py` & `pmvcs-1.0.1/pmvcs/core/views/base_view.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/core/views/sample.py` & `pmvcs-1.0.1/pmvcs/core/views/sample.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/pmvcs.py` & `pmvcs-1.0.1/pmvcs/pmvcs.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/config.ini` & `pmvcs-1.0.1/pmvcs/setup/config.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/defaults/controllers/base_controller.py` & `pmvcs-1.0.1/pmvcs/setup/defaults/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/defaults/languages/en.about.ini` & `pmvcs-1.0.1/pmvcs/setup/defaults/languages/en.about.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/defaults/languages/es.about.ini` & `pmvcs-1.0.1/pmvcs/setup/defaults/languages/es.about.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/defaults/models/base_model.py` & `pmvcs-1.0.1/pmvcs/setup/defaults/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/controllers/base_controller.py` & `pmvcs-1.0.1/pmvcs/setup/example/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/controllers/example_one.py` & `pmvcs-1.0.1/pmvcs/setup/example/controllers/example_one.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/languages/en.ini` & `pmvcs-1.0.1/pmvcs/setup/example/languages/en.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/languages/en.sample.ini` & `pmvcs-1.0.1/pmvcs/setup/example/languages/en.sample.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/languages/es.ini` & `pmvcs-1.0.1/pmvcs/setup/example/languages/es.ini`

 * *Files 5% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 LANG_SELECT_LANGUAGE = Idioma: {}Opción:
 LANG_INPUT_PRESS_A_KEY_START = Presiona ENTER para iniciar:
 LANG_INPUT_PRESS_A_KEY_CONTINUE = Presiona ENTER para continuar:
 LANG_INPUT_SELECT_OPTION = Selecciona una opción:
 LANG_QUIT_LEYEND = Salir del programa
 LANG_EXIT_PROGRAM = El programa finalizó
 ERROR_TYPE_NOT_FLOAT_OR_INTEGER = [>] ERROR: Error de tipo, {} no es entero o flotante
-ERROR_IMPORT_UNKNOWN_FORMAT = [>] ERROR: Unknown format "{}"
+ERROR_IMPORT_UNKNOWN_FORMAT = [>] ERROR: Formato desconocido "{}"
 LANG_EXAMPLE_STRING = Este es un string de ejemplo
 LANG_EXAMPLE_SPRINTF = Valor de String-Print-Format aquí: "{}"
 LANG_EXAMPLE_SPRINTF2 = Uno: "{}". Dos: "{}". Tres: "{}".
 dictionary = Diccionario
```

### Comparing `pmvcs-1.0.0/pmvcs/setup/example/languages/es.sample.ini` & `pmvcs-1.0.1/pmvcs/setup/example/languages/es.sample.ini`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/module_unique/controllers/unique.py` & `pmvcs-1.0.1/pmvcs/setup/module_unique/controllers/unique.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/setup/modules_base/controllers/controller.py` & `pmvcs-1.0.1/pmvcs/setup/modules_base/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs/tests/test_default.py` & `pmvcs-1.0.1/pmvcs/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `pmvcs-1.0.0/pmvcs.egg-info/SOURCES.txt` & `pmvcs-1.0.1/pmvcs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.ES.md
 README.md
 pyproject.toml
 requirements.txt
 pmvcs/__init__.py
```

### Comparing `pmvcs-1.0.0/pyproject.toml` & `pmvcs-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmvcs"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.md"
 authors = [
   { name="Gonzalo Mahserdjian", email="gsmx64@outlook.com" },
 ]
 description = "Python MVC Shell Framework Package is a tiny framework for shell projects in Python."
 requires-python = ">=3.7"
 license = {text = "GNU/GPL version 3"}
```

