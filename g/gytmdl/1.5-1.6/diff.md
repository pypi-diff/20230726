# Comparing `tmp/gytmdl-1.5.tar.gz` & `tmp/gytmdl-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytmdl-1.5.tar", last modified: Sat May 13 22:32:33 2023, max compression
+gzip compressed data, was "gytmdl-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gytmdl-1.5.tar` & `gytmdl-1.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1176 2023-05-13 22:32:29.661591 gytmdl-1.5/.github/workflows/main.yml
--rw-r--r--   0        0        0       80 2023-05-13 22:32:29.661591 gytmdl-1.5/.gitignore
--rw-r--r--   0        0        0     2692 2023-05-13 22:32:29.661591 gytmdl-1.5/README.md
--rw-r--r--   0        0        0     4145 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/__init__.py
--rw-r--r--   0        0        0       58 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/__main__.py
--rw-r--r--   0        0        0     6718 2023-05-13 22:32:29.661591 gytmdl-1.5/gytmdl/gytmdl.py
--rw-r--r--   0        0        0      456 2023-05-13 22:32:29.661591 gytmdl-1.5/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-13 22:32:29.661591 gytmdl-1.5/requirements.txt
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 gytmdl-1.5/PKG-INFO
+-rw-r--r--   0        0        0     1176 2023-07-26 13:38:41.672486 gytmdl-1.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0       80 2023-07-26 13:38:41.672486 gytmdl-1.6/.gitignore
+-rw-r--r--   0        0        0     3767 2023-07-26 13:38:41.672486 gytmdl-1.6/README.md
+-rw-r--r--   0        0        0       20 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/__main__.py
+-rw-r--r--   0        0        0     7906 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/cli.py
+-rw-r--r--   0        0        0     8809 2023-07-26 13:38:41.672486 gytmdl-1.6/gytmdl/dl.py
+-rw-r--r--   0        0        0      460 2023-07-26 13:38:41.672486 gytmdl-1.6/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-26 13:38:41.672486 gytmdl-1.6/requirements.txt
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 gytmdl-1.6/PKG-INFO
```

### Comparing `gytmdl-1.5/.github/workflows/main.yml` & `gytmdl-1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gytmdl-1.5/gytmdl/gytmdl.py` & `gytmdl-1.6/gytmdl/dl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,187 +1,255 @@
+import functools
+import re
 import shutil
 import subprocess
 from pathlib import Path
-import functools
-from ytmusicapi import YTMusic
-from yt_dlp import YoutubeDL
+
 import requests
 from mutagen.mp4 import MP4, MP4Cover
+from yt_dlp import YoutubeDL
+from ytmusicapi import YTMusic
 
-
-class Gytmdl:
-    def __init__(self, cookies_location, itag, final_path, temp_path, overwrite, skip_cleanup):
+MP4_TAGS_MAP = {
+    "album": "\xa9alb",
+    "album_artist": "aART",
+    "artist": "\xa9ART",
+    "comment": "\xa9cmt",
+    "lyrics": "\xa9lyr",
+    "media_type": "stik",
+    "rating": "rtng",
+    "title": "\xa9nam",
+    "year": "\xa9day",
+}
+
+
+class Dl:
+    def __init__(
+        self,
+        final_path: Path,
+        temp_path: Path,
+        cookies_location: Path,
+        ffmpeg_location: str,
+        itag: str,
+        cover_size: int,
+        cover_format: str,
+        cover_quality: int,
+        final_path_structure: str,
+        exclude_tags: str,
+        truncate: int,
+        overwrite: bool,
+        **kwargs,
+    ):
         self.ytmusic = YTMusic()
-        self.cookies_location = Path(cookies_location)
+        self.final_path = final_path
+        self.temp_path = temp_path
+        self.cookies_location = cookies_location
+        self.ffmpeg_location = ffmpeg_location
         self.itag = itag
-        self.final_path = Path(final_path)
-        self.temp_path = Path(temp_path)
+        self.cover_size = cover_size
+        self.cover_format = cover_format
+        self.cover_quality = cover_quality
+        self.final_path_structure = final_path_structure
+        self.exclude_tags = (
+            [i.lower() for i in exclude_tags.split(",")]
+            if exclude_tags is not None
+            else []
+        )
+        self.truncate = None if truncate < 4 else truncate
         self.overwrite = overwrite
-        self.skip_cleanup = skip_cleanup
-    
 
     @functools.lru_cache()
     def get_ydl_extract_info(self, url):
         ydl_opts = {
-            'quiet': True,
-            'no_warnings': True,
-            'extract_flat': True,
+            "quiet": True,
+            "no_warnings": True,
+            "extract_flat": True,
         }
-        if self.cookies_location.exists():
-            ydl_opts['cookiefile'] = str(self.cookies_location)
+        if self.cookies_location is not None:
+            ydl_opts["cookiefile"] = str(self.cookies_location)
         with YoutubeDL(ydl_opts) as ydl:
             return ydl.extract_info(url, download=False)
-    
 
     def get_download_queue(self, url):
-        url = url.split('&')[0]
-        download_info = []
+        url = url.split("&")[0]
+        download_queue = []
         ydl_extract_info = self.get_ydl_extract_info(url)
-        if not 'youtube' in ydl_extract_info['webpage_url']:
-            raise Exception('Not a YouTube URL')
-        if 'MPREb_' in ydl_extract_info['webpage_url_basename']:
-            ydl_extract_info = self.get_ydl_extract_info(ydl_extract_info['url'])
-        if 'playlist' in ydl_extract_info['webpage_url_basename']:
-            download_info.extend(ydl_extract_info['entries'])
-        if 'watch' in ydl_extract_info['webpage_url_basename']:
-            download_info.append(ydl_extract_info)
-        return download_info
-    
+        if "youtube" not in ydl_extract_info["webpage_url"]:
+            raise Exception("Not a YouTube URL")
+        if "MPREb_" in ydl_extract_info["webpage_url_basename"]:
+            ydl_extract_info = self.get_ydl_extract_info(ydl_extract_info["url"])
+        if "playlist" in ydl_extract_info["webpage_url_basename"]:
+            download_queue.extend(ydl_extract_info["entries"])
+        if "watch" in ydl_extract_info["webpage_url_basename"]:
+            download_queue.append(ydl_extract_info)
+        return download_queue
 
     def get_artist(self, artist_list):
         if len(artist_list) == 1:
-            return artist_list[0]['name']
-        artist = ', '.join([i['name'] for i in artist_list][:-1])
+            return artist_list[0]["name"]
+        artist = ", ".join([i["name"] for i in artist_list][:-1])
         artist += f' & {artist_list[-1]["name"]}'
         return artist
-    
 
     def get_ytmusic_watch_playlist(self, video_id):
         ytmusic_watch_playlist = self.ytmusic.get_watch_playlist(video_id)
-        if not ytmusic_watch_playlist['tracks'][0]['length'] and ytmusic_watch_playlist['tracks'][0].get('album'):
-            raise Exception('Track is not available')
-        if not ytmusic_watch_playlist['tracks'][0].get('album'):
+        if not ytmusic_watch_playlist["tracks"][0]["length"] and ytmusic_watch_playlist[
+            "tracks"
+        ][0].get("album"):
+            raise Exception("Track is not available")
+        if not ytmusic_watch_playlist["tracks"][0].get("album"):
             return None
         return ytmusic_watch_playlist
-    
 
     def search_track(self, title):
-        return self.ytmusic.search(title, 'songs')[0]['videoId']
-    
-    
+        return self.ytmusic.search(title, "songs")[0]["videoId"]
+
     @functools.lru_cache()
     def get_ytmusic_album(self, browse_id):
         return self.ytmusic.get_album(browse_id)
-    
 
     @functools.lru_cache()
     def get_cover(self, url):
         return requests.get(url).content
-    
 
     def get_tags(self, ytmusic_watch_playlist):
-        video_id = ytmusic_watch_playlist['tracks'][0]['videoId']
-        ytmusic_album = self.ytmusic.get_album(ytmusic_watch_playlist['tracks'][0]['album']['id'])
+        video_id = ytmusic_watch_playlist["tracks"][0]["videoId"]
+        ytmusic_album = self.ytmusic.get_album(
+            ytmusic_watch_playlist["tracks"][0]["album"]["id"]
+        )
         tags = {
-            '\xa9alb': [ytmusic_album['title']],
-            'aART': [self.get_artist(ytmusic_album['artists'])],
-            '\xa9ART': [self.get_artist(ytmusic_watch_playlist['tracks'][0]['artists'])],
-            '\xa9cmt': [f'https://music.youtube.com/watch?v={video_id}'],
-            'covr': [MP4Cover(self.get_cover(f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}=w1200-l94'))],
-            '\xa9nam': [ytmusic_watch_playlist['tracks'][0]['title']],
-            'stik': [1],
+            "album": ytmusic_album["title"],
+            "album_artist": self.get_artist(ytmusic_album["artists"]),
+            "artist": self.get_artist(ytmusic_watch_playlist["tracks"][0]["artists"]),
+            "comment": f"https://music.youtube.com/watch?v={video_id}",
+            "cover": self.get_cover(
+                f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}'
+                + f'=w{self.cover_size}-l{self.cover_quality}-{"rj" if self.cover_format == "jpg" else "rp"}'
+            ),
+            "media_type": 1,
+            "title": ytmusic_watch_playlist["tracks"][0]["title"],
+            "track_total": ytmusic_album["trackCount"],
         }
-        if ytmusic_album.get('year'):
-            tags['\xa9day'] = [ytmusic_album['year']]
-        if ytmusic_watch_playlist['lyrics']:
-            lyrics = self.ytmusic.get_lyrics(ytmusic_watch_playlist['lyrics'])['lyrics']        
-            if lyrics is not None:
-                tags['\xa9lyr'] = [lyrics]
-        total_tracks = ytmusic_album['trackCount']
-        track_number = 1
-        for video in self.get_ydl_extract_info(f'https://www.youtube.com/playlist?list={ytmusic_album["audioPlaylistId"]}')['entries']:
-            if video['id'] == video_id:
-                if ytmusic_album['tracks'][track_number - 1]['isExplicit']:
-                    tags['rtng'] = [1]
+        for i, video in enumerate(
+            self.get_ydl_extract_info(
+                f'https://www.youtube.com/playlist?list={ytmusic_album["audioPlaylistId"]}'
+            )["entries"]
+        ):
+            if video["id"] == video_id:
+                if ytmusic_album["tracks"][i]["isExplicit"]:
+                    tags["rating"] = 1
                 else:
-                    tags['rtng'] =  [0]
+                    tags["rating"] = 0
+                tags["track"] = i + 1
                 break
-            track_number += 1
-        tags['trkn'] = [(track_number, total_tracks)]
+        if ytmusic_watch_playlist["lyrics"]:
+            lyrics = self.ytmusic.get_lyrics(ytmusic_watch_playlist["lyrics"])["lyrics"]
+            if lyrics is not None:
+                tags["lyrics"] = lyrics
+        if ytmusic_album.get("year"):
+            tags["year"] = ytmusic_album["year"]
         return tags
-    
 
     def get_sanizated_string(self, dirty_string, is_folder):
-        for character in ['\\', '/', ':', '*', '?', '"', '<', '>', '|', ';']:
-            dirty_string = dirty_string.replace(character, '_')
+        dirty_string = re.sub(r'[\\/:*?"<>|;]', "_", dirty_string)
         if is_folder:
-            dirty_string = dirty_string[:40]
-            if dirty_string[-1:] == '.':
-                dirty_string = dirty_string[:-1] + '_'
+            dirty_string = dirty_string[: self.truncate]
+            if dirty_string.endswith("."):
+                dirty_string = dirty_string[:-1] + "_"
         else:
-            dirty_string = dirty_string[:36]
+            if self.truncate is not None:
+                dirty_string = dirty_string[: self.truncate - 4]
         return dirty_string.strip()
 
-    
     def get_temp_location(self, video_id):
-        return self.temp_path / f'{video_id}.mp4'
-    
+        return self.temp_path / f"{video_id}.m4a"
 
     def get_fixed_location(self, video_id):
-        return self.temp_path / f'{video_id}_fixed.m4a'
-    
+        return self.temp_path / f"{video_id}_fixed.m4a"
 
     def get_final_location(self, tags):
-        return self.final_path / self.get_sanizated_string(tags['aART'][0], True) / self.get_sanizated_string(tags['©alb'][0], True) / (self.get_sanizated_string(f'{tags["trkn"][0][0]:02d} {tags["©nam"][0]}', False) + '.m4a')
-    
+        final_location = self.final_path_structure.split("/")
+        final_location[-1] = (
+            self.get_sanizated_string(final_location[-1].format(**tags), False) + ".m4a"
+        )
+        for i, path in enumerate(final_location[:-1]):
+            final_location[i] = self.get_sanizated_string(path.format(**tags), True)
+        return self.final_path.joinpath(*final_location)
+
+    def get_cover_location(self, final_location):
+        return final_location.parent / f"Cover.{self.cover_format}"
 
     def download(self, video_id, temp_location):
         ydl_opts = {
-            'quiet': True,
-            'no_warnings': True,
-            'overwrites': self.overwrite,
-            'fixup': 'never',
-            'format': self.itag,
-            'outtmpl': str(temp_location),
+            "quiet": True,
+            "no_warnings": True,
+            "overwrites": self.overwrite,
+            "fixup": "never",
+            "format": self.itag,
+            "outtmpl": str(temp_location),
         }
-        if self.cookies_location.exists():
-            ydl_opts['cookiefile'] = str(self.cookies_location)
+        if self.cookies_location is not None:
+            ydl_opts["cookiefile"] = str(self.cookies_location)
         with YoutubeDL(ydl_opts) as ydl:
-            ydl.download('music.youtube.com/watch?v=' + video_id) 
-    
+            ydl.download("music.youtube.com/watch?v=" + video_id)
 
     def fixup(self, temp_location, fixed_location):
         fixup = [
-            'ffmpeg',
-            '-loglevel',
-            'error',
-            '-i',
+            self.ffmpeg_location,
+            "-loglevel",
+            "error",
+            "-i",
             temp_location,
         ]
-        if self.itag == '251':
-            fixup.extend([
-                '-f',
-                'mp4',
-            ])
+        if self.itag == "251":
+            fixup.extend(
+                [
+                    "-f",
+                    "mp4",
+                ]
+            )
         subprocess.run(
             [
                 *fixup,
-                '-c',
-                'copy',
+                "-movflags",
+                "+faststart",
+                "-c",
+                "copy",
                 fixed_location,
             ],
             check=True,
         )
-    
 
-    def make_final(self, final_location, fixed_location, tags):
+    def apply_tags(self, fixed_location, tags):
+        mp4 = MP4(fixed_location)
+        mp4.clear()
+        mp4["trkn"] = [[0, 0]]
+        for k, v in tags.items():
+            if k in self.exclude_tags:
+                continue
+            if k == "cover":
+                mp4["covr"] = [
+                    MP4Cover(
+                        v,
+                        imageformat=MP4Cover.FORMAT_JPEG
+                        if self.cover_format == "jpg"
+                        else MP4Cover.FORMAT_PNG,
+                    )
+                ]
+            elif k == "track":
+                mp4["trkn"][0][0] = v
+            elif k == "track_total":
+                mp4["trkn"][0][1] = v
+            else:
+                mp4[MP4_TAGS_MAP[k]] = [v]
+        mp4.save()
+
+    def move_to_final_location(self, fixed_location, final_location):
         final_location.parent.mkdir(parents=True, exist_ok=True)
-        shutil.copy(fixed_location, final_location)
-        file = MP4(final_location)
-        file.clear()
-        file.update(tags)
-        file.save(final_location)
-    
+        shutil.move(fixed_location, final_location)
+
+    def save_cover(self, tags, cover_location):
+        with open(cover_location, "wb") as f:
+            f.write(tags["cover"])
 
     def cleanup(self):
-        if not self.skip_cleanup and self.temp_path.exists():
-            shutil.rmtree(self.temp_path)
+        shutil.rmtree(self.temp_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

