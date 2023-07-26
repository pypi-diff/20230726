# Comparing `tmp/gif_pygame-0.1.0.tar.gz` & `tmp/gif_pygame-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-0.1.0.tar", last modified: Wed Jul 26 14:52:32 2023, max compression
+gzip compressed data, was "gif_pygame-0.1.1.tar", last modified: Wed Jul 26 17:16:15 2023, max compression
```

## Comparing `gif_pygame-0.1.0.tar` & `gif_pygame-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.218022 gif_pygame-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4440 2023-07-26 14:52:32.217022 gif_pygame-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3456 2023-07-26 14:43:13.000000 gif_pygame-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.202004 gif_pygame-0.1.0/gif_pygame/
--rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.1.0/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0    22554 2023-07-26 14:47:22.000000 gif_pygame-0.1.0/gif_pygame/_pygame_gif.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:52:32.216016 gif_pygame-0.1.0/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     4440 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 14:52:32.000000 gif_pygame-0.1.0/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:52:32.218022 gif_pygame-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-07-26 14:51:46.000000 gif_pygame-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.451869 gif_pygame-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5023 2023-07-26 17:16:15.451869 gif_pygame-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4039 2023-07-26 15:03:01.000000 gif_pygame-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.439414 gif_pygame-0.1.1/gif_pygame/
+-rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.1.1/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0    22554 2023-07-26 14:47:22.000000 gif_pygame-0.1.1/gif_pygame/_pygame_gif.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.450867 gif_pygame-0.1.1/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     5023 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:16:15.452870 gif_pygame-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-07-26 17:15:33.000000 gif_pygame-0.1.1/setup.py
```

### Comparing `gif_pygame-0.1.0/LICENSE` & `gif_pygame-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.1.0/PKG-INFO` & `gif_pygame-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif_pygame
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,26 +46,28 @@
 
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             pygame.quit(); sys.exit()
 
         if event.type == pygame.KEYDOWN:
             if event.key == pygame.K_ESCAPE:
-                if example_gif.paused:
-                    example_gif.unpause()
+                if example_gif.paused: # Check whether `example_gif` is paused or not
+                    example_gif.unpause() # unpauses `example_gif` if it was paused
                 else:
-                    example_gif.pause()
-                if example_png.paused:
-                    example_png.unpause()
+                    example_gif.pause() # pauses `example_gif` if it was unpaused
+
+                if example_png.paused: # Check whether `example_png` is paused or not, since this is a non-animated image, it will not be affected
+                    example_png.unpause() # unpauses `example_png` if it was paused, since this is a non-animated image, it will not be affected
                 else:
-                    example_png.pause()
-                if example_apng.paused:
-                    example_apng.unpause()
+                    example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
+
+                if example_apng.paused: # Check whether `example_apng` is paused or not
+                    example_apng.unpause() # unpauses `example_apng` if it was paused
                 else:
-                    example_apng.pause()
+                    example_apng.pause() # pauses `example_apng` if it was unpaused
                     
     pygame.display.update()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
```

### Comparing `gif_pygame-0.1.0/README.md` & `gif_pygame-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -23,26 +23,28 @@
 
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             pygame.quit(); sys.exit()
 
         if event.type == pygame.KEYDOWN:
             if event.key == pygame.K_ESCAPE:
-                if example_gif.paused:
-                    example_gif.unpause()
+                if example_gif.paused: # Check whether `example_gif` is paused or not
+                    example_gif.unpause() # unpauses `example_gif` if it was paused
                 else:
-                    example_gif.pause()
-                if example_png.paused:
-                    example_png.unpause()
+                    example_gif.pause() # pauses `example_gif` if it was unpaused
+
+                if example_png.paused: # Check whether `example_png` is paused or not, since this is a non-animated image, it will not be affected
+                    example_png.unpause() # unpauses `example_png` if it was paused, since this is a non-animated image, it will not be affected
                 else:
-                    example_png.pause()
-                if example_apng.paused:
-                    example_apng.unpause()
+                    example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
+
+                if example_apng.paused: # Check whether `example_apng` is paused or not
+                    example_apng.unpause() # unpauses `example_apng` if it was paused
                 else:
-                    example_apng.pause()
+                    example_apng.pause() # pauses `example_apng` if it was unpaused
                     
     pygame.display.update()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
```

### Comparing `gif_pygame-0.1.0/gif_pygame/_pygame_gif.py` & `gif_pygame-0.1.1/gif_pygame/_pygame_gif.py`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.1.0/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-0.1.1/gif_pygame.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif-pygame
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,26 +46,28 @@
 
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             pygame.quit(); sys.exit()
 
         if event.type == pygame.KEYDOWN:
             if event.key == pygame.K_ESCAPE:
-                if example_gif.paused:
-                    example_gif.unpause()
+                if example_gif.paused: # Check whether `example_gif` is paused or not
+                    example_gif.unpause() # unpauses `example_gif` if it was paused
                 else:
-                    example_gif.pause()
-                if example_png.paused:
-                    example_png.unpause()
+                    example_gif.pause() # pauses `example_gif` if it was unpaused
+
+                if example_png.paused: # Check whether `example_png` is paused or not, since this is a non-animated image, it will not be affected
+                    example_png.unpause() # unpauses `example_png` if it was paused, since this is a non-animated image, it will not be affected
                 else:
-                    example_png.pause()
-                if example_apng.paused:
-                    example_apng.unpause()
+                    example_png.pause() # pauses `example_png` if it was unpaused, since this is a non-animated image, it will not be affected
+
+                if example_apng.paused: # Check whether `example_apng` is paused or not
+                    example_apng.unpause() # unpauses `example_apng` if it was paused
                 else:
-                    example_apng.pause()
+                    example_apng.pause() # pauses `example_apng` if it was unpaused
                     
     pygame.display.update()
 ```
 
 To recap:
 
 `gif_pygame.load` loads in the image
```

### Comparing `gif_pygame-0.1.0/setup.py` & `gif_pygame-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="0.1.0",
+    version="0.1.1",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["pygame-ce", "pillow", "warnings"],
+    install_requires=["pygame-ce", "pillow"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
     classifiers=[
         "Development Status :: 6 - Mature",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

