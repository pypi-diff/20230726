# Comparing `tmp/todd_ai-0.3.0.tar.gz` & `tmp/todd_ai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todd_ai-0.3.0.tar", last modified: Tue Jan 24 16:28:01 2023, max compression
+gzip compressed data, was "todd_ai-0.4.0.tar", last modified: Wed Jul 26 04:28:57 2023, max compression
```

## Comparing `todd_ai-0.3.0.tar` & `todd_ai-0.4.0.tar`

### file list

```diff
@@ -1,87 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.194449 todd_ai-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-01-24 16:27:50.000000 todd_ai-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-01-24 16:28:01.194449 todd_ai-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-01-24 16:27:50.000000 todd_ai-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.174448 todd_ai-0.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-01-24 16:27:50.000000 todd_ai-0.3.0/bin/git_rev_parse_head
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-01-24 16:27:50.000000 todd_ai-0.3.0/bin/git_status_porcelain
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-01-24 16:27:50.000000 todd_ai-0.3.0/bin/odpsrun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1690 2023-01-24 16:27:50.000000 todd_ai-0.3.0/bin/odpsrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-24 16:27:50.000000 todd_ai-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 16:28:01.194449 todd_ai-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-24 16:27:50.000000 todd_ai-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.174448 todd_ai-0.3.0/todd/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.178448 todd_ai-0.3.0/todd/adapts/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/decouple.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/detach.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/label_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/list_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/adapts/roi_align.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.182448 todd_ai-0.3.0/todd/base/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/base/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.182448 todd_ai-0.3.0/todd/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/datasets/lmdb_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/datasets/pth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/datasets/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.182448 todd_ai-0.3.0/todd/distillers/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/distillers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/distillers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/distillers/single_student.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.186448 todd_ai-0.3.0/todd/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/hooks/duplicated.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/hooks/multi_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/hooks/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.186448 todd_ai-0.3.0/todd/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/mimic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/losses/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.190449 todd_ai-0.3.0/todd/reproduction/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/reproduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/reproduction/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/reproduction/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.190449 todd_ai-0.3.0/todd/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/scripts/convert_ckpts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/scripts/convert_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/scripts/merge_lmdbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.190449 todd_ai-0.3.0/todd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/utils/generic_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/utils/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.190449 todd_ai-0.3.0/todd/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/visuals/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/visuals/cv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-01-24 16:27:50.000000 todd_ai-0.3.0/todd/visuals/pptx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 16:28:01.194449 todd_ai-0.3.0/todd_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-24 16:28:01.000000 todd_ai-0.3.0/todd_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.535079 todd_ai-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-26 04:28:48.000000 todd_ai-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-26 04:28:57.535079 todd_ai-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-26 04:28:48.000000 todd_ai-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/git_rev_parse_head
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/git_status_porcelain
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/odpsrun
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1690 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/odpsrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-26 04:28:48.000000 todd_ai-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 04:28:57.535079 todd_ai-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 04:28:48.000000 todd_ai-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/todd/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/todd/adapts/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/decouple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/detach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/label_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/list_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/roi_align.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/lmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/pth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/distillers/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/single_student.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/duplicated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/multi_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/mimic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/reproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/runners/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/composed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/runners/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/convert_ckpts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/convert_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/merge_lmdbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/generic_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/metas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/sgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/cv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/pptx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.535079 todd_ai-0.4.0/todd_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/top_level.txt
```

### Comparing `todd_ai-0.3.0/LICENSE` & `todd_ai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/PKG-INFO` & `todd_ai-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todd_ai
-Version: 0.3.0
+Version: 0.4.0
 Summary: Toolkit for Object Detection Distillation
 Author-email: Luting Wang <wangluting@buaa.edu.cn>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `todd_ai-0.3.0/README.md` & `todd_ai-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/bin/git_rev_parse_head` & `todd_ai-0.4.0/bin/git_rev_parse_head`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/bin/odpsrun` & `todd_ai-0.4.0/bin/odpsrun`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/bin/odpsrun.py` & `todd_ai-0.4.0/bin/odpsrun.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/pyproject.toml` & `todd_ai-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'todd_ai'
-version = '0.3.0'
+version = '0.4.0'
 description = 'Toolkit for Object Detection Distillation'
 readme = 'README.md'
 requires-python = '>=3.10'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
@@ -40,27 +40,30 @@
 [project.optional-dependencies]
 dev = [
     'commitizen',
     'ipdb',
     'ipykernel',
     'jupyter',
     'matplotlib',
+    'mypy',
+    'pandas-stubs',
     'pre-commit',
     'tensorboard',
     'torch-tb-profiler',
+    'types-Pillow',
 ]
 doc = [
-    'mmcv',
+    'mmcv<2.0',
     'python-docs-theme',
     'sphinx',
     'sphinx_rtd_theme',
 ]
 test = [
     'coverage',
-    'mmcv',
+    'mmcv<2.0',
     'pytest',
 ]
 
 [project.scripts]
 configs_diff = 'todd.base.configs:diff_cli'
 
 [tool.setuptools.packages.find]
@@ -73,14 +76,17 @@
 coalesce_brackets = true
 dedent_closing_brackets = true
 split_arguments_when_comma_terminated = true
 split_complex_comprehension = true
 split_before_arithmetic_operator = true
 
 [tool.isort]
+extra_standard_library = [
+    'typing_extensions',
+]
 profile = 'hug'
 src_paths = [
     'tests',
     'todd',
 ]
 line_length = 79
 multi_line_output = 3
@@ -103,15 +109,18 @@
     'todd.base._patches.*',
 ]
 ignore_errors = true
 
 [tool.pytest.ini_options]
 norecursedirs = 'tests/helpers'
 filterwarnings = [
-    'ignore:lib2to3 package is deprecated and may not be able to parse Python 3.10+:PendingDeprecationWarning',
+    'ignore::DeprecationWarning:pkg_resources:121',
+    'ignore::DeprecationWarning:pkg_resources:2870',
+    'ignore::DeprecationWarning:yapf:16',
+    'ignore::UserWarning:mmcv:20',
 ]
 testpaths = 'tests todd'
 addopts = '--doctest-modules'
 
 [tool.coverage.run]
 branch = true
 command_line = '-m pytest'
@@ -134,14 +143,15 @@
     'class .*\(.*\bProtocol\b.*\):',
     '@(abc\.)?abstractmethod',
     '@overload',
 ]
 
 [tool.commitizen]
 name = 'cz_conventional_commits'
-version = "0.3.0"
+version = "0.4.0"
 tag_format = 'v$version'
 version_files = [
     'pyproject.toml:^version',
     'docs/source/conf.py:^release',
     'CITATION.cff:^version',
+    'todd/__init__.py:^__version__',
 ]
```

### Comparing `todd_ai-0.3.0/todd/adapts/__init__.py` & `todd_ai-0.4.0/todd/adapts/__init__.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/attention.py` & `todd_ai-0.4.0/todd/adapts/attention.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/base.py` & `todd_ai-0.4.0/todd/adapts/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import inspect
 import itertools
 
 import einops.layers.torch
 import torch.nn as nn
 
-from ..base import Module, Registry
+from ..base import Registry
+from ..utils import Module
 
 
 class BaseAdapt(Module):
     pass
 
 
 class AdaptRegistry(Registry):
```

### Comparing `todd_ai-0.3.0/todd/adapts/custom.py` & `todd_ai-0.4.0/todd/adapts/custom.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/decouple.py` & `todd_ai-0.4.0/todd/adapts/decouple.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/dict_tensor.py` & `todd_ai-0.4.0/todd/adapts/dict_tensor.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/iou.py` & `todd_ai-0.4.0/todd/adapts/iou.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/label_enc.py` & `todd_ai-0.4.0/todd/adapts/label_enc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from ..base import Module, Sequential
+from ..utils import Module, Sequential
 from .base import AdaptRegistry, BaseAdapt
 
 
 class Bottleneck(Module):
 
     def __init__(
         self,
```

### Comparing `todd_ai-0.3.0/todd/adapts/mask.py` & `todd_ai-0.4.0/todd/adapts/mask.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/adapts/roi_align.py` & `todd_ai-0.4.0/todd/adapts/roi_align.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from ..base import ModuleList
+from ..utils import ModuleList
 from .base import AdaptRegistry, BaseAdapt
 
 
 @AdaptRegistry.register()
 class RoIAlign(BaseAdapt):
 
     def __init__(self, strides: list[int], *args, **kwargs):
```

### Comparing `todd_ai-0.3.0/todd/base/bboxes.py` & `todd_ai-0.4.0/todd/base/bboxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     'BBoxesXYWH',
     'BBoxesCXCYWH',
 ]
 
 import numbers
 from abc import ABC, abstractmethod
 from typing import Generator, TypeVar
+from typing_extensions import Self
 
 import einops
 import torch
 
 BBox = tuple[numbers.Real, numbers.Real, numbers.Real, numbers.Real]
 T = TypeVar('T', bound='BBoxes')
 
@@ -57,15 +58,15 @@
             2
         """
         return self._bboxes.shape[0]
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self._bboxes})'
 
-    def __add__(self: T, other: T) -> T:
+    def __add__(self, other: Self) -> Self:
         """Concatenate bboxes.
 
         Args:
             other: :math:`n' \\times 4`.
 
         Returns:
             :math:`(n + n') \\times 4`, where `n` is the length of `self`.
@@ -77,15 +78,15 @@
             >>> BBoxesXYXY(a) + BBoxesXYXY(b)
             BBoxesXYXY(tensor([[ 5., 15.,  8., 18.],
                     [ 5., 15.,  8., 60.]]))
         """
         bboxes = torch.cat([self._bboxes, other._bboxes])
         return self.__class__(bboxes)
 
-    def __getitem__(self: T, indices) -> T:
+    def __getitem__(self, indices) -> Self:
         """Get specific bboxes.
 
         Args:
             indices: a index or multiple indices.
 
         Returns:
             If `indices` refers to a single box, return a ``tuple``.
@@ -292,30 +293,30 @@
             :math:`n \\times n'`.
         """
         intersections = self & other
         unions = self.unions(other, intersections).clamp_min_(eps)
         return intersections / unions
 
     @classmethod
-    def from_bboxes(cls: type[T], *args, **kwargs) -> T:
+    def from_bboxes(cls, *args, **kwargs) -> Self:
         return cls(cls._from_bboxes(*args, **kwargs))
 
-    def round(self: T, *args, **kwargs) -> T:
+    def round(self, *args, **kwargs) -> Self:
         return self.__class__(self._round(*args, **kwargs))
 
-    def expand(self: T, *args, **kwargs) -> T:
+    def expand(self, *args, **kwargs) -> Self:
         return self.__class__(self._expand(*args, **kwargs))
 
-    def clamp(self: T, *args, **kwargs) -> T:
+    def clamp(self, *args, **kwargs) -> Self:
         return self.__class__(self._clamp(*args, **kwargs))
 
-    def scale(self: T, *args, **kwargs) -> T:
+    def scale(self, *args, **kwargs) -> Self:
         return self.__class__(self._scale(*args, **kwargs))
 
-    def translate(self: T, *args, **kwargs) -> T:
+    def translate(self, *args, **kwargs) -> Self:
         return self.__class__(self._translate(*args, **kwargs))
 
     def indices(
         self,
         *,
         min_area: numbers.Real | None = None,
         min_wh: tuple[int, int] | None = None,
```

### Comparing `todd_ai-0.3.0/todd/base/checkpoints.py` & `todd_ai-0.4.0/todd/base/checkpoints.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 __all__ = [
-    'load_open_mmlab_models',
+    # 'load_open_mmlab_models',
     'transfer_weight',
     'transfer_weights',
 ]
 
-from .configs import Config
-from .patches import Module, get_, logger
-from .types import RegistryMeta
+from ..utils import Module
+from .patches import get_, logger
 
-
-def load_open_mmlab_models(
-    registry: RegistryMeta,
-    config: Config,
-    config_options: Config | None = None,  # TODO: rename overload
-    ckpt: str | None = None,
-) -> Module:
-    model = (
-        registry.build(config)
-        if config_options is None else registry.build(config_options, config)
-    )
-    if ckpt is not None:
-        import mmcv.runner
-        mmcv.runner.load_checkpoint(model, ckpt, map_location='cpu')
-        model._is_init = True
-    return model
+# from .configs import Config
+# from .registries import RegistryMeta
+# def load_open_mmlab_models(
+#     registry: RegistryMeta,
+#     config: Config,
+#     config_options: Config | None = None,  # TODO: rename overload
+#     ckpt: str | None = None,
+# ) -> Module:
+#     model = (
+#         registry.build(config)
+#         if config_options is None else registry.build(config_options, config)
+#     )
+#     if ckpt is not None:
+#         import mmcv.runner
+#         mmcv.runner.load_checkpoint(model, ckpt, map_location='cpu')
+#         model._is_init = True
+#     return model
 
 
 def transfer_weight(target: Module, source: Module) -> None:
     state_dict = source.state_dict()
     missing_keys, unexpected_keys = target.load_state_dict(
         state_dict,
         strict=False,
```

### Comparing `todd_ai-0.3.0/todd/base/configs.py` & `todd_ai-0.4.0/todd/base/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,26 @@
     'AttrDict',
     'Config',
     'DictAction',
 ]
 
 import argparse
 import difflib
+import importlib
 import pathlib
 import tempfile
 import webbrowser
 from collections import UserDict
-from typing import Any, Mapping, MutableMapping, Sequence, TypeVar, cast
+from typing import Any, Mapping, MutableMapping, Sequence, cast
+from typing_extensions import Self
 
 import yapf.yapflib.yapf_api as yapf
 
 from .patches import exec_, set_
 
-AttrDictType = TypeVar('AttrDictType', bound='AttrDict')
-ConfigType = TypeVar('ConfigType', bound='Config')
-
 
 class AttrDict(UserDict):
 
     @classmethod
     def _map(cls, item):
         if isinstance(item, (list, tuple, set)):
             return item.__class__(map(cls._map, item))
@@ -90,15 +89,15 @@
             value = self[name].__class__(
                 old_value[k] for k in range(len(old_value))
             )
 
         super().__setitem__(name, value)
 
     @classmethod
-    def loads(cls: type[ConfigType], s: str) -> ConfigType:
+    def loads(cls, s: str) -> Self:
         """Load config from string.
 
         Args:
             s: config string.
 
         Returns:
             The corresponding config.
@@ -107,17 +106,33 @@
 
             >>> Config.loads('a = 1\\nb = dict(c=3)')
             {'a': 1, 'b': {'c': 3}}
         """
         return cls(exec_(s))
 
     @classmethod
-    def load(cls: type[ConfigType], file) -> ConfigType:
+    def load(cls, file) -> Self:
+
+        class ModuleProxy:
+
+            def __init__(self, name: str) -> None:
+                self.__name = name
+                self.__module = importlib.import_module(name)
+
+            def __getattr__(self, attr: str):
+                return getattr(self.__module, attr)
+
+            def __repr__(self) -> str:
+                return f"_import_({repr(self.__name)})"
+
         file = pathlib.Path(file)
-        config = cls.loads(file.read_text())
+        config = exec_(  # do not use `loads`
+            file.read_text(),
+            _import_=ModuleProxy,
+        )
         base_config = cls()
         for base in config.pop('_base_', []):
             base_config.update(cls.load(file.parent / base))
         base_config.update(config)
         return base_config
 
     def dumps(self) -> str:
```

### Comparing `todd_ai-0.3.0/todd/base/enums.py` & `todd_ai-0.4.0/todd/utils/sgr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 __all__ = [
     'SGR',
 ]
 
 import enum
-from typing import Iterable, TypeVar, final
+from typing import Iterable
+from typing_extensions import Self
 
-SGRType = TypeVar('SGRType', bound='SGR')
 
-
-@final
 class SGR(enum.IntEnum):
     """Select Graphic Rendition.
 
     Refer to https://en.wikipedia.org/wiki/ANSI_escape_code.
     """
     NORMAL = 0
     BOLD = enum.auto()
@@ -40,20 +38,20 @@
     BG_YELLOW = enum.auto()
     BG_BLUE = enum.auto()
     BG_MAGENTA = enum.auto()
     BG_CYAN = enum.auto()
     BG_WHITE = enum.auto()
 
     @classmethod
-    def CSI(cls: type[SGRType], parameters: Iterable[SGRType]) -> str:
+    def CSI(cls, parameters: Iterable[Self]) -> str:
         """Control Sequence Introducer."""
         return f'\033[{";".join(str(p.value) for p in parameters)}m'
 
     @classmethod
-    def format(cls: type[SGRType], text: str, *args: SGRType) -> str:
+    def format(cls, text: str, *args: Self) -> str:
         return cls.CSI(args) + text + cls.CSI(tuple())
 
 
 if __name__ == '__main__':
     import itertools
 
     for fg, bg in itertools.product(range(30, 38), range(40, 48)):
```

### Comparing `todd_ai-0.3.0/todd/base/status.py` & `todd_ai-0.4.0/todd/base/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from typing import Any, Callable, Generic, Sequence, TypeVar, no_type_check
 
 T = TypeVar('T', bound=enum.Enum)
 
 
 class StatusMixin(Generic[T]):
 
-    def __init__(self, status: T) -> None:
+    def __init__(self, *args, status: T, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
         self._status = status
 
     @property
     def status(self) -> T:
         return self._status
 
     @staticmethod
```

### Comparing `todd_ai-0.3.0/todd/base/workflows.py` & `todd_ai-0.4.0/todd/base/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,47 +11,37 @@
 ]
 
 from abc import ABC, abstractmethod
 from collections import UserDict, UserList
 from functools import partial
 from itertools import repeat
 from symtable import symtable
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Iterable,
-    NamedTuple,
-    TypeVar,
-    final,
-)
+from typing import TYPE_CHECKING, Any, Callable, Iterable, NamedTuple, final
+from typing_extensions import Self
 
 import pandas as pd
 
 from .configs import Config
 from .patches import logger
-from .types import RegistryMeta
+from .registries import RegistryMeta
 
 Message = dict[str, Any]
 
-TaskType = TypeVar('TaskType', bound='Task')
-JobType = TypeVar('JobType', bound='Job')
-
 
 class Spec(NamedTuple):
     inputs: set[str]
     outputs: set[str]
 
 
 class Task(ABC):
     """Base class for `Step`, `Job`, and `Workflow`."""
 
     @classmethod
     @abstractmethod
-    def build(cls: type[TaskType], config: Config) -> TaskType:
+    def build(cls, config: Config) -> Self:
         """Builds a task.
 
         Args:
             config: task configuration.
 
         Returns:
             The built task.
@@ -149,15 +139,15 @@
         config = config.copy()
         registry: RegistryMeta = config.pop('registry')
         action: Config = config.pop('action')
         build = partial(registry.build, action)
 
         parallel = config.pop('parallel', False)
         if isinstance(parallel, Iterable):
-            return ParallelStep(tuple(map(build, parallel)), **config)
+            return ParallelStep(tuple(build(**p) for p in parallel), **config)
         if isinstance(parallel, int) and not isinstance(parallel, bool):
             return ParallelStep(
                 tuple(build() for _ in range(parallel)),
                 **config,
             )
         if parallel:
             return ParallelSingleStep(build(), **config)
@@ -324,15 +314,15 @@
     def actions(self) -> tuple[Callable]:
         return next(self._actions),
 
 
 class Job(UserList[Step], Task):
 
     @classmethod
-    def build(cls: type[JobType], config: Config) -> JobType:
+    def build(cls, config: Config) -> Self:
         config = config.copy()
         steps: Config = config.pop('steps')
         return cls([
             Step.build(Config(**v, **config, outputs=k))
             for k, v in steps.items()
         ])
```

### Comparing `todd_ai-0.3.0/todd/datasets/base.py` & `todd_ai-0.4.0/todd/datasets/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,73 @@
 __all__ = [
-    'AccessLayerRegistry',
-    'DatasetRegistry',
     'BaseAccessLayer',
     'BaseDataset',
 ]
 
 import reprlib
-from abc import abstractmethod
-from enum import Enum
-from typing import Any, Generic, MutableMapping, TypeVar
+from abc import ABC, abstractmethod
+from typing import Generic, MutableMapping, TypeVar
 
 from torch.utils.data import Dataset
 
-from ..base import Registry, logger
-
-T = TypeVar('T')
+from ..base import AccessLayerRegistry, Config, logger
 
+KT = TypeVar('KT')
+VT = TypeVar('VT')
 
-class Codec(Enum):
-    NONE = 'None'
-    PYTORCH = 'pytorch'
 
-
-class BaseAccessLayer(MutableMapping[T, Any]):
+class BaseAccessLayer(MutableMapping[KT, VT]):
 
     def __init__(
         self,
-        *args,
         data_root: str,
         task_name: str = '',
-        codec: str | Codec = 'pytorch',
-        readonly: bool = True,
-        exist_ok: bool = False,
-        **kwargs,
-    ):
+    ) -> None:
         self._data_root = data_root
         self._task_name = task_name
-        self._codec = Codec(codec)
-        self._readonly = readonly
-        self._exist_ok = exist_ok
-
-        self._init(*args, **kwargs)
-
-        if readonly and not self.exists:
-            raise FileNotFoundError(
-                f'{self._data_root} ({self._task_name}) does not exist.',
-            )
-        if not readonly and self.exists and not exist_ok:
-            raise FileExistsError(
-                f'{self._data_root} ({self._task_name}) already exists.',
-            )
-        if not readonly and not self.exists:
-            self.touch()
-
-    @abstractmethod
-    def _init(self, *args, **kwargs):
-        pass
 
     @property
     @abstractmethod
     def exists(self) -> bool:
         pass
 
     @abstractmethod
-    def touch(self):
+    def touch(self) -> None:
         pass
 
 
-class AccessLayerRegistry(Registry):
-    pass
+T = TypeVar('T')
 
 
-class BaseDataset(Dataset, Generic[T]):
-    ACCESS_LAYER: type = BaseAccessLayer[T]
+class BaseDataset(Dataset[T], Generic[T, KT, VT], ABC):
 
-    def __init__(self, *args, access_layer, **kwargs):
+    def __init__(
+        self,
+        *args,
+        access_layer: Config,
+        keys: Config | None = None,
+        **kwargs,
+    ) -> None:
         super().__init__(*args, **kwargs)
-        self._access_layer = AccessLayerRegistry.build(
-            access_layer,
-            default_config=dict(type=self.ACCESS_LAYER),
-        )
+        self._build_access_layer(access_layer)
+        if keys is None:
+            keys = Config()
+        self._build_keys(keys)
+
+    def _build_access_layer(self, config: Config) -> None:
+        self._access_layer: BaseAccessLayer[KT, VT] = \
+            AccessLayerRegistry.build(config)
 
+    def _build_keys(self, config: Config) -> None:
         logger.debug("Initializing keys.")
         self._keys = list(self._access_layer.keys())
         logger.debug(
             f"Keys {reprlib.repr(self._keys)} initialized "
             f"with length {len(self)}."
         )
 
     def __len__(self) -> int:
         return len(self._keys)
 
-    def __getitem__(self, index: int) -> Any:
+    def _access(self, index: int) -> VT:
         key = self._keys[index]
         return self._access_layer[key]
-
-
-class DatasetRegistry(Registry):
-    pass
```

### Comparing `todd_ai-0.3.0/todd/datasets/lmdb_.py` & `todd_ai-0.4.0/todd/datasets/lmdb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import io
-from functools import cached_property
-from typing import Any, Literal
+# import io
+# from functools import cached_property
+# from typing import Any, Literal
 
-import lmdb
-import torch
+# import lmdb
+# import torch
 
-from .base import BaseDataset, DatasetRegistry
+# from ..base import DatasetRegistry
+# from .base import BaseDataset
 
 # TODO: update
 
+# @DatasetRegistry.register()
+# class LmdbDataset(BaseDataset[bytes]):
 
-@DatasetRegistry.register()
-class LmdbDataset(BaseDataset[bytes]):
+#     def __init__(
+#         self,
+#         *args,
+#         filepath: str,
+#         db: str | None = None,
+#         decoder: Literal['None', 'pytorch'] | None = 'pytorch',
+#         **kwargs,
+#     ):
+#         self._env: lmdb.Environment = lmdb.open(
+#             filepath, readonly=True, max_dbs=1
+#         )
+#         self._db: lmdb._Database | None = (  # yapf: disable
+#             None if db is None else self._env.open_db(db.encode())
+#         )
+#         self._decoder = decoder
+#         super().__init__(*args, **kwargs)
+
+#     @classmethod
+#     def load_from(cls, source: BaseDataset, *args, **kwargs):
+#         pass
+
+#     def _map_indices(self) -> list[bytes]:
+#         with self.begin() as txn, txn.cursor() as cur:
+#             return list(cur.iternext(keys=True, values=False))
+
+#     @cached_property
+#     def _len(self) -> int:
+#         with self.begin() as txn:
+#             return txn.stat()['entries']
+
+#     def _getitem(self, index: bytes) -> Any:
+#         if not isinstance(index, bytes):
+#             index = str(index).encode()
+#         with self.begin() as txn:
+#             buffer = txn.get(index)
+#         if self._decoder is None or self._decoder == 'None':
+#             return buffer
+#         if self._decoder == 'pytorch':
+#             buffer = io.BytesIO(buffer)
+#             return torch.load(buffer, map_location='cpu')
+#         raise Exception
 
-    def __init__(
-        self,
-        *args,
-        filepath: str,
-        db: str | None = None,
-        decoder: Literal['None', 'pytorch'] | None = 'pytorch',
-        **kwargs,
-    ):
-        self._env: lmdb.Environment = lmdb.open(
-            filepath, readonly=True, max_dbs=1
-        )
-        self._db: lmdb._Database | None = (  # yapf: disable
-            None if db is None else self._env.open_db(db.encode())
-        )
-        self._decoder = decoder
-        super().__init__(*args, **kwargs)
-
-    @classmethod
-    def load_from(cls, source: BaseDataset, *args, **kwargs):
-        pass
-
-    def _map_indices(self) -> list[bytes]:
-        with self.begin() as txn, txn.cursor() as cur:
-            return list(cur.iternext(keys=True, values=False))
-
-    @cached_property
-    def _len(self) -> int:
-        with self.begin() as txn:
-            return txn.stat()['entries']
-
-    def _getitem(self, index: bytes) -> Any:
-        if not isinstance(index, bytes):
-            index = str(index).encode()
-        with self.begin() as txn:
-            buffer = txn.get(index)
-        if self._decoder is None or self._decoder == 'None':
-            return buffer
-        if self._decoder == 'pytorch':
-            buffer = io.BytesIO(buffer)
-            return torch.load(buffer, map_location='cpu')
-        raise Exception
-
-    def begin(self) -> lmdb.Transaction:
-        return self._env.begin(self._db)
+#     def begin(self) -> lmdb.Transaction:
+#         return self._env.begin(self._db)
```

### Comparing `todd_ai-0.3.0/todd/datasets/zip.py` & `todd_ai-0.4.0/todd/datasets/zip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,68 @@
-import os
-import zipfile
-from io import BytesIO
-from pathlib import Path
-from typing import Any, Iterator
-
-import torch
-
-from .base import (
-    AccessLayerRegistry,
-    BaseAccessLayer,
-    BaseDataset,
-    Codec,
-    DatasetRegistry,
-)
-
-# TODO: update
-
-
-@AccessLayerRegistry.register()
-class ZipAccessLayer(BaseAccessLayer[str]):
-
-    def _init(self):
-        assert self._readonly, 'ZipAccessLayer is read-only.'
-        assert self._codec is Codec.PYTORCH, \
-            'ZipAccessLayer only supports PyTorch.'
-        data_root_parts = Path(self._data_root).parts
-        zip_indices = [  # yapf: disable
-            i for i, part in enumerate(data_root_parts)
-            if part.endswith('.zip')
-        ]
-        if len(zip_indices) == 0:
-            raise ValueError(f'{self._data_root} does not contain a zip file.')
-        elif len(zip_indices) > 1:
-            raise ValueError(f'{self._data_root} contains multiple zip files.')
-        zip_index = zip_indices[0]
-        self._zip_root = zipfile.Path(
-            os.path.join(*data_root_parts[:zip_index + 1]),
-            os.path.join(
-                *data_root_parts[zip_index + 1:],
-                self._task_name,
-                '',
-            ),
-        )
-
-    @property
-    def exists(self) -> bool:
-        return self._zip_root.exists()
-
-    def touch(self):
-        raise NotImplementedError
-
-    def __iter__(self) -> Iterator[str]:
-        return (path.name for path in self._zip_root.iterdir())
-
-    def __len__(self) -> int:
-        return len(list(self._zip_root.iterdir()))
-
-    def __getitem__(self, key: str) -> Any:
-        data_file = self._zip_root / key
-        bytes_io = BytesIO(data_file.read_bytes())
-        return torch.load(bytes_io, map_location='cpu')
-
-    def __setitem__(self, key: str, value: Any):
-        raise NotImplementedError
-
-    def __delitem__(self, key: str):
-        raise NotImplementedError
-
-
-@DatasetRegistry.register()
-class ZipDataset(BaseDataset[str]):
-    ACCESS_LAYER = ZipAccessLayer
+# import os
+# import zipfile
+# from io import BytesIO
+# from pathlib import Path
+# from typing import Any, Iterator
+
+# import torch
+
+# from ..base import DatasetRegistry
+# from .base import AccessLayerRegistry, BaseAccessLayer, BaseDataset
+
+# # TODO: update
+
+# @AccessLayerRegistry.register()
+# class ZipAccessLayer(BaseAccessLayer[str]):
+
+#     def _init(self):
+#         assert self._readonly, 'ZipAccessLayer is read-only.'
+#         data_root_parts = Path(self._data_root).parts
+#         zip_indices = [  # yapf: disable
+#             i for i, part in enumerate(data_root_parts)
+#             if part.endswith('.zip')
+#         ]
+#         if len(zip_indices) == 0:
+#             raise ValueError(
+#                 f'{self._data_root} does not contain a zip file.'
+#             )
+#         elif len(zip_indices) > 1:
+#             raise ValueError(
+#                 f'{self._data_root} contains multiple zip files.'
+#             )
+#         zip_index = zip_indices[0]
+#         self._zip_root = zipfile.Path(
+#             os.path.join(*data_root_parts[:zip_index + 1]),
+#             os.path.join(
+#                 *data_root_parts[zip_index + 1:],
+#                 self._task_name,
+#                 '',
+#             ),
+#         )
+
+#     @property
+#     def exists(self) -> bool:
+#         return self._zip_root.exists()
+
+#     def touch(self):
+#         raise NotImplementedError
+
+#     def __iter__(self) -> Iterator[str]:
+#         return (path.name for path in self._zip_root.iterdir())
+
+#     def __len__(self) -> int:
+#         return len(list(self._zip_root.iterdir()))
+
+#     def __getitem__(self, key: str) -> Any:
+#         data_file = self._zip_root / key
+#         bytes_io = BytesIO(data_file.read_bytes())
+#         return torch.load(bytes_io, map_location='cpu')
+
+#     def __setitem__(self, key: str, value: Any):
+#         raise NotImplementedError
+
+#     def __delitem__(self, key: str):
+#         raise NotImplementedError
+
+# @DatasetRegistry.register()
+# class ZipDataset(BaseDataset[str]):
+#     ACCESS_LAYER = ZipAccessLayer
```

### Comparing `todd_ai-0.3.0/todd/distillers/base.py` & `todd_ai-0.4.0/todd/distillers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 __all__ = [
     'DistillerRegistry',
     'BaseDistiller',
     'DistillerStore',
 ]
 
 import warnings
-from typing import Callable, Iterable, Mapping, TypeVar, cast
+from typing import Callable, Iterable, Mapping, cast
+from typing_extensions import Self
 
 import torch.nn as nn
 
 from ..adapts import AdaptRegistry
 from ..base import (
     Config,
+    HookRegistry,
     Job,
+    LossRegistry,
     Message,
-    Module,
-    ModuleList,
     Registry,
     Spec,
     StoreMeta,
     Workflow,
     transfer_weights,
 )
-from ..hooks import BaseHook, HookRegistry
-from ..losses import LossRegistry
-from ..losses.base import BaseLoss
-
-T = TypeVar('T', bound='BaseDistiller')
+from ..hooks import BaseHook
+from ..losses import BaseLoss
+from ..utils import Module, ModuleList
 
 
 class DistillerStore(metaclass=StoreMeta):
     CHECK_INPUTS: bool
     INTERMEDIATE_OUTPUTS: str
 
 
 class BaseDistiller(Module, Workflow):
 
     @classmethod
-    def build(cls: type[T], config: Config) -> T:
+    def build(cls, config: Config) -> Self:
         config = config.copy()
 
         models = tuple(config.pop('models'))
 
         hooks: Config = config.pop('hooks')
         adapts: Config = config.pop('adapts')
         losses: Config = config.pop('losses')
@@ -131,15 +130,15 @@
             loss_spec.outputs,
         )
 
     @property
     def models(self) -> tuple[nn.Module, ...]:
         return self._models
 
-    def _apply(self: T, fn: Callable[..., None]) -> T:
+    def _apply(self, fn: Callable[..., None]) -> Self:
         for model in self._models:
             if getattr(model, 'sync_apply', True):
                 model._apply(fn)
         return super()._apply(fn)
 
     def track_tensors(self) -> None:
         hooks = cast(tuple[BaseHook, ...], self['hooks'].actions)
```

### Comparing `todd_ai-0.3.0/todd/distillers/single_student.py` & `todd_ai-0.4.0/todd/distillers/single_student.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,27 @@
     'MultiTeacherDistiller',
     'SingleTeacherDistiller',
     'SelfDistiller',
     'Student',
 ]
 
 from typing import Generic, TypeVar, final
+from typing_extensions import Self
 
 import torch.nn as nn
 
-from ..base import Config, ModuleList
-from ..reproduction import freeze
+from ..base import Config
+from ..utils import ModuleList
 from .base import BaseDistiller, DistillerRegistry
 
-SSDType = TypeVar('SSDType', bound='SingleStudentDistiller')
-MTDType = TypeVar('MTDType', bound='MultiTeacherDistiller')
-STDType = TypeVar('STDType', bound='SingleTeacherDistiller')
-SDType = TypeVar('SDType', bound='SelfDistiller')
-
 
 class SingleStudentDistiller(BaseDistiller):
 
     @classmethod
-    def build(cls: type[SSDType], config: Config) -> SSDType:
+    def build(cls, config: Config) -> Self:
         assert 'models' not in config
         assert 'hooks' not in config
 
         config = config.copy()
 
         student = config.pop('student'),
         teachers = config.pop('teachers', tuple())
@@ -46,23 +42,25 @@
         return self.models[0]
 
 
 @DistillerRegistry.register()
 class MultiTeacherDistiller(SingleStudentDistiller):
 
     @classmethod
-    def build(cls: type[MTDType], config: Config) -> MTDType:
+    def build(cls, config: Config) -> Self:
         assert 'teachers' not in config
         assert 'teacher_hooks' not in config
         assert 'num_onlines' not in config
 
         config = config.copy()
 
-        online_teachers = config.pop('online_teachers', tuple())
-        offline_teachers = config.pop('offline_teachers', tuple())
+        online_teachers: tuple[nn.Module] = \
+            config.pop('online_teachers', tuple())
+        offline_teachers: tuple[nn.Module] = \
+            config.pop('offline_teachers', tuple())
         config.teachers = online_teachers + offline_teachers
 
         config.num_onlines = len(online_teachers)
 
         teacher_hooks = config.pop('online_hook', dict())
         if 'offline_hooks' in config:
             offline_hooks: Config = config.pop('offline_hooks')
@@ -71,15 +69,16 @@
                 for k, v in offline_hooks.items()
             })
         config.teacher_hooks = teacher_hooks
 
         distiller = super().build(config)
 
         for offline_teacher in offline_teachers:
-            freeze(offline_teacher)
+            offline_teacher.requires_grad_(False)
+            offline_teacher.eval()
         distiller.add_module('_teachers', ModuleList(online_teachers))
 
         return distiller
 
     def __init__(self, *args, num_onlines: int = 0, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._num_onlines = num_onlines
@@ -97,44 +96,45 @@
         return self.models[1 + self._num_onlines:]
 
 
 @DistillerRegistry.register()
 class SingleTeacherDistiller(SingleStudentDistiller):
 
     @classmethod
-    def build(cls: type[STDType], config: Config) -> STDType:
+    def build(cls, config: Config) -> Self:
         assert 'teachers' not in config
 
         config = config.copy()
 
-        teacher = config.pop('teacher')
+        teacher: nn.Module = config.pop('teacher')
         config.teachers = teacher,
 
         if 'teacher_hooks' in config:
             config.teacher_hooks = {0: config.teacher_hooks}
 
         distiller = super().build(config)
 
         if config.pop('online', False):
             distiller.add_module('_teacher', teacher)
         else:
-            freeze(teacher)
+            teacher.requires_grad_(False)
+            teacher.eval()
 
         return distiller
 
     @property
     def teacher(self) -> nn.Module:
         return self.models[1]
 
 
 @DistillerRegistry.register()
 class SelfDistiller(SingleStudentDistiller):
 
     @classmethod
-    def build(cls: type[SDType], config: Config) -> SDType:
+    def build(cls, config: Config) -> Self:
         assert 'teachers' not in config
         assert 'teacher_hooks' not in config
 
         config = config.copy()
 
         if 'weight_transfer' in config:
             weight_transfer: Config = config.weight_transfer
@@ -150,15 +150,15 @@
 
 
 class Student(Generic[T]):
 
     def __init__(self, distiller: Config) -> None:
         self._distiller = DistillerRegistry.build(
             distiller,
-            Config(student=self),
+            student=self,
         )
 
     @property
     def distiller(self) -> T:
         return self._distiller
 
     @property
```

### Comparing `todd_ai-0.3.0/todd/hooks/base.py` & `todd_ai-0.4.0/todd/hooks/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 __all__ = [
-    'HookRegistry',
     'BaseHook',
 ]
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from enum import IntEnum, auto
-from typing import TYPE_CHECKING, Protocol
 
 import torch.nn as nn
 
-from ..base import Registry, StatusMixin, get_
+from ..base import StatusMixin, get_
 
-if TYPE_CHECKING:
+# from typing import TYPE_CHECKING, Protocol
 
-    class _HookProto(Protocol):
-        _path: str
+# if TYPE_CHECKING:
 
-        def register_tensor(self, tensor) -> None:
-            pass
+#     class _HookProto(Protocol):
+#         _path: str
 
-else:
-    _HookProto = object
+#         def register_tensor(self, tensor) -> None:
+#             pass
+
+# else:
+#     _HookProto = object
 
 
 class Status(IntEnum):
     INITIALIZED = auto()
     BINDED = auto()
     REGISTERED = auto()
 
 
-class _HookMixin(_HookProto):
+class BaseMixin(ABC):
+
+    def __init__(self, *args, path: str, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self._path = path
+
+    @abstractmethod
+    def register_tensor(self, tensor) -> None:
+        pass
+
+
+class HookMixin(BaseMixin):
 
     def _forward_hook(self, module: nn.Module, input_, output) -> None:
         self.register_tensor(output)
 
     def bind(self, model: nn.Module) -> None:
         module: nn.Module = get_(model, self._path)
         self._handle = module.register_forward_hook(self._forward_hook)
 
     def unbind(self) -> None:
         self._handle.remove()
 
 
-class _TrackingMixin(_HookProto):
+class TrackingMixin(BaseMixin):
 
     def __init__(
         self,
+        *args,
         tracking_mode: bool = False,
+        **kwargs,
     ) -> None:
+        super().__init__(*args, **kwargs)
         self._tracking_mode = tracking_mode
 
     @property
     def tracking_mode(self) -> bool:
         return self._tracking_mode
 
     def bind(self, model: nn.Module) -> None:
@@ -63,25 +77,18 @@
     def track_tensor(self) -> None:
         if not self._tracking_mode:
             raise AttributeError(f"Hook {self._path} does not support track.")
         tensor = get_(self._model, self._path)
         self.register_tensor(tensor)
 
 
-class BaseHook(StatusMixin[Status], _HookMixin, _TrackingMixin):
+class BaseHook(StatusMixin[Status], HookMixin, TrackingMixin):
 
-    def __init__(
-        self,
-        path: str,
-        tracking_mode: bool = False,
-    ) -> None:
-        StatusMixin.__init__(self, Status.INITIALIZED)
-        _HookMixin.__init__(self)
-        _TrackingMixin.__init__(self, tracking_mode)
-        self._path = path
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(self, *args, status=Status.INITIALIZED, **kwargs)
         self._reset()
 
     def __call__(self):
         if self.status != Status.REGISTERED:
             raise RuntimeError(f"Hook {self._path} is not registered.")
         return self._tensor()
 
@@ -100,35 +107,31 @@
     @abstractmethod
     def _tensor(self):
         pass
 
     @StatusMixin.transit(Status.INITIALIZED, Status.BINDED)
     def bind(self, model: nn.Module) -> None:
         if self._tracking_mode:
-            _TrackingMixin.bind(self, model)
+            TrackingMixin.bind(self, model)
         else:
-            _HookMixin.bind(self, model)
+            HookMixin.bind(self, model)
 
     @StatusMixin.transit(Status.BINDED, Status.INITIALIZED)
     def unbind(self) -> None:
         if self._tracking_mode:
-            _TrackingMixin.unbind(self)
+            TrackingMixin.unbind(self)
         else:
-            _HookMixin.unbind(self)
+            HookMixin.unbind(self)
 
     @StatusMixin.transit(
         (Status.BINDED, Status.REGISTERED),
         Status.REGISTERED,
     )
     def register_tensor(self, tensor) -> None:
         self._register_tensor(tensor)
 
     @StatusMixin.transit(
         (Status.BINDED, Status.REGISTERED),
         Status.BINDED,
     )
     def reset(self) -> None:
         self._reset()
-
-
-class HookRegistry(Registry):
-    pass
```

### Comparing `todd_ai-0.3.0/todd/losses/base.py` & `todd_ai-0.4.0/todd/losses/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __all__ = [
     'BaseLoss',
-    'LossRegistry',
 ]
 
 from typing import Literal
 
 import torch
 
-from ..base import Config, Module, Registry
+from ..base import Config
+from ..utils import Module
 from .schedulers import BaseScheduler, SchedulerRegistry
 
 Reduction = Literal['none', 'mean', 'sum', 'prod']
 
 
 class BaseLoss(Module):
 
@@ -75,11 +75,7 @@
     # if bound < weight * output
     if coef < 1.0:
         # weight = bound / output
         weight *= coef
 
     output = weight * output
     return output
-
-
-class LossRegistry(Registry):
-    pass
```

### Comparing `todd_ai-0.3.0/todd/losses/ckd.py` & `todd_ai-0.4.0/todd/losses/ckd.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
     'CKDLoss',
 ]
 
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 
-from ..base import BBoxesXYXY, get_rank, get_world_size
-from .base import BaseLoss, LossRegistry
+from ..base import BBoxesXYXY, LossRegistry
+from ..utils import get_rank, get_world_size
+from .base import BaseLoss
 
 
 def ckd_loss(
     pred: torch.Tensor,
     target: torch.Tensor,
     ignore: tuple[torch.Tensor, torch.Tensor] | None = None,
     gamma: float = 0.07,
```

### Comparing `todd_ai-0.3.0/todd/losses/focal.py` & `todd_ai-0.4.0/todd/losses/focal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = [
     'FocalLoss',
     'FocalWithLogitsLoss',
 ]
 
 import torch
 
-from .base import LossRegistry
+from ..base import LossRegistry
 from .functional import BCELoss, BCEWithLogitsLoss, FunctionalLoss
 
 
 class FocalMixin(FunctionalLoss):
 
     def __init__(
         self,
```

### Comparing `todd_ai-0.3.0/todd/losses/functional.py` & `todd_ai-0.4.0/todd/losses/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 ]
 
 from abc import abstractmethod
 
 import torch
 import torch.nn.functional as F
 
-from .base import BaseLoss, LossRegistry
+from ..base import LossRegistry
+from .base import BaseLoss
 
 
 class FunctionalLoss(BaseLoss):
 
     @staticmethod
     @abstractmethod
     def func(*args, **kwargs) -> torch.Tensor:
```

### Comparing `todd_ai-0.3.0/todd/losses/mimic.py` & `todd_ai-0.4.0/todd/losses/mimic.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'FGFILoss',
 ]
 
 import einops
 import torch
 import torch.nn.functional as F
 
-from .base import LossRegistry
+from ..base import LossRegistry
 from .functional import FunctionalLoss, L1Loss, MSELoss
 
 
 class _2DMixin(FunctionalLoss):
 
     def forward(
         self,
```

### Comparing `todd_ai-0.3.0/todd/losses/rcnn.py` & `todd_ai-0.4.0/todd/losses/rcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Callable
 
 import einops
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from .base import LossRegistry
+from ..base import LossRegistry
 from .functional import MSELoss
 
 
 @LossRegistry.register()
 class SGFILoss(MSELoss):
 
     def __init__(
```

### Comparing `todd_ai-0.3.0/todd/losses/schedulers.py` & `todd_ai-0.4.0/todd/losses/schedulers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 __all__ = [
     'BaseScheduler',
-    'SchedulerRegistry',
     'ConstantScheduler',
     'WarmupScheduler',
     'EarlyStopScheduler',
     'DecayScheduler',
     'StepScheduler',
     'CosineAnnealingScheduler',
     'ChainedScheduler',
@@ -13,15 +12,15 @@
 import bisect
 import math
 from abc import ABC, abstractmethod
 from typing import Iterable
 
 import torch
 
-from ..base import Registry
+from ..base import SchedulerRegistry
 
 
 class BaseScheduler(torch.nn.Module, ABC):
     """Base class for schedulers.
 
     Under most cases, schedulers are used as a variable loss weight.
     Schedulers are functions of `steps`, which could mean iterations or
@@ -74,18 +73,14 @@
         pass
 
 
 def forward_hook(module: BaseScheduler, input_, output: float) -> float:
     return output * module.gain
 
 
-class SchedulerRegistry(Registry):
-    pass
-
-
 @SchedulerRegistry.register()
 class ConstantScheduler(BaseScheduler):
     """Unvarying scheduler.
 
     The value of this scheduler is always the `gain`:
 
         >>> constant = ConstantScheduler(5)
```

### Comparing `todd_ai-0.3.0/todd/reproduction/seed.py` & `todd_ai-0.4.0/todd/reproduction/seed.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from typing import Generator
 
 import numpy as np
 import torch
 import torch.backends.cudnn as cudnn
 import torch.distributed as dist
 
-from ..base import Store, get_world_size, logger
+from ..base import Store, logger
+from ..utils import get_world_size
 
 
 def randint(high: int = 2**30) -> int:
     seed = np.random.randint(high)
     if get_world_size() <= 1:
         return seed
     tensor = torch.tensor(seed, dtype=torch.int)
@@ -27,15 +28,15 @@
 
 def init_seed(seed: int) -> None:
     seed %= 2**30
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     if Store.CUDA:
-        torch.cuda.manual_seed_all(seed)
+        torch.cuda.manual_seed(seed)
 
 
 @contextmanager
 def set_seed_temp(
     seed=None,
     deterministic: bool = False,
     benchmark: bool = True,
```

### Comparing `todd_ai-0.3.0/todd/scripts/convert_ckpts.py` & `todd_ai-0.4.0/todd/scripts/convert_ckpts.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/scripts/convert_logs.py` & `todd_ai-0.4.0/todd/scripts/convert_logs.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/scripts/merge_lmdbs.py` & `todd_ai-0.4.0/todd/scripts/merge_lmdbs.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/utils/generic_tensors.py` & `todd_ai-0.4.0/todd/utils/generic_tensors.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.3.0/todd/utils/runners.py` & `todd_ai-0.4.0/todd/runners/runners.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,421 +1,435 @@
 __all__ = [
-    'Control',
     'BaseRunner',
     'Validator',
     'Trainer',
     'IterBasedTrainer',
     'EpochBasedTrainer',
-    'RunnerRegistry',
-    'Memo',
+    'RunnerHolderMixin',
 ]
 
-import enum
+import contextlib
 import getpass
 import itertools
 import logging
+import os
 import pathlib
 import socket
-from abc import ABC, abstractmethod
-from datetime import datetime
-from typing import Any, Mapping, Protocol, runtime_checkable
+import weakref
+from abc import abstractmethod
+from typing import TYPE_CHECKING, Any, Mapping, cast
 
 import torch
 import torch.distributed
 import torch.utils.data
 
 from ..base import (
+    CallbackRegistry,
     Config,
-    Formatter,
-    LrSchedulerRegistry,
-    OptimizerRegistry,
-    Registry,
-    Store,
+    DatasetRegistry,
+    SamplerRegistry,
+    StateDictMixin,
+    StrategyRegistry,
 )
+from ..base import logger as base_logger
+from ..utils import get_rank
 
-Memo = dict[str, Any]
-
-
-@runtime_checkable
-class DistributedSamplerProto(Protocol):
-
-    def set_epoch(self, epoch: int) -> None:
-        ...
+if TYPE_CHECKING:
+    from .callbacks import BaseCallback
+    from .strategies import BaseStrategy
 
+Memo = dict[str, Any]
 
-class Control(enum.Enum):
-    BREAK = enum.auto()
-    CONTINUE = enum.auto()
+# TODO: split into multiple files
 
 
-class BaseRunner(ABC):
+class BaseRunner(StateDictMixin):
 
     def __init__(
         self,
         name: str,
-        model: torch.nn.Module,
-        dataloader: Config,
-        log: Config,
-        load_state_dict: Config,
-        state_dict: Config,
+        *args,
+        load_from: str | None = None,
+        **kwargs,
     ) -> None:
-        self._work_dir = self._build_work_dir(name)
-        self._model = model
-        self._logger = self._build_logger()
-
-        self._dataloader = self._build_dataloader(dataloader)
-        self._log = log
-        self._load_state_dict = load_state_dict
-        self._state_dict = state_dict
+        self._name = name
+        self._load_from = load_from
 
         self._iter = 0
+        self._build(*args, **kwargs)
+        self._callbacks.connect()
+
         self._logger.debug(
-            f"Runner initialized by {getpass.getuser()}@{socket.gethostname()}"
+            f"Rank {get_rank()} initialized by "
+            f"{getpass.getuser()}@{socket.gethostname()}"
         )
 
     @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def load_from(self) -> str | None:
+        return self._load_from
+
+    @property
+    def iter_(self) -> int:
+        return self._iter
+
+    @property
+    def work_dir(self) -> pathlib.Path:
+        return self._work_dir
+
+    @property
+    def logger(self) -> logging.Logger:
+        return self._logger
+
+    @property
+    def strategy(self) -> 'BaseStrategy':
+        return self._strategy
+
+    @property
     def iters(self) -> int:
         return len(self._dataloader)
 
-    def _build_logger(self) -> logging.Logger:
-        file = self._work_dir / '_.log'
-        file = file.with_stem(datetime.now().astimezone().isoformat())
-        handler = logging.FileHandler(file)
-        handler.setFormatter(Formatter())
-
-        from ..base import logger
-        name = f'{logger.name}.{self.__class__.__name__}'
-        logger = logging.getLogger(name)
-        logger.addHandler(handler)
-        return logger
-
-    def _build_work_dir(self, name: str) -> pathlib.Path:
-        work_dir = pathlib.Path('work_dirs') / name
-        work_dir.mkdir(parents=True, exist_ok=True)
-        return work_dir
-
-    @property
-    def model(self) -> torch.nn.Module:
-        """The underlying model if being wrapped."""
-        model = self._model
-        if isinstance(model, torch.nn.parallel.DistributedDataParallel):
-            model = model.module
-        return model
+    @property
+    def dataloader(self) -> torch.utils.data.DataLoader:
+        return self._dataloader
 
-    @abstractmethod
-    def _build_dataloader(self, config: Config) -> torch.utils.data.DataLoader:
+    def _build_dataloader(self, *args, dataloader: Config, **kwargs) -> None:
         """Build the dataloader.
 
         Args:
             config: dataloader config.
         """
-        pass
-
-    def _control_run_iter(self, batch, memo: Memo) -> Control | None:
-        """Whether the current iteration should execute or not.
+        dataloader = dataloader.copy()
+        dataset = DatasetRegistry.build(dataloader.pop('dataset'))
+        if 'sampler' in dataloader:
+            dataloader.sampler = SamplerRegistry.build(
+                dataloader.pop('sampler'),
+                dataset=dataset,
+            )
+        self._dataloader = torch.utils.data.DataLoader(dataset, **dataloader)
 
-        Args:
-            i: iteration index.
-            batch: inputs.
-            memo: runtime memory.
+    def _build_strategy(
+        self,
+        *args,
+        strategy: Config,
+        **kwargs,
+    ) -> None:
+        self._strategy: 'BaseStrategy' = StrategyRegistry.build(
+            strategy,
+            runner=self,
+        )
 
-        Returns:
-            The control action or `None` for no control.
+    def _build_callbacks(
+        self,
+        *args,
+        callbacks: Config | list[Config] | None = None,
+        **kwargs,
+    ) -> None:
+        if callbacks is None:
+            callbacks = []
+        if isinstance(callbacks, list):
+            callbacks = Config(type='ComposedCallback', callbacks=callbacks)
+        self._callbacks: 'BaseCallback' = CallbackRegistry.build(
+            callbacks,
+            runner=self,
+        )
 
-        Override this method for early stopping, error detection, etc.
-        By default, this method supports `DRY_RUN` by returning
-        `Control.BREAK` after the first log message.
-        """
-        if Store.DRY_RUN and self._iter > self._log.interval:
-            return Control.BREAK
-        return None
+    def _build_work_dir(
+        self,
+        *args,
+        work_dir: Config | None = None,
+        **kwargs,
+    ) -> None:
+        if work_dir is None:
+            work_dir = Config()
+        root = work_dir.get('root', 'work_dirs')
+        name = work_dir.get('name', self._name)
+        path = os.path.join(root, name)
+        self._work_dir = pathlib.Path(path)
+        self._work_dir.mkdir(parents=True, exist_ok=True)
 
-    def _before_run_iter(self, batch, memo: Memo) -> None:
-        pass
+    def _build_logger(
+        self,
+        *args,
+        logger: Config | None = None,
+        **kwargs,
+    ) -> None:
+        if logger is None:
+            logger = Config()
+        name = logger.get(
+            'name',
+            f'{self.__class__.__name__}.{self._name}',
+        )
+        self._logger = logging.getLogger(f'{base_logger.name}.{name}')
 
-    def _before_run_iter_log(self, batch, memo: Memo) -> str | None:
-        pass
+    def _build(self, *args, **kwargs) -> None:
+        self._build_strategy(*args, **kwargs)
+        self._build_dataloader(*args, **kwargs)
+        self._build_callbacks(*args, **kwargs)
+        self._build_work_dir(*args, **kwargs)
+        self._build_logger(*args, **kwargs)
 
     @abstractmethod
-    def _run_iter(self, batch, memo: Memo) -> torch.Tensor:
-        pass
+    def _run_iter(self, batch, memo: Memo) -> Memo:
+        """Run iteration.
 
-    def _after_run_iter_log(self, batch, memo: Memo) -> str | None:
-        loss: torch.Tensor = memo['loss']
-        return f"Iter [{self._iter}/{self.iters}] Loss {loss.item():.3f}"
+        Args:
+            batch: input data
+            memo: runtime memory
 
-    def _after_run_iter(self, batch, memo: Memo) -> None:
+        Returns:
+            Updated runtime memory.
+        """
         pass
 
-    def _before_run(self) -> Memo:
-        return dict(dataloader=self._dataloader)
-
-    def _run(self, memo: Memo) -> None:
+    def _run(self, memo: Memo) -> Memo:
         dataloader = memo['dataloader']
         for batch in dataloader:
             self._iter += 1
-            control = self._control_run_iter(batch, memo)
-            if control is Control.BREAK:
+
+            if self._callbacks.should_break(batch, memo):
                 break
-            if control is Control.CONTINUE:
+            if self._callbacks.should_continue(batch, memo):
                 continue
-            assert control is None, control
-            self._before_run_iter(batch, memo)
-            if log := self._iter % self._log.interval == 0:
-                info = self._before_run_iter_log(batch, memo)
-                if info is not None:
-                    self._logger.info(info)
-            try:
-                memo['loss'] = self._run_iter(batch, memo)
-            except Exception:
-                self._logger.exception(
-                    f"Unable to run iter {self._iter}\n{batch=}\n{memo=}"
-                )
-                raise
-            if log:
-                info = self._after_run_iter_log(batch, memo)
-                if info is not None:
-                    self._logger.info(info)
-            self._after_run_iter(batch, memo)
 
-    def _after_run(self, memo: Memo) -> None:
+            self._callbacks.before_run_iter(batch, memo)
+            with contextlib.ExitStack() as exit_stack:
+                self._callbacks.run_iter_context(exit_stack, batch, memo)
+                memo = self._run_iter(batch, memo)
+            self._callbacks.after_run_iter(batch, memo)
+        return memo
+
+    def _setup(self) -> Memo:
+        return dict(dataloader=self._dataloader)
+
+    def _teardown(self, memo: Memo) -> None:
         pass
 
     def run(self) -> Memo:
-        memo = self._before_run()
-        self._run(memo)
-        self._after_run(memo)
+        memo = self._setup()
+        self._callbacks.before_run(memo)
+        memo = self._run(memo)
+        self._callbacks.after_run(memo)
+        self._teardown(memo)
         return memo
 
-    def load_state_dict(self, state_dict: Mapping[str, Any]) -> None:
-        self.model.load_state_dict(
+    def load_state_dict(
+        self,
+        state_dict: Mapping[str, Any],
+        *args,
+        **kwargs,
+    ) -> None:
+        super().load_state_dict(state_dict, *args, **kwargs)
+        self._iter = state_dict['meta']['iter_']
+        self._strategy.load_model_state_dict(
             state_dict['model'],
-            **self._load_state_dict.model,
+            *args,
+            **kwargs,
+        )
+        self._strategy.load_state_dict(
+            state_dict['strategy'],
+            *args,
+            **kwargs,
+        )
+        self._callbacks.load_state_dict(
+            state_dict['callbacks'],
+            *args,
+            **kwargs,
         )
-        self._iter = state_dict['iter_']
 
-    def state_dict(self) -> dict[str, Any]:
-        model = self.model.state_dict(**self._state_dict.model)
-        return dict(model=model, iter_=self._iter)
-
-    def write_state_dict(self, f: pathlib.Path) -> None:
-        self._logger.info(f"Writing state dict to {f}")
-        torch.save(self.state_dict(), f)
-
-    def read_state_dict(self, f: pathlib.Path) -> None:
-        self._logger.info(f"Reading state dict from {f}")
-        self.load_state_dict(torch.load(f, 'cpu'))
+    def state_dict(self, *args, **kwargs) -> dict[str, Any]:
+        state_dict = super().state_dict(*args, **kwargs)
+        state_dict['meta'] = dict(iter_=self._iter)
+        state_dict['model'] = self._strategy.model_state_dict(*args, **kwargs)
+        state_dict['strategy'] = self._strategy.state_dict(*args, **kwargs)
+        state_dict['callbacks'] = self._callbacks.state_dict(*args, **kwargs)
+        return state_dict
 
 
 class Validator(BaseRunner):
 
-    def _before_run(self) -> Memo:
-        self._model.eval()
-        return super()._before_run()
+    def _setup(self) -> Memo:
+        self._strategy.model.eval()
+        return super()._setup()
 
     @torch.no_grad()
     def run(self) -> Memo:
         return super().run()
 
 
 class Trainer(BaseRunner):
 
-    def __init__(
+    @property
+    def optimizer(self) -> torch.optim.Optimizer:
+        return self._optimizer
+
+    def _build_optimizer(
         self,
         *args,
         optimizer: Config,
-        lr_scheduler: Config | None = None,
-        validator: Config | None = None,
         **kwargs,
     ) -> None:
-        super().__init__(*args, **kwargs)
-        self._optimizer = self._build_optimizer(optimizer)
-        self._lr_scheduler = (
-            None if lr_scheduler is None else
-            self._build_lr_scheduler(lr_scheduler)
-        )
-        self._validator: Validator | None = (
-            None if validator is None else RunnerRegistry.build(validator)
-        )
+        self._optimizer = self._strategy.build_optimizer(optimizer)
 
-    def _build_optimizer(self, config: Config) -> torch.optim.Optimizer:
-        return OptimizerRegistry.build(config, Config(model=self.model))
+    def _build(self, *args, **kwargs) -> None:
+        super()._build(*args, **kwargs)
+        self._build_optimizer(*args, **kwargs)
+
+    def _setup(self) -> Memo:
+        self._strategy.model.train()
+        return super()._setup()
+
+    def state_dict(self, *args, **kwargs) -> dict[str, Any]:
+        state_dict = super().state_dict(*args, **kwargs)
+        state_dict['optim'] = self._strategy.optim_state_dict(*args, **kwargs)
+        return state_dict
 
-    def _build_lr_scheduler(
+    def load_state_dict(
         self,
-        config: Config,
-    ) -> torch.optim.lr_scheduler._LRScheduler:
-        return LrSchedulerRegistry.build(config)
-
-    def _after_run_iter(self, batch, memo: Memo) -> None:
-        super()._after_run_iter(batch, memo)
-        loss: torch.Tensor = memo['loss']
-        loss.backward()
-        self._optimizer.step()
-        self._model.zero_grad()
-
-    def _after_run_iter_log(self, batch, memo: Memo) -> str | None:
-        info = super()._after_run_iter_log(batch, memo)
-        if self._lr_scheduler is None:
-            return info
-        last_lr = [f'{lr:.3e}' for lr in self._lr_scheduler.get_last_lr()]
-        info = "" if info is None else f"{info} "
-        info += f"LR {last_lr}"
-        return info
-
-    def _before_run(self) -> Memo:
-        self._model.train()
-        return super()._before_run()
-
-    def _after_run(self, memo: Memo) -> None:
-        super()._after_run(memo)
-        self.validate()
-
-    def validate(self) -> None:
-        if self._validator is None:
-            self._logger.info(
-                "Skipping validation since validator is undefined"
-            )
-            return
-        torch.distributed.barrier()
-        self._validator.run()
-        self._model.train()
-
-    def load_state_dict(self, state_dict: Mapping[str, Any]) -> None:
-        super().load_state_dict(state_dict)
-        self._optimizer.load_state_dict(
-            state_dict['optimizer'],
-            **self._load_state_dict.optimizer,
-        )
-        if self._lr_scheduler is not None:
-            self._lr_scheduler.load_state_dict(
-                state_dict['lr_scheduler'],
-                **self._load_state_dict.lr_scheduler,
-            )
-
-    def state_dict(self) -> dict[str, Any]:
-        state_dict = super().state_dict()
-        state_dict['optimizer'] = self._optimizer.state_dict(
-            **self._state_dict.optimizer,
+        state_dict: Mapping[str, Any],
+        *args,
+        **kwargs,
+    ) -> None:
+        super().load_state_dict(state_dict, *args, **kwargs)
+        self._strategy.load_optim_state_dict(
+            state_dict['optim'],
+            *args,
+            **kwargs,
         )
-        if self._lr_scheduler is not None:
-            state_dict['lr_scheduler'] = self._lr_scheduler.state_dict(
-                **self._state_dict.lr_scheduler,
-            )
-        return state_dict
 
 
 class IterBasedTrainer(Trainer):
 
     def __init__(self, *args, iters: int, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._iters = iters
 
     @property
     def iters(self) -> int:
         return self._iters
 
-    def _after_run_iter(self, batch, memo: Memo) -> None:
-        super()._after_run_iter(batch, memo)
-        if self._iter % self._state_dict.interval == 0:
-            self.validate()
-            self.write_state_dict(self._work_dir / f'iter_{self._iter}.pth')
-        if self._lr_scheduler is not None:
-            self._lr_scheduler.step()
-
-    def _before_run(self) -> Memo:
-        memo = super()._before_run()
-        memo['dataloader'] = itertools.islice(
-            itertools.cycle(memo['dataloader']),
-            self._iters,
-        )
+    def _setup(self) -> Memo:
+        memo = super()._setup()
+        dataloader = memo['dataloader']
+        dataloader = itertools.cycle(dataloader)
+        dataloader = itertools.islice(dataloader, self._iters)
+        memo['dataloader'] = dataloader
         return memo
 
-    def _after_run(self, memo: Memo) -> None:
-        self.write_state_dict(self._work_dir / 'latest.pth')
-        super()._after_run(memo)
-
 
 class EpochBasedTrainer(Trainer):
 
     def __init__(self, *args, epochs: int, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-        self._epoch = 0
         self._epochs = epochs
 
-    def _control_run_epoch(self, memo: Memo) -> Control | None:
-        return None
+        # must be set before _callbacks.connect() to allow loading state dict
+        self._epoch = 0
+
+        super().__init__(*args, **kwargs)
+
+    @property
+    def epoch(self) -> int:
+        return self._epoch
+
+    @property
+    def iters(self) -> int:
+        return super().iters * self._epochs
+
+    @property
+    def epochs(self) -> int:
+        return self._epochs
+
+    def _run_epoch(self, epoch_memo: Memo, memo: Memo) -> Memo:
+        return super()._run(epoch_memo)
 
-    def _before_run_epoch(self, memo: Memo) -> Memo:
+    def _setup_epoch(self, memo: Memo) -> Memo:
         sampler = self._dataloader.batch_sampler
         if sampler is None:
             sampler = self._dataloader.sampler
-        if isinstance(sampler, DistributedSamplerProto):
+        if isinstance(sampler, torch.utils.data.DistributedSampler):
             sampler.set_epoch(self._epoch)
-        return super()._before_run()
+        return super()._setup()
 
-    def _before_run_epoch_log(
-        self,
-        epoch_memo: Memo,
-        memo: Memo,
-    ) -> str | None:
-        return f"Epoch [{self._epoch}/{self._epochs}] beginning"
-
-    def _run_epoch(self, epoch_memo: Memo, memo: Memo) -> None:
-        super()._run(epoch_memo)
-
-    def _after_run_epoch_log(
-        self,
-        epoch_memo: Memo,
-        memo: Memo,
-    ) -> str | None:
-        return f"Epoch [{self._epoch}/{self._epochs}] ended"
-
-    def _after_run_epoch(
-        self,
-        epoch_memo: Memo,
-        memo: Memo,
-    ) -> None:
-        super()._after_run(epoch_memo)
+    def _teardown_epoch(self, epoch_memo: Memo, memo: Memo) -> None:
+        super()._teardown(epoch_memo)
         memo['epoch_memos'][self._epoch] = epoch_memo
-        self.write_state_dict(self._work_dir / f'epoch_{self._epoch}.pth')
-        if self._lr_scheduler is not None:
-            self._lr_scheduler.step()
-
-    def _before_run(self) -> Memo:
-        memo: Memo = dict(epoch_memos=dict())
-        return memo
 
-    def _run(self, memo: Memo) -> None:
+    def _run(self, memo: Memo) -> Memo:
         while self._epoch < self._epochs:
             self._epoch += 1
-            self._iter = 0
+            epoch_memo = self._setup_epoch(memo)
 
-            control = self._control_run_epoch(memo)
-            if control is Control.BREAK:
+            if self._callbacks.should_break_epoch(epoch_memo, memo):
                 break
-            if control is Control.CONTINUE:
+            if self._callbacks.should_continue_epoch(epoch_memo, memo):
                 continue
-            assert control is None, control
-            epoch_memo = self._before_run_epoch(memo)
-            info = self._before_run_epoch_log(epoch_memo, memo)
-            if info is not None:
-                self._logger.info(info)
-            try:
-                self._run_epoch(epoch_memo, memo)
-            except Exception:
-                self._logger.exception(
-                    f"Unable to run epoch {self._epoch}\n{epoch_memo=}\n"
-                    f"{memo=}"
+
+            self._callbacks.before_run_epoch(epoch_memo, memo)
+            with contextlib.ExitStack() as exit_stack:
+                self._callbacks.run_epoch_context(
+                    exit_stack,
+                    epoch_memo,
+                    memo,
                 )
-                raise
-            info = self._after_run_epoch_log(epoch_memo, memo)
-            if info is not None:
-                self._logger.info(info)
-            self._after_run_epoch(epoch_memo, memo)
+                epoch_memo = self._run_epoch(epoch_memo, memo)
+            self._callbacks.after_run_epoch(epoch_memo, memo)
+
+            self._teardown_epoch(epoch_memo, memo)
+        return memo
+
+    def _setup(self) -> Memo:
+        return dict(epoch_memos=dict())
 
-    def _after_run(self, memo: Memo) -> None:
+    def _teardown(self, memo: Memo) -> None:
         pass
 
+    def load_state_dict(
+        self,
+        state_dict: Mapping[str, Any],
+        *args,
+        **kwargs,
+    ) -> None:
+        super().load_state_dict(state_dict, *args, **kwargs)
+        self._epoch = state_dict['meta']['epoch']
 
-class RunnerRegistry(Registry):
-    pass
+    def state_dict(self, *args, **kwargs) -> dict[str, Any]:
+        state_dict = super().state_dict(*args, **kwargs)
+        state_dict['meta']['epoch'] = self._epoch
+        return state_dict
+
+
+class RunnerHolderMixin:
+
+    def __init__(self, *args, runner: BaseRunner, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        runner_proxy = (
+            runner if isinstance(runner, weakref.ProxyTypes) else
+            weakref.proxy(runner)
+        )
+        self._runner = cast(BaseRunner, runner_proxy)
+
+    @property
+    def trainer(self) -> Trainer:
+        assert isinstance(self._runner, Trainer)
+        return self._runner
+
+    @property
+    def validator(self) -> Validator:
+        assert isinstance(self._runner, Validator)
+        return self._runner
+
+    @property
+    def runner(self) -> BaseRunner:
+        return self._runner
+
+    @property
+    def iter_based_trainer(self) -> IterBasedTrainer:
+        assert isinstance(self._runner, IterBasedTrainer)
+        return self._runner
+
+    @property
+    def epoch_based_trainer(self) -> EpochBasedTrainer:
+        assert isinstance(self._runner, EpochBasedTrainer)
+        return self._runner
```

### Comparing `todd_ai-0.3.0/todd/visuals/base.py` & `todd_ai-0.4.0/todd/visuals/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 __all__ = [
     'XAnchor',
     'YAnchor',
     'BaseVisual',
-    'VisualRegistry',
 ]
 
 import enum
 from abc import ABC, abstractmethod
 from typing import Any, NamedTuple
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 import torch
 
-from ..base import Registry
-
 
 class Color(NamedTuple):
     red: float
     green: float
     blue: float
 
 
@@ -226,11 +223,7 @@
         text_ = self.text(
             text,
             left,
             top,
             color=color,
         )
         return (rectangle, text_)
-
-
-class VisualRegistry(Registry):
-    pass
```

### Comparing `todd_ai-0.3.0/todd/visuals/cv2.py` & `todd_ai-0.4.0/todd/visuals/cv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from typing import cast
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 
-from .base import BaseVisual, Color, VisualRegistry, XAnchor, YAnchor
+from ..base import VisualRegistry
+from .base import BaseVisual, Color, XAnchor, YAnchor
 
 
 @VisualRegistry.register()
 class CV2Visual(BaseVisual):
 
     def __init__(self, width: int, height: int) -> None:
         self._image = np.zeros((height, width, 3))
```

### Comparing `todd_ai-0.3.0/todd/visuals/pptx.py` & `todd_ai-0.4.0/todd/visuals/pptx.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import pptx.presentation
 import pptx.shapes.autoshape
 import pptx.shapes.picture
 import pptx.shapes.shapetree
 import pptx.slide
 import pptx.util
 
-from .base import BaseVisual, Color, VisualRegistry, XAnchor, YAnchor
+from ..base import VisualRegistry
+from .base import BaseVisual, Color, XAnchor, YAnchor
 
 
 @VisualRegistry.register()
 class PPTXVisual(BaseVisual):
     """Visualize data in the format of PowerPoint.
 
     The PowerPoint contains only one slide.
```

### Comparing `todd_ai-0.3.0/todd_ai.egg-info/PKG-INFO` & `todd_ai-0.4.0/todd_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todd-ai
-Version: 0.3.0
+Version: 0.4.0
 Summary: Toolkit for Object Detection Distillation
 Author-email: Luting Wang <wangluting@buaa.edu.cn>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

