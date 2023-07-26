# Comparing `tmp/bcedit_madeby_train-0.0.9.tar.gz` & `tmp/bcedit_madeby_train-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcedit_madeby_train-0.0.9.tar", last modified: Wed Jul 26 07:04:51 2023, max compression
+gzip compressed data, was "bcedit_madeby_train-1.0.tar", last modified: Wed Jul 26 07:17:23 2023, max compression
```

## Comparing `bcedit_madeby_train-0.0.9.tar` & `bcedit_madeby_train-1.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.387432 bcedit_madeby_train-0.0.9/
--rw-rw-rw-   0        0        0      479 2023-07-26 07:04:51.386299 bcedit_madeby_train-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.089738 bcedit_madeby_train-0.0.9/bcedit_madeby_train/
--rw-rw-rw-   0        0        0      281 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/__init__.py
--rw-rw-rw-   0        0        0     8301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.137065 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/
--rw-rw-rw-   0        0        0       67 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.168305 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-07-16 12:52:21.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16533 2023-07-16 12:52:20.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.217681 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     3145 2023-07-18 11:00:13.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1555 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1661 2023-07-18 11:44:06.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     6658 2023-07-18 12:33:12.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.240404 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-07-16 12:52:19.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2794 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3393 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-07-16 12:52:18.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.309163 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-07-16 12:52:16.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6307 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4408 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2323 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3031 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8458 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1043 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-07-16 12:52:17.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.361096 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/
--rw-rw-rw-   0        0        0      276 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2187 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3825 2023-07-17 08:14:21.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     6773 2023-07-18 11:00:49.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0      914 2023-07-18 11:01:47.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-07-16 12:52:15.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.383149 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2578 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/load.py
--rw-rw-rw-   0        0        0      644 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1862 2023-07-16 12:52:14.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12118 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/game_data_getter.py
--rw-rw-rw-   0        0        0    22858 2023-07-18 12:48:49.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/helper.py
--rw-rw-rw-   0        0        0     7075 2023-07-16 12:52:10.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/item.py
--rw-rw-rw-   0        0        0     3505 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/managed_item.py
--rw-rw-rw-   0        0        0    66964 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/serialise_save.py
--rw-rw-rw-   0        0        0    24970 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/server_handler.py
--rw-rw-rw-   0        0        0     3247 2023-07-26 07:04:33.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/tracker.py
--rw-rw-rw-   0        0        0     3496 2023-07-18 12:57:46.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/updater.py
--rw-rw-rw-   0        0        0     8297 2023-07-16 12:52:11.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-26 07:04:51.137065 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/
--rw-rw-rw-   0        0        0      479 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3853 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 07:04:50.000000 bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 07:04:51.388427 bcedit_madeby_train-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-26 07:04:39.000000 bcedit_madeby_train-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.233534 bcedit_madeby_train-1.0/
+-rw-rw-rw-   0        0        0      477 2023-07-26 07:17:23.232535 bcedit_madeby_train-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:22.938885 bcedit_madeby_train-1.0/bcedit_madeby_train/
+-rw-rw-rw-   0        0        0      281 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/__init__.py
+-rw-rw-rw-   0        0        0     8301 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-07-16 12:52:10.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/adb_handler.py
+-rw-rw-rw-   0        0        0     9550 2023-07-26 07:16:55.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-07-16 12:52:10.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:22.989015 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/
+-rw-rw-rw-   0        0        0       67 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.009192 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-07-16 12:52:21.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16533 2023-07-16 12:52:20.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.071121 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     3145 2023-07-18 11:00:13.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1555 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1661 2023-07-18 11:44:06.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     6658 2023-07-18 12:33:12.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.091279 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-07-16 12:52:19.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-07-16 12:52:18.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2794 2023-07-16 12:52:18.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3393 2023-07-16 12:52:18.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-07-16 12:52:18.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.156491 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-07-16 12:52:16.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-07-16 12:52:16.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-07-16 12:52:16.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-07-16 12:52:16.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-07-16 12:52:16.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6307 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4408 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2323 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3031 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8458 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1043 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-07-16 12:52:17.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.206174 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2187 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3825 2023-07-17 08:14:21.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     6773 2023-07-18 11:00:49.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0      914 2023-07-18 11:01:47.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-07-16 12:52:15.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:23.229144 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2578 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      644 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1862 2023-07-16 12:52:14.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12118 2023-07-16 12:52:10.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-07-16 12:52:10.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/game_data_getter.py
+-rw-rw-rw-   0        0        0    22858 2023-07-18 12:48:49.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-07-16 12:52:10.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/item.py
+-rw-rw-rw-   0        0        0     3505 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/managed_item.py
+-rw-rw-rw-   0        0        0    66964 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/serialise_save.py
+-rw-rw-rw-   0        0        0    24970 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/server_handler.py
+-rw-rw-rw-   0        0        0     3247 2023-07-26 07:04:33.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/tracker.py
+-rw-rw-rw-   0        0        0     3496 2023-07-18 12:57:46.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-07-16 12:52:11.000000 bcedit_madeby_train-1.0/bcedit_madeby_train/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-26 07:17:22.985818 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/
+-rw-rw-rw-   0        0        0      477 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3853 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 07:17:22.000000 bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 07:17:23.234527 bcedit_madeby_train-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-07-26 07:17:10.000000 bcedit_madeby_train-1.0/setup.py
```

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/__main__.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/__main__.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/adb_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/config_manager.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/config_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,40 +6,21 @@
 
 import yaml
 
 from . import helper, user_input_handler, locale_handler
 
 
 def get_config_value_category(category: str, key: str) -> Any:
-    """
-    Returns the value of the given key in the config file.
-    """
-    config = get_config_file()
-    category_data: Optional[dict[str, Any]] = config.get(category)
-    if category_data is None:
-        create_config_file()
-        return get_config_value_category(category, key)
-    key_data = category_data.get(key)
-    if key_data is None:
-        create_config_file()
-        return get_config_value_category(category, key)
-    return key_data
+
+    return
 
 
 def get_config_file() -> dict[str, Any]:
-    """
-    Get the config file
 
-    Returns:
-        dict: Config file
-    """
-    config_file = get_config_path()
-    with open(config_file, "r", encoding="utf-8") as file:
-        config = yaml.safe_load(file)
-    return config
+    return
 
 
 def get_config_path() -> str:
     """
     Get the path to the config file
 
     Returns:
@@ -67,67 +48,40 @@
     """
     helper.write_file_string(helper.get_file("config_path.txt"), path)
     if not os.path.exists(path):
         create_config_file()
 
 
 def get_config_value(setting: str) -> Any:
-    """
-    Get a config setting
-
-    Args:
-        setting (str): Setting to get
-
-    Returns:
-        Any: Value of setting
-    """
-    config = get_config_file()
-    setting_data = config.get(setting)
-    if setting_data is None:
-        create_config_file()
-        return get_config_value(setting)
-    return setting_data
+   return
 
 
 def set_config_setting_category(category: str, key: str, value: Any) -> None:
     """
     Set a config setting
 
     Args:
         setting (str): Setting to set
         value (Any): Value to set setting to
     """
-    config = get_config_file()
-    config[category][key] = value
-    with open(get_config_path(), "w", encoding="utf-8") as file:
-        yaml.safe_dump(config, file)
-
+    print(1)
 
 def set_config_setting(setting: str, value: Any) -> None:
     """
     Set a config setting
 
     Args:
         setting (str): Setting to set
         value (Any): Value to set setting to
     """
-    config = get_config_file()
-    config[setting] = value
-    with open(get_config_path(), "w", encoding="utf-8") as file:
-        yaml.safe_dump(config, file)
-
-
+    print(1)
 def create_config_file(config_path: Optional[str] = None) -> None:
     """
     Create the config file if it doesn't exist
     """
-    if config_path is None:
-        config_file = get_config_path()
-    else:
-        config_file = config_path
     file_data = "# Configuration file for BCSFE\n"
     file_data += "# This file is automatically created when the program is run for the first time\n"
     file_data += "# You can edit this file to change the settings\n"
     file_data += "# You can also edit the settings in the program\n#\n"
     file_data += "# The following settings are available:\n#\n"
     file_data += """DEFAULT_COUNTRY_CODE: "" # The default game version when downloading / pulling / loading save data. E.g en, jp, kr, tw. Empty means the game version is not specified and will be asked for when needed.
 DEFAULT_SAVE_FILE_PATH: "SAVE_DATA" # The default file path for your save data when saving changes / downloading save data / pulling etc
@@ -152,15 +106,14 @@
   ALWAYS_EXPORT_JSON: False # Always export your save data as json when saving changes.
 
 SERVER:
   UPLOAD_METADATA: True # Upload metadata (catfood, rare ticket, platinum ticket, and legend ticket changes) to the ponos servers when uploading and saving your save data - prevents bans.
   WIPE_TRACKED_ITEMS_ON_START: True # Wipe all tracked items stored when the editor starts up - if disabled, it allows you to upload metadata changes after you exit and re-enter the editor.
 """
 
-    helper.write_file_string(config_file, file_data)
 
 
 def get_app_data_folder() -> str:
     """
     Get the path to the app data folder cross platform
 
     Returns:
@@ -182,108 +135,49 @@
     return path
 
 
 def edit_default_gv(_: Any) -> None:
     """
     Edit the default game version
     """
-    locale_manager = locale_handler.LocalManager.from_config()
-    default_gv = get_config_value("DEFAULT_COUNTRY_CODE")
-    default_gv = user_input_handler.colored_input(
-        locale_manager.search_key("enter_default_gv") % default_gv
-    )
-    set_config_setting("DEFAULT_COUNTRY_CODE", default_gv)
-
+    print(1)
 
 def edit_default_save_file_path(_: Any) -> None:
     """
     Edit the default save file path
     """
     locale_manager = locale_handler.LocalManager.from_config()
-    default_save_file_path = get_config_value("DEFAULT_SAVE_FILE_PATH")
     default_save_file_path = helper.select_dir(
         locale_manager.search_key("select_default_save_path"),
         default_save_file_path,
     )
     set_config_setting(
         "DEFAULT_SAVE_FILE_PATH", os.path.join(default_save_file_path, "SAVE_DATA")
     )
 
 
 def edit_fixed_save_path(_: Any) -> None:
     """
     Edit the fixed save path
     """
-    locale_manager = locale_handler.LocalManager.from_config()
-
-    fixed_save_path = get_config_value("FIXED_SAVE_PATH")
-    if fixed_save_path:
-        fixed_save_path = locale_manager.search_key("enabled")
-    else:
-        fixed_save_path = locale_manager.search_key("disabled")
-    fixed_save_path = user_input_handler.colored_input(
-        locale_manager.search_key("flag_set_config")
-        % (locale_manager.search_key("fixed_save_path"), fixed_save_path)
-    )
-    if fixed_save_path == "1":
-        fixed_save_path = True
-    else:
-        fixed_save_path = False
-    set_config_setting("FIXED_SAVE_PATH", fixed_save_path)
+    print(1)
 
 
 def edit_locale(_: Any) -> None:
     """
     Edit the locale
     """
-    all_locales = locale_handler.LocalManager.get_locales()
-    locale_manager = locale_handler.LocalManager.from_config()
-    locale = get_config_value("LOCALE")
-    locale = all_locales[
-        user_input_handler.select_single(
-            all_locales,
-            locale_manager.search_key("select_l"),
-            locale_manager.search_key("select_locale") % locale,
-        )
-        - 1
-    ]
-    set_config_setting("LOCALE", locale)
+    print(1)
 
 
 def edit_editor_settings(_: Any) -> None:
     """
     Edit the editor settings
     """
-    locale_manager = locale_handler.LocalManager.from_config()
-    options = [
-        "DISABLE_MAXES",
-        "SHOW_BAN_WARNING",
-        "SHOW_CATEGORIES",
-        "SHOW_FEATURE_SELECT_EXPLANATION",
-        "ONLY_GET_EN_DATA",
-    ]
-    option_values = [get_config_value_category("EDITOR", option) for option in options]
-    ids = user_input_handler.select_not_inc(options, "select", option_values)
-    for option_id in ids:
-        option_name = options[option_id]
-        current_value = option_values[option_id]
-        if current_value:
-            current_value = locale_manager.search_key("enabled")
-        else:
-            current_value = locale_manager.search_key("disabled")
-        enable = (
-            user_input_handler.colored_input(
-                locale_manager.search_key("flag_set_config")
-                % (option_name, current_value)
-            )
-            == "1"
-        )
-        set_config_setting_category("EDITOR", option_name, enable)
-
-
+    print(1)
 def edit_start_up_settings(_: Any) -> None:
     """
     Edit the start up settings
 
     Raises:
         Exception: If the option type is not int or bool
     """
@@ -291,24 +185,20 @@
     options = {
         "CHECK_FOR_UPDATES": bool,
         "UPDATE_TO_BETAS": bool,
         "HIDE_START_TEXT": bool,
         "DEFAULT_START_OPTION": int,
         "CREATE_BACKUP": bool,
     }
-    option_values = [
-        get_config_value_category("START_UP", option) for option in options
-    ]
     ids = user_input_handler.select_not_inc(
-        list(options.keys()), locale_manager.search_key("select_l"), option_values
+        list(options.keys()), locale_manager.search_key("select_l"), 2
     )
     for option_id in ids:
         option_name = list(options.keys())[option_id]
         option_type = options[option_name]
-        current_value = option_values[option_id]
         if option_type == bool:
             if current_value:
                 current_value = locale_manager.search_key("enabled")
             else:
                 current_value = locale_manager.search_key("disabled")
             enable = (
                 user_input_handler.colored_input(
@@ -333,17 +223,15 @@
     Edit the save changes settings
     """
     locale_manager = locale_handler.LocalManager.from_config()
     options = [
         "SAVE_CHANGES_ON_EDIT",
         "ALWAYS_EXPORT_JSON",
     ]
-    option_values = [
-        get_config_value_category("SAVE_CHANGES", option) for option in options
-    ]
+    option_values = 2
     ids = user_input_handler.select_not_inc(
         options, locale_manager.search_key("select_l"), option_values
     )
     for option_id in ids:
         option_name = options[option_id]
         current_value = option_values[option_id]
         if current_value:
@@ -365,15 +253,15 @@
     Edit the server settings
     """
     locale_manager = locale_handler.LocalManager.from_config()
     options = [
         "UPLOAD_METADATA",
         "WIPE_TRACKED_ITEMS_ON_START",
     ]
-    option_values = [get_config_value_category("SERVER", option) for option in options]
+    option_values = 2
     ids = user_input_handler.select_not_inc(
         options, locale_manager.search_key("select_l"), option_values
     )
     for option_id in ids:
         option_name = options[option_id]
         current_value = option_values[option_id]
         if current_value:
@@ -391,13 +279,12 @@
 
 
 def edit_config_path(_: Any) -> None:
     """
     Edit the config path
     """
     locale_manager = locale_handler.LocalManager.from_config()
-    config_path = os.path.dirname(get_config_path())
     config_path = helper.select_dir(
         locale_manager.search_key("select_config_path"), config_path
     )
     config_path = os.path.join(config_path, "config.yaml")
     set_config_path(config_path)
```

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/csv_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/basic_items.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/catfruit.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/catseyes.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/ototo_base_mats.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/talent_orbs.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/basic/talent_orbs_new.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/cat_helper.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/cat_id_selector.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/chara_drop.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/clear_cat_guide.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/evolve_cats.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/get_remove_cats.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/talents.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/upgrade_blue.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/cats/upgrade_cats.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/helpers.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/aku.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/behemoth_culling.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/clear_tutorial.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/enigma_stages.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/event_stages.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/gauntlet.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/itf_timed_scores.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/legend_quest.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/main_story.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/outbreaks.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/story_level_id_selector.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/towers.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/treasures.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/uncanny.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/levels/unlock_aku_realm.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/cat_shrine.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/create_new_account.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/fix_elsewhere.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/fix_time_issues.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/get_gold_pass.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/meow_medals.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/missions.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/play_time.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/scheme_item.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/trade_progress.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/other/unlock_enemy_guide.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/convert.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/load.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/other.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/save.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/edits/save_management/server_upload.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/feature_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/game_data_getter.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/helper.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/helper.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/item.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/locale_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/locale_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/managed_item.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/parse_save.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/patcher.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/patcher.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/root_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/serialise_save.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/server_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/server_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/tracker.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/tracker.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/updater.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/updater.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train/user_input_handler.py` & `bcedit_madeby_train-1.0/bcedit_madeby_train/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/bcedit_madeby_train.egg-info/SOURCES.txt` & `bcedit_madeby_train-1.0/bcedit_madeby_train.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcedit_madeby_train-0.0.9/setup.py` & `bcedit_madeby_train-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bcedit_madeby_train',
-    version='0.0.9',
+    version='1.0',
     description='This is a project developed by Serem for development purposes',
     author='serem',
     author_email='gangh9230@gmail.com',
     url='https://github.com/hayul0629/wdex',
     install_requires=[
         "colored==1.4.4",
         "tk",
```

