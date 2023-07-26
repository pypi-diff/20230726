# Comparing `tmp/aioslimproto-2.3.2.tar.gz` & `tmp/aioslimproto-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslimproto-2.3.2.tar", last modified: Fri Jun  9 08:04:49 2023, max compression
+gzip compressed data, was "aioslimproto-2.3.3.tar", last modified: Wed Jul 26 19:17:43 2023, max compression
```

## Comparing `aioslimproto-2.3.2.tar` & `aioslimproto-2.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:04:49.897158 aioslimproto-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-09 08:04:49.897158 aioslimproto-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:04:49.885158 aioslimproto-2.3.2/aioslimproto/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    33850 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:04:49.893159 aioslimproto-2.3.2/aioslimproto/font/
--rw-r--r--   0 runner    (1001) docker     (123)   480716 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   540048 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   448868 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   499228 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   438596 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   504492 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   309664 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   201752 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   289124 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   209552 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   303604 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   475244 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   569008 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/aioslimproto/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:04:49.885158 aioslimproto-2.3.2/aioslimproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-09 08:04:49.000000 aioslimproto-2.3.2/aioslimproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-09 08:04:49.000000 aioslimproto-2.3.2/aioslimproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:04:49.000000 aioslimproto-2.3.2/aioslimproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:04:47.000000 aioslimproto-2.3.2/aioslimproto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 08:04:49.000000 aioslimproto-2.3.2/aioslimproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 08:04:49.000000 aioslimproto-2.3.2/aioslimproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-09 08:04:32.000000 aioslimproto-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:04:49.897158 aioslimproto-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:17:43.227552 aioslimproto-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 19:17:43.227552 aioslimproto-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:17:43.219552 aioslimproto-2.3.3/aioslimproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:17:43.227552 aioslimproto-2.3.3/aioslimproto/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   480716 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   540048 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   448868 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   499228 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   438596 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   504492 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   309664 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   201752 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   289124 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   209552 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   303604 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   475244 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   569008 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/aioslimproto/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:17:43.223552 aioslimproto-2.3.3/aioslimproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 19:17:42.000000 aioslimproto-2.3.3/aioslimproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-26 19:17:43.000000 aioslimproto-2.3.3/aioslimproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:17:42.000000 aioslimproto-2.3.3/aioslimproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:17:41.000000 aioslimproto-2.3.3/aioslimproto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-26 19:17:43.000000 aioslimproto-2.3.3/aioslimproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 19:17:43.000000 aioslimproto-2.3.3/aioslimproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-26 19:17:31.000000 aioslimproto-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:17:43.227552 aioslimproto-2.3.3/setup.cfg
```

### Comparing `aioslimproto-2.3.2/LICENSE` & `aioslimproto-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/PKG-INFO` & `aioslimproto-2.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Author-email: Marcel van der Veldt <marcelveldt@users.noreply.github.com>
 License: Apache-2.0
 Platform: any
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aioslimproto-2.3.2/aioslimproto/cli.py` & `aioslimproto-2.3.3/aioslimproto/cli.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/client.py` & `aioslimproto-2.3.3/aioslimproto/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 from collections.abc import Callable
 from enum import Enum, IntEnum
 from typing import TypedDict
 from urllib.parse import parse_qsl, urlparse
 
 from async_timeout import timeout
 
-from aioslimproto.display import SlimProtoDisplay
-
 from .const import FALLBACK_CODECS, EventType
+from .display import SlimProtoDisplay
 from .errors import UnsupportedContentType
 from .util import parse_capabilities, parse_headers
 from .visualisation import SpectrumAnalyser, VisualisationType
 from .volume import SlimProtoVolume
 
 # pylint: disable=unused-argument
 # ruff: noqa: ARG002
@@ -234,14 +233,15 @@
         self._jiffies: int = 0
         self._last_timestamp: float = 0
         self._elapsed_milliseconds: float = 0
         self._next_url: str | None = None
         self._next_metadata: Metadata | None = None
         self._connected: bool = False
         self._last_heartbeat = 0
+        self._auto_play: bool = False
         self._reader_task = create_task(self._socket_reader())
         self._heartbeat_task: asyncio.Task | None = None
 
     def disconnect(self) -> None:
         """Disconnect and/or cleanup socket client."""
         if self._reader_task and not self._reader_task.done():
             self._reader_task.cancel()
@@ -340,15 +340,14 @@
     def jiffies(self) -> int:
         """Return (realtime) epoch timestamp from player."""
         return self._jiffies + int((time.time() - self._last_timestamp) * 1000)
 
     async def stop(self) -> None:
         """Send stop command to player."""
         await self.send_strm(b"q", flags=0)
-        await self.set_display()
         # some players do not update their state by event so we force it here
         if self._state != PlayerState.STOPPED:
             self._state = PlayerState.STOPPED
             self.callback(EventType.PLAYER_UPDATED, self)
 
     async def play(self) -> None:
         """Send play/unpause command to player."""
@@ -378,15 +377,14 @@
         # mute is the same as power
         if not powered:
             await self.stop()
         power_int = 1 if powered else 0
         await self._send_frame(b"aude", struct.pack("2B", power_int, 1))
         self._powered = powered
         self.callback(EventType.PLAYER_UPDATED, self)
-        await self.set_display()
 
     async def toggle_power(self) -> None:
         """Toggle power command."""
         await self.power(not self.powered)
 
     async def volume_set(self, volume_level: int) -> None:
         """Send new volume level command to player."""
@@ -482,43 +480,42 @@
 
         if mime_type is None:
             # try to get the audio format from file extension
             ext = f'audio/{url.split(".")[-1]}'
             if ext in CODEC_MAPPING:
                 mime_type = ext
 
-        codec_details = self._parse_codc(mime_type)
+        codec_details = self._parse_codc(mime_type) if mime_type else b"?????"
 
         if port not in (80, 443, "80", "443"):
             host += f":{port}"
         httpreq = (
             b"GET %s HTTP/1.0\r\n"
             b"Host: %s\r\n"
             b"Connection: close\r\n"
             b"Accept: */*\r\n"
             b"Cache-Control: no-cache\r\n"
             b"User-Agent: VLC/3.0.9 LibVLC/3.0.9\r\n"
             b"Range: bytes=0-\r\n"
             b"\r\n" % (path.encode(), host.encode())
         )
-
+        self._auto_play = autostart
         await self.send_strm(
             command=b"s",
             codec_details=codec_details,
-            autostart=b"1" if autostart else b"0",
+            autostart=b"3" if autostart else b"0",
             server_port=port,
             server_ip=int(ipaddress.ip_address(ipaddr)),
             threshold=200,
             output_threshold=10,
             trans_duration=transition_duration,
             trans_type=transition.value,
             flags=0x20 if scheme == "https" else 0x00,
             httpreq=httpreq,
         )
-        await self.set_display()
 
     async def set_brightness(self, level=4):
         """Set brightness command on (supported) display."""
         assert 0 <= level <= 4
         await self._send_frame(b"grfb", struct.pack("!H", level))
 
     async def set_visualisation(self, visualisation: VisualisationType | None = None) -> None:
@@ -528,42 +525,32 @@
 
         def _handle():
             return visualisation.pack()
 
         data = await asyncio.get_running_loop().run_in_executor(None, _handle)
         await self._send_frame(b"visu", data)
 
-    async def render(
+    async def render_display_text(
         self,
         text: str,
         size: int = 16,
         position: tuple[int, int] = (0, 0),
         font: str = "DejaVu-Sans",
     ) -> None:
         """Render given text on display of (supported) slimproto client."""
 
         def _render():
             self._display_control.clear()
             self._display_control.renderText(text, font, size, position)
             return self._display_control.frame()
 
         bitmap = await asyncio.get_running_loop().run_in_executor(None, _render)
-        await self._update_display(bitmap)
+        await self.update_display(bitmap)
 
-    async def set_display(self) -> None:
-        """Render default text on player display."""
-        await self.set_visualisation()
-        if not self.powered:
-            await self.render("")
-        elif self._next_metadata and "title" in self._next_metadata:
-            await self.render(self._next_metadata["title"])
-        else:
-            await self.render(self.name)
-
-    async def _update_display(
+    async def update_display(
         self, bitmap: bytes, transition: str = "c", offset: int = 0, param: int = 0
     ) -> None:
         """Update display of (supported) slimproto client."""
         frame = struct.pack("!Hcb", offset, transition.encode(), param) + bitmap
         await self._send_frame(b"grfe", frame)
 
     async def _send_heartbeat(self) -> None:
@@ -619,19 +606,19 @@
         self.disconnect()
 
     async def send_strm(  # noqa: PLR0913
         self,
         command=b"q",
         autostart=b"0",
         codec_details=b"p1321",
-        threshold=255,
+        threshold=0,
         spdif=b"0",
         trans_duration=0,
         trans_type=b"0",
-        flags=0x40,
+        flags=0x20,
         output_threshold=0,
         replay_gain=0,
         server_port=0,
         server_ip=0,
         httpreq=b"",
     ) -> None:
         """Create stream request message based on given arguments."""
@@ -663,26 +650,23 @@
         self._player_id = str(device_mac).lower()
         self._device_type = DEVICE_TYPE.get(dev_id, "unknown device")
         self._capabilities = parse_capabilities(data)
         self.logger.debug("Player connected: %s", self.player_id)
         # Set some startup settings for the player
         await self._send_frame(b"vers", b"7.999.999")
         await self.stop()
-        await self.set_brightness()
-        await self.set_visualisation()
         await self._send_frame(b"setd", struct.pack("B", 0))
         await self._send_frame(b"setd", struct.pack("B", 4))
         await self.stop()
         # restore last power and volume levels
         # NOTE: this can be improved by storing the previous volume/power levels
         # so they can be restored when the player (re)connects.
         await self.power(self._powered)
         await self.volume_set(self.volume_level)
         self._connected = True
-        await self.set_display()
         self._heartbeat_task = asyncio.create_task(self._send_heartbeat())
         self.callback(EventType.PLAYER_CONNECTED, self)
 
     def _process_butn(self, data: bytes) -> None:
         """Handle 'butn' command from client."""
         timestamp, button = struct.unpack("!LL", data)
         # handle common buttons
@@ -804,14 +788,18 @@
     def _process_stat_stmo(self, data: bytes) -> None:
         """
         Process incoming stat STMo message.
 
         No more decoded (uncompressed) data to play; triggers rebuffering.
         """
         self.logger.debug("STMo received - output underrun.")
+        if self._auto_play:
+            asyncio.create_task(self.stop())
+        else:
+            self.callback(EventType.PLAYER_OUTPUT_UNDERRUN, self)
 
     def _process_stat_stmp(self, data: bytes) -> None:
         """Process incoming stat STMp message: Pause confirmed."""
         self.logger.debug("STMp received - pause confirmed.")
         self._state = PlayerState.PAUSED
         self.callback(EventType.PLAYER_UPDATED, self)
 
@@ -901,15 +889,16 @@
             codc_msg = self._parse_codc(content_type)
 
             # send the codc message to the player to inform about the codec that needs to be used
             self.logger.debug("send CODC for contenttype %s: %s", content_type, codc_msg)
             await self._send_frame(b"codc", codc_msg)
 
         # send continue (used when autoplay 1 or 3)
-        # await self._send_frame(b"cont", b"1")
+        if self._auto_play:
+            await self._send_frame(b"cont", b"1")
 
     def _process_setd(self, data: bytes) -> None:
         """Process incoming SETD message: Get/set player firmware settings."""
         data_id = data[0]
         if data_id == 0:
             # received player name
             self._device_name = data[1:-1].decode()
```

### Comparing `aioslimproto-2.3.2/aioslimproto/const.py` & `aioslimproto-2.3.3/aioslimproto/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     PLAYER_UPDATED = "player_updated"
     PLAYER_HEARTBEAT = "player_heartbeat"
     PLAYER_CONNECTED = "player_connected"
     PLAYER_DISCONNECTED = "player_disconnected"
     PLAYER_NAME_RECEIVED = "player_name_received"
     PLAYER_DECODER_READY = "player_decoder_ready"
     PLAYER_DECODER_ERROR = "player_decoder_error"
+    PLAYER_OUTPUT_UNDERRUN = "player_output_underrun"
     PLAYER_BUFFER_READY = "player_buffer_ready"
     PLAYER_CLI_EVENT = "player_cli_event"
     PLAYER_BTN_EVENT = "player_btn_event"
 
 
 @dataclass
 class SlimEvent:
```

### Comparing `aioslimproto-2.3.2/aioslimproto/discovery.py` & `aioslimproto-2.3.3/aioslimproto/discovery.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/display.py` & `aioslimproto-2.3.3/aioslimproto/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,21 @@
 
     def __init__(self, name):  # noqa
         self.filename = os.path.join(fontdir, name + ".ttf")
         self.cache = {}
 
     def render(self, s, size=15):
         """Return a PIL image with this string rendered into it."""
-        self.cache.setdefault(size, ImageFont.truetype(self.filename, size))
-        font = self.cache[size]
-        _size = font.getsize(s)
-        im = Image.new("RGB", _size)
+        if size not in self.cache:
+            self.cache[size] = ImageFont.truetype(self.filename, size)
+        font: ImageFont.FreeTypeFont = self.cache[size]
+        bbox = font.getbbox(s)
+        width = abs(bbox[0] - bbox[2])
+        height = abs(bbox[1] - bbox[3])
+        im = Image.new("RGB", (width, height))
         draw = ImageDraw.Draw(im)
         draw.text((0, 0), s, font=font)
         return im
 
 
 class SlimProtoDisplay:
     """Reresentation of a Slimproto display."""
```

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Bold.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Condensed.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Condensed.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Mono.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Mono.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans-Oblique.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/font/DejaVu-Sans.ttf` & `aioslimproto-2.3.3/aioslimproto/font/DejaVu-Sans.ttf`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/server.py` & `aioslimproto-2.3.3/aioslimproto/server.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/util.py` & `aioslimproto-2.3.3/aioslimproto/util.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/visualisation.py` & `aioslimproto-2.3.3/aioslimproto/visualisation.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto/volume.py` & `aioslimproto-2.3.3/aioslimproto/volume.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/aioslimproto.egg-info/PKG-INFO` & `aioslimproto-2.3.3/aioslimproto.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Author-email: Marcel van der Veldt <marcelveldt@users.noreply.github.com>
 License: Apache-2.0
 Platform: any
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aioslimproto-2.3.2/aioslimproto.egg-info/SOURCES.txt` & `aioslimproto-2.3.3/aioslimproto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.3.2/pyproject.toml` & `aioslimproto-2.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioslimproto"
-version = "2.3.2"
+version = "2.3.3"
 license     = {text = "Apache-2.0"}
 description = "Python module to talk to Logitech Squeezebox players directly (without Logitech server)."
 readme = "README.md"
 requires-python = ">=3.10"
 authors     = [
     {name = "Marcel van der Veldt", email = "marcelveldt@users.noreply.github.com"}
 ]
@@ -20,23 +20,23 @@
 dependencies = [
   "async-timeout",
   "pillow",
 ]
 
 [project.optional-dependencies]
 test = [
-  "black==23.3.0",
-  "codespell==2.2.4",
-  "mypy==1.3.0",
-  "ruff==0.0.270",
-  "pytest==7.3.1",
-  "pytest-asyncio==0.21.0",
+  "black==23.7.0",
+  "codespell==2.2.5",
+  "mypy==1.4.1",
+  "ruff==0.0.280",
+  "pytest==7.4.0",
+  "pytest-asyncio==0.21.1",
   "pytest-aiohttp==1.0.4",
   "pytest-cov==4.1.0",
-  "pre-commit==3.3.2",
+  "pre-commit==3.3.3",
   "pylint==2.17.4",
 ]
 
 [tool.black]
 target-version = ['py311']
 line-length = 100
```

