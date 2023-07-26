# Comparing `tmp/image-go-nord-0.1.6.tar.gz` & `tmp/image-go-nord-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-go-nord-0.1.6.tar", last modified: Sun Jul 23 22:24:56 2023, max compression
+gzip compressed data, was "image-go-nord-0.1.7.tar", last modified: Wed Jul 26 18:58:56 2023, max compression
```

## Comparing `image-go-nord-0.1.6.tar` & `image-go-nord-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/
--rwxr-xr-x   0 root         (0) root         (0)    20646 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/GoNord.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/GoNord_test.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/palettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/palettes/Nord/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/palettes/Nord/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/palettes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/ImageGoNord/utility/
--rwxr-xr-x   0 root         (0) root         (0)     2330 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/ConvertUtility.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/palette_loader.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/ImageGoNord/utility/quantize.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       16 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4870 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/image_go_nord.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5904 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-23 22:24:56.000000 image-go-nord-0.1.6/image_go_nord.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 22:24:56.881472 image-go-nord-0.1.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1553 2023-07-23 22:24:35.000000 image-go-nord-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/
+-rwxr-xr-x   0 root         (0) root         (0)    21892 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/GoNord.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/GoNord_test.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/palettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/palettes/Nord/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/palettes/Nord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/palettes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/ImageGoNord/utility/
+-rwxr-xr-x   0 root         (0) root         (0)     2330 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/ConvertUtility.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/palette_loader.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/ImageGoNord/utility/quantize.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       16 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:58:56.886544 image-go-nord-0.1.7/image_go_nord.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      506 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 18:58:56.000000 image-go-nord-0.1.7/image_go_nord.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:58:56.890544 image-go-nord-0.1.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1553 2023-07-26 18:58:34.000000 image-go-nord-0.1.7/setup.py
```

### Comparing `image-go-nord-0.1.6/ImageGoNord/GoNord.py` & `image-go-nord-0.1.7/ImageGoNord/GoNord.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import threading
 
 from PIL import Image, ImageFilter
 
 import numpy as np
 import ffmpeg
 import uuid
+import shutil
 
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
@@ -573,28 +574,28 @@
         # If images is a list, convert to ndarray
         if not isinstance(images, np.ndarray):
             images = np.asarray(images)
         height, width = images.shape[1:3]
         process = (
             ffmpeg
                 .input('pipe:', format='rawvideo', pix_fmt='rgb24', r=framerate, s='{}x{}'.format(width, height))
-                .output(fn, pix_fmt='yuv420p', vcodec=vcodec, loglevel='quiet')
+                .output(fn, pix_fmt='yuv420p', vcodec=vcodec, loglevel='quiet', tune='fastdecode', preset='ultrafast')
                 .overwrite_output()
                 .run_async(pipe_stdin=True)
         )
         for idx, frame in enumerate(images):
             process.stdin.write(
                 ConvertUtility.convert_palette(cube, frame)
                     .astype(np.uint8)
                     .tobytes()
             )
         process.stdin.close()
         process.wait()
 
-    def concat_video(self, uid, out):
+    def concat_video(self, uid, out, save_path):
         """
         Concatenate two videos
 
         Parameters
         ----------
         uid : str
             Unique identifier for the session
@@ -604,50 +605,79 @@
         Returns
         -------
         None
             Concatenate two videos and save to disk
         """
         
         main = ffmpeg.input(out)
-        temp = ffmpeg.input(f'temp_{uid}.mp4')
+        temp = ffmpeg.input(os.path.join(save_path, f'temp_{uid}.mp4'))
         (
             ffmpeg
             .filter([main, temp],'concat')
-            .output(f'output_{uid}.mp4', pix_fmt='rgb24', loglevel='quiet')
+            .output(os.path.join(save_path, f'output_{uid}.mp4'), pix_fmt='rgb24', loglevel='quiet', tune='fastdecode', preset='ultrafast')
             .overwrite_output()
             .run(capture_stdout=True)
         )
         os.remove(out)
-        os.remove(f'temp_{uid}.mp4')
-        os.rename(f'output_{uid}.mp4', out)
+        os.remove(os.path.join(save_path, f'temp_{uid}.mp4'))
+        os.rename(os.path.join(save_path, f'output_{uid}.mp4'), out)
 
-    def convert_video(self, _input, palette_name, _frames_per_batch = 200):
+    def apply_original_audio(self, _input, _output):
+        """
+        Concatenate two videos
+
+        Parameters
+        ----------
+        _input : str
+            Input video file path
+        _output : str
+            Output video file path
+
+        Returns
+        -------
+        None
+            Apply the original audio to the output video
+        """
+        tmp_filename = '/tmp/' + str(uuid.uuid4())
+        shutil.copyfile(_output, tmp_filename)
+        output_video_stream = ffmpeg.input(tmp_filename).video
+        input_audio_stream = ffmpeg.input(_input).audio
+        (ffmpeg
+          .output(output_video_stream, input_audio_stream, _output, loglevel='quiet', tune='fastdecode', preset='ultrafast')
+          .overwrite_output()
+          .run()
+        )
+        os.remove(tmp_filename)
+
+    def convert_video(self, _input, palette_name, _frames_per_batch = 200, save_path = '/tmp'):
         """
         Concatenate two videos
 
         Parameters
         ----------
         _input : str
             Input video file path
         palette_name : str
             Name of palette to choose
         _frames_per_batch : int / optional
             Number of frames to keep in a batch
             Higher number indicates more memory usage but faster execution due to lesser number of parts 
+        save_path : str
+            Location where to save the output video
 
         Returns
         -------
         None
             Convert input video and save to disk
         """
         # Generate some random unique identifier that is generated for each session for the temporary files.
         uid = uuid.uuid4()
         palette = list(self.PALETTE_DATA.values())
 
-        _output = _input.split('.')[0] + str(uid) +'_converted.mp4'
+        _output = os.path.join(save_path, _input.split('.')[0] + str(uid) +'_converted.mp4')
         # run once to generate the color map file
         try:
             # for all colors (256*256*256) assign color from palette
             precalculated = np.load(f'{palette_name}.npz')['color_cube']
         except:
             pl.generate_color_map(palette, palette_name)
             precalculated = np.load(f'{palette_name}.npz')['color_cube']
@@ -661,17 +691,21 @@
         batch_dur = frames_per_batch / framerate
         batch_dur = batch_dur if duration > batch_dur else duration
 
         # Process the entire video in batches of `frames_per_batch` frames
         while frame_number < total_frames:
             np_arr = self.convert_vid_to_np_arr(_input, width, height, timestamp, batch_dur)
             if os.path.exists(_output):
-                self.vidwrite(f'temp_{uid}.mp4', precalculated, np_arr, framerate, frame_number, total_frames)
-                self.concat_video(uid, _output)
+                self.vidwrite(os.path.join(save_path, f'temp_{uid}.mp4'), precalculated, np_arr, framerate, frame_number, total_frames)
+                self.concat_video(uid, _output, save_path)
             else:
                 self.vidwrite(_output, precalculated, np_arr, framerate, frame_number, total_frames)
             if (total_frames - frame_number) < frames_per_batch:
                 frames_per_batch = total_frames - frame_number
             frame_number += frames_per_batch
             duration -= batch_dur
             timestamp += batch_dur 
             batch_dur = batch_dur if duration > batch_dur else duration
+
+        self.apply_original_audio(_input, _output)
+
+        return _output
```

### Comparing `image-go-nord-0.1.6/ImageGoNord/GoNord_test.py` & `image-go-nord-0.1.7/ImageGoNord/GoNord_test.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/ImageGoNord/utility/ConvertUtility.py` & `image-go-nord-0.1.7/ImageGoNord/utility/ConvertUtility.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/ImageGoNord/utility/palette_loader.py` & `image-go-nord-0.1.7/ImageGoNord/utility/palette_loader.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/ImageGoNord/utility/quantize.py` & `image-go-nord-0.1.7/ImageGoNord/utility/quantize.py`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/LICENSE` & `image-go-nord-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/PKG-INFO` & `image-go-nord-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool for converting RGB image to Nordtheme palette
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: MIT
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
```

### Comparing `image-go-nord-0.1.6/README.md` & `image-go-nord-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `image-go-nord-0.1.6/image_go_nord.egg-info/PKG-INFO` & `image-go-nord-0.1.7/image_go_nord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-go-nord
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool for converting RGB image to Nordtheme palette
 Home-page: https://github.com/Schrodinger-Hat/ImageGoNord-pip
 Author: Schrodinger Hat
 Author-email: schrodinger.hat.show@gmail.com
 License: MIT
 Download-URL: https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases
 Project-URL: Homepage, https://ign.schrodinger-hat.it
```

### Comparing `image-go-nord-0.1.6/setup.py` & `image-go-nord-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 ROOT = pathlib.Path('.')
 README = (ROOT / "README.md").read_text()
 
 setup(
     name="image-go-nord",
-    version="0.1.6",
+    version="0.1.7",
     description="A tool for converting RGB image to Nordtheme palette",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Schrodinger-Hat/ImageGoNord-pip",
     download_url = 'https://github.com/Schrodinger-Hat/ImageGoNord-pip/releases',
     keywords = ['nordtheme', 'pillow', 'image', 'conversion', 'rgb', 'color-scheme', 'color-palette'], 
     author="Schrodinger Hat",
```

