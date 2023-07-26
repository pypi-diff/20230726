# Comparing `tmp/pyppbox-3.1b1.tar.gz` & `tmp/pyppbox-3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.1b1.tar", last modified: Mon Jul 24 18:37:58 2023, max compression
+gzip compressed data, was "pyppbox-3.1b2.tar", last modified: Wed Jul 26 21:54:02 2023, max compression
```

## Comparing `pyppbox-3.1b1.tar` & `pyppbox-3.1b2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-24 18:37:43.000000 pyppbox-3.1b1/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 18:37:43.000000 pyppbox-3.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 18:37:43.000000 pyppbox-3.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-24 18:37:58.935798 pyppbox-3.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-24 18:37:43.000000 pyppbox-3.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-24 18:37:43.000000 pyppbox-3.1b1/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    65550 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.919798 pyppbox-3.1b1/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.927797 pyppbox-3.1b1/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.931798 pyppbox-3.1b1/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/standalone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51396 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/standalone/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26550 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.923797 pyppbox-3.1b1/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 18:37:58.000000 pyppbox-3.1b1/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-24 18:37:43.000000 pyppbox-3.1b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:37:58.935798 pyppbox-3.1b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 18:37:43.000000 pyppbox-3.1b1/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:37:58.935798 pyppbox-3.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-24 18:37:43.000000 pyppbox-3.1b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 18:37:43.000000 pyppbox-3.1b1/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-26 21:53:46.000000 pyppbox-3.1b2/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 21:53:46.000000 pyppbox-3.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 21:53:46.000000 pyppbox-3.1b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-26 21:54:02.751511 pyppbox-3.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-26 21:53:46.000000 pyppbox-3.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-07-26 21:53:46.000000 pyppbox-3.1b2/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/cfg.7z
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65085 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.727511 pyppbox-3.1b2/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.739511 pyppbox-3.1b2/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   833181 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23388 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.743511 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.747511 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51191 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/standalone/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25586 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.735511 pyppbox-3.1b2/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 21:54:02.000000 pyppbox-3.1b2/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 21:53:46.000000 pyppbox-3.1b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:54:02.751511 pyppbox-3.1b2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-26 21:53:46.000000 pyppbox-3.1b2/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:54:02.751511 pyppbox-3.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-26 21:53:46.000000 pyppbox-3.1b2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 21:53:46.000000 pyppbox-3.1b2/setup_extra.yaml
```

### Comparing `pyppbox-3.1b1/GETSTARTED.md` & `pyppbox-3.1b2/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/LICENSE` & `pyppbox-3.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/PKG-INFO` & `pyppbox-3.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.1b1
+Version: 3.1b2
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -45,10 +45,10 @@
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
-* Support YAML/JSON configurations -> File, raw string and ready dictionary.
+* Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.1b1/README.md` & `pyppbox-3.1b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
-* Support YAML/JSON configurations -> File, raw string and ready dictionary.
+* Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.1b1/RELEASENOTES.md` & `pyppbox-3.1b2/RELEASENOTES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 # Release Notes 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.1b2](https://github.com/rathaumons/pyppbox/tree/v3.1b2)
+
+  - Improve all supported trackers
+  - Improve evatools
+  - Change some default configurations
+  - Update and improve examples
+  - Improve documentations
+  - **Known issue/limitation**: 
+    - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
+
 * `pyppbox` [v3.1b1](https://github.com/rathaumons/pyppbox/tree/v3.1b1)
 
   - Add multithreading support for standalone -> `ppbox.standalone.mt.MT`
   - Add multithreading example -> See example 13
   - Add CPU support for `Torchreid`
   - Implement install requirements/dependencies -> See setup.py
   - Simplify and improve requirements
   - Update default config files
   - Update and improve documentations
   - Update and improve GUI
+  - **Known issue/limitation**: 
+    - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
 
 * `pyppbox` [v3.0b5](https://github.com/rathaumons/pyppbox/tree/v3.0b5)
 
   - Fix a critical bug in GUI of FaceNet which can cause missing `train_data` configuration
   - Fix and improve documentation
   - **Known issue/limitation**: 
     - [Issue] YOLO Ultralytics: May throw `CUDA error: an illegal memory access was encountered` in multithread application
```

### Comparing `pyppbox-3.1b1/pyppbox/__init__.py` & `pyppbox-3.1b2/pyppbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.1b1'
+__version__ = '3.1b2'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.1b1/pyppbox/config/__init__.py` & `pyppbox-3.1b2/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.1b2/pyppbox/config/cfg/detectors.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 model_image_size: 416
 repspoint_calibration: 0.25
 ---
 dt_name: YOLO_Ultralytics
 conf: 0.5
 iou: 0.7
 imgsz: 416
-boxes: True
+boxes: False
 device: 0
 max_det: 100
 line_width: 500
 model_file: data/modules/yolo_ultralytics/yolov8l-pose.pt
 repspoint_calibration: 0.25
 ---
 dt_name: GT
```

### Comparing `pyppbox-3.1b1/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.1b2/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.1b2/pyppbox/config/cfg/trackers.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###########################################################
 # Tracker config:
 ###########################################################
 # --- # Centroid
 # tk_name: Centroid
-# max_spread: 50
+# max_spread: 64
 ###########################################################
 # --- # SORT
 # tk_name: SORT
 # max_age: 1
 # min_hits: 3
 # iou_threshold: 0.3
 ###########################################################
@@ -15,15 +15,15 @@
 # tk_name: DeepSORT
 # nn_budget: 100
 # nms_max_overlap: 0.5
 # max_cosine_distance: 0.1
 # model_file: data/modules/deepsort/mars-small128.pb
 ###########################################################
 tk_name: Centroid
-max_spread: 50
+max_spread: 64
 ---
 tk_name: SORT
 max_age: 1
 min_hits: 3
 iou_threshold: 0.3
 ---
 tk_name: DeepSORT
```

### Comparing `pyppbox-3.1b1/pyppbox/config/configtools.py` & `pyppbox-3.1b2/pyppbox/config/configtools.py`

 * *Files 14% similar despite different names*

```diff
@@ -133,21 +133,21 @@
         self.cfg_dir = cfg_dir
         self.setYAMLPath()
 
 
 #########################################################################################
 
 
-def isRawYAMLString(input_string):
-    """Check whether the :obj:`input_string` is a valid YAML/JSON dictionary.
+def isDictString(input_string):
+    """Check whether the :obj:`input_string` is a valid raw dictionary.
 
     Parameters
     ----------
     input_string : str
-        An input of YAML/JSON string.
+        An input of raw string.
 
     Returns
     -------
     bool
         Validation status.
     """
     res = True
@@ -164,73 +164,73 @@
         except ValueError as e:
             res = False
     else:
         res = False
     return res
 
 def getCFGDict(input):
-    """Get a YAML/JSON dictionary of a single document from the given :obj:`input`.
+    """Get a configuration dictionary of a single document from the given :obj:`input`.
 
     Parameters
     ----------
     input : str or dict
-        A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+        A YAML/JSON file path, or a raw/ready dictionary.
 
     Returns
     -------
     dict
-        A YAML/JSON dictionary of a single document.
+        A configuration dictionary of a single document.
     """
     doc = {}
     if isinstance(input, str):
         if ".yaml" in input.lower() or ".json" in input.lower():
             doc = loadDocument(getAbsPathFDS(input))
         else:
             doc = loadRawYAMLString(input)
     elif isinstance(input, dict):
         doc = input
     return doc
 
 def getListCFGDoc(input):
-    """Get a list of YAML/JSON dictionary of document from the given :obj:`input`.
+    """Get a list of configuration dictionary of document from the given :obj:`input`.
 
     Parameters
     ----------
     input : str or dict
-        A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+        A YAML/JSON file path, or a raw/ready dictionary.
 
     Returns
     -------
-    list[dict{}, ...]
-        A list of YAML/JSON dictionary.
+    list[dict, ...]
+        A list of configuration dictionary.
     """
     doc_list = []
     if isinstance(input, str):
         if ".yaml" in input.lower():
             doc_list = loadListDocument(getAbsPathFDS(input))
         else:
             doc_list = loadRawYAMLStringMT(input)
     elif isinstance(input, dict):
         for doc in input:
             doc_list.append(doc)
     return doc_list
 
 def loadDocument(yaml_json):
-    """Return a YAML/JSON dictionary of a single document from the given file 
+    """Return a configuration dictionary of a single document from the given file 
     :obj:`yaml_json`.
 
     Parameters
     ----------
     yaml_json : str
         A path of a YAML/JSON file.
 
     Returns
     -------
     dict
-        A YAML/JSON dictionary of a single document.
+        A configuration dictionary of a single document.
     """
     document = {}
     if isExist(yaml_json):
         with open(yaml_json, 'rb') as cfg:
             try:
                 if '.json' in yaml_json.lower():
                     document = json.load(cfg)
@@ -243,25 +243,25 @@
     else:
         msg = "loadDocument() -> " + str(yaml_json) + "' does not exist!"
         add_error_log(msg)
         raise ValueError(msg)
     return document
 
 def loadListDocument(yaml_json):
-    """Return a list of YAML/JSON dictionary from the given file :obj:`yaml_json`.
+    """Return a list of configuration dictionary from the given file :obj:`yaml_json`.
 
     Parameters
     ----------
     yaml_json : str
         A path of a YAML/JSON file.
     
     Returns
     -------
-    list[dict{}, ...]
-        A list of YAML/JSON dictionary.
+    list[dict, ...]
+        A list of configuration dictionary.
     """
     document_list = []
     if isExist(yaml_json):
         with open(yaml_json, 'rb') as cfg:
             try:
                 if '.json' in yaml_json.lower():
                     docs = json.load(cfg)
@@ -276,27 +276,27 @@
     else:
         msg = "loadListDocument() -> " + str(yaml_json) + "' does not exist!"
         add_error_log(msg)
         raise ValueError(msg)
     return document_list
 
 def loadRawYAMLString(raw_string):
-    """Return a YAML/JSON dictionary of a single document from the given string 
+    """Return a configuration dictionary of a single document from the given string 
     :obj:`raw_string`.
 
     Parameters
     ----------
     raw_string : str
         A raw string of JSON or YAML; for example, 
         :code:`raw_string="[{'tk_name': 'SORT'}]"`.
     
     Returns
     -------
     dict
-        A YAML/JSON dictionary of a single document.
+        A configuration dictionary of a single document.
     """
     document = {}
     try:
         d = yaml.load(raw_string, Loader=SafeLoader)
         document = next(iter(d))
     except ValueError as e:
         msg = 'loadRawYAMLString() -> ' + str(e)
@@ -311,38 +311,38 @@
     ----------
     raw_string : str
         A raw string of JSON or YAML; for example, 
         :code:`raw_string="[{'tk_name': 'SORT'}, {'tk_name': 'DeepSORT'}]"`.
     
     Returns
     -------
-    list[dict{}, ...]
-        A list of YAML/JSON dictionary.
+    list[dict, ...]
+        A list of configuration dictionary.
     """
     document_list = []
     try:
         ds = yaml.load_all(raw_string, Loader=SafeLoader)
         for d in ds:
             document_list.append(d)
     except ValueError as e:
         msg = 'loadRawYAMLStringMT() -> ' + str(e)
         add_error_log(msg)
         raise ValueError(msg)
     return document_list
 
 def dumpDocDict(output_file, doc, header):
-    """Dump a YAML/JSON dictionary of a single document into a YAML file 
+    """Dump a configuration dictionary of a single document into a YAML file 
     with simple format.
 
     Parameters
     ----------
     output_file : str
         A path file to dump.
     doc : dict
-        A YAML/JSON dictionary of a single document.
+        A configuration dictionary of a single document.
     header : str
         A file header descriptoin.
     """
     try:
         with open(output_file, 'w') as dumping:
             dumping.write(header)
             for key, value in doc.items():
@@ -355,16 +355,16 @@
 def dumpListDocDict(output_file, doc_list, header):
     """Dump a list of YAML dictionary into a YAML file with simple format.
 
     Parameters
     ----------
     output_file : str
         A path file to dump.
-    doc_list : list[dict{}, ...]
-        A list of YAML/JSON dictionary.
+    doc_list : list[dict, ...]
+        A list of configuration dictionary.
     header : str
         A file header descriptoin.
     """
     try: 
         with open(output_file, 'w') as dumping:
             dumping.write(header)
             sep_index = 1
```

### Comparing `pyppbox-3.1b1/pyppbox/config/myconfig.py` & `pyppbox-3.1b2/pyppbox/config/myconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,39 +45,39 @@
     An base CFG class used to store the necessary configurations of a module.
 
     Attributes
     ----------
     unified_strings : MyStrings, auto
         A :class:`MyStrings` object used to store unified strings.
     configs : dict or list[dict], default={}
-        A YAML/JSON dictionary of a single document or a list of multiple documents 
+        A configuration dictionary of a single document or a list of multiple documents 
         of the configurations.
     """
 
     def __init__(self):
         self.unified_strings = unified_strings
         self.configs = {}
     
     def loadDoc(self, input):
         """Load and set dictionary of a single document from a YAML/JSON file or string.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         self.configs = getCFGDict(input)
     
     def loadDocs(self, input):
         """Load and set a list of multiple documents from a YAML/JSON file or string.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         self.configs = getListCFGDoc(input)
     
     def dumpDoc(self, output, header=""):
         """Dump the :attr:`configs` into a YAML file with simple format.
 
         Parameters
@@ -159,15 +159,15 @@
     def set(self, input):
         """
         Set main configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.detector = self.unified_strings.getUnifiedFormat(self.configs['detector'])
                 self.tracker = self.unified_strings.getUnifiedFormat(self.configs['tracker'])
                 self.reider = self.unified_strings.getUnifiedFormat(self.configs['reider'])
@@ -176,21 +176,21 @@
                 msg = "MainCFG : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("MainCFG : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the parameters of the 
+        """Return a configuration dictionary of a single document of the parameters of the 
         main configurations.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         main_doc = {
             "detector": self.detector,
             "tracker": self.tracker,
             "reider": self.reider,
         }
         return main_doc
@@ -251,15 +251,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.dt_name = self.unified_strings.getUnifiedFormat(self.configs['dt_name'])
                 self.nms = self.configs['nms']
                 self.conf = self.configs['conf']
@@ -277,21 +277,21 @@
                 msg = "DCFGYOLOCLS : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("DCFGYOLOCLS : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of detector YOLO Classic.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         yolocs_doc = {
             "dt_name": self.dt_name,
             "nms": self.nms,
             "conf": self.conf,
             "class_file": normalizePathFDS(internal_root_dir, self.class_file),
             "model_cfg_file": normalizePathFDS(internal_root_dir, self.model_cfg_file),
@@ -358,15 +358,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.dt_name = self.unified_strings.getUnifiedFormat(self.configs['dt_name'])
                 self.conf = self.configs['conf']
                 self.iou = self.configs['iou']
@@ -383,21 +383,21 @@
                 msg = "DCFGYOLOULT : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("DCFGYOLOULT : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return yolout_doc, a YAML/JSON dictionary of a single document of the attributes which 
+        """Return yolout_doc, a configuration dictionary of a single document of the attributes which 
         are the parameters of detector YOLO_Ultralytics.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         yolout_doc = {
             "dt_name": self.dt_name,
             "conf": self.conf,
             "iou": self.iou,
             "imgsz": self.imgsz,
             "boxes": self.boxes,
@@ -452,15 +452,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.dt_name = self.unified_strings.getUnifiedFormat(self.configs['dt_name'])
                 self.gt_file = getAdaptiveAbsPathFDS(self.from_dir, self.configs['gt_file'])
                 self.gt_map_file = getAdaptiveAbsPathFDS(self.from_dir, self.configs['gt_map_file'])
@@ -469,21 +469,21 @@
                 msg = "DCFGGT : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("DCFGGT : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of detector GT (Ground-truth).
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         gt_doc = {
             "dt_name": self.dt_name,
             "gt_file": normalizePathFDS(internal_root_dir, self.gt_file),
             "gt_map_file": normalizePathFDS(internal_root_dir, self.gt_map_file)
         }
         return gt_doc
@@ -505,15 +505,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.tk_name = self.unified_strings.getUnifiedFormat(self.configs['tk_name'])
                 self.max_spread = self.configs['max_spread']
                 self.configs = self.getDocument()
@@ -521,21 +521,21 @@
                 msg = "TCFGCentroid : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("TCFGCentroid : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of tracker Centroid.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         centroid_doc = {
             "tk_name": self.tk_name,
             "max_spread": self.max_spread
         }
         return centroid_doc
 
@@ -560,15 +560,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.tk_name = self.unified_strings.getUnifiedFormat(self.configs['tk_name'])
                 self.max_age = self.configs['max_age']
                 self.min_hits = self.configs['min_hits']
@@ -579,21 +579,21 @@
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("TCFGSORT : set() -> The configuration is empty.")
 
     def getDocument(self):
         """
-        Return a YAML/JSON dictionary of a single document of the attributes which 
+        Return a configuration dictionary of a single document of the attributes which 
         are the parameters of tracker SORT.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         sort_doc = {
             "tk_name": self.tk_name,
             "max_age": self.max_age,
             "min_hits": self.min_hits,
             "iou_threshold": self.iou_threshold
         }
@@ -645,15 +645,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.tk_name = self.unified_strings.getUnifiedFormat(self.configs['tk_name'])
                 self.nn_budget = self.configs['nn_budget']
                 self.nms_max_overlap = self.configs['nms_max_overlap']
@@ -664,21 +664,21 @@
                 msg = "TCFGDeepSORT : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("TCFGDeepSORT : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of tracker DeepSORT.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         deepsort_doc = {
             "tk_name": self.tk_name,
             "nn_budget": self.nn_budget,
             "nms_max_overlap": self.nms_max_overlap,
             "max_cosine_distance": self.max_cosine_distance,
             "model_file": normalizePathFDS(internal_root_dir, self.model_file)
@@ -749,15 +749,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 self.ri_name = self.unified_strings.getUnifiedFormat(self.configs['ri_name'])
                 self.gpu_mem = self.configs['gpu_mem']
                 self.model_det = getAdaptiveAbsPathFDS(self.from_dir, self.configs['model_det'])
@@ -773,21 +773,21 @@
                 msg = "RCFGFaceNet : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("RCFGFaceNet : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of reider FaceNet.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         facenet_doc = {
             "ri_name": self.ri_name,
             "gpu_mem": self.gpu_mem,
             "model_det": normalizePathFDS(internal_root_dir, self.model_det), 
             "model_file": normalizePathFDS(internal_root_dir, self.model_file),
             "classifier_pkl": normalizePathFDS(internal_root_dir, self.classifier_pkl),
@@ -860,15 +860,15 @@
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
         Parameters
         ----------
         input : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary.
+            A YAML/JSON file path, or a raw/ready dictionary.
         """
         super().loadDoc(input)
         if self.configs:
             try:
                 from pyppbox.modules.reiders.torchreid.model_dict import TorchreidModelDict
                 self.ri_name = self.unified_strings.getUnifiedFormat(self.configs['ri_name'])
                 self.classifier_pkl = getAdaptiveAbsPathFDS(self.from_dir, 
@@ -891,21 +891,21 @@
                 msg = "RCFGTorchreid : set() -> " + str(e)
                 add_error_log(msg)
                 raise ValueError(msg)
         else:
             add_warning_log("RCFGTorchreid : set() -> The configuration is empty.")
 
     def getDocument(self):
-        """Return a YAML/JSON dictionary of a single document of the attributes which 
+        """Return a configuration dictionary of a single document of the attributes which 
         are the parameters of reider Torchreid.
 
         Returns
         -------
         dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         torchreid_doc = {
             "ri_name": self.ri_name,
             "classifier_pkl": normalizePathFDS(internal_root_dir, self.classifier_pkl),
             "train_data": normalizePathFDS(internal_root_dir, self.train_data),
             "model_name": self.model_name,
             "model_path": normalizePathFDS(internal_root_dir, self.model_path),
@@ -986,15 +986,15 @@
             Header string for trackers.yaml file.
         """
         header=("###########################################################\n"
                 "# Tracker config:\n"
                 "###########################################################\n"
                 "# --- # Centroid\n"
                 "# tk_name: Centroid\n"
-                "# max_spread: 50\n"
+                "# max_spread: 64\n"
                 "###########################################################\n"
                 "# --- # SORT\n"
                 "# tk_name: SORT\n"
                 "# max_age: 1\n"
                 "# min_hits: 3\n"
                 "# iou_threshold: 0.3\n"
                 "###########################################################\n"
@@ -1144,17 +1144,17 @@
     def setMCFG(self, main_yaml=None):
         """Load and set the main configurations which used to identify the main 
         detector/tracker/reider.
 
         Parameters
         ----------
         main_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary 
-            of the main configurations or main.yaml. This :obj:`main_yaml` helps overwrite 
-            the original one configured during the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the main configurations 
+            or main.yaml. This :obj:`main_yaml` helps overwrite the original one configured 
+            during the :meth:`__init__()`.
             Leave it as default :code:`main_yaml=None`, to load and set according to the 
             configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         """
         self.mcfg = MainCFG()
         if main_yaml is None:
             self.mcfg.set(self.main_yaml)
         else:
@@ -1162,17 +1162,17 @@
     
     def setMainModules(self, main_yaml=None):
         """Call :meth:`setMCFG()` and then load and set the main detector/tracker/reider accordingly.
 
         Parameters
         ----------
         main_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary 
-            of the main configurations or main.yaml. This :obj:`main_yaml` helps overwrite 
-            the original one configured during the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the main configurations 
+            or main.yaml. This :obj:`main_yaml` helps overwrite the original one configured 
+            during the :meth:`__init__()`.
             Leave it as default :code:`main_yaml=None`, to load and set according to the 
             configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         """
         self.setMCFG(main_yaml=main_yaml)
         selected_dt = self.mcfg.configs['detector']
         dt_list = loadListDocument(self.detectors_yaml)
         for dt in dt_list:
@@ -1194,19 +1194,19 @@
     
     def setGTCFG(self, detectors_yaml=None, relative_to_pyppbox_root=None):
         """Manually load and set the configurations for :attr:`dcfg_gt`.
 
         Parameters
         ----------
         detectors_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of 
-            the detectors' configurations or detectors.yaml. This :obj:`detectors_yaml` helps 
-            overwrite the original one configured during the :meth:`__init__()`. Leave it as 
-            default :code:`detectors_yaml=None`, to load and set according to the configurations 
-            inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the detectors' configurations 
+            or detectors.yaml. This :obj:`detectors_yaml` helps overwrite the original one 
+            configured during the :meth:`__init__()`. 
+            Leave it as default :code:`detectors_yaml=None`, to load and set according to the 
+            configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         relative_to_pyppbox_root : bool, default=None
             An indication of whether the paths inside your configuration file are relative 
             to :code:`{pyppbox root}` or not. This indication or behavior was automatically 
             decided during the :meth:`__init__()`, and you don't need to set or change it 
             unless you set :obj:`detectors_yaml` to overwrite the original configurations. If 
             all the paths inside your configuration file have full absolute paths, setting 
             :obj:`relative_to_pyppbox_root` is optional.
@@ -1235,19 +1235,19 @@
 
     def setAllDCFG(self, detectors_yaml=None, relative_to_pyppbox_root=None):
         """Load and set the configurations for all supported detectors.
 
         Parameters
         ----------
         detectors_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of 
-            the detectors' configurations or detectors.yaml. This :obj:`detectors_yaml` helps 
-            overwrite the original one configured during the :meth:`__init__()`. Leave it as 
-            default :code:`detectors_yaml=None`, to load and set according to the configurations 
-            inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the detectors' configurations 
+            or detectors.yaml. This :obj:`detectors_yaml` helps overwrite the original one 
+            configured during the :meth:`__init__()`. 
+            Leave it as default :code:`detectors_yaml=None`, to load and set according to the 
+            configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         relative_to_pyppbox_root : bool, default=None
             An indication of whether the paths inside your configuration file are relative 
             to :code:`{pyppbox root}` or not. This indication or behavior was automatically 
             decided during the :meth:`__init__()`, and you don't need to set or change it 
             unless you set :obj:`detectors_yaml` to overwrite the original configurations. If 
             all the paths inside your configuration file have full absolute paths, setting 
             :obj:`relative_to_pyppbox_root` is optional.
@@ -1292,19 +1292,19 @@
 
     def setAllTCFG(self, trackers_yaml=None, relative_to_pyppbox_root=None):
         """Load and set the configurations for all supported trackers.
 
         Parameters
         ----------
         trackers_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of 
-            the trackers' configurations or trackers.yaml. This :obj:`trackers_yaml` helps 
-            overwrite the original one configured during the :meth:`__init__()`. Leave it as 
-            default :code:`trackers_yaml=None`, to load and set according to the configurations 
-            inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the trackers' configurations 
+            or trackers.yaml. This :obj:`trackers_yaml` helps overwrite the original one 
+            configured during the :meth:`__init__()`. 
+            Leave it as default :code:`trackers_yaml=None`, to load and set according to the 
+            configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         relative_to_pyppbox_root : bool, default=None
             An indication of whether the paths inside your configuration file are relative 
             to :code:`{pyppbox root}` or not. This indication or behavior was automatically 
             decided during the :meth:`__init__()`, and you don't need to set or change it 
             unless you set :obj:`trackers_yaml` to overwrite the original configurations. If 
             all the paths inside your configuration file have full absolute paths, setting 
             :obj:`relative_to_pyppbox_root` is optional.
@@ -1348,19 +1348,19 @@
 
     def setAllRCFG(self, reiders_yaml=None, relative_to_pyppbox_root=None):
         """Load and set the configurations for all reiders.
 
         Parameters
         ----------
         reiders_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of 
-            the reiders' configurations or reiders.yaml. This :obj:`reiders_yaml` helps 
-            overwrite the original one configured during the :meth:`__init__()`. Leave it as 
-            default :code:`reiders_yaml=None`, to load and set according to the configurations 
-            inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
+            A YAML/JSON file path, or a raw/ready dictionary of the reiders' configurations or 
+            reiders.yaml. This :obj:`reiders_yaml` helps overwrite the original one configured 
+            during the :meth:`__init__()`. 
+            Leave it as default :code:`reiders_yaml=None`, to load and set according to the 
+            configurations inside config directory :attr:`cfg_dir` set in the :meth:`__init__()`.
         relative_to_pyppbox_root : bool, default=None
             An indication of whether the paths inside your configuration file are relative 
             to :code:`{pyppbox root}` or not. This indication or behavior was automatically 
             decided during the :meth:`__init__()`, and you don't need to set or change it 
             unless you set :obj:`reiders_yaml` to overwrite the original configurations. If 
             all the paths inside your configuration file have full absolute paths, setting 
             :obj:`relative_to_pyppbox_root` is optional.
@@ -1399,16 +1399,16 @@
     def setASupportedModuleCFG(self, input_cfg, relative_to_pyppbox_root=False):
         """Load and set configurations for a supported module. Be aware that calling 
         this method will overwrite the original or previous configurations.
 
         Parameters
         ----------
         input_cfg: str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary 
-            of the configurations of a supported module.
+            A YAML/JSON file path, or a raw/ready dictionary of the configurations 
+            of a supported module.
         relative_to_pyppbox_root : bool, defualt=False
             An indication of whether the paths inside the given :obj:`input_cfg` are 
             relative to :code:`{pyppbox root}` or not. 
         """
         cfg = getCFGDict(input_cfg)
         k_list = list(input_cfg.keys())
         if "dt_name" in k_list:
@@ -1469,28 +1469,27 @@
     def addAnAbstractCFG(self, input_cfg):
         """Add the configurations for an anbstract or unsupported module as a :class:`BaseCGF` 
         object and add it to the independent config list :attr:`abstractCFGs`.
 
         Parameters
         ----------
         input_cfg : str or dict
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary 
-            of the configurations of a module.
+            A YAML/JSON file path, or a raw/ready dictionary of the configurations of a module.
         """
         tmpCFG = BaseCGF()
         tmpCFG.loadDoc(input_cfg)
         self.abstractCFGs.append(tmpCFG)
 
     def dumpMainCFG(self, document):
         """Dump the main configurations to main.yaml.
 
         Parameters
         ----------
         document : dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         dumpDocDict(self.main_yaml, document, self.cfg_headers.mainHeader())
 
     def dumpAllDCFG(self, document_list):
         """Dump the detectors' configurations to detectors.yaml.
 
         Parameters
```

### Comparing `pyppbox-3.1b1/pyppbox/config/unifiedstrings.py` & `pyppbox-3.1b2/pyppbox/config/unifiedstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,33 +90,33 @@
         ----------
         strings_yaml : str, default='{pyppbox root}/config/strings/strings.yaml'
             A path of a YAML file which stores the unified strings.
         """
         self.load(strings_yaml=strings_yaml)
 
     def load(self, strings_yaml): 
-        """Load a YAML/JSON dictionary of a single document as a dictionary from 
+        """Load a configuration dictionary of a single document as a dictionary from 
         a :obj:`strings_yaml` file and automatically pass to :meth:`set()`.
 
         Parameters
         ----------
         strings_yaml : str
             A path of a YAML file which stores the unified strings.
         """
         with open(strings_yaml, 'r') as str_cfg:
             self.data = yaml.load(str_cfg, Loader=SafeLoader)
         self.set(self.data)
 
     def set(self, data):
-        """Set a YAML/JSON dictionary of a single document to all attributes.
+        """Set a configuration dictionary of a single document to all attributes.
 
         Parameters
         ----------
         data : dict
-            A YAML/JSON dictionary of a single document of the unified strings.
+            A configuration dictionary of a single document of the unified strings.
         """
         # module
         self.none = data['none']
         self.detector = data['detector']
         self.tracker = data['tracker']
         self.reider = data['reider']
         # detector
```

### Comparing `pyppbox-3.1b1/pyppbox/gui/__init__.py` & `pyppbox-3.1b2/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/assets/TReID.png` & `pyppbox-3.1b2/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/assets/icon.ico` & `pyppbox-3.1b2/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/assets/settings.ico` & `pyppbox-3.1b2/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/guidemo.py` & `pyppbox-3.1b2/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/guihub.py` & `pyppbox-3.1b2/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/guitools.py` & `pyppbox-3.1b2/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_centroid.py` & `pyppbox-3.1b2/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.1b2/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_facenet.py` & `pyppbox-3.1b2/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_gt.py` & `pyppbox-3.1b2/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_launcher.py` & `pyppbox-3.1b2/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_sort.py` & `pyppbox-3.1b2/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.1b2/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.1b2/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.1b2/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,18 @@
         min_width_filter : int, default=35
             Mininum width filter of a detected object.
 
         Returns
         -------
         Mat
             A cv :obj:`Mat` image.
-        list[ndarray[int int int int], ...]
-            A list of bounding box :code:`ndarray[x y width height]`.
-        list[ndarray[int int int int], ...]
-            A list of bounding box :code:`ndarray[x1 y1 x2 y2]`.
+        list[ndarray[int, int, int, int], ...]
+            A list of bounding box :code:`ndarray[x, y, width, height]`.
+        list[ndarray[int, int, int, int], ...]
+            A list of bounding box :code:`ndarray[x1, y1, x2, y2]`.
         list[tuple(int, int)]
             A lsit of represented 2D point :code:`(x, y)` of every detected object.
         float
             A list of the detection confidence of every detected object.
         """
         pboxes_xywh = []
         pboxes_xyxy = []
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,21 @@
         min_width_filter : int, default=35
             Mininum width filter of a detected object.
 
         Returns
         -------
         Mat
             A cv :obj:`Mat` image.
-        list[ndarray[int int int int], ...]
-            A list of bounding box :code:`ndarray[x y width height]`.
-        list[ndarray[int int int int], ...]
-            A list of bounding box :code:`ndarray[x1 y1 x2 y2]`.
+        list[ndarray[int, int, int, int], ...]
+            A list of bounding box :code:`ndarray[x, y, width, height]`.
+        list[ndarray[int, int, int, int], ...]
+            A list of bounding box :code:`ndarray[x1, y1, x2, y2]`.
         list[tuple(int, int)]
             A lsit of represented 2D point :code:`(x, y)` of every detected object.
-        list[ndarray[int]]
+        list[ndarray[int, ...], ...]
             A list of :obj:`ndarray` of body keypoints. 
         float
             A list of the detection confidence of every detected object.
         """
         numpy_dets = []
         pboxes_xyxy = []
         pboxes_xywh = []
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 import numpy as np
 
 from pyppbox.utils.commontools import getFileName, silencer
 from pyppbox.utils.logtools import add_info_log, add_warning_log, ignore_this_logger
 
 ignore_this_logger("tensorflow")
 ignore_this_logger("facenet")
+ignore_this_logger("skimage")
+ignore_this_logger("scipy")
+
+import warnings
+warnings.filterwarnings("ignore", module="skimage", category=RuntimeWarning) 
+warnings.filterwarnings("ignore", module="scipy", category=RuntimeWarning) 
 
 import tensorflow as tf
 tf.autograph.set_verbosity(1)
 
 from .origin import facenet as fn
 from .origin import detect_face as df
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 # Upated on 07/03/2022 by Ratha Siv
 
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from scipy import misc
 import imageio
 import skimage.transform
 import sys
 import os
 import argparse
 import tensorflow as tf
 import numpy as np
@@ -125,15 +124,14 @@
                                 det = np.squeeze(det)
                                 bb = np.zeros(4, dtype=np.int32)
                                 bb[0] = np.maximum(det[0]-args.margin/2, 0)
                                 bb[1] = np.maximum(det[1]-args.margin/2, 0)
                                 bb[2] = np.minimum(det[2]+args.margin/2, img_size[1])
                                 bb[3] = np.minimum(det[3]+args.margin/2, img_size[0])
                                 cropped = img[bb[1]:bb[3],bb[0]:bb[2],:]
-                                #scaled = misc.imresize(cropped, (args.image_size, args.image_size), interp='bilinear')
                                 scaled = skimage.transform.resize(cropped, (args.image_size, args.image_size), anti_aliasing=True)
                                 nrof_successfully_aligned += 1
                                 filename_base, file_extension = os.path.splitext(output_filename)
                                 if args.detect_multiple_faces:
                                     output_filename_n = "{}_{}{}".format(filename_base, i, file_extension)
                                 else:
                                     output_filename_n = "{}{}".format(filename_base, file_extension)
@@ -141,15 +139,14 @@
                                 text_file.write('%s %d %d %d %d\n' % (output_filename_n, bb[0], bb[1], bb[2], bb[3]))
                         else:
                             print('Unable to align "%s"' % image_path)
                             text_file.write('%s\n' % (output_filename))
                             
     print('Total number of images: %d' % nrof_images_total)
     print('Number of successfully aligned images: %d' % nrof_successfully_aligned)
-            
 
 def parse_arguments(argv):
     parser = argparse.ArgumentParser()
     
     parser.add_argument('input_dir', type=str, help='Directory with unaligned images.')
     parser.add_argument('output_dir', type=str, help='Directory with aligned face thumbnails.')
     parser.add_argument('--image_size', type=int,
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def set(self, mcfg):
         """Set attributes according to the input :obj:`mcfg`.
 
         Parameters
         ----------
         mcfg : dict
-            A YAML/JSON dictionary of a single document of the configurations.
+            A configuration dictionary of a single document of the configurations.
         """
         self.name = mcfg['name']
         self.arch = mcfg['arch']
         self.height = mcfg['height']
         self.width = mcfg['width']
         self.model_files = mcfg['model_files']
 
@@ -68,15 +68,15 @@
 
     """
     A class used to store a dictionary for mapping name, arch, height, width, pretrained files, and base files of Torchreid models.
 
     Attributes
     ----------
     raw_model : dict, auto
-        A YAML/JSON dictionary of a single document of the Torchreid model configurations.
+        A configuration dictionary of a single document of the Torchreid model configurations.
     model_list : list[TorchreidModel, ...], auto
         A list of all :class:`TorchreidModel` objects.
     """
 
     def __init__(self, model_dict_yaml=default_model_dict_yaml):
         """Initailize and set attributes according to model_dict_yaml.
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.1b2/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/sort/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,62 +15,73 @@
 #                                                                           #
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
-from math import hypot
-from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.utils.persontools import Person
-from pyppbox.utils.logtools import add_error_log
+from pyppbox.utils.logtools import add_error_log, ignore_this_logger
 
+ignore_this_logger("sort")
 
-__ustrings__ = UnifiedStrings()
+from .origin.sort import Sort
 
-class MyCentroid(object):
+
+class MySORT(object):
+
+    """Class used as a custom layer or interface for interacting with SORT tracker.
+    """
 
     def __init__(self, cfg):
         """Initialize according to the given :obj:`cfg` and :obj:`auto_load`.
 
         Parameters
         ----------
-        cfg : TCFGCentroid
-            A :class:`TCFGCentroid` object which manages the configurations of tracker Centroid.
+        cfg : TCFGSORT
+            A :class:`TCFGDeepSORT` object which manages the configurations of tracker SORT.
         """
-        self.max_spread = cfg.max_spread
+        self.st = Sort(cfg.max_age, cfg.min_hits, cfg.iou_threshold)
         self.previous_list = []
         self.current_list = []
 
-    def __getDist__(self, p1, p2):
-        dist = 0.0
-        (x1, y1) = p1
-        (x2, y2) = p2
-        dist = hypot(x2 - x1, y2 - y1)
-        return dist
-    
-    def __getIndexFromPreviousList__(self, point):
+
+    def __getIndexFromSORTTracks__(self, box_xyxy, sort_tracks, max_spread=128):
+        track_index = -1
+        updated_cid = -1
+        box_list = box_xyxy.tolist()
+        tracks_list = sort_tracks.tolist()
+        spread_list = []
+
+        if len(box_list) > 0 and len(tracks_list) > 0:
+            for b in tracks_list:
+                max_spread = -1
+                for i in range(0, 4):
+                    sub_spread = abs(box_list[i] - b[i])
+                    if sub_spread > max_spread:
+                        max_spread = sub_spread
+                spread_list.append(max_spread)
+            
+            if len(spread_list) > 0:
+                sm_spread = min(spread_list)
+                if sm_spread <= max_spread:
+                    track_index = spread_list.index(sm_spread)
+                    updated_cid = int(tracks_list[track_index][4])
+
+        return track_index, updated_cid
+
+
+    def __getIndexFromPreviousList__(self, cid):
         pindex = -1
-        dist_list = []
-        if len(self.previous_list) > 0:
-            for p in self.previous_list:
-                dist_list.append(self.__getDist__(point, p.repspoint))
-            min_dist = min(dist_list)
-            if min_dist <= self.max_spread:
-                pindex = dist_list.index(min_dist)
+        for i in range(0, len(self.previous_list)):
+            if cid == self.previous_list[i].cid:
+                pindex = i
+                break
         return pindex
 
-    def __getAnAvailableID__(self, usedIDs): 
-        if len(usedIDs) == 0: usedIDs.append(-1)
-        aID = max(usedIDs) + 1
-        pIDs = [p.cid for p in self.previous_list]
-        aIDs = list(set(usedIDs) ^ set(pIDs))
-        aIDs = list(set(aIDs) - set(usedIDs))
-        if len(aIDs) > 0: aID = sorted(aIDs)[0]
-        return aID
 
     def update(self, person_list, img=None):
         """Update the tracker and return the updated list of :class:`Person`.
 
         Parameters
         ----------
         person_list : list[Person, ...]
@@ -84,42 +95,23 @@
             The updated list of :class:`Person` object.
         """
         self.previous_list = self.current_list
         self.current_list = []
 
         if len(person_list) > 0:
             if isinstance(person_list[0], Person):
-                self.current_list = person_list
-                hang_indexes_in_clist = []
-                used_cids = []
-                len_clist = len(self.current_list)
-
-                if len_clist > 0:
-                    for i in range(0, len_clist):
-                        pindex = self.__getIndexFromPreviousList__(self.current_list[i].repspoint)
+                self.current_list = self.st.update_pyppbox(person_list)
+                for i in range (0, len(self.current_list)):
+                    if len(self.previous_list) > 0:
+                        pindex = self.__getIndexFromPreviousList__(self.current_list[i].cid)
                         if pindex >= 0:
-                            prev_cid = self.previous_list[pindex].cid
-                            if prev_cid in used_cids:
-                                hang_indexes_in_clist.append(i)
-                            else:
-                                self.current_list[i].updateIDs(
-                                    prev_cid, 
-                                    self.previous_list[pindex].faceid, 
-                                    self.previous_list[pindex].deepid,
-                                    self.previous_list[pindex].faceid_conf,
-                                    self.previous_list[pindex].deepid_conf
-                                )
-                                used_cids.append(prev_cid)
-                        else:
-                            hang_indexes_in_clist.append(i)
-                    
-                    len_hlist = len(hang_indexes_in_clist)
-                    if len_hlist > 0:
-                        for index in hang_indexes_in_clist:
-                            self.current_list[index].cid = self.__getAnAvailableID__(used_cids)
+                            self.current_list[i].faceid = self.previous_list[pindex].faceid
+                            self.current_list[i].deepid = self.previous_list[pindex].deepid
+                            self.current_list[i].faceid_conf = self.previous_list[pindex].faceid_conf
+                            self.current_list[i].deepid_conf = self.previous_list[pindex].deepid_conf
             else:
-                msg = ("MyCentroid : update() -> The element of input 'person_list' " + 
-                       "list has unsupported type.")
+                msg = ("MySORT : update() -> The element of input 'person_list' list " + 
+                       "has unsupported type.")
                 add_error_log(msg)
                 raise ValueError(msg)
 
         return self.current_list
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 import numpy as np
 
-from pyppbox.config.unifiedstrings import UnifiedStrings
 from pyppbox.utils.persontools import Person
 from pyppbox.utils.logtools import add_error_log, ignore_this_logger
 
 ignore_this_logger("tensorflow")
 ignore_this_logger("preprocessing")
 ignore_this_logger("nn_matching")
 ignore_this_logger("generate_detections")
@@ -35,69 +34,63 @@
 from .origin import preprocessing
 from .origin import nn_matching
 from .origin import generate_detections as gdet
 from .origin.detection import Detection as DSDetection
 from .origin.tracker import Tracker as DSTracker
 
 
-__ustrings__ = UnifiedStrings()
-
 class MyDeepSORT(object):
 
+    """Class used as a custom layer or interface for interacting with DeepSORT tracker.
+    """
 
     def __init__(self, cfg):
         """Initialize according to the given :obj:`cfg` and :obj:`auto_load`.
 
         Parameters
         ----------
         cfg : TCFGDeepSORT
             A :class:`TCFGDeepSORT` object which manages the configurations of tracker DeepSORT.
         """
         self.previous_list = []
         self.current_list = []
         self.current_frame = 0
         self.nms_max_overlap = cfg.nms_max_overlap
-        self.encoder = gdet.create_box_encoder(cfg.model_file, batch_size=1)
+        self.encoder = gdet.create_box_encoder(cfg.model_file, batch_size=16)
         self.metric = nn_matching.NearestNeighborDistanceMetric("cosine", cfg.max_cosine_distance, 
                                                                 cfg.nn_budget)
         self.tracker = DSTracker(self.metric)
 
 
-    def __getCurrentIndexByBoxXYXY__(self, box, max_spread=50):
+    def __getCurrentIndexByBoxXYXY__(self, box, max_spread=128):
         index = -1
         box_list = box.tolist()
-        spread_list = []
-
+        min_box_spread = 8192
+        i = 0
         for p in self.current_list:
-            max_spread = -1
             pbbox_list = p.box_xyxy.tolist()
-            for i in range(0, 4):
-                sub_spread = abs(box_list[i] - pbbox_list[i])
-                if sub_spread > max_spread:
-                    max_spread = sub_spread
-            spread_list.append(max_spread)
-        
-        if len(spread_list) > 0:
-            sm_spread = min(spread_list)
-            if sm_spread <= max_spread:
-                index = spread_list.index(sm_spread)
-        
+            max_ss = max([abs(box_list[j] - pbbox_list[j]) for j in range(0, 4)])
+            if max_ss < min_box_spread:
+                min_box_spread = max_ss
+                index = i
+            i += 1
+        if min_box_spread > max_spread: index = -1
         return index
 
 
     def __getIndexFromPreviousList__(self, cid):
         pindex = -1
         for i in range(0, len(self.previous_list)):
             if cid == self.previous_list[i].cid:
                 pindex = i
                 break
         return pindex
 
 
-    def update(self, person_list, img=None, max_spread=5):
+    def update(self, person_list, img=None, max_spread=128):
         """Update the tracker and return the updated list of :class:`Person`.
 
         Parameters
         ----------
         person_list : list[Person, ...]
             A list of :class:`Person` object which stores the detected people in the given :obj:`img`.
         img : any, default=None
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,123 +15,104 @@
 #                                                                           #
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
-import numpy as np
-
-from pyppbox.config.unifiedstrings import UnifiedStrings
+from math import hypot
 from pyppbox.utils.persontools import Person
-from pyppbox.utils.logtools import add_error_log, ignore_this_logger
-
-ignore_this_logger("sort")
-
-from .origin.sort import Sort
+from pyppbox.utils.logtools import add_error_log
 
 
-__ustrings__ = UnifiedStrings()
-
-class MySORT(object):
+class MyCentroid(object):
 
+    """Class reprensented a Centroid tracker.
+    """
 
     def __init__(self, cfg):
         """Initialize according to the given :obj:`cfg` and :obj:`auto_load`.
 
         Parameters
         ----------
-        cfg : TCFGSORT
-            A :class:`TCFGDeepSORT` object which manages the configurations of tracker SORT.
+        cfg : TCFGCentroid
+            A :class:`TCFGCentroid` object which manages the configurations of tracker Centroid.
         """
-        self.st = Sort(cfg.max_age, cfg.min_hits, cfg.iou_threshold)
+        self.max_spread = cfg.max_spread
         self.previous_list = []
         self.current_list = []
 
-
-    def __getIndexFromSORTTracks__(self, box_xyxy, sort_tracks, max_spread=50):
-        track_index = -1
-        updated_cid = -1
-        box_list = box_xyxy.tolist()
-        tracks_list = sort_tracks.tolist()
-        spread_list = []
-
-        if len(box_list) > 0 and len(tracks_list) > 0:
-            for b in tracks_list:
-                max_spread = -1
-                for i in range(0, 4):
-                    sub_spread = abs(box_list[i] - b[i])
-                    if sub_spread > max_spread:
-                        max_spread = sub_spread
-                spread_list.append(max_spread)
-            
-            if len(spread_list) > 0:
-                sm_spread = min(spread_list)
-                if sm_spread <= max_spread:
-                    track_index = spread_list.index(sm_spread)
-                    updated_cid = int(tracks_list[track_index][4])
-
-        return track_index, updated_cid
-
-
-    def __getIndexFromPreviousList__(self, cid):
+    def __generateID__(self):
+        self.used_cids = list(set(self.used_cids))
+        if len(self.used_cids) == 0: aID = 0
+        else: aID = max(self.used_cids) + 1
+        self.used_cids.append(aID)
+        return aID
+    
+    def __findPID__(self, point):
         pindex = -1
-        for i in range(0, len(self.previous_list)):
-            if cid == self.previous_list[i].cid:
+        min_dist = 8192
+        i = 0
+        for p in self.previous_list:
+            dist = hypot(p.repspoint[0] - point[0], 
+                         p.repspoint[1] - point[1])
+            if dist < min_dist:
+                min_dist = dist
                 pindex = i
-                break
+            i += 1
+        if min_dist > self.max_spread: pindex = -1
         return pindex
 
-
-    def update(self, person_list, img=None, max_spread=5):
+    def update(self, person_list, img=None):
         """Update the tracker and return the updated list of :class:`Person`.
 
         Parameters
         ----------
         person_list : list[Person, ...]
             A list of :class:`Person` object which stores the detected people in the given :obj:`img`.
         img : any, default=None
             Being consistent with other trackers, will be ignored.
-        max_spread : int, default=5
-            Max spread or max margin used to decide whether 2 bounding boxes are the same by comparing 
-            the differences between the elements in the bounding box given by the embedded SORT and the 
-            coressponding elements of a person's bounding box in the :obj:`person_list`.
 
         Returns
         -------
         list[Person, ...]
             The updated list of :class:`Person` object.
         """
         self.previous_list = self.current_list
         self.current_list = []
+        self.used_cids = []
 
         if len(person_list) > 0:
             if isinstance(person_list[0], Person):
                 self.current_list = person_list
-
-                dets = np.empty((0, 5))
-                for i in range(0, len(person_list)):
-                    row = np.append(person_list[i].box_xyxy, 0).reshape(1, 5)
-                    dets = np.append(dets, row, axis=0)
-
-                sort_tracks = self.st.update(dets)
-                for i in range (0, len(self.current_list)):
-                    track_index, updated_cid = self.__getIndexFromSORTTracks__(
-                        self.current_list[i].box_xyxy, sort_tracks, 
-                        max_spread=max_spread
-                    )
-                    if track_index >= 0:
-                        self.current_list[i].cid = updated_cid
-                        if len(self.previous_list) > 0:
-                            pindex = self.__getIndexFromPreviousList__(updated_cid)
-                            if pindex >= 0:
-                                self.current_list[i].faceid = self.previous_list[pindex].faceid
-                                self.current_list[i].deepid = self.previous_list[pindex].deepid
-                                self.current_list[i].faceid_conf = self.previous_list[pindex].faceid_conf
-                                self.current_list[i].deepid_conf = self.previous_list[pindex].deepid_conf
+                hang_indexes_in_clist = []
+                len_clist = len(self.current_list)
+                if len_clist > 0:
+                    for i in range(0, len_clist):
+                        pindex = self.__findPID__(self.current_list[i].repspoint)
+                        if pindex >= 0:
+                            prev_cid = self.previous_list[pindex].cid
+                            if prev_cid in self.used_cids:
+                                hang_indexes_in_clist.append(i)
+                            else:
+                                self.current_list[i].updateIDs(
+                                    prev_cid, 
+                                    self.previous_list[pindex].faceid, 
+                                    self.previous_list[pindex].deepid,
+                                    self.previous_list[pindex].faceid_conf,
+                                    self.previous_list[pindex].deepid_conf
+                                )
+                                self.used_cids.append(prev_cid)
+                                # self.previous_list.pop(pindex)
+                        else:
+                            hang_indexes_in_clist.append(i)
+                    len_hlist = len(hang_indexes_in_clist)
+                    if len_hlist > 0:
+                        for index in hang_indexes_in_clist:
+                            self.current_list[index].cid = self.__generateID__()
             else:
-                msg = ("MySORT : update() -> The element of input 'person_list' list " + 
-                       "has unsupported type.")
+                msg = ("MyCentroid : update() -> The element of input 'person_list' " + 
+                       "list has unsupported type.")
                 add_error_log(msg)
                 raise ValueError(msg)
 
         return self.current_list
```

### Comparing `pyppbox-3.1b1/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.1b2/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,22 +28,25 @@
 from skimage import io
 
 import glob
 import time
 import argparse
 from filterpy.kalman import KalmanFilter
 
+import lap
+# from scipy.optimize import linear_sum_assignment
+
 np.random.seed(0)
 
 
 def linear_assignment(cost_matrix):
   try:
-    import lap
+    # import lap
     _, x, y = lap.lapjv(cost_matrix, extend_cost=True)
-    return np.array([[y[i],i] for i in x if i >= 0]) #
+    return np.array([[y[i],i] for i in x if i >= 0])
   except ImportError:
     from scipy.optimize import linear_sum_assignment
     x, y = linear_sum_assignment(cost_matrix)
     return np.array(list(zip(x, y)))
 
 
 def iou_batch(bb_test, bb_gt):
@@ -100,15 +103,16 @@
   count = 0
   def __init__(self,bbox):
     """
     Initialises a tracker using initial bounding box.
     """
     #define constant velocity model
     self.kf = KalmanFilter(dim_x=7, dim_z=4) 
-    self.kf.F = np.array([[1,0,0,0,1,0,0],[0,1,0,0,0,1,0],[0,0,1,0,0,0,1],[0,0,0,1,0,0,0],  [0,0,0,0,1,0,0],[0,0,0,0,0,1,0],[0,0,0,0,0,0,1]])
+    self.kf.F = np.array([[1,0,0,0,1,0,0],[0,1,0,0,0,1,0],[0,0,1,0,0,0,1],[0,0,0,1,0,0,0],
+                          [0,0,0,0,1,0,0],[0,0,0,0,0,1,0],[0,0,0,0,0,0,1]])
     self.kf.H = np.array([[1,0,0,0,0,0,0],[0,1,0,0,0,0,0],[0,0,1,0,0,0,0],[0,0,0,1,0,0,0]])
 
     self.kf.R[2:,2:] *= 10.
     self.kf.P[4:,4:] *= 1000. #give high uncertainty to the unobservable initial velocities
     self.kf.P *= 10.
     self.kf.Q[-1,-1] *= 0.01
     self.kf.Q[4:,4:] *= 0.01
@@ -149,21 +153,21 @@
   def get_state(self):
     """
     Returns the current bounding box estimate.
     """
     return convert_x_to_bbox(self.kf.x)
 
 
-def associate_detections_to_trackers(detections,trackers,iou_threshold = 0.3):
+def associate_detections_to_trackers(detections, trackers, iou_threshold=0.3):
   """
   Assigns detections to tracked object (both represented as bounding boxes)
 
   Returns 3 lists of matches, unmatched_detections and unmatched_trackers
   """
-  if(len(trackers)==0):
+  if len(trackers) == 0:
     return np.empty((0,2),dtype=int), np.arange(len(detections)), np.empty((0,5),dtype=int)
 
   iou_matrix = iou_batch(detections, trackers)
 
   if min(iou_matrix.shape) > 0:
     a = (iou_matrix > iou_threshold).astype(np.int32)
     if a.sum(1).max() == 1 and a.sum(0).max() == 1:
@@ -195,14 +199,15 @@
   else:
     matches = np.concatenate(matches,axis=0)
 
   return matches, np.array(unmatched_detections), np.array(unmatched_trackers)
 
 
 class Sort(object):
+
   def __init__(self, max_age=1, min_hits=3, iou_threshold=0.3):
     """
     Sets key parameters for SORT
     """
     self.max_age = max_age
     self.min_hits = min_hits
     self.iou_threshold = iou_threshold
@@ -235,29 +240,97 @@
 
     # update matched trackers with assigned detections
     for m in matched:
       self.trackers[m[1]].update(dets[m[0], :])
 
     # create and initialise new trackers for unmatched detections
     for i in unmatched_dets:
-        trk = KalmanBoxTracker(dets[i,:])
-        self.trackers.append(trk)
+      trk = KalmanBoxTracker(dets[i,:])
+      self.trackers.append(trk)
     i = len(self.trackers)
     for trk in reversed(self.trackers):
-        d = trk.get_state()[0]
-        if (trk.time_since_update < 1) and (trk.hit_streak >= self.min_hits or self.frame_count <= self.min_hits):
-          ret.append(np.concatenate((d,[trk.id+1])).reshape(1,-1)) # +1 as MOT benchmark requires positive
-        i -= 1
-        # remove dead tracklet
-        if(trk.time_since_update > self.max_age):
-          self.trackers.pop(i)
-    if(len(ret)>0):
+      d = trk.get_state()[0]
+      if (trk.time_since_update < 1) and (trk.hit_streak >= self.min_hits or self.frame_count <= self.min_hits):
+        ret.append(np.concatenate((d,[trk.id+1])).reshape(1,-1)) # +1 as MOT benchmark requires positive
+      i -= 1
+      # remove dead tracklet
+      if(trk.time_since_update > self.max_age):
+        self.trackers.pop(i)
+    if len(ret) > 0:
       return np.concatenate(ret)
     return np.empty((0,5))
 
+
+  def update_pyppbox(self, current_people):
+    """
+    Similar to update(). Made for pyppbox's Person list.
+    """    
+    self.frame_count += 1
+
+    people_trackers = []
+    updated_people = []
+
+    dets = np.empty((0, 5))
+    for i in range(0, len(current_people)):
+      row = current_people[i].getDetRS()
+      dets = np.append(dets, row, axis=0)
+
+    # get predicted locations from existing trackers.
+    trks = np.zeros((len(self.trackers), 5))
+    to_del = []
+    ret = []
+    for t, trk in enumerate(trks):
+      pos = self.trackers[t].predict()[0]
+      trk[:] = [pos[0], pos[1], pos[2], pos[3], 0]
+      if np.any(np.isnan(pos)):
+        to_del.append(t)
+    trks = np.ma.compress_rows(np.ma.masked_invalid(trks))
+    for t in reversed(to_del):
+      self.trackers.pop(t)
+
+    matched, unmatched_dets, unmatched_trks = associate_detections_to_trackers(dets, trks, self.iou_threshold)
+
+    # Example:
+    """
+    matched = [[0 2]
+               [1 1]
+               [2 3]
+               [3 4]
+               [4 0]]
+    # Meaning: matched[i] = [det_index, track_index]
+    """
+    # update matched trackers with assigned detections
+    for m in matched:
+      self.trackers[m[1]].update(dets[m[0],:])
+      p = current_people[m[0]]
+      p.cid = self.trackers[m[1]].id
+      # print(p.__print_self__())
+      people_trackers.append([p, m[1]])
+
+    # create and initialise new trackers for unmatched detections
+    for u in unmatched_dets:
+      trk = KalmanBoxTracker(dets[u,:])
+      self.trackers.append(trk)
+      if u < len(current_people):
+        p = current_people[u]
+        p.cid = trk.id
+        # print(p.__print_self__())
+        people_trackers.append([p, len(self.trackers) - 1])
+
+    for pp_trk in people_trackers:
+      trk = self.trackers[pp_trk[1]]
+      if (trk.time_since_update < 1) and (trk.hit_streak >= self.min_hits or self.frame_count <= self.min_hits):
+        updated_people.append(pp_trk[0])
+      # remove dead tracklet
+      if(trk.time_since_update > self.max_age):
+        self.trackers.pop(pp_trk[1])
+
+    return updated_people
+
+
 def parse_args():
     """Parse input arguments."""
     parser = argparse.ArgumentParser(description='SORT demo')
     parser.add_argument('--display', dest='display', help='Display online tracker output (slow) [False]',action='store_true')
     parser.add_argument("--seq_path", help="Path to detections.", type=str, default='data')
     parser.add_argument("--phase", help="Subdirectory in seq_path.", type=str, default='train')
     parser.add_argument("--max_age",
```

### Comparing `pyppbox-3.1b1/pyppbox/standalone/__init__.py` & `pyppbox-3.1b2/pyppbox/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/standalone/mt.py` & `pyppbox-3.1b2/pyppbox/standalone/mt.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pyppbox.utils.logtools import add_info_log, add_warning_log, add_error_log
 
 # Common
 import cv2
 from collections import Counter
 
 # Configurations
-from pyppbox.config.configtools import isRawYAMLString, getCFGDict
+from pyppbox.config.configtools import isDictString, getCFGDict
 from pyppbox.config.myconfig import (
     MyConfigurator, NoneCFG,
     DCFGYOLOCLS, DCFGYOLOULT, DCFGGT, 
     TCFGCentroid, TCFGSORT, TCFGDeepSORT, 
     RCFGFaceNet, RCFGTorchreid, 
 )
 
@@ -194,18 +194,18 @@
         """Load and set the main detector, the main tracker, and the main reider all at once 
         according to the given main configurations, :obj:`main_yaml`. If the :func:`setConfigDir()` 
         has not yet been called, internal config directory will be used.
 
         Parameters
         ----------
         main_yaml : str or dict, default=None
-            A YAML/JSON file path, a raw YAML/JSON string, or ready YAML/JSON dictionary of the 
-            main configurations or main.yaml. This :obj:`main_yaml` helps overwrite the original one 
-            configured earlier. Leave it as default :obj:`main_yaml=None`, to load and set according 
-            to the configurations in the config directory.
+            A YAML/JSON file path, or a raw/ready dictionary of the main configurations or main.yaml. 
+            This :obj:`main_yaml` helps overwrite the original one configured earlier. 
+            Leave it as default :obj:`main_yaml=None`, to load and set according to the configurations 
+            in the config directory.
         load_all : bool, default=True
             Set :code:`load_all=True` to set and load the selected detector/tracker/reider according 
             to the main configurations, which it is meant for using this :func:`setMainModules()` method.
             Set :code:`load_all=False` to select and load a detector/tracker/reider manually later.
         """
         if not self.__cfg_is_set__: self.setConfigDir()
         self.__cfg__.setMainModules(main_yaml=main_yaml)
@@ -337,43 +337,42 @@
                 add_info_log("---PYPPBOX : Set detector='" + self.__dt_cfg__.dt_name + "'")
             else: 
                 self.__dt_is_set__ = False
                 add_warning_log("---PYPPBOX : detector='" + detector_dict['dt_name'] + 
                                 "' is not recognized.")
 
     def setMainDetector(self, detector=""):
-        """Set the main detector by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-        is optional. Different from the rest, setting the main detector by its name results 
-        in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-        If :func:`setConfigDir()` has not been called before, setting the main detector by a supported 
-        name results in referencing the internal config directory in order to load the 
-        corresponding configurations. 
+        """Set the main detector by a supported name, a raw/ready dictionary, or a YAML/JSON file. 
+        Calling :func:`setConfigDir()` before :func:`setMainTracker()` is optional. Different from 
+        the rest, setting the main detector by its name results in loading the configurations from 
+        the config directory set by the last :func:`setConfigDir()`. If :func:`setConfigDir()` has 
+        not been called before, setting the main detector by a supported name results in referencing 
+        the internal config directory in order to load the corresponding configurations. 
 
         Parameters
         ----------
         detector : str or dict, default=""
             (1) Set :code:`detector=""` to set the main detector according to the main configurations 
             or main.yaml and load its configurations from the detectors.yaml. 
             (2) Set :code:`detector="YOLO_Classic"`.etc, to set YOLO Classic as the main detector and 
             load its configurations from detectors.yaml.
-            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            (3) Set a raw string or ready dictionary is also possible; for example, 
             :code:`detector="[{'dt_name': 'YOLO_Ultralytics', 'conf': 0.5, 'iou': 0.7, 'imgsz': 416, 
             'boxes': True, 'device': 0, 'max_det': 100, 'line_width': 500, 
             'model_file': 'data/modules/yolo_ultralytics/yolov8l-pose.pt', 
             'repspoint_calibration': 0.25}]"`.
             (4) Set :code:`detector="a_supported_detector.yaml"` or :code:`detector="a_supported_detector.json"` 
             to set the main detector and its configuration from a YAML file. 
         """
         self.__dt_is_set__ = False
         self.__dt__ = []
         if isinstance(detector, dict):
             self.__setCustomDetector__(detector)
         elif isinstance(detector, str):
-            if (isRawYAMLString(detector) or "yaml" in detector.lower() or 
+            if (isDictString(detector) or "yaml" in detector.lower() or 
                 "json" in detector.lower()):
                 self.__setCustomDetector__(getCFGDict(detector))
             elif detector.lower() == "":
                 if not self.__cfg_is_set__: self.setConfigDir()
                 self.__loadDefaultDetector__()
                 add_info_log("---PYPPBOX : Use detector according to the \"main.yaml\"")
             elif detector.lower() == self.__unistrings__.yolo_cls:
@@ -523,40 +522,39 @@
                 add_info_log("---PYPPBOX : Set tracker='" + self.__tk_cfg__.tk_name + "'")
             else:
                 self.__tk_is_set__ = False
                 add_warning_log("---PYPPBOX : tracker='" + tracker_dict['tk_name'] + 
                                 "' is not recognized")
 
     def setMainTracker(self, tracker=""):
-        """Set the main tracker by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-        is optional. Different from the rest, setting the main tracker by its name results 
-        in loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-        If :func:`setConfigDir()` has not been called before, setting the main tracker by a supported 
-        name results in referencing the internal config directory in order to load the 
-        corresponding configurations. 
+        """Set the main tracker by a supported name, a raw/ready dictionary, or a YAML/JSON file. 
+        Calling :func:`setConfigDir()` before :func:`setMainTracker()` is optional. Different from 
+        the rest, setting the main tracker by its name results in loading the configurations from 
+        the config directory set by the last :func:`setConfigDir()`. If :func:`setConfigDir()` has 
+        not been called before, setting the main tracker by a supported name results in referencing 
+        the internal config directory in order to load the corresponding configurations. 
 
         Parameters
         ----------
         tracker : str or dict, default=""
             (1) Set :code:`tracker=""` to set the main tracker according to the main configurations or 
             main.yaml and load its configurations from the trackers.yaml. 
             (2) Set :code:`tracker="Centroid"`.etc, to set Centroid as the main tracker and load its 
             configurations from trackers.yaml.
-            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            (3) Set a raw string or ready dictionary is also possible; for example, 
             :code:`tracker="[{'tk_name': 'SORT', 'max_age': 1, 'min_hits': 3, 'iou_threshold': 0.3}]"`.
             (4) Set :code:`tracker="a_supported_tracker.yaml"` or :code:`tracker="a_supported_tracker.json"` 
             to set the main tracker and its configuration from a YAML file. 
         """
         self.__tk_is_set__ = False
         self.__tk__ = []
         if isinstance(tracker, dict):
             self.__setCustomTracker__(tracker)
         elif isinstance(tracker, str):
-            if (isRawYAMLString(tracker) or "yaml" in tracker.lower() or 
+            if (isDictString(tracker) or "yaml" in tracker.lower() or 
                 "json" in tracker.lower()):
                 self.__setCustomTracker__(getCFGDict(tracker))
             elif tracker.lower() == "default":
                 if not self.__cfg_is_set__: self.setConfigDir()
                 self.__loadDefaultTracker__()
                 add_info_log("---PYPPBOX : Use tracker according to the \"main.yaml\"")
             elif tracker.lower() == self.__unistrings__.centroid:
@@ -689,35 +687,34 @@
                 self.__revokeGTDTOnly__()
             else :
                 self.__ri_is_set__ = False
                 add_warning_log("---PYPPBOX : reider='" + reider_dict['ri_name'] + 
                                 "' is not recognized")
 
     def setMainReIDer(self, reider="", auto_load=True):
-        """Set the main reider by a supported name, a raw YAML/JSON string, a ready YAML/JSON 
-        dictionary, or a YAML/JSON file. Calling :func:`setConfigDir()` before :func:`setMainTracker()` 
-        is optional. Different from the rest, setting the main reider by its name results in 
-        loading the configurations from the config directory set by the last :func:`setConfigDir()`. 
-        If :func:`setConfigDir()` has not been called before, setting the main reider by a supported 
-        name results in referencing the internal config directory in order to load the 
-        corresponding configurations. 
+        """Set the main reider by a supported name, a raw/ready dictionary, or a YAML/JSON file. 
+        Calling :func:`setConfigDir()` before :func:`setMainTracker()` is optional. Different from 
+        the rest, setting the main reider by its name results in loading the configurations from the 
+        config directory set by the last :func:`setConfigDir()`. If :func:`setConfigDir()` has not 
+        been called before, setting the main reider by a supported name results in referencing the 
+        internal config directory in order to load the corresponding configurations. 
 
         Parameters
         ----------
         reider : str or dict, default=""
             (1) Set :code:`reider=""` to set the main reider according to the main configurations 
             or main.yaml and load its configurations from the reiders.yaml. 
             (2) Set :code:`reider="FaceNet"`.etc, to set FaceNet as a reider and load its 
             configurations from reiders.yaml.
-            (3) Set a raw JSON string or a ready JSON dictionary is also possible; for example, 
+            (3) Set a raw string or ready dictionary is also possible; for example, 
             :code:`reider="[{'ri_name': 'Torchreid', 
             'classifier_pkl': 'data/modules/torchreid/classifier/gta5_osnet_ain_ms_d_c.pkl', 
             'train_data': 'data/datasets/GTA_V_DATASET/body_128x256', 'model_name': 'osnet_ain_x1_0', 
             'model_path': 'data/modules/torchreid/models/torchreid/osnet_ain_ms_d_c.pth.tar', 
-            'min_confidence': 0.35}]"`.
+            'min_confidence': 0.35, 'device': 'cuda'}]"`.
             (4) Set :code:`reider="a_supported_reider.yaml"` or :code:`reider="a_supported_reider.json"` 
             to set a the main reider and its configurations from a YAML file. 
         auto_load : bool, default=True
             All supported reiders are Pytorch or Tensorflow based module, thus they need to 
             initial and load their models/weights. :obj:`auto_load` is used to decide whether to 
             load the reider automatically once the reider is set. Keep the :code:`auto_load=True` 
             if it is meant for using :func:`reidPeople()`; however, even if the :code:`auto_load=False`, 
@@ -725,15 +722,15 @@
             some time to do so.
         """
         self.__ri_is_set__ = False
         self.__ri__ = []
         if isinstance(reider, dict):
             self.__setCustomReIDer__(reider, auto_load)
         elif isinstance(reider, str):
-            if (isRawYAMLString(reider) or "yaml" in reider.lower() or 
+            if (isDictString(reider) or "yaml" in reider.lower() or 
                 "json" in reider.lower()):
                 self.__setCustomReIDer__(getCFGDict(reider), auto_load)
             elif reider.lower() == "default":
                 if not self.__cfg_is_set__: self.setConfigDir()
                 self.__loadDefaultReIDer__(auto_load=auto_load)
                 add_info_log("---PYPPBOX : Use reider according to the \"main.yaml\"")
             elif reider.lower() == self.__unistrings__.facenet:
@@ -943,16 +940,16 @@
     def trainReIDClassifier(self, reider="Default", train_data="", classifier_pkl=""):
         """Train classifier of a reider by pointing to a data directory. Calling 
         :func:`setConfigDir()` or :func:`setMainReIDer()` in advance is not required.
 
         Parameters
         ----------
         reider : str or dict, default="Default" 
-            A supported name, a raw YAML/JSON string, a ready YAML/JSON dictionary, or a 
-            YAML/JSON file which is passed to :func:`setMainReIDer(reider=reider, auto_load=False)`.
+            A supported name, a raw/ready dictionary, or a YAML/JSON file which is passed to 
+            :func:`setMainReIDer(reider=reider, auto_load=False)`.
         train_data : str, default=""
             A path of data to train, where consists of 2 or more sub-folders which classify 
             2 or more people. Set :code:`train_data=""` or keep default to use the configured 
             :obj:`train_data` according to the input :code:`reider`. All images in this the sub-folders 
             must be 128x256 for Torchreid and 182x182 for FaceNet.
         classifier_pkl : str, default=""
             A file path for the classifier PKL file. Set :code:`classifier_pkl=""` or keep default
```

### Comparing `pyppbox-3.1b1/pyppbox/utils/__init__.py` & `pyppbox-3.1b2/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/utils/commontools.py` & `pyppbox-3.1b2/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/utils/evatools.py` & `pyppbox-3.1b2/pyppbox/utils/evatools.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 #                                                                           #
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
+import timeit
+
 from .gttools import GTInterpreter, convertStringToNPL
 from .commontools import joinFPathFull, getAbsPathFDS, isExist, getAncestorDir
 from .logtools import add_info_log, add_warning_log, add_error_log
 
 
 class MyEVA(object):
 
@@ -173,30 +175,30 @@
         fault_detect = 0
         tmp = len(gt_frame) - len(people_dt)
         i = 0
         if tmp >= 0:
             missed_detect = tmp
             for i in range(0, len(people_dt)):
                 person_index_to_compare = findPersonIndexGTFrame(gt_frame, people_dt[i].box_xyxy, 
-                                                                 max_spread_limit=15)
+                                                                 max_spread_limit=16)
                 if person_index_to_compare >= 0:
                     tmp_deepid = people_dt[i].deepid
                     if '%' in tmp_deepid: tmp_deepid = tmp_deepid[:-4]
                     if gt_frame[person_index_to_compare][2].lower() != tmp_deepid.lower():
                         msg = ("-------EVA : Frame \t@" + str(self.current_frame) + 
                                "\t   ---------->   (GT) " + str(gt_frame[person_index_to_compare][2]) + 
                                "\t -v.s- \t " + str(tmp_deepid))
                         add_info_log(msg)
                         diff_count += 1
                 else: fault_detect += 1
         else:
             fault_detect = abs(tmp)
             for i in range(0, len(gt_frame)):
                 person_index_to_compare = findPersonIndexGTFrame(gt_frame, people_dt[i].box_xyxy, 
-                                                                 max_spread_limit=15)
+                                                                 max_spread_limit=16)
                 if person_index_to_compare >= 0:
                     tmp_deepid = people_dt[i].deepid
                     if '%' in tmp_deepid: tmp_deepid = tmp_deepid[:-4]
                     if gt_frame[person_index_to_compare][2].lower() != tmp_deepid.lower():
                         msg = ("-------EVA : Frame \t@" + str(self.current_frame) + 
                                "\t   ---------->   (GT) " + str(gt_frame[person_index_to_compare][2]) + 
                                "\t -v.s- \t " + str(tmp_deepid))
@@ -211,30 +213,30 @@
         fault_detect = 0
         tmp = len(gt_frame) - len(people_dt)
         i = 0
         if tmp >= 0:
             missed_detect = tmp
             for i in range(0, len(people_dt)):
                 person_index_to_compare = findPersonIndexGTFrame(gt_frame, people_dt[i].box_xyxy, 
-                                                                 max_spread_limit=5)
+                                                                 max_spread_limit=16)
                 if person_index_to_compare >= 0:
                     tmp_faceid = people_dt[i].faceid
                     if '%' in tmp_faceid: tmp_faceid = tmp_faceid[:-4]
                     if gt_frame[person_index_to_compare][2].lower() != tmp_faceid.lower():
                         msg = ("-------EVA : Frame \t@" + str(self.current_frame) + 
                                "\t   ---------->   (GT) " + str(gt_frame[person_index_to_compare][2]) + 
                                "\t -v.s- \t " + str(tmp_faceid))
                         add_info_log(msg)
                         diff_count += 1
                 else: fault_detect += 1
         else:
             fault_detect = abs(tmp)
             for i in range(0, len(gt_frame)):
                 person_index_to_compare = findPersonIndexGTFrame(gt_frame, people_dt[i].box_xyxy, 
-                                                                 max_spread_limit=5)
+                                                                 max_spread_limit=16)
                 if person_index_to_compare >= 0:
                     tmp_faceid = people_dt[i].faceid
                     if '%' in tmp_faceid: tmp_faceid = tmp_faceid[:-4]
                     if gt_frame[person_index_to_compare][2].lower() != tmp_faceid.lower():
                         msg = ("-------EVA : Frame \t@" + str(self.current_frame) + 
                                "\t   ---------->   (GT) " + str(gt_frame[person_index_to_compare][2]) + 
                                "\t -v.s- \t " + str(tmp_faceid))
@@ -406,62 +408,30 @@
             for _ in range(0, plus_random):
                 self.static_ids.append(self.generateID(self.string_length))
 
 
 ###############################################################################################
 
 
-def findPersonIndexPeopleList(people, box_xyxy, max_spread_limit=5):
+def findPersonIndexGTFrame(gt_frame, box_xyxy, box_xyxy_index=4, max_spread_limit=16):
     """
     :meta private:
     """
-    index = -1
-    spread_list = []
     box_list = box_xyxy.tolist()
-
-    if len(people) > 0 and len(box_list) == 4:
-        for person in people:
-            max_spread = -1
-            pbox_list = person.box_xyxy.tolist()
-            for i in range(0, 4):
-                sub_spread = abs(box_list[i] - pbox_list[i])
-                if sub_spread > max_spread:
-                    max_spread = sub_spread
-            spread_list.append(max_spread)
-
-        if len(spread_list) > 0:
-            sm_spread = min(spread_list)
-            if sm_spread <= max_spread_limit:
-                index = spread_list.index(sm_spread)
-
-    return index
-
-def findPersonIndexGTFrame(gt_frame, box_xyxy, box_xyxy_index=4, max_spread_limit=5):
-    """
-    :meta private:
-    """
+    min_box_spread = 8192
     index = -1
-    spread_list = []
-    box_list = box_xyxy.tolist()
-
-    if len(gt_frame) > 0 and len(box_list) == 4:
-        for person in gt_frame:
-            max_spread = -1
-            pbox_list = convertStringToNPL(person[box_xyxy_index]).tolist()
-            for i in range(0, 4):
-                sub_spread = abs(box_list[i] - pbox_list[i])
-                if sub_spread > max_spread:
-                    max_spread = sub_spread
-            spread_list.append(max_spread)
-
-        if len(spread_list) > 0:
-            sm_spread = min(spread_list)
-            if sm_spread <= max_spread_limit:
-                index = spread_list.index(sm_spread)
-
+    i = 0
+    for p in gt_frame:
+        pbbox_list = convertStringToNPL(p[box_xyxy_index]).tolist()
+        max_ss = max([abs(box_list[j] - pbbox_list[j]) for j in range(0, 4)])
+        if max_ss < min_box_spread:
+            min_box_spread = max_ss
+            index = i
+        i += 1
+    if min_box_spread > max_spread_limit: index = -1
     return index
 
 def compareRes2Ref(res_txt, ref_txt, res_box_xyxy_index=5, ref_box_xyxy_index=4, 
                    res_compare_index=2, ref_compare_index=2, box_max_spread=5):
     """Compare the result text file generated by :class:`ResIO` to any reference 
     or GT (Ground-truth) text file, ideally used for comparing the strings of 
     :obj:`deepid` or :obj:`faceid` in result to the reference.
@@ -469,17 +439,17 @@
     Parameters
     ----------
     res_txt : str
         A path of the result text file.
     ref_txt : str
         A path of the reference text file.
     res_box_xyxy_index : int, default=5
-        Index of bounding box :code:`[X1 Y1 X2 Y2]` in the result text file.
+        Index of bounding box :code:`[X1, Y1, X2, Y2]` in the result text file.
     ref_box_xyxy_index : int, default=4
-        Index of bounding box :code:`[X1 Y1 X2 Y2]` in the reference text file.
+        Index of bounding box :code:`[X1, Y1, X2, Y2]` in the reference text file.
     res_compare_index : int, default=2
         Index of what to compare in the result text file.
     ref_compare_index : int, default=2
         Index of what to compare in the reference text file.
     box_max_spread : int, default=10
         Max spread or max margin used to decide whether 2 bounding boxes are the same 
         by comparing the differences between the elements in the result's bounding
```

### Comparing `pyppbox-3.1b1/pyppbox/utils/gttools.py` & `pyppbox-3.1b2/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/utils/logtools.py` & `pyppbox-3.1b2/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/utils/persontools.py` & `pyppbox-3.1b2/pyppbox/utils/persontools.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #                                                                           #
 #   You should have received a copy of the GNU General Public License       #
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.  #
 #                                                                           #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
+import numpy as np
 from pyppbox.config.unifiedstrings import UnifiedStrings
 
 
 __ustrings__ = UnifiedStrings()
 
 class Person(object):
 
@@ -65,32 +66,32 @@
             box_xywh=[], 
             box_xyxy=[], 
             keypoints=[],
             repspoint=(0, 0), 
             det_conf=0.5,
             faceid=__ustrings__.unk_fid, 
             deepid=__ustrings__.unk_did, 
-            fraceid_conf=100.0, 
+            faceid_conf=100.0, 
             deepid_conf=100.0
         ):
 
         """
         Construct a Person.
 
         Parameters
         ----------
         init_id : int
             Initial ID.
         cid : int
             Current ID.
         box_xywh : ndarray, optional
-            Bounding box :code:`[x y width height]`, :code:`shape=(4,)`, 
+            Bounding box :code:`[x, y, width, height]`, :code:`shape=(4,)`, 
             :code:`dtype=int`, :code:`ndim=1`.
         box_xyxy : ndarray, optional
-            Bounding box :code:`[x1 y1 x2 y2]`, :code:`shape=(4,)`, 
+            Bounding box :code:`[x1, y1, x2, y2]`, :code:`shape=(4,)`, 
             :code:`dtype=int`, :code:`ndim=1`.
         keypoints : list[], optional
             Keypoints of the body.
         repspoint : tuple(int, int), default=(0, 0)
             Respesented 2D point (x, y).
         det_conf : float, default=0.5
             Confience of detection.
@@ -110,15 +111,15 @@
         self.box_xywh = box_xywh
         self.box_xyxy = box_xyxy
         self.keypoints = keypoints
         self.repspoint = repspoint
         self.det_conf = det_conf
         self.faceid = faceid
         self.deepid = deepid
-        self.faceid_conf = fraceid_conf
+        self.faceid_conf = faceid_conf
         self.deepid_conf = deepid_conf
         self.ontracked = 0
 
     def incrementOnTracked(self):
         """
         Increment ontracked by 1.
         """
@@ -156,27 +157,51 @@
         """
         self.cid = new_cid
         self.faceid = new_faceid
         self.deepid = new_deepid
         self.faceid_conf = new_faceid_conf
         self.deepid_conf = new_deepid_conf
 
+    def getDet(self):
+        """Get a numpy array of detection bounding box with confidence in shape (5,).
+
+        Returns
+        -------
+        ndarray
+            Numpy array of x1, y1, x2, y2, and confidence.
+        """
+        return np.concatenate((np.asarray(self.box_xyxy), [self.det_conf]))
+    
+    def getDetRS(self):
+        """Get a numpy array of detection bounding box with confidence in shape (1, 5).
+
+        Returns
+        -------
+        ndarray
+            Numpy array of x1, y1, x2, y2, and confidence.
+        """
+        return np.concatenate((np.asarray(self.box_xyxy), [self.det_conf])).reshape(1, 5)
+
+    def __print_self__(self):
+        print("Person: " + "\t" + str(self.box_xyxy) + "\t" + str(self.cid) + 
+              "\t" + str(self.facid) + "\t" + str(self.deepid))
+
 
 #####################################################################################
 
 
 def findRepspoint(box_xyxy, calibrate_weight):
     """Find respesented point :code:`(x, y)` of a :class:`Person` object by its bounding 
-    :code:`box_xyxy` of :code:`[x1 y1 x2 y2]`. The :obj:`calibrate_weight` indicates, 
+    :code:`box_xyxy` of :code:`[x1, y1, x2, y2]`. The :obj:`calibrate_weight` indicates, 
     in between :code:`min(y1, y2)` and :code:`max(y1, y2)`, where the :code:`y` is.
 
     Parameters
     ----------
     box_xyxy : ndarray, optional
-        Bounding box :code:`[x1 y1 x2 y2]`, :code:`shape=(4,)`, :code:`dtype=int`, 
+        Bounding box :code:`[x1, y1, x2, y2]`, :code:`shape=(4,)`, :code:`dtype=int`, 
         :code:`ndim=1`.
     calibrate_weight : float
         Calibration weight.
 
     Returns
     -------
     tuple(int, int)
@@ -186,21 +211,21 @@
     y_start = min(box_xyxy[1], box_xyxy[3])
     y_dist = abs(box_xyxy[1] - box_xyxy[3])
     y = int(y_start + calibrate_weight*y_dist)
     return (x, y)
 
 def findRepspointList(box_xyxy, calibrate_weight):
     """Find respesented point :code:`(x, y)` of a :class:`Person` object by its bounding 
-    :code:`box_xyxy` of :code:`[x1 y1 x2 y2]`. The :obj:`calibrate_weight` indicates, 
+    :code:`box_xyxy` of :code:`[x1, y1, x2, y2]`. The :obj:`calibrate_weight` indicates, 
     in between :code:`min(y1, y2)` and :code:`max(y1, y2)`, where the :code:`y` is.
 
     Parameters
     ----------
     box_xyxy : ndarray, optional
-        Bounding box :code:`[x1 y1 x2 y2]`, :code:`shape=(4,)`, :code:`dtype=int`, 
+        Bounding box :code:`[x1, y1, x2, y2]`, :code:`shape=(4,)`, :code:`dtype=int`, 
         :code:`ndim=1`.
     calibrate_weight : float
         Calibration weight.
 
     Returns
     -------
     list[int, int]
```

### Comparing `pyppbox-3.1b1/pyppbox/utils/restools.py` & `pyppbox-3.1b2/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox/utils/visualizetools.py` & `pyppbox-3.1b2/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.1b2/pyppbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.1b1
+Version: 3.1b2
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -45,10 +45,10 @@
 **[📗 Documentation](https://rathaumons.github.io/pyppbox/) > [🚀 Getting started](https://rathaumons.github.io/pyppbox/getstarted.html) > [💡 Examples](https://rathaumons.github.io/pyppbox/examples.html)**
 
 </div>
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
 * Integrate GUI for easy configurations and demo.
-* Support YAML/JSON configurations -> File, raw string and ready dictionary.
+* Support dictionary and YAML/JSON configurations.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.1b1/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.1b2/pyppbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/requirements/requirements.txt` & `pyppbox-3.1b2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/requirements/test_gpu.py` & `pyppbox-3.1b2/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/setup.py` & `pyppbox-3.1b2/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.1b1/setup_extra.yaml` & `pyppbox-3.1b2/setup_extra.yaml`

 * *Files identical despite different names*

