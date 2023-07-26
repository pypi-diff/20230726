# Comparing `tmp/rec_spotify-1.5.tar.gz` & `tmp/rec_spotify-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.5.tar", max compression
+gzip compressed data, was "rec_spotify-1.5.1.tar", max compression
```

## Comparing `rec_spotify-1.5.tar` & `rec_spotify-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.5/etc/screen.png
--rw-r--r--   0        0        0     1289 2023-07-26 08:54:03.334265 rec_spotify-1.5/pyproject.toml
--rw-r--r--   0        0        0     3380 2023-07-26 08:52:42.903775 rec_spotify-1.5/README.md
--rw-r--r--   0        0        0       21 2023-07-26 08:53:59.383139 rec_spotify-1.5/rec_spotify/__init__.py
--rw-r--r--   0        0        0     2144 2023-07-25 11:36:59.044706 rec_spotify-1.5/rec_spotify/cli.py
--rw-r--r--   0        0        0     4278 2023-07-25 10:23:46.440401 rec_spotify-1.5/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.5/rec_spotify/console.py
--rw-r--r--   0        0        0     7312 2023-07-26 08:42:49.459812 rec_spotify-1.5/rec_spotify/database.py
--rw-r--r--   0        0        0     6429 2023-07-25 10:24:08.681879 rec_spotify-1.5/rec_spotify/items.py
--rw-r--r--   0        0        0     2197 2023-07-25 10:24:14.620839 rec_spotify-1.5/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     7165 2023-07-26 08:48:15.677634 rec_spotify-1.5/rec_spotify/manager.py
--rw-r--r--   0        0        0     2398 2023-07-26 08:47:13.584024 rec_spotify-1.5/rec_spotify/messages.py
--rw-r--r--   0        0        0     3391 2023-07-25 10:24:40.331450 rec_spotify-1.5/rec_spotify/recorder.py
--rw-r--r--   0        0        0     6895 2023-07-26 08:43:31.230906 rec_spotify-1.5/rec_spotify/spotify.py
--rw-r--r--   0        0        0     2207 2023-07-25 10:25:06.194956 rec_spotify-1.5/rec_spotify/utils.py
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 rec_spotify-1.5/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.5.1/etc/screen.png
+-rw-r--r--   0        0        0     1291 2023-07-26 17:17:11.671633 rec_spotify-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3380 2023-07-26 08:52:42.903775 rec_spotify-1.5.1/README.md
+-rw-r--r--   0        0        0       21 2023-07-26 08:53:59.383139 rec_spotify-1.5.1/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     2167 2023-07-26 17:17:41.729242 rec_spotify-1.5.1/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4278 2023-07-25 10:23:46.440401 rec_spotify-1.5.1/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.5.1/rec_spotify/console.py
+-rw-r--r--   0        0        0     7312 2023-07-26 08:42:49.459812 rec_spotify-1.5.1/rec_spotify/database.py
+-rw-r--r--   0        0        0     6429 2023-07-25 10:24:08.681879 rec_spotify-1.5.1/rec_spotify/items.py
+-rw-r--r--   0        0        0     2197 2023-07-25 10:24:14.620839 rec_spotify-1.5.1/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     7165 2023-07-26 08:48:15.677634 rec_spotify-1.5.1/rec_spotify/manager.py
+-rw-r--r--   0        0        0     2398 2023-07-26 08:47:13.584024 rec_spotify-1.5.1/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3391 2023-07-25 10:24:40.331450 rec_spotify-1.5.1/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     6895 2023-07-26 08:43:31.230906 rec_spotify-1.5.1/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     2207 2023-07-25 10:25:06.194956 rec_spotify-1.5.1/rec_spotify/utils.py
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rec_spotify-1.5.1/PKG-INFO
```

### Comparing `rec_spotify-1.5/etc/screen.png` & `rec_spotify-1.5.1/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/pyproject.toml` & `rec_spotify-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.5"
+version = "1.5.1"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.5/README.md` & `rec_spotify-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/cli.py` & `rec_spotify-1.5.1/rec_spotify/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
                 manager.record_collection(collection)
         else:
             console.print(m.LINK_ERR)
             sys.exit(1)
     elif args.sync:
         manager.sync()
     else:
+        Config.init()
         parser.print_help()
 
     manager.close()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rec_spotify-1.5/rec_spotify/config.py` & `rec_spotify-1.5.1/rec_spotify/config.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/console.py` & `rec_spotify-1.5.1/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/database.py` & `rec_spotify-1.5.1/rec_spotify/database.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/items.py` & `rec_spotify-1.5.1/rec_spotify/items.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/lyrics.py` & `rec_spotify-1.5.1/rec_spotify/lyrics.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/manager.py` & `rec_spotify-1.5.1/rec_spotify/manager.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/messages.py` & `rec_spotify-1.5.1/rec_spotify/messages.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/recorder.py` & `rec_spotify-1.5.1/rec_spotify/recorder.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/spotify.py` & `rec_spotify-1.5.1/rec_spotify/spotify.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/rec_spotify/utils.py` & `rec_spotify-1.5.1/rec_spotify/utils.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.5/PKG-INFO` & `rec_spotify-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.5
+Version: 1.5.1
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
```

