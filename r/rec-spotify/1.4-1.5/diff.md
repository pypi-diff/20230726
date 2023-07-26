# Comparing `tmp/rec_spotify-1.4.tar.gz` & `tmp/rec_spotify-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rec_spotify-1.4.tar", max compression
+gzip compressed data, was "rec_spotify-1.5.tar", max compression
```

## Comparing `rec_spotify-1.4.tar` & `rec_spotify-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.4/etc/screen.png
--rw-r--r--   0        0        0     1289 2023-07-25 08:31:43.317279 rec_spotify-1.4/pyproject.toml
--rw-r--r--   0        0        0     2407 2023-07-24 16:16:52.249892 rec_spotify-1.4/README.md
--rw-r--r--   0        0        0       21 2023-07-25 08:31:22.204023 rec_spotify-1.4/rec_spotify/__init__.py
--rw-r--r--   0        0        0     1735 2023-07-24 09:38:53.871492 rec_spotify-1.4/rec_spotify/cli.py
--rw-r--r--   0        0        0     4278 2023-07-24 16:17:06.052316 rec_spotify-1.4/rec_spotify/config.py
--rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.4/rec_spotify/console.py
--rw-r--r--   0        0        0     7310 2023-07-23 19:42:31.072891 rec_spotify-1.4/rec_spotify/database.py
--rw-r--r--   0        0        0     6427 2023-07-23 15:53:09.981754 rec_spotify-1.4/rec_spotify/items.py
--rw-r--r--   0        0        0     2195 2023-07-23 16:28:40.968471 rec_spotify-1.4/rec_spotify/lyrics.py
--rw-r--r--   0        0        0     6507 2023-07-24 16:37:50.030511 rec_spotify-1.4/rec_spotify/manager.py
--rw-r--r--   0        0        0     1968 2023-07-23 16:07:01.827794 rec_spotify-1.4/rec_spotify/messages.py
--rw-r--r--   0        0        0     3317 2023-07-23 18:16:28.832707 rec_spotify-1.4/rec_spotify/recorder.py
--rw-r--r--   0        0        0     6079 2023-07-24 16:58:47.535112 rec_spotify-1.4/rec_spotify/spotify.py
--rw-r--r--   0        0        0     2207 2023-07-24 14:59:10.819037 rec_spotify-1.4/rec_spotify/utils.py
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 rec_spotify-1.4/PKG-INFO
+-rw-r--r--   0        0        0    41650 2023-07-23 20:18:21.052582 rec_spotify-1.5/etc/screen.png
+-rw-r--r--   0        0        0     1289 2023-07-26 08:54:03.334265 rec_spotify-1.5/pyproject.toml
+-rw-r--r--   0        0        0     3380 2023-07-26 08:52:42.903775 rec_spotify-1.5/README.md
+-rw-r--r--   0        0        0       21 2023-07-26 08:53:59.383139 rec_spotify-1.5/rec_spotify/__init__.py
+-rw-r--r--   0        0        0     2144 2023-07-25 11:36:59.044706 rec_spotify-1.5/rec_spotify/cli.py
+-rw-r--r--   0        0        0     4278 2023-07-25 10:23:46.440401 rec_spotify-1.5/rec_spotify/config.py
+-rw-r--r--   0        0        0      758 2023-07-23 15:35:03.891743 rec_spotify-1.5/rec_spotify/console.py
+-rw-r--r--   0        0        0     7312 2023-07-26 08:42:49.459812 rec_spotify-1.5/rec_spotify/database.py
+-rw-r--r--   0        0        0     6429 2023-07-25 10:24:08.681879 rec_spotify-1.5/rec_spotify/items.py
+-rw-r--r--   0        0        0     2197 2023-07-25 10:24:14.620839 rec_spotify-1.5/rec_spotify/lyrics.py
+-rw-r--r--   0        0        0     7165 2023-07-26 08:48:15.677634 rec_spotify-1.5/rec_spotify/manager.py
+-rw-r--r--   0        0        0     2398 2023-07-26 08:47:13.584024 rec_spotify-1.5/rec_spotify/messages.py
+-rw-r--r--   0        0        0     3391 2023-07-25 10:24:40.331450 rec_spotify-1.5/rec_spotify/recorder.py
+-rw-r--r--   0        0        0     6895 2023-07-26 08:43:31.230906 rec_spotify-1.5/rec_spotify/spotify.py
+-rw-r--r--   0        0        0     2207 2023-07-25 10:25:06.194956 rec_spotify-1.5/rec_spotify/utils.py
+-rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 rec_spotify-1.5/PKG-INFO
```

### Comparing `rec_spotify-1.4/etc/screen.png` & `rec_spotify-1.5/etc/screen.png`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.4/pyproject.toml` & `rec_spotify-1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rec-spotify"
-version = "1.4"
+version = "1.5"
 description = "📻 Record and sync Spotify tracks, albums, and playlists."
 repository = "https://github.com/oSeeLight/rec-spotify"
 authors = ["Jacov Rainz <oSeeLight@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rec_spotify"}]
 include = ["README.md", "etc"]
```

### Comparing `rec_spotify-1.4/README.md` & `rec_spotify-1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -22,20 +22,39 @@
 
 First, you need to create a Spotify app to obtain the credentials. You can create an app at the Spotify Developer Dashboard: https://developer.spotify.com/dashboard
 
 Also change Spotify Output Device to Virtual Audio Cable: [Guide](https://youtu.be/EH-VzIpX7e0?t=86)
 
 ```sh
 # Perform a full synchronization.
-rec-spotify
+rec-spotify --sync
 
 # Record single track/album/playlist.
 # Spotify URL format example: https://open.spotify.com/track/42vwak6ZIFMscDhzz3S52f
 # Output path format example: C:\Users\<username>\Desktop or just "." to save in current directory
 rec-spotify --url <url> --path <where_to_save>
+
+______                 _____             _   _  __       
+| ___ \               /  ___|           | | (_)/ _|      
+| |_/ /___  ___ ______\ `--. _ __   ___ | |_ _| |_ _   _ 
+|    // _ \/ __|______|`--. \ '_ \ / _ \| __| |  _| | | |
+| |\ \  __/ (__       /\__/ / |_) | (_) | |_| | | | |_| |
+\_| \_\___|\___|      \____/| .__/ \___/ \__|_|_|  \__, |
+                            | |                     __/ |
+                            |_|                    |___/ 
+
+usage: rec-spotify [-h] [-c] [-s] [-u URL] [-p PATH] [-v]
+
+options:
+  -h, --help            show this help message and exit
+  -c, --check           Run database cleanup.
+  -s, --sync            Synchronize all of your Spotify playlists with local music library.
+  -u URL, --url URL     Spotify link or ID for a separate track, playlist, or album.
+  -p PATH, --path PATH  The output directory for saving recorded files
+  -v, --version         show program's version number and exit
 ```
 
 ## Configration
 
 On the first run, the program will launch a setup wizard. This will prompt you to enter your Spotify app credentials and other required information.
 
 The config file is located at: ```C:\Users\<username>\.rec_spotify\config.ini```
```

### Comparing `rec_spotify-1.4/rec_spotify/cli.py` & `rec_spotify-1.5/rec_spotify/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import argparse
 import sys
-import rec_spotify
 
+import rec_spotify
 import rec_spotify.messages as m
-from rec_spotify.items import Collection, Track
-from rec_spotify.manager import Manager
 from rec_spotify.config import Config
 from rec_spotify.console import console, get_logo
+from rec_spotify.items import Collection, Track
+from rec_spotify.manager import Manager
 from rec_spotify.utils import parse_spotify_url
 
 
 def app() -> None:
     """CLI entrypoint."""
 
     console.print(get_logo(), style="green")
 
     parser = argparse.ArgumentParser()
-
+    parser.add_argument(
+        "-c",
+        "--check",
+        action="store_true",
+        required=False,
+        help="Run database cleanup.",
+    )
+    parser.add_argument(
+        "-s",
+        "--sync",
+        action="store_true",
+        required=False,
+        help="Synchronize all of your Spotify playlists with local music library.",
+    )
     parser.add_argument(
         "-u",
         "--url",
         type=str,
         required=False,
         help="Spotify link or ID for a separate track, playlist, or album.",
     )
@@ -28,39 +41,38 @@
         "-p",
         "--path",
         type=str,
         required=False,
         help="The output directory for saving recorded files",
     )
     ver = f"Author: oSeeLight | Version: {rec_spotify.__version__}"
-    parser.add_argument('-v', '--version', action='version', version=ver)
-
+    parser.add_argument("-v", "--version", action="version", version=ver)
 
     args = parser.parse_args()
     manager = Manager()
-    if args.url and args.path:
+    if args.check:
+        manager.database_cleanup()
+    elif args.url and args.path:
         match = parse_spotify_url(args.url)
         if match is not None:
             link_type, id = match
             manager.init()
             Config.MUSIC_DIR = args.path
             if link_type == "track":
                 track = Track(id)
                 manager.record_track(track)
             else:
                 collection = Collection(id, kind=link_type)
                 manager.record_collection(collection)
-
         else:
             console.print(m.LINK_ERR)
             sys.exit(1)
-
-    elif len(sys.argv) == 1:
-        manager.init()
+    elif args.sync:
         manager.sync()
+    else:
+        parser.print_help()
 
     manager.close()
-    sys.exit(0)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rec_spotify-1.4/rec_spotify/config.py` & `rec_spotify-1.5/rec_spotify/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import os
 import sys
 
-from rec_spotify.console import console
 import rec_spotify.messages as m
+from rec_spotify.console import console
 
 
 class Config(object):
     """
     Main configuration class for the rec_spotify module.
     """
```

### Comparing `rec_spotify-1.4/rec_spotify/console.py` & `rec_spotify-1.5/rec_spotify/console.py`

 * *Files identical despite different names*

### Comparing `rec_spotify-1.4/rec_spotify/database.py` & `rec_spotify-1.5/rec_spotify/database.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
         return track
 
     @classmethod
     def close(cls) -> None:
         "Close database connection"
         if cls._init:
             cls._connection.commit()
-            cls._connection.close()
+            cls._connection.close()
```

### Comparing `rec_spotify-1.4/rec_spotify/items.py` & `rec_spotify-1.5/rec_spotify/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import typing as t
 import os
+import shutil
+import typing as t
+
 from rec_spotify.config import Config
 from rec_spotify.utils import clear_unwanted
-import shutil
 
 
 class Collection(object):
     """Represents playlist or album."""
 
     def __init__(self, id: str, kind: str = "playlist") -> None:
         self._id = id
```

### Comparing `rec_spotify-1.4/rec_spotify/lyrics.py` & `rec_spotify-1.5/rec_spotify/lyrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 import eyed3
 import requests
 
 from rec_spotify.items import Track
 
 
 class Lyrics(object):
```

### Comparing `rec_spotify-1.4/rec_spotify/manager.py` & `rec_spotify-1.5/rec_spotify/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import os
 import sys
 import typing as t
 
-from rec_spotify.database import Database
 import rec_spotify.messages as m
+from rec_spotify.config import Config
 from rec_spotify.console import console
+from rec_spotify.database import Database
+from rec_spotify.items import Collection, Track
+from rec_spotify.lyrics import Lyrics
+from rec_spotify.recorder import Recorder
 from rec_spotify.spotify import SpotifyClient
-from rec_spotify.items import Track, Collection
-from rec_spotify.config import Config
 from rec_spotify.utils import download_cover, get_estimate_time, trim_silence
-from rec_spotify.recorder import Recorder
-from rec_spotify.lyrics import Lyrics
 
 
 class Manager(object):
     @classmethod
     def sync(cls) -> None:
         "Synchronize Spotify content with local database"
         Database.init_db()
+        cls.init()
 
         # Print db stats
         playlists = Database.get_playlists()
         tracks = Database.get_tracks(total=True)
         undownloaded = list(filter(lambda x: not x.downloaded, tracks))
         console.print(
             m.STATS.format(
                 playlists_count=len(playlists),
                 tracks_count=len(tracks),
                 undownloaded_count=len(undownloaded),
             )
         )
-
         # Sync Playlists
         process_play_ids = []
         sp_playlists = SpotifyClient.get_user_playlists()
         for sp_playlist in sp_playlists:
             loc_playlist = Database.get_playlist(sp_playlist.id)
             if loc_playlist is None:
                 sp_playlist.create_dir()
@@ -91,14 +91,15 @@
         # Recording
         total_time = get_estimate_time(
             sum(track.duration for track in tracks_to_download)
         )
         console.print(
             m.SYNC_START.format(
                 total_time=total_time,
+                track_count=len(tracks_to_download),
             )
         )
         console.print()
         console.rule(":radio: Recorder Log")
         for track in tracks_to_download:
             cls._record_and_save(track)
             Database.mark_downloaded(track, state=True)
@@ -131,14 +132,15 @@
         total_time = get_estimate_time(
             sum(track.duration for track in collection.get_tracks())
         )
 
         console.print(
             m.SYNC_START.format(
                 total_time=total_time,
+                track_count=collection.track_count,
             )
         )
         console.print()
         console.rule(":radio: Recorder Log")
         for track in collection.get_tracks():
             cls._record_and_save(track)
 
@@ -164,14 +166,28 @@
             Lyrics.embed_lyrics(track, lyrics)
 
         os.remove(song_cover.name)
         console.print(m.TRACK_SAVED.format(filepath=track.filepath))
         console.print()
 
     @classmethod
+    def database_cleanup(cls) -> None:
+        Database.init_db()
+        tracks = Database.get_tracks(total=True)
+        fixed = 0
+        for track in tracks:
+            if track.downloaded and track.filepath:
+                if not os.path.exists(track.filepath):
+                    console.print(m.TRACK_NO_LOCAL.format(track=track))
+                    Database.mark_downloaded(track, state=False)
+                    fixed += 1
+        if fixed == 0:
+            console.print(m.DB_CHECK_OK)
+
+    @classmethod
     def init(cls) -> None:
         "Initialize main dependencies."
         Config.init()
         SpotifyClient.init()
         Recorder.init()
 
     @classmethod
```

### Comparing `rec_spotify-1.4/rec_spotify/messages.py` & `rec_spotify-1.5/rec_spotify/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 
 SELECT_SPOTIFY_DEVICE = ":mobile_phone: SELECT DEVICE: "
 SELECT_AUDIO_DEVICE = ":speaker: AUDIO DEVICE: "
 
 JOB_TYPE = "[[green bold]OK[/green bold]] Ready to record the [magenta bold]{job_type}[/magenta bold]: {name}"
 LINK_ERR = "[[red bold]ERROR[/red bold]] The link provided does not match the required format. Please ensure the link follows the correct format, such as this example: https://open.spotify.com/playlist/4weVyheZdSUIdDpmJyx2zf"
 
-
 NEW_PLAYLIST = "[[green bold]ADDED[/green bold]] :file_folder: Playlist: {playlist}"
 RENAME_PLAYLIST = (
     "[[green bold]RENAME[/green bold]] :file_folder: Playlist: {from_name} -> {to_name}"
 )
 DEL_PLAYLIST = "[[red bold]DELETE[/red bold]] :x: Playlist: {playlist}"
 
 
 TRACK = ":musical_note: {title}"
 NEW_TRACK = "[[green bold]ADDED[/green bold]] :musical_note: Track: {track_title}"
 DEL_TRACK = "[[red bold]DELETE[/red bold]] :x: Track: {track_title}"
 TRACK_SAVED = ":white_check_mark: Recorded: {filepath}"
+TRACK_NO_LOCAL = "[[blue bold]INFO[/blue bold]] :musical_note: [magenta bold]{track}[/magenta bold] was not located in the local library. It has been noted as not yet downloaded."
+TRACK_NOT_AVAILABLE = "[[blue bold]INFO[/blue bold]] :x: Track: {track_name} is not available for download."
+
 
 DATABASE_OK = "[[green bold]OK[/green bold]] Database initialization."
 STATS = "[[magenta bold]STATS[/magenta bold]] :file_folder: Playlists: {playlists_count} | :musical_note: Total Tracks: {tracks_count} | :fire: Tracks not downloaded: {undownloaded_count}"
+DB_CHECK_OK = "[[blue bold]INFO[/blue bold]] :white_check_mark: No issues were detected during the check process."
 
-SYNC_START = "[[blue bold]INFO[/blue bold]] The recording process has started. It will take about ~ {total_time}"
+SYNC_START = "[[blue bold]INFO[/blue bold]] The recording process has started. It will take about ~ {total_time} ({track_count} tracks)"
 SYNC_OK = "[[blue bold]INFO[/blue bold]] :white_check_mark: Everything is up to date."
 
 PB_ERROR = "[[red bold]ERROR[/red bold]] Please toggle Spotify playback and try again. This is a common problem."
 REQ_ERROR = "[[red bold]ERROR[/red bold]][[blue bold]RETRY[/blue bold]] Error: {error}."
```

### Comparing `rec_spotify-1.4/rec_spotify/recorder.py` & `rec_spotify-1.5/rec_spotify/recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import io
 import sys
 import threading
-
-import pyaudiowpatch as pyaudio
-from pydub import AudioSegment
 import time
-import io
 import typing as t
+from threading import Thread
 
-
-from rec_spotify.spotify import SpotifyClient
-from rec_spotify.console import clear_lines, console
-from rec_spotify.config import Config
-import rec_spotify.messages as m
-
+import pyaudiowpatch as pyaudio
+from pydub import AudioSegment
 from rich.progress import Progress
-from threading import Thread
 
+import rec_spotify.messages as m
+from rec_spotify.config import Config
+from rec_spotify.console import clear_lines, console
 from rec_spotify.items import Track
+from rec_spotify.spotify import SpotifyClient
 
 
 class Recorder(object):
     "Handles audio recording functionality."
 
     DEVICE_ID: int
     PYAUDIO: pyaudio.PyAudio  # type: ignore
 
+    _init: bool = False
+
     @t.no_type_check
     @classmethod
     def record(cls, track: Track) -> AudioSegment:
         stop_flag = threading.Event()
         frames = io.BytesIO()
 
         def callback(in_data, frame_count, time_info, status) -> t.Any:
@@ -97,12 +96,14 @@
         clear_lines(idx + 1)
 
     @classmethod
     def init(cls) -> None:
         "Initialize PyAudio and set recording device."
         cls.PYAUDIO = pyaudio.PyAudio()
         cls._set_device_id()
+        cls._init = True
 
     @classmethod
     def close(cls) -> None:
         "Close PyAudio instance."
-        cls.PYAUDIO.terminate()
+        if cls._init:
+            cls.PYAUDIO.terminate()
```

### Comparing `rec_spotify-1.4/rec_spotify/spotify.py` & `rec_spotify-1.5/rec_spotify/spotify.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 import typing as t
-from requests.exceptions import RequestException
 
 import spotipy
+from requests.exceptions import RequestException
 from spotipy.client import Spotify
-from spotipy.oauth2 import SpotifyOAuth, CacheFileHandler
-from rec_spotify.items import Track, Collection
+from spotipy.oauth2 import CacheFileHandler, SpotifyOAuth
 
 import rec_spotify.messages as m
 from rec_spotify.config import Config
 from rec_spotify.console import clear_lines, console
+from rec_spotify.items import Collection, Track
 
 
 class SpotifyClient(object):
     """
     Class for Spotify API interactions.
     """
 
@@ -38,27 +38,51 @@
         data: dict = cls._make_request(cls._client.track, track.id)
         track = cls._parse_track(track, data)
         return track
 
     @classmethod
     def get_collection(cls, collection: Collection) -> Collection:
         sp_col: dict
+
         if collection.kind == "playlist":
             sp_col = cls._make_request(cls._client.playlist, collection.id)
         else:
             sp_col = cls._make_request(cls._client.album, collection.id)
 
         collection.name = sp_col["name"]
-        for track_data in sp_col["tracks"]["items"]:
+        total_tracks = sp_col["tracks"]["total"]
+
+        for offset in range(0, total_tracks, 100):
             if collection.kind == "playlist":
-                track_data = track_data["track"]
-            track = Track(track_data["id"])
-            track.collection = collection
-            track = cls._parse_track(track, track_data)
-            collection.add_track(track)
+                sp_col = cls._make_request(
+                    cls._client.playlist_tracks,
+                    collection.id,
+                    offset=offset,
+                )
+            else:
+                sp_col = cls._make_request(
+                    cls._client.album_tracks,
+                    collection.id,
+                    offset=offset,
+                )
+
+            for track_data in sp_col["items"]:
+                if collection.kind == "playlist":
+                    track_data = track_data["track"]
+
+                track_id = track_data["id"]
+                if track_id is None:
+                    name = track_data["name"]
+                    console.print(m.TRACK_NOT_AVAILABLE.format(track_name=name))
+                else:
+                    track = Track(track_data["id"])
+                    track.collection = collection
+                    track = cls._parse_track(track, track_data)
+                    collection.add_track(track)
+
         return collection
 
     @classmethod
     def get_user_playlists(cls) -> t.List[Collection]:
         sp_playlists: dict = cls._make_request(cls._client.current_user_playlists)
         collections: t.List[Collection] = []
         for playlist in sp_playlists["items"]:
```

### Comparing `rec_spotify-1.4/rec_spotify/utils.py` & `rec_spotify-1.5/rec_spotify/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import math
 import re
-import tempfile
 import shutil
-import requests
-import math
+import tempfile
 import typing as t
 
+import requests
 from pydub import AudioSegment
 from pydub.silence import detect_leading_silence
 
 
 def parse_spotify_url(url: str) -> tuple[str, str] | None:
     "Parses a Spotify URL and returns the type of link and its ID."
     match = re.search(r"open\.spotify\.com/(track|album|playlist)/(\w+)", url.strip())
```

### Comparing `rec_spotify-1.4/PKG-INFO` & `rec_spotify-1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-spotify
-Version: 1.4
+Version: 1.5
 Summary: 📻 Record and sync Spotify tracks, albums, and playlists.
 Home-page: https://github.com/oSeeLight/rec-spotify
 License: MIT
 Keywords: spotify,record
 Author: Jacov Rainz
 Author-email: oSeeLight@proton.me
 Requires-Python: >=3.11,<4.0
@@ -44,20 +44,39 @@
 
 First, you need to create a Spotify app to obtain the credentials. You can create an app at the Spotify Developer Dashboard: https://developer.spotify.com/dashboard
 
 Also change Spotify Output Device to Virtual Audio Cable: [Guide](https://youtu.be/EH-VzIpX7e0?t=86)
 
 ```sh
 # Perform a full synchronization.
-rec-spotify
+rec-spotify --sync
 
 # Record single track/album/playlist.
 # Spotify URL format example: https://open.spotify.com/track/42vwak6ZIFMscDhzz3S52f
 # Output path format example: C:\Users\<username>\Desktop or just "." to save in current directory
 rec-spotify --url <url> --path <where_to_save>
+
+______                 _____             _   _  __       
+| ___ \               /  ___|           | | (_)/ _|      
+| |_/ /___  ___ ______\ `--. _ __   ___ | |_ _| |_ _   _ 
+|    // _ \/ __|______|`--. \ '_ \ / _ \| __| |  _| | | |
+| |\ \  __/ (__       /\__/ / |_) | (_) | |_| | | | |_| |
+\_| \_\___|\___|      \____/| .__/ \___/ \__|_|_|  \__, |
+                            | |                     __/ |
+                            |_|                    |___/ 
+
+usage: rec-spotify [-h] [-c] [-s] [-u URL] [-p PATH] [-v]
+
+options:
+  -h, --help            show this help message and exit
+  -c, --check           Run database cleanup.
+  -s, --sync            Synchronize all of your Spotify playlists with local music library.
+  -u URL, --url URL     Spotify link or ID for a separate track, playlist, or album.
+  -p PATH, --path PATH  The output directory for saving recorded files
+  -v, --version         show program's version number and exit
 ```
 
 ## Configration
 
 On the first run, the program will launch a setup wizard. This will prompt you to enter your Spotify app credentials and other required information.
 
 The config file is located at: ```C:\Users\<username>\.rec_spotify\config.ini```
```

