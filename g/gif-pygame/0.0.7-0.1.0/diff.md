# Comparing `tmp/gif_pygame-0.0.7.tar.gz` & `tmp/gif_pygame-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-0.0.7.tar", last modified: Mon May  1 02:38:47 2023, max compression
+gzip compressed data, was "gif_pygame-0.1.0.tar", last modified: Wed Jul 26 14:52:32 2023, max compression
```

## Comparing `gif_pygame-0.0.7.tar` & `gif_pygame-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.017755 gif_pygame-0.0.7/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4436 2023-05-01 02:38:47.015742 gif_pygame-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-03-27 21:27:19.000000 gif_pygame-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.003222 gif_pygame-0.0.7/gif_pygame/
--rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.0.7/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0    18959 2023-05-01 02:37:59.000000 gif_pygame-0.0.7/gif_pygame/_pygame_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:38:47.015742 gif_pygame-0.0.7/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     4436 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 02:38:46.000000 gif_pygame-0.0.7/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 02:38:47.017755 gif_pygame-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-05-01 02:38:28.000000 gif_pygame-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.218022 gif_pygame-0.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4440 2023-07-26 14:52:32.217022 gif_pygame-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3456 2023-07-26 14:43:13.000000 gif_pygame-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.202004 gif_pygame-0.1.0/gif_pygame/
+-rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.1.0/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0    22554 2023-07-26 14:47:22.000000 gif_pygame-0.1.0/gif_pygame/_pygame_gif.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.216016 gif_pygame-0.1.0/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     4440 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:52:32.218022 gif_pygame-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2023-07-26 14:51:46.000000 gif_pygame-0.1.0/setup.py
```

### Comparing `gif_pygame-0.0.7/LICENSE` & `gif_pygame-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.0.7/PKG-INFO` & `gif_pygame-0.1.0/gif_pygame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gif_pygame
-Version: 0.0.7
+Name: gif-pygame
+Version: 0.1.0
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -77,18 +77,18 @@
 There are other extra functions. The ones showcased in the example code are `img.pause()` and `img.unpause()`.
 
 There are also:
 - `.get_width()`, returns the width of the image
 - `.get_height()`, returns the height of the image
 - `.get_size()`, returns the size of the image
 - `.get_rect()`, returns the rect of the image
-- `.get_surface()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
+- `.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
-- `.get_duration()`, returns a list of all durations in the animation, you can also pass in certain indexes
+- `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
 - `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_data()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
+- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
 - `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alpha()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
+- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
 - `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
 - `.convert()`, converts all the surfaces in the animation, you can also pass in a `colorkey` and certain indexes
 
 Please use python's `help()` function for more in-depth explanation
```

### Comparing `gif_pygame-0.0.7/README.md` & `gif_pygame-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 There are other extra functions. The ones showcased in the example code are `img.pause()` and `img.unpause()`.
 
 There are also:
 - `.get_width()`, returns the width of the image
 - `.get_height()`, returns the height of the image
 - `.get_size()`, returns the size of the image
 - `.get_rect()`, returns the rect of the image
-- `.get_surface()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
+- `.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
-- `.get_duration()`, returns a list of all durations in the animation, you can also pass in certain indexes
+- `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
 - `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_data()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
+- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
 - `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alpha()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
+- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
 - `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
 - `.convert()`, converts all the surfaces in the animation, you can also pass in a `colorkey` and certain indexes
 
 Please use python's `help()` function for more in-depth explanation
```

### Comparing `gif_pygame-0.0.7/gif_pygame/_pygame_gif.py` & `gif_pygame-0.1.0/gif_pygame/_pygame_gif.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     >>> # rendering
     >>> loaded_gif.render(surface, (x, y)) # Renders and animates the animated image. THIS FUNCTION SHOULD NOT BE USED WITH `surface.blit()`
     >>> # or
     >>> surface.blit(loaded_gif.blit_ready(), (x, y)) # Animates the animated image and returns the current frame. Unlike `gif.render()`, this can be used with `surface.blit()`
 """
 
-import pygame, time
+import pygame, time, warnings
 
 from PIL import Image
 from typing import Union, Tuple, Sequence, List, SupportsIndex, Iterable, Optional
 
 _Coordinate = Union[Tuple[float, float], Sequence[float], pygame.Vector2]
 _CanBeRect = Union[pygame.Rect, Tuple[int, int, int, int], Tuple[_Coordinate, _Coordinate], Tuple[_Coordinate]]
 _FileArg = Union[str, bytes]
@@ -107,24 +107,46 @@
         """
         Returns the rect of the .gif/.apng file
 
         :param kwargs: (optional) The the keyword arguments that will be passed in to the `surface.get_rect()` function.
         """
         return self.frames[0][0].get_rect(**kwargs)
 
+    def get_surfaces(self, frames=[]):
+        """
+        Returns the surface of the selected frame(s)
+        
+        :param frames: (optional) Get the surface of the selected frames, leave empty to get all of the surfaces
+        """
+        if len(frames) == 0:
+            selected_frames = self.frames.copy()
+        else:
+            selected_frames = []
+            for frame in frames:
+                try:
+                    selected_frames.append(self.frames[frame])
+                except IndexError:
+                    print(f"Index {frame} does not exist, so it will be skipped")
+
+        l = [frame[0] for frame in selected_frames]
+        if len(l) == 1:
+            l = l[0]
+        return l
+
     def get_surface(self, select_frame: Optional[Union[None, SupportsIndex]] = None, first_frame: Optional[Union[None, SupportsIndex]] = None, last_frame: Optional[Union[None, SupportsIndex]] = None) -> List[pygame.Surface]:
         """
         Returns the surface of the selected frame(s)
         
         :param select_frame: (optional) Get the surface of only 1 frame, will ignore `first_frame` and `last_frame`, leave as `None` to use `first_frame` and `last_frame`
         :param first_frame: (optional) The first frame in the frames to get the surface from, leave as `None` to start from the first frame
         :param last_frame: (optional) The last frame in the frames to get the surface from, leave as `None` to end at the last frame
         
         Leave everything as `None` to get the surface all of the frames
         """
+        warnings.warn("gif_pygame.PygameGIF.get_surface deprecated since 0.1.0, use gif_pygame.PygameGIF.get_surfaces instead", DeprecationWarning, 2)
         selected_frames = self._grab_frame(select_frame, first_frame, last_frame)
 
         l = [frame[0] for frame in selected_frames]
         if len(l) == 1:
             l = l[0]
         return l
 
@@ -167,24 +189,46 @@
                 print(failed_str)
             if len(duplicated_frames):
                 duplicated_str = "There were some duplicated frames, they were:\n"
                 for duplicated_frame in duplicated_frames:
                     duplicated_str += f"Frame Number: {duplicated_frame[1]}, Index: {duplicated_frame[0]}"
                 print(duplicated_str)
 
+    def get_durations(self, frames=[]):
+        """
+        Returns the duration of the selected frame(s)
+        
+        :param frames: (optional) Get the surface of the selected frames, leave empty to get all of the durations
+        """
+        if len(frames) == 0:
+            selected_frames = self.frames.copy()
+        else:
+            selected_frames = []
+            for frame in frames:
+                try:
+                    selected_frames.append(self.frames[frame])
+                except IndexError:
+                    print(f"Index {frame} does not exist, so it will be skipped")
+
+        l = [frame[1] for frame in selected_frames]
+        if len(l) == 1:
+            l = l[0]
+        return l
+
     def get_duration(self, select_frame: Optional[Union[None, SupportsIndex]] = None, first_frame: Optional[Union[None, SupportsIndex]] = None, last_frame: Optional[Union[None, SupportsIndex]] = None) -> List[float]:
         """
         Returns the duration of the selected frame(s) in seconds
         
         :param select_frame: (optional) Get the duration of only 1 frame, will ignore `first_frame` and `last_frame`, leave as `None` to use `first_frame` and `last_frame`
         :param first_frame: (optional) The first frame in the frames to get the duration from, leave as `None` to start from the first frame
         :param last_frame: (optional) The last frame in the frames to get the duration from, leave as `None` to end at the last frame
 
         Leave everything as `None` to get the duration all of the frames
         """
+        warnings.warn("gif_pygame.PygameGIF.get_duration deprecated since 0.1.0, use gif_pygame.PygameGIF.get_durations instead", DeprecationWarning, 2)
         selected_frames = self._grab_frame(select_frame, first_frame, last_frame)
 
         l = [frame[1] for frame in selected_frames]
         if len(l) == 1:
             l = l[0]
         return l
 
@@ -227,24 +271,46 @@
                 print(failed_str)
             if len(duplicated_frames):
                 duplicated_str = "There were some duplicated frames, they were:\n"
                 for duplicated_frame in duplicated_frames:
                     duplicated_str += f"Frame Number: {duplicated_frame[1]}, Index: {duplicated_frame[0]}"
                 print(duplicated_str)
 
+    def get_datas(self, frames=[]):
+        """
+        Returns both the surface and the duration of the selected frame(s)
+        
+        :param frames: (optional) Get the surface of the selected frames, leave empty to get the surface and duration of all of the frames
+        """
+        if len(frames) == 0:
+            selected_frames = self.frames.copy()
+        else:
+            selected_frames = []
+            for frame in frames:
+                try:
+                    selected_frames.append(self.frames[frame])
+                except IndexError:
+                    print(f"Index {frame} does not exist, so it will be skipped")
+
+        l = [frame for frame in selected_frames]
+        if len(l) == 1:
+            l = l[0]
+        return l
+
     def get_data(self, select_frame: Optional[Union[None, SupportsIndex]] = None, first_frame: Optional[Union[None, SupportsIndex]] = None, last_frame: Optional[Union[None, SupportsIndex]] = None) -> List[Tuple[pygame.Surface, float]]:
         """
         Returns both the surface and the duration (in seconds) of the selected frame(s)
         
         :param select_frame: (optional) Get the surface & duration of only 1 frame, will ignore `first_frame` and `last_frame`, leave as `None` to use `first_frame` and `last_frame`
         :param first_frame: (optional) The first frame in the frames to get the surface & duration from, leave as `None` to start from the first frame
         :param last_frame: (optional) The last frame in the frames to get the surface & duration from, leave as `None` to end at the last frame
 
         Leave everything as `None` to get the surface & duration all of the frames
         """
+        warnings.warn("gif_pygame.PygameGIF.get_data deprecated since 0.1.0, use gif_pygame.PygameGIF.get_datas instead", DeprecationWarning, 2)
         selected_frames = self._grab_frame(select_frame, first_frame, last_frame)
 
         l = [frame for frame in selected_frames]
         if len(l) == 1:
             l = l[0]
         return l
 
@@ -288,25 +354,46 @@
                 print(failed_str)
             if len(duplicated_frames):
                 duplicated_str = "There were some duplicated frames, they were:\n"
                 for duplicated_frame in duplicated_frames:
                     duplicated_str += f"Frame Number: {duplicated_frame[1]}, Index: {duplicated_frame[0]}"
                 print(duplicated_str)
 
+    def get_alphas(self, frames=[]):
+        """
+        Returns the alpha of the selected frame(s)
+        
+        :param frames: (optional) Get the surface of the selected frames, leave empty to get all of the alphas
+        """
+        if len(frames) == 0:
+            selected_frames = self.frames.copy()
+        else:
+            selected_frames = []
+            for frame in frames:
+                try:
+                    selected_frames.append(self.frames[frame])
+                except IndexError:
+                    print(f"Index {frame} does not exist, so it will be skipped")
+
+        l = [frame[0].get_alpha() for frame in selected_frames]
+        if len(l) == 1:
+            l = l[0]
+        return l
 
     def get_alpha(self, select_frame: Optional[Union[None, SupportsIndex]] = None, first_frame: Optional[Union[None, SupportsIndex]] = None, last_frame: Optional[Union[None, SupportsIndex]] = None) -> List[int]:
         """
         Returns the alpha of the selected frame(s)
 
         :param select_frame: (optional) Get the alpha of only 1 frame, will ignore `first_frame` and `last_frame`, leave as `None` to use `first_frame` and `last_frame`
         :param first_frame: (optional) The first frame in the frames to get the alpha from, leave as `None` to start from the first frame
         :param last_frame: (optional) The last frame in the frames to get the alpha from, leave as `None` to end at the last frame
 
         Leave everything as `None` to get the alpha all of the frames
         """
+        warnings.warn("gif_pygame.PygameGIF.get_alpha deprecated since 0.1.0, use gif_pygame.PygameGIF.get_alphas instead", DeprecationWarning, 2)
         selected_frames = self._grab_frame(select_frame, first_frame, last_frame)
 
         alphas = [frame[0].get_alpha() for frame in selected_frames]
         if len(alphas) == 1:
             alphas = alphas[0]
         return alphas
```

### Comparing `gif_pygame-0.0.7/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gif-pygame
-Version: 0.0.7
+Name: gif_pygame
+Version: 0.1.0
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -77,18 +77,18 @@
 There are other extra functions. The ones showcased in the example code are `img.pause()` and `img.unpause()`.
 
 There are also:
 - `.get_width()`, returns the width of the image
 - `.get_height()`, returns the height of the image
 - `.get_size()`, returns the size of the image
 - `.get_rect()`, returns the rect of the image
-- `.get_surface()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
+- `.get_surfaces()`, returns a list of all surfaces in the animation, you can also pass in certain indexes
 - `.set_surface()`, replaces some of the surfaces in the animation with newer surfaces
-- `.get_duration()`, returns a list of all durations in the animation, you can also pass in certain indexes
+- `.get_durations()`, returns a list of all durations in the animation, you can also pass in certain indexes
 - `.set_duration()`, replaces some of the durations in the animation with newer durations
-- `.get_data()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
+- `.get_datas()`, returns a list of all surfaces and durations in the animation, you can also pass in certain indexes
 - `.set_data()`, replaces some of the surfaces and durations in the animation with newer surfaces and durations
-- `.get_alpha()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
+- `.get_alphas()`, returns a list of that includes the alphas of all surfaces in the animation, you can also pass in certain indexes
 - `.set_alpha()`, replaces all the alphas of surfaces with newer alphas, you can also pass in certain indexes
 - `.convert()`, converts all the surfaces in the animation, you can also pass in a `colorkey` and certain indexes
 
 Please use python's `help()` function for more in-depth explanation
```

### Comparing `gif_pygame-0.0.7/setup.py` & `gif_pygame-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="0.0.7",
+    version="0.1.0",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["pygame-ce", "pillow"],
+    install_requires=["pygame-ce", "pillow", "warnings"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
     classifiers=[
         "Development Status :: 6 - Mature",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

