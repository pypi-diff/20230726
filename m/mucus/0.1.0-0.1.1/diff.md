# Comparing `tmp/mucus-0.1.0.tar.gz` & `tmp/mucus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mucus-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mucus-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mucus-0.1.0.tar` & `mucus-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1080 2023-07-08 19:18:21.319940 mucus-0.1.0/LICENSE
--rw-r--r--   0        0        0        8 2023-07-26 08:26:32.928030 mucus-0.1.0/README.md
--rw-r--r--   0        0        0      460 2023-07-23 09:19:31.118921 mucus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-23 09:20:19.278311 mucus-0.1.0/src/mucus/__init__.py
--rw-r--r--   0        0        0     1660 2023-07-26 08:06:09.788590 mucus-0.1.0/src/mucus/cli.py
--rw-r--r--   0        0        0     1123 2023-07-26 09:50:40.666457 mucus-0.1.0/src/mucus/command.py
--rw-r--r--   0        0        0        0 2023-07-14 18:45:04.594124 mucus-0.1.0/src/mucus/commands/__init__.py
--rw-r--r--   0        0        0      131 2023-07-26 10:02:35.095993 mucus-0.1.0/src/mucus/commands/clear.py
--rw-r--r--   0        0        0     1047 2023-07-26 09:56:08.823151 mucus-0.1.0/src/mucus/commands/download.py
--rw-r--r--   0        0        0      162 2023-07-26 09:56:28.079625 mucus-0.1.0/src/mucus/commands/exit.py
--rw-r--r--   0        0        0      191 2023-07-26 09:56:46.319443 mucus-0.1.0/src/mucus/commands/next.py
--rw-r--r--   0        0        0      233 2023-07-26 09:57:01.405959 mucus-0.1.0/src/mucus/commands/pause.py
--rw-r--r--   0        0        0      657 2023-07-26 09:59:34.777771 mucus-0.1.0/src/mucus/commands/queue.py
--rw-r--r--   0        0        0     1063 2023-07-26 10:01:03.160234 mucus-0.1.0/src/mucus/commands/search.py
--rw-r--r--   0        0        0      237 2023-07-26 10:01:27.036665 mucus-0.1.0/src/mucus/commands/start.py
--rw-r--r--   0        0        0      258 2023-07-26 10:01:43.083174 mucus-0.1.0/src/mucus/commands/state.py
--rw-r--r--   0        0        0      139 2023-07-26 10:02:00.846331 mucus-0.1.0/src/mucus/commands/stop.py
--rw-r--r--   0        0        0      350 2023-07-23 09:20:41.448033 mucus-0.1.0/src/mucus/config.py
--rw-r--r--   0        0        0      145 2023-07-20 20:26:15.274026 mucus-0.1.0/src/mucus/config_default.yaml
--rw-r--r--   0        0        0      651 2023-07-26 08:07:23.174223 mucus-0.1.0/src/mucus/deezer/auth.py
--rw-r--r--   0        0        0     1353 2023-07-26 08:24:55.954642 mucus-0.1.0/src/mucus/deezer/client.py
--rw-r--r--   0        0        0      458 2023-07-25 19:32:10.645725 mucus-0.1.0/src/mucus/deezer/decrypter.py
--rw-r--r--   0        0        0       83 2023-07-25 19:37:45.409177 mucus-0.1.0/src/mucus/deezer/exception.py
--rw-r--r--   0        0        0      999 2023-07-25 19:30:43.073236 mucus-0.1.0/src/mucus/deezer/page.py
--rw-r--r--   0        0        0     1136 2023-07-25 19:31:46.095962 mucus-0.1.0/src/mucus/deezer/stream.py
--rw-r--r--   0        0        0       41 2023-07-18 12:20:36.232004 mucus-0.1.0/src/mucus/exception.py
--rw-r--r--   0        0        0     1049 2023-07-18 18:49:14.290250 mucus-0.1.0/src/mucus/history.py
--rw-r--r--   0        0        0      352 2023-07-16 08:38:14.066367 mucus-0.1.0/src/mucus/lazy.py
--rw-r--r--   0        0        0     1591 2023-07-23 09:20:04.105169 mucus-0.1.0/src/mucus/play.py
--rw-r--r--   0        0        0      531 2023-07-20 20:28:58.582002 mucus-0.1.0/src/mucus/song.py
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 mucus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-08 19:18:21.319940 mucus-0.1.1/LICENSE
+-rw-r--r--   0        0        0        8 2023-07-26 08:26:32.928030 mucus-0.1.1/README.md
+-rw-r--r--   0        0        0      460 2023-07-23 09:19:31.118921 mucus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-26 18:11:24.351570 mucus-0.1.1/src/mucus/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-26 18:05:10.835235 mucus-0.1.1/src/mucus/cli.py
+-rw-r--r--   0        0        0     1122 2023-07-26 18:05:00.691998 mucus-0.1.1/src/mucus/command.py
+-rw-r--r--   0        0        0        0 2023-07-14 18:45:04.594124 mucus-0.1.1/src/mucus/commands/__init__.py
+-rw-r--r--   0        0        0      131 2023-07-26 10:02:35.095993 mucus-0.1.1/src/mucus/commands/clear.py
+-rw-r--r--   0        0        0     1047 2023-07-26 09:56:08.823151 mucus-0.1.1/src/mucus/commands/download.py
+-rw-r--r--   0        0        0      153 2023-07-26 18:05:29.498390 mucus-0.1.1/src/mucus/commands/exit.py
+-rw-r--r--   0        0        0      191 2023-07-26 09:56:46.319443 mucus-0.1.1/src/mucus/commands/next.py
+-rw-r--r--   0        0        0      233 2023-07-26 09:57:01.405959 mucus-0.1.1/src/mucus/commands/pause.py
+-rw-r--r--   0        0        0      657 2023-07-26 09:59:34.777771 mucus-0.1.1/src/mucus/commands/queue.py
+-rw-r--r--   0        0        0     1063 2023-07-26 10:01:03.160234 mucus-0.1.1/src/mucus/commands/search.py
+-rw-r--r--   0        0        0      237 2023-07-26 10:01:27.036665 mucus-0.1.1/src/mucus/commands/start.py
+-rw-r--r--   0        0        0      230 2023-07-26 14:12:18.880166 mucus-0.1.1/src/mucus/commands/state.py
+-rw-r--r--   0        0        0      139 2023-07-26 10:02:00.846331 mucus-0.1.1/src/mucus/commands/stop.py
+-rw-r--r--   0        0        0      350 2023-07-23 09:20:41.448033 mucus-0.1.1/src/mucus/config.py
+-rw-r--r--   0        0        0      145 2023-07-20 20:26:15.274026 mucus-0.1.1/src/mucus/config_default.yaml
+-rw-r--r--   0        0        0      563 2023-07-26 14:47:10.039749 mucus-0.1.1/src/mucus/deezer/auth.py
+-rw-r--r--   0        0        0     1353 2023-07-26 08:24:55.954642 mucus-0.1.1/src/mucus/deezer/client.py
+-rw-r--r--   0        0        0      428 2023-07-26 10:11:22.690777 mucus-0.1.1/src/mucus/deezer/decrypter.py
+-rw-r--r--   0        0        0       83 2023-07-25 19:37:45.409177 mucus-0.1.1/src/mucus/deezer/exception.py
+-rw-r--r--   0        0        0      999 2023-07-25 19:30:43.073236 mucus-0.1.1/src/mucus/deezer/page.py
+-rw-r--r--   0        0        0     1136 2023-07-25 19:31:46.095962 mucus-0.1.1/src/mucus/deezer/stream.py
+-rw-r--r--   0        0        0      150 2023-07-26 18:08:39.539866 mucus-0.1.1/src/mucus/exception.py
+-rw-r--r--   0        0        0     1253 2023-07-26 14:48:46.268852 mucus-0.1.1/src/mucus/history.py
+-rw-r--r--   0        0        0      352 2023-07-16 08:38:14.066367 mucus-0.1.1/src/mucus/lazy.py
+-rw-r--r--   0        0        0     1633 2023-07-26 18:08:41.023185 mucus-0.1.1/src/mucus/play.py
+-rw-r--r--   0        0        0      531 2023-07-20 20:28:58.582002 mucus-0.1.1/src/mucus/song.py
+-rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 mucus-0.1.1/PKG-INFO
```

### Comparing `mucus-0.1.0/LICENSE` & `mucus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/cli.py` & `mucus-0.1.1/src/mucus/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python3
 
 import click
 
 import mucus.command
 import mucus.config
 import mucus.deezer.client
+import mucus.deezer.exception
 import mucus.exception
 import mucus.history
 import mucus.play
 
 
 @click.command()
 @click.option('--alias', '-a', 'aliases', type=(str, str), multiple=True)
 def command(aliases):
     aliases = dict(aliases)
     config = mucus.config.Config()
 
     with mucus.history.History(__name__) as history:
-        client = mucus.deezer.client.Client()
+        try:
+            client = mucus.deezer.client.Client()
+        except mucus.deezer.exception.AuthException as e:
+            raise click.ClickException(e)
         player = mucus.play.Player(client)
         player.start()
 
         def inputs():
             while True:
                 try:
                     yield input('> ')
@@ -49,15 +53,15 @@
                     'history': history,
                     'player': player
                 }
             )
 
             try:
                 runner()
-            except mucus.exception.ExitException:
+            except mucus.exception.Exit:
                 break
             except Exception as e:
                 raise click.ClickException(e)
 
 
 def main():
     return command(default_map=mucus.config.Config().flatten())
```

### Comparing `mucus-0.1.0/src/mucus/command.py` & `mucus-0.1.1/src/mucus/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+from mucus.exception import NoSuchCommand
 from mucus.lazy import import_module as lazy_import
 
 
 class Command:
     pass
 
 
@@ -36,11 +37,7 @@
 class Runner:
     def __init__(self, loader, context):
         self.loader = loader
         self.context = context
 
     def __call__(self):
         return self.loader.cmd(**self.context)
-
-
-class NoSuchCommand(Exception):
-    pass
```

### Comparing `mucus-0.1.0/src/mucus/commands/download.py` & `mucus-0.1.1/src/mucus/commands/download.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/commands/queue.py` & `mucus-0.1.1/src/mucus/commands/queue.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/commands/search.py` & `mucus-0.1.1/src/mucus/commands/search.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/deezer/client.py` & `mucus-0.1.1/src/mucus/deezer/client.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/deezer/page.py` & `mucus-0.1.1/src/mucus/deezer/page.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/deezer/stream.py` & `mucus-0.1.1/src/mucus/deezer/stream.py`

 * *Files identical despite different names*

### Comparing `mucus-0.1.0/src/mucus/history.py` & `mucus-0.1.1/src/mucus/history.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 class History:
     def __init__(self, namespace, n=1000, sep=':'):
         self.namespace = namespace
         self.n = n
         self.sep = sep
 
     def __enter__(self):
-        with redis.Redis(decode_responses=True) as db:
-            self.backup = [readline.get_history_item(i+1)
-                           for i in range(readline.get_current_history_length())] # noqa
-            readline.clear_history()
-            for item in db.lrange(self.key, -self.n, -1):
-                readline.add_history(item)
-            db.expire(self.key, 86400)
+        try:
+            with redis.Redis(decode_responses=True) as db:
+                self.backup = [readline.get_history_item(i+1)
+                               for i in range(readline.get_current_history_length())] # noqa
+                readline.clear_history()
+                for item in db.lrange(self.key, -self.n, -1):
+                    readline.add_history(item)
+                db.expire(self.key, 86400)
+        except redis.exceptions.RedisError:
+            pass
 
     def __exit__(self, *args):
-        with redis.Redis(decode_responses=True) as db:
-            for i in range(readline.get_current_history_length()):
-                db.rpush(self.key, readline.get_history_item(i+1))
-            db.expire(self.key, 86400)
-            readline.clear_history()
-            for item in self.backup:
-                readline.add_history(item)
+        try:
+            with redis.Redis(decode_responses=True) as db:
+                for i in range(readline.get_current_history_length()):
+                    db.rpush(self.key, readline.get_history_item(i+1))
+                db.expire(self.key, 86400)
+                readline.clear_history()
+                for item in self.backup:
+                    readline.add_history(item)
+        except redis.exceptions.RedisError:
+            pass
 
     @property
     def key(self):
         return self.sep.join((__name__, self.namespace))
```

### Comparing `mucus-0.1.0/src/mucus/play.py` & `mucus-0.1.1/src/mucus/play.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import queue
 import subprocess
 import threading
 import time
 
-import mucus.song
+from mucus.exception import NoMedia, NoSource
+from mucus.song import Song
 
 
 class Player:
     def __init__(self, client):
         self.client = client
         self.queue = queue.Queue()
         self.events = {name: threading.Event() for name in ('pause', 'stop')}
@@ -15,21 +16,21 @@
         self.state = {}
 
     def play(self, song):
         data = self.client.stream(song)
 
         media = next(data)
         if media is None:
-            raise Exception
+            raise NoMedia
 
         source = next(data)
         if source is None:
-            raise Exception
+            raise NoSource
 
-        song = mucus.song.Song(data=song)
+        song = Song(data=song)
 
         self.state.update({'song': song})
 
         with subprocess.Popen(['sox', '-', '-d', '-q', '-V0'], stdin=subprocess.PIPE) as p: # noqa
             for chunk in data:
                 if self.events['stop'].is_set():
                     break
@@ -37,15 +38,15 @@
                     time.sleep(0.1)
                 p.stdin.write(chunk)
 
         self.state.update({'last_song': song, 'song': None})
 
     def loop(self):
         self.events['stop'].clear()
-        self.state.update({'state': 'running'})
+        self.state.update({'state': 'playing'})
         while not self.events['stop'].is_set():
             try:
                 song = self.queue.get(timeout=1)
             except queue.Empty:
                 continue
             if song is None:
                 break
```

### Comparing `mucus-0.1.0/src/mucus/song.py` & `mucus-0.1.1/src/mucus/song.py`

 * *Files identical despite different names*

