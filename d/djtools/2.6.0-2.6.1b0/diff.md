# Comparing `tmp/djtools-2.6.0.tar.gz` & `tmp/djtools-2.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djtools-2.6.0.tar", last modified: Mon Jul 24 22:05:42 2023, max compression
+gzip compressed data, was "djtools-2.6.1b0.tar", last modified: Wed Jul 26 19:15:13 2023, max compression
```

## Comparing `djtools-2.6.0.tar` & `djtools-2.6.1b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.502386 djtools-2.6.0/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.6.0/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.6.0/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2169 2023-07-24 22:05:42.502486 djtools-2.6.0/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)      939 2023-07-24 22:04:12.000000 djtools-2.6.0/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.473557 djtools-2.6.0/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.486734 djtools-2.6.0/djtools/collection/
--rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27200 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7582 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/collection/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.492219 djtools-2.6.0/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.6.0/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1300 2023-07-22 20:27:28.000000 djtools-2.6.0/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    20888 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.6.0/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.0/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.492823 djtools-2.6.0/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.0/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.495758 djtools-2.6.0/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.498216 djtools-2.6.0/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5415 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.501855 djtools-2.6.0/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.6.0/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       89 2023-07-22 20:25:43.000000 djtools-2.6.0/djtools/version.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-24 22:05:42.478160 djtools-2.6.0/djtools.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2169 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1209 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-24 22:05:42.000000 djtools-2.6.0/djtools.egg-info/top_level.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.6.0/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-24 22:05:42.502893 djtools-2.6.0/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2340 2023-07-24 22:03:16.000000 djtools-2.6.0/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.742177 djtools-2.6.1b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 djtools-2.6.1b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 djtools-2.6.1b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2677 2023-07-26 19:15:13.742304 djtools-2.6.1b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1445 2023-07-26 18:56:00.000000 djtools-2.6.1b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.710611 djtools-2.6.1b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2541 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1885 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.720596 djtools-2.6.1b0/djtools/collection/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1428 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12876 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2914 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2985 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27429 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7697 2023-07-26 18:56:00.000000 djtools-2.6.1b0/djtools/collection/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15832 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2404 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13886 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/collection/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.728238 djtools-2.6.1b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-26 18:24:13.000000 djtools-2.6.1b0/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1334 2023-07-26 19:13:43.000000 djtools-2.6.1b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    21130 2023-07-26 17:53:37.000000 djtools-2.6.1b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.729254 djtools-2.6.1b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.733493 djtools-2.6.1b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.738879 djtools-2.6.1b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      874 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3693 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7682 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5415 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.741757 djtools-2.6.1b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-22 20:25:43.000000 djtools-2.6.1b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 djtools-2.6.1b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-26 19:15:02.000000 djtools-2.6.1b0/djtools/version.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-26 19:15:13.713575 djtools-2.6.1b0/djtools.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2677 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1209 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-26 19:15:13.000000 djtools-2.6.1b0/djtools.egg-info/top_level.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 djtools-2.6.1b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-26 19:15:13.742684 djtools-2.6.1b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2340 2023-07-24 23:14:57.000000 djtools-2.6.1b0/setup.py
```

### Comparing `djtools-2.6.0/LICENSE` & `djtools-2.6.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/PKG-INFO` & `djtools-2.6.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.6.0
+Version: 2.6.1b0
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,19 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [x] Script for removing situation tags and resolving album, label, and year for tracks
+    - [x] Allow `build_config` to accept an override for the path to `config.yaml`
+    - [x] Fix missing typehints for the `NonEmptyListElementAction` class
+    - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
+    - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
     - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
 * 2.7.0
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
```

### Comparing `djtools-2.6.0/README.md` & `djtools-2.6.1b0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [x] Script for removing situation tags and resolving album, label, and year for tracks
+    - [x] Allow `build_config` to accept an override for the path to `config.yaml`
+    - [x] Fix missing typehints for the `NonEmptyListElementAction` class
+    - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
+    - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
     - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
 * 2.7.0
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
```

### Comparing `djtools-2.6.0/djtools/__init__.py` & `djtools-2.6.1b0/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/__main__.py` & `djtools-2.6.1b0/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/__init__.py` & `djtools-2.6.1b0/djtools/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/collections.py` & `djtools-2.6.1b0/djtools/collection/collections.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/config.py` & `djtools-2.6.1b0/djtools/collection/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 logger = logging.getLogger(__name__)
 
 
 class CollectionConfig(BaseConfig):
     """Configuration object for the collection package."""
 
     COLLECTION_PATH: Path = None
+    COLLECTION_PLAYLIST_FILTERS: List[
+        Literal["HipHopFilter", "MinimalDeepTechFilter"]
+    ] = []
     COLLECTION_PLAYLISTS: bool = False
     COLLECTION_PLAYLISTS_REMAINDER: Literal["folder", "playlist"] = "folder"
     COPY_PLAYLISTS:  List[str] = []
     COPY_PLAYLISTS_DESTINATION: Path = None
     PLATFORM: Literal["rekordbox"] = "rekordbox"
     SHUFFLE_PLAYLISTS:  List[str] = []
```

### Comparing `djtools-2.6.0/djtools/collection/copy_playlists.py` & `djtools-2.6.1b0/djtools/collection/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/helpers.py` & `djtools-2.6.1b0/djtools/collection/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 #   - PLATFROM_REGISTRY: used to determine which abstraction implementations to
 #       use e.g. "rekordbox"
 #   - build_tag_playlists: builds collection playlists using "tags" component
 #       of the PlaylistConfig
 #   - PlaylistFilter: abstraction for filtering Tracks from Playlists
 #   - HipHopFilter: used to distinguish between actual hip hop tracks and bass
 #       tracks that have hip hop influences
-#   - MinimalDeepTech: used to distinguish between minimal deep tech tracks
-#       with predominately house and techno influences
+#   - MinimalDeepTechFilter: used to distinguish between minimal deep tech
+#       tracks with predominately house and techno influences
 #   - filter_tag_playlists: applies PlaylistFilter implementations to built tag
 #       playlists
 #   - aggregate_playlists: aggregates tracks from playlists in folders to
 #       create an "All <folder name>" playlist in each folder
 #   - add_selectors_to_tags: parses combiner playlist names and finds BPM,
 #       rating, and playlist selectors to update the tag -> track lookup
 #   - parse_bpms_and_ratings: used to parse BPM and rating selectors
@@ -275,24 +275,26 @@
 
         Args:
             track: Track object to apply filter to.
 
         Returns:
             Whether or not this track should be included in the playlist.
         """
-        genre_tags = track.get_genre_tags()
-        index = genre_tags.index("Minimal Deep Tech")
-        prefix_tag = genre_tags[index - 1]
-        techno_with_no_techno_prefix = (
-            self._techno and prefix_tag.lower() != "techno"
-        )
-        not_techno_with_techno_prefix = (
-            not self._techno and prefix_tag.lower() == "techno"
-        )
-        if techno_with_no_techno_prefix or not_techno_with_techno_prefix:
+        house_exp = re.compile(r".*house.*")
+        techno_exp = re.compile(r".*techno.*")
+        house_tag = techno_tag = False
+        for tag in track.get_genre_tags():
+            if re.search(house_exp, tag.lower()):
+                house_tag = True
+            if re.search(techno_exp, tag.lower()):
+                techno_tag = True
+        if (
+            (self._techno and not techno_tag) or
+            (self._house and not house_tag)
+        ):
             return False
 
         return True
 
     def is_filter_playlist(self, playlist: Playlist) -> bool:
         """Returns True if this playlist's name is "Minimal Deep Tech".
 
@@ -302,18 +304,21 @@
         Returns:
             Whether or not to filter this playlist.
         """
         if not playlist.get_name() == "Minimal Deep Tech":
             return False
 
         self._techno = False  #pylint: disable=attribute-defined-outside-init
+        self._house = False  #pylint: disable=attribute-defined-outside-init
         parent = playlist.get_parent()
         while parent:
             if parent.get_name() == "Techno":
                 self._techno = True  #pylint: disable=attribute-defined-outside-init
+            if parent.get_name() == "House":
+                self._house = True  #pylint: disable=attribute-defined-outside-init
             parent = parent.get_parent()
 
         return True
 
 
 def filter_tag_playlists(
     playlist: Playlist, playlist_filters: List[PlaylistFilter]
```

### Comparing `djtools-2.6.0/djtools/collection/playlist_builder.py` & `djtools-2.6.1b0/djtools/collection/playlist_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from collections import defaultdict
 import logging
 from pathlib import Path
 
 import yaml
 
 from djtools.collection.config import PlaylistConfig, PlaylistConfigContent
+from djtools.collection import helpers
 from djtools.collection.helpers import (
     add_selectors_to_tags,
     aggregate_playlists,
     build_combiner_playlists,
     build_tag_playlists,
     filter_tag_playlists,
-    HipHopFilter,
-    MinimalDeepTechFilter,
     PLATFORM_REGISTRY,
     print_playlists_tag_statistics,
 )
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
@@ -116,17 +115,21 @@
         )
 
         # The tag playlists must have their "parent" attribute set so that
         # PlaylistFilter implementations may apply logic that depends on the
         # relative position of the playlist with the playlist tree.
         tag_playlists.set_parent()
 
-        # Apply the filtering logic of these PlaylistFilter implementations.
+        # Apply the filtering logic of the configured PlaylistFilter implementations.
         filter_tag_playlists(
-            tag_playlists, [HipHopFilter(), MinimalDeepTechFilter()]
+            tag_playlists,
+            [
+                getattr(helpers, playlist_filter)()
+                for playlist_filter in config.COLLECTION_PLAYLIST_FILTERS
+            ]
         )
 
         # Recursively traverse the playlist tree and create "all" playlists
         # within each folder containing more than one playlist. These "all"
         # playlists aggregate the set of tracks contained within all the other
         # playlists within the same folder.
         _ = aggregate_playlists(tag_playlists, playlist_class)
```

### Comparing `djtools-2.6.0/djtools/collection/playlists.py` & `djtools-2.6.1b0/djtools/collection/playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/shuffle_playlists.py` & `djtools-2.6.1b0/djtools/collection/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/collection/tracks.py` & `djtools-2.6.1b0/djtools/collection/tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/configs/collection_playlists.yaml` & `djtools-2.6.1b0/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/configs/config.py` & `djtools-2.6.1b0/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/configs/config.yaml` & `djtools-2.6.1b0/djtools/configs/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 collection:
   COLLECTION_PATH: null
   COLLECTION_PLAYLISTS: false
   COLLECTION_PLAYLISTS_REMAINDER: folder
+  COLLECTION_PLAYLIST_FILTERS: []
   COPY_PLAYLISTS: []
   COPY_PLAYLISTS_DESTINATION: null
   PLATFORM: rekordbox
   SHUFFLE_PLAYLISTS: []
 configs:
   LOG_LEVEL: INFO
   VERBOSITY: 0
```

### Comparing `djtools-2.6.0/djtools/configs/helpers.py` & `djtools-2.6.1b0/djtools/configs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 overrides the corresponding configuration options with these arguments.
 """
 from argparse import Action, ArgumentParser, Namespace, RawTextHelpFormatter
 import json
 import logging
 from pathlib import Path
 import sys
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 import yaml
 
 from djtools.collection.config import CollectionConfig
 from djtools.configs.config import BaseConfig
 from djtools.spotify.config import SpotifyConfig
 from djtools.sync.config import SyncConfig
@@ -35,15 +35,21 @@
 
     Some configuration options, like UPLOAD_EXCLUDE_DIRS, may be set to some
     sensible default in config.yaml. Because of this users will be unable to
     run "--upload-music" in conjunction with "--download-include-dirs" without
     having to first make an edit to their config.yaml (because the
     include/exclude options are mutually exclusive).
     """
-    def __call__(self, parser, namespace, values, option_string=None):
+    def __call__(
+        self,
+        parser: ArgumentParser,
+        namespace: Namespace,
+        values: List[str],
+        option_string: Optional[str] = None,
+    ):
         """Filter list-type arguments for empty strings.
 
         Args:
             parser: The ArgumentParser object which contains this action.
             namespace: The Namespace object returned by parse_args().
             values: The associated command-line arguments.
             option_string: The option string used to invoke this action.
@@ -496,29 +502,33 @@
         package_root = Path(__file__).parent.parent
         configs_dir = package_root / "configs"
         args.link_configs.symlink_to(configs_dir, target_is_directory=True)
 
     return vars(args)
 
 
-def build_config() -> BaseConfig:
+def build_config(config_file: Optional[Path] = None) -> BaseConfig:
     """This function loads configurations for the library.
     
     Configurations are loaded from config.yaml. If command-line arguments are
     provided, these override the configuration options set in config.yaml.
 
+    Args:
+        config_file: Optional path to a config.yaml.
+
     Raises:
         RuntimeError: config.yaml must be a valid YAML.
 
     Returns:
         Global configuration object.
     """
     # Load "config.yaml".
-    config_dir = Path(__file__).parent.parent / "configs"
-    config_file = config_dir / "config.yaml"
+    if not config_file:
+        config_dir = Path(__file__).parent.parent / "configs"
+        config_file = config_dir / "config.yaml"
     if config_file.exists():
         try:
             with open(config_file, mode="r", encoding="utf-8") as _file:
                 config = yaml.load(_file, Loader=yaml.FullLoader) or {}
         except Exception as exc:
             msg = f'Error reading "config.yaml": {exc}'
             logger.critical(msg)
```

### Comparing `djtools-2.6.0/djtools/spotify/__init__.py` & `djtools-2.6.1b0/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/spotify/config.py` & `djtools-2.6.1b0/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/spotify/helpers.py` & `djtools-2.6.1b0/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/spotify/playlist_builder.py` & `djtools-2.6.1b0/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/sync/__init__.py` & `djtools-2.6.1b0/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/sync/config.py` & `djtools-2.6.1b0/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/sync/helpers.py` & `djtools-2.6.1b0/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/sync/sync_operations.py` & `djtools-2.6.1b0/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/utils/__init__.py` & `djtools-2.6.1b0/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/utils/check_tracks.py` & `djtools-2.6.1b0/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/utils/config.py` & `djtools-2.6.1b0/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/utils/helpers.py` & `djtools-2.6.1b0/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools/utils/url_download.py` & `djtools-2.6.1b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/djtools.egg-info/PKG-INFO` & `djtools-2.6.1b0/djtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djtools
-Version: 2.6.0
+Version: 2.6.1b0
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,19 @@
 # DJ Tools
 [![image](https://img.shields.io/pypi/v/djtools.svg)](https://pypi.org/project/djtools/)
 
 Please see the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual guides, and references!
 
 # Release Plan
 * 2.6.1
+    - [x] Script for removing situation tags and resolving album, label, and year for tracks
+    - [x] Allow `build_config` to accept an override for the path to `config.yaml`
+    - [x] Fix missing typehints for the `NonEmptyListElementAction` class
+    - [x] [Make PlaylistFilter implementations configurable](https://github.com/a-rich/DJ-Tools/issues/120)
+    - [x] [Make MinimalDeepTechFilter more robust to the relative position of House and Techno tags](https://github.com/a-rich/DJ-Tools/issues/122)
     - [ ] [Stability issues with requests to the search endpoint of the Spotify API](https://github.com/a-rich/DJ-Tools/issues/58)
     - [ ] [Make Spotify API calls asynchronous](https://github.com/a-rich/DJ-Tools/issues/38)
 * 2.7.0
     - [ ] [Improve Reddit submission title parsing in order to improve precision and recall of Spotify API search results](https://github.com/a-rich/DJ-Tools/issues/59)
     - [ ] [Derive boolean algebra expressions that generate a given playlist](https://github.com/a-rich/DJ-Tools/issues/106)
     - [ ] [Create graphic user interface for djtools](https://github.com/a-rich/DJ-Tools/issues/118)
```

### Comparing `djtools-2.6.0/djtools.egg-info/SOURCES.txt` & `djtools-2.6.1b0/djtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djtools-2.6.0/setup.py` & `djtools-2.6.1b0/setup.py`

 * *Files identical despite different names*

