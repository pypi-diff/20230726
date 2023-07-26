# Comparing `tmp/lazyinit-0.0.262.tar.gz` & `tmp/lazyinit-0.0.263.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.262.tar", last modified: Wed Jul 26 04:51:36 2023, max compression
+gzip compressed data, was "lazyinit-0.0.263.tar", last modified: Wed Jul 26 05:01:47 2023, max compression
```

## Comparing `lazyinit-0.0.262.tar` & `lazyinit-0.0.263.tar`

### file list

```diff
@@ -1,20 +1,328 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.858404 lazyinit-0.0.262/
--rw-r--r--   0 dengyifan   (501) staff       (20)       84 2023-07-26 04:36:39.000000 lazyinit-0.0.262/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:51:36.858185 lazyinit-0.0.262/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.262/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.856926 lazyinit-0.0.262/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.262/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.262/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8118 2023-07-26 04:51:31.000000 lazyinit-0.0.262/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.262/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.262/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4979 2023-07-26 04:50:29.000000 lazyinit-0.0.262/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.857885 lazyinit-0.0.262/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:51:36.858476 lazyinit-0.0.262/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-26 04:51:34.000000 lazyinit-0.0.262/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.502827 lazyinit-0.0.263/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.444707 lazyinit-0.0.263/.git/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/COMMIT_EDITMSG
+-rw-r--r--   0 dengyifan   (501) staff       (20)       98 2023-07-26 05:01:40.000000 lazyinit-0.0.263/.git/FETCH_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 03:36:41.000000 lazyinit-0.0.263/.git/ORIG_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.263/.git/config
+-rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/description
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.448170 lazyinit-0.0.263/.git/hooks/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/post-update.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/hooks/update.sample
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4305 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/index
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.448403 lazyinit-0.0.263/.git/info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/info/exclude
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.448562 lazyinit-0.0.263/.git/logs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1447 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/logs/HEAD
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.433733 lazyinit-0.0.263/.git/logs/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.448753 lazyinit-0.0.263/.git/logs/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1447 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/logs/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.433786 lazyinit-0.0.263/.git/logs/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.449208 lazyinit-0.0.263/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1884 2023-07-26 05:00:14.000000 lazyinit-0.0.263/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1430 2023-07-26 05:00:12.000000 lazyinit-0.0.263/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.441199 lazyinit-0.0.263/.git/objects/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.449598 lazyinit-0.0.263/.git/objects/00/
+-r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.450357 lazyinit-0.0.263/.git/objects/01/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.451401 lazyinit-0.0.263/.git/objects/04/
+-r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
+-r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.452470 lazyinit-0.0.263/.git/objects/05/
+-r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
+-r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.453659 lazyinit-0.0.263/.git/objects/0a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.455072 lazyinit-0.0.263/.git/objects/0e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
+-r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.455416 lazyinit-0.0.263/.git/objects/11/
+-r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.455973 lazyinit-0.0.263/.git/objects/1f/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.457235 lazyinit-0.0.263/.git/objects/22/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.263/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
+-r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.457584 lazyinit-0.0.263/.git/objects/24/
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.458021 lazyinit-0.0.263/.git/objects/28/
+-r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.458610 lazyinit-0.0.263/.git/objects/2a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.459042 lazyinit-0.0.263/.git/objects/2b/
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.459315 lazyinit-0.0.263/.git/objects/2d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.459860 lazyinit-0.0.263/.git/objects/2e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.460631 lazyinit-0.0.263/.git/objects/32/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
+-r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.460964 lazyinit-0.0.263/.git/objects/33/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.263/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.461527 lazyinit-0.0.263/.git/objects/38/
+-r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.462527 lazyinit-0.0.263/.git/objects/39/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.263/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.463748 lazyinit-0.0.263/.git/objects/3d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
+-r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.464215 lazyinit-0.0.263/.git/objects/40/
+-r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.263/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.464513 lazyinit-0.0.263/.git/objects/43/
+-r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.464806 lazyinit-0.0.263/.git/objects/4d/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.465069 lazyinit-0.0.263/.git/objects/52/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.263/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.465248 lazyinit-0.0.263/.git/objects/55/
+-r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.465428 lazyinit-0.0.263/.git/objects/56/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.465615 lazyinit-0.0.263/.git/objects/5a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.465900 lazyinit-0.0.263/.git/objects/5e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.466290 lazyinit-0.0.263/.git/objects/5f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
+-r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.468627 lazyinit-0.0.263/.git/objects/60/
+-r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.469458 lazyinit-0.0.263/.git/objects/63/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
+-r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.469741 lazyinit-0.0.263/.git/objects/64/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.469992 lazyinit-0.0.263/.git/objects/67/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.470235 lazyinit-0.0.263/.git/objects/69/
+-r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.470526 lazyinit-0.0.263/.git/objects/6a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.470778 lazyinit-0.0.263/.git/objects/6b/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.471317 lazyinit-0.0.263/.git/objects/6c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
+-r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.471539 lazyinit-0.0.263/.git/objects/6d/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.471832 lazyinit-0.0.263/.git/objects/6e/
+-r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.472234 lazyinit-0.0.263/.git/objects/6f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.472535 lazyinit-0.0.263/.git/objects/73/
+-r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.473327 lazyinit-0.0.263/.git/objects/74/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
+-r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.473600 lazyinit-0.0.263/.git/objects/7e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.473832 lazyinit-0.0.263/.git/objects/7f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.474032 lazyinit-0.0.263/.git/objects/80/
+-r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.474453 lazyinit-0.0.263/.git/objects/83/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.263/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
+-r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.474823 lazyinit-0.0.263/.git/objects/84/
+-r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.475069 lazyinit-0.0.263/.git/objects/88/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.475360 lazyinit-0.0.263/.git/objects/89/
+-r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.475710 lazyinit-0.0.263/.git/objects/8f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/8f/821694556aac2a278c288de223659193dd2489
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.475969 lazyinit-0.0.263/.git/objects/91/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.476498 lazyinit-0.0.263/.git/objects/96/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.476718 lazyinit-0.0.263/.git/objects/99/
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.477286 lazyinit-0.0.263/.git/objects/9c/
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.477643 lazyinit-0.0.263/.git/objects/9d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
+-r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.478351 lazyinit-0.0.263/.git/objects/a0/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
+-r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
+-r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.478803 lazyinit-0.0.263/.git/objects/a1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
+-r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.479076 lazyinit-0.0.263/.git/objects/a3/
+-r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.479468 lazyinit-0.0.263/.git/objects/a8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.479720 lazyinit-0.0.263/.git/objects/a9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.480971 lazyinit-0.0.263/.git/objects/aa/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
+-r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
+-r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.481264 lazyinit-0.0.263/.git/objects/ad/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.481838 lazyinit-0.0.263/.git/objects/ae/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
+-r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.482449 lazyinit-0.0.263/.git/objects/af/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.482973 lazyinit-0.0.263/.git/objects/b0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.483247 lazyinit-0.0.263/.git/objects/b1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.485684 lazyinit-0.0.263/.git/objects/b4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.486261 lazyinit-0.0.263/.git/objects/b6/
+-r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
+-r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.486496 lazyinit-0.0.263/.git/objects/b7/
+-r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.263/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.488609 lazyinit-0.0.263/.git/objects/bc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
+-r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.263/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
+-r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.488827 lazyinit-0.0.263/.git/objects/c1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.489035 lazyinit-0.0.263/.git/objects/c4/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.263/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.489526 lazyinit-0.0.263/.git/objects/c5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
+-r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.489719 lazyinit-0.0.263/.git/objects/c7/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.489917 lazyinit-0.0.263/.git/objects/c9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.490062 lazyinit-0.0.263/.git/objects/ca/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.490783 lazyinit-0.0.263/.git/objects/cc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
+-r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.491010 lazyinit-0.0.263/.git/objects/cd/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.491288 lazyinit-0.0.263/.git/objects/ce/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.491524 lazyinit-0.0.263/.git/objects/d9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.491819 lazyinit-0.0.263/.git/objects/da/
+-r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.492092 lazyinit-0.0.263/.git/objects/de/
+-r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.492328 lazyinit-0.0.263/.git/objects/df/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.492512 lazyinit-0.0.263/.git/objects/e4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.263/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.492769 lazyinit-0.0.263/.git/objects/e6/
+-r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.493177 lazyinit-0.0.263/.git/objects/e8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
+-r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.493679 lazyinit-0.0.263/.git/objects/eb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
+-r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.493863 lazyinit-0.0.263/.git/objects/ec/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.494124 lazyinit-0.0.263/.git/objects/ef/
+-r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.494613 lazyinit-0.0.263/.git/objects/f0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
+-r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.263/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.494886 lazyinit-0.0.263/.git/objects/f1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-26 04:07:28.000000 lazyinit-0.0.263/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.495066 lazyinit-0.0.263/.git/objects/f2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.495244 lazyinit-0.0.263/.git/objects/f5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.263/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.495423 lazyinit-0.0.263/.git/objects/f6/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.263/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.441428 lazyinit-0.0.263/.git/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.495629 lazyinit-0.0.263/.git/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 05:00:09.000000 lazyinit-0.0.263/.git/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.441485 lazyinit-0.0.263/.git/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.496004 lazyinit-0.0.263/.git/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 05:00:14.000000 lazyinit-0.0.263/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 05:00:12.000000 lazyinit-0.0.263/.git/refs/remotes/origin/master
+-rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.263/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 05:01:47.502521 lazyinit-0.0.263/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.263/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.496965 lazyinit-0.0.263/lazyinit/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.498482 lazyinit-0.0.263/lazyinit/ProjectTemplate/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.498609 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1569 2023-07-25 13:48:22.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/default_config.yaml
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.498757 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/exps/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.499049 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/exps/focusl/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/exps/focusl/baseline.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)    74072 2023-07-25 04:24:11.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/exps/focusl/exp_plan.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)      644 2023-07-23 08:07:15.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/configs/exps/overfit_test.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/minist.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/requirements.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.263/lazyinit/ProjectTemplate/start.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.263/lazyinit/__init__.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.499424 lazyinit-0.0.263/lazyinit/__pycache__/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8725 2023-07-26 04:15:42.000000 lazyinit-0.0.263/lazyinit/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.263/lazyinit/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.263/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8118 2023-07-26 04:51:31.000000 lazyinit-0.0.263/lazyinit/init.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.500486 lazyinit-0.0.263/lazyinit/ranger/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.263/lazyinit/ranger/.DS_Store
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.501412 lazyinit-0.0.263/lazyinit/ranger/colorschemes/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/default.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/jungle.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/snow.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/snow.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/colorschemes/zenburn.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/commands.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.502222 lazyinit-0.0.263/lazyinit/ranger/plugins/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/devicons.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/devicons.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/devicons_linemode.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/plugins/devicons_linemode.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/rc-sample.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/rc.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/rifle.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.263/lazyinit/ranger/scope.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.263/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.263/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4995 2023-07-26 04:54:51.000000 lazyinit-0.0.263/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 05:01:47.497787 lazyinit-0.0.263/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)     9583 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 05:01:47.000000 lazyinit-0.0.263/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.263/push.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 05:01:47.502899 lazyinit-0.0.263/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-26 05:01:44.000000 lazyinit-0.0.263/setup.py
```

### Comparing `lazyinit-0.0.262/lazyinit/bash_config.txt` & `lazyinit-0.0.263/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.262/lazyinit/init.py` & `lazyinit-0.0.263/lazyinit/init.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.262/lazyinit/redis.conf` & `lazyinit-0.0.263/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.262/lazyinit/run.py` & `lazyinit-0.0.263/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.262/lazyinit/utils.py` & `lazyinit-0.0.263/lazyinit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def echo(msg, color="green"):
     console.print(msg, style=color)
 
 def run_cmd(cmd_list):
     if not isinstance(cmd_list, list):
         cmd_list = [cmd_list]
     outputs = []
-    for cmd in track(cmd_list, description="命令执行中..."):
+    for cmd in track(cmd_list, description="命令执行中...", transient=True):
         echo(cmd, "blue")
         while True:
             exitcode, output = subprocess.getstatusoutput(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
                 echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
                 cmd = input()
```

### Comparing `lazyinit-0.0.262/setup.py` & `lazyinit-0.0.263/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.262',
+    version='0.0.263',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

